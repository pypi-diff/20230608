# Comparing `tmp/codezen-0.3.0.tar.gz` & `tmp/codezen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codezen-0.3.0.tar", max compression
+gzip compressed data, was "codezen-0.4.0.tar", max compression
```

## Comparing `codezen-0.3.0.tar` & `codezen-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.3.0/LICENSE
--rw-r--r--   0        0        0     1918 2023-06-07 08:58:11.099573 codezen-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.3.0/codezen/__init__.py
--rw-r--r--   0        0        0       30 2023-05-23 13:08:17.312100 codezen-0.3.0/codezen/__main__.py
--rw-r--r--   0        0        0     4633 2023-06-07 13:39:21.600172 codezen-0.3.0/codezen/app.py
--rw-r--r--   0        0        0      582 2023-06-07 13:38:29.938525 codezen-0.3.0/codezen/ignore_files.py
--rw-r--r--   0        0        0      542 2023-06-07 13:41:03.444856 codezen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 codezen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 14:43:11.360293 codezen-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2271 2023-06-08 14:21:18.685910 codezen-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 12:54:22.029545 codezen-0.4.0/codezen/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-08 13:42:35.710816 codezen-0.4.0/codezen/__main__.py
+-rw-r--r--   0        0        0     5312 2023-06-08 14:18:41.767917 codezen-0.4.0/codezen/app.py
+-rw-r--r--   0        0        0      930 2023-06-08 14:06:48.835996 codezen-0.4.0/codezen/ignore_files.py
+-rw-r--r--   0        0        0      579 2023-06-08 14:21:41.826360 codezen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 codezen-0.4.0/PKG-INFO
```

### Comparing `codezen-0.3.0/LICENSE` & `codezen-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codezen-0.3.0/README.md` & `codezen-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 The differences from Github Copilot:
 * This is a CLI tool, meaning it can be used regardless of your chosen IDE.
 * This provides the LLM with the entire codebase, so it can do things that require a more holistic view of your project.
 
 Current limitations:
-* Only works for small codebases- currently it sends the entire codebase on each request. 😆
+* Only works for small codebases- currently it sends the entire codebase on each request (except the ignored files). 😆
 * It can't change files autonomously, it only offers a solution.
 * It uses gitignore file to know which files to ignore, so you must run this in a git repo and you can't currently ignore files that don't appear there.
 
 
 ## Installation
 ### Using PyPi
 You can install the application using `pip` or `pipx`:
@@ -59,14 +59,22 @@
 
 ```bash
 codezen <issue_description>
 ```
 
 `<issue_description>`: Describe the issue you are facing with your code
 
+If you want to ignore additional files without adding them to your `.gitignore`, You can create a `.czignore` file at the project's root and add them there.
+
+If you want to estimate the number of used tokens and show the files that are included in the prompt you can use:
+
+``` bash
+codezen <issue_description> --estimate
+```
+
 
 ## Contributing
 
 If you would like to contribute to this project, please feel free to fork the repository, create a feature branch, and submit a pull request.
 
 ## License
```

### Comparing `codezen-0.3.0/codezen/app.py` & `codezen-0.4.0/codezen/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-import argparse
 import logging
-import subprocess
 from pathlib import Path
+from typing import Annotated, List
 
+import typer
 from binaryornot.check import is_binary
 from langchain import LLMChain, PromptTemplate
 from langchain.callbacks import get_openai_callback
 from langchain.chat_models import ChatOpenAI
 from langchain.docstore.document import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 
-from codezen.ignore_files import filter_files, load_ignore_file
+from codezen.ignore_files import (
+    filter_files,
+    get_filepaths_not_gitignored,
+    load_ignore_file,
+)
 
 
 prompt = """You are an AI coder who is trying to help the user develop and debug an application based on their file system. The user has provided you with the following files and their contents, finally folllowed by the error message or issue they are facing.
 
 The file list is given between the triple backticks (```), Each file is separated by three dashes (---). There are no files in the project besides the ones listed here.
 ```
 {file_context}
@@ -28,24 +32,17 @@
 If you are not sure what the answer is, say that explicitly.
 """
 prompt_template = PromptTemplate(
     input_variables=["file_context", "issue_description"], template=prompt
 )
 
 
-def get_project_files_paths(root_dir: str) -> list[Path]:
-    result = subprocess.run(
-        ["git", "ls-files"], cwd=root_dir, capture_output=True, text=True
-    ).stdout
-    file_paths_strings = result.splitlines()
-    file_paths = [Path(root_dir) / Path(fp) for fp in file_paths_strings]
-    return file_paths
-
-
-def load_files_to_langchain_documents(root_dir: Path, project_files_paths: list[Path]):
+def load_files_to_langchain_documents(
+    root_dir: Path, project_files_paths: list[Path]
+) -> List[Document]:
     text_splitter = RecursiveCharacterTextSplitter()
 
     docs = []
     for file_path in project_files_paths:
         try:
             if is_binary(str(file_path)):
                 logging.info(f"Skipping binary file {file_path}")
@@ -61,87 +58,103 @@
             docs.extend(split_document)
         except Exception as e:
             raise Exception(f"Exception loading the document {file_path}:\n") from e
 
     return docs
 
 
-def build_context_string(docs):
+def build_context_string_from_docs(docs: List[Document]) -> str:
     all_context = []
     for doc in docs:
         current_file = f"""Relative file path: {doc.metadata["source"]}\nFile content:\n{doc.page_content}\n---\n"""
         all_context.append(current_file)
     all_context_string = "\n".join(all_context)
     return all_context_string
 
 
-def main():
-    parser = argparse.ArgumentParser(description="LLMChain CLI")
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        dest="verbose",
-        action="store_true",
-        help="Enable verbose logging",
-    )
-    parser.add_argument(
-        "-m",
-        "--model",
-        dest="model_name",
-        default="gpt-4",
-        help="The model name to use for the LLMChain",
-    )
-    parser.add_argument(
-        "-d",
-        "--root-dir",
-        dest="root_dir",
-        default=".//",
-        help="The root directory of the project",
-    )
-    parser.add_argument(
-        "-i",
-        "--ignore-file",
-        dest="ignore_file",
-        default="./.czignore",
-        help="The path to the .czignore file",
+def get_relevant_filepaths(root_dirpath: Path, czignore_filepath: Path) -> List[Path]:
+    project_files_paths = get_filepaths_not_gitignored(root_dirpath)
+    czignore_patterns = load_ignore_file(czignore_filepath)
+    project_files_paths = (
+        filter_files(project_files_paths, czignore_patterns)
+        if czignore_patterns
+        else project_files_paths
     )
-    parser.add_argument(
-        "issue_description",
-        help="The issue description",
+    return project_files_paths
+
+
+def create_model(model_name: str) -> ChatOpenAI:
+    return ChatOpenAI(model_name=model_name)
+
+
+def build_context_string(root_dirpath: Path, relevant_filepaths: List[Path]) -> str:
+    docs = load_files_to_langchain_documents(root_dirpath, relevant_filepaths)
+    logging.info(
+        f"Loaded {len(docs)} documents, total of {sum([len(doc.page_content) for doc in docs])} characters"
     )
-    args = parser.parse_args()
+    context_string = build_context_string_from_docs(docs)
+    return context_string
+
+
+app = typer.Typer(add_completion=False)
+
 
+@app.command(help="Ask the LLM a question or make a request")
+def main(
+    issue_description: Annotated[str, typer.Argument(help="The issue description")],
+    verbose: Annotated[
+        bool, typer.Option("-v", "--verbose", help="Enable verbose logging")
+    ] = False,
+    estimate: Annotated[
+        bool,
+        typer.Option(
+            "--estimate", help="Estimate request token count and show included files"
+        ),
+    ] = False,
+    model_name: Annotated[
+        str,
+        typer.Option("-m", "--model", help="The model name to use for the LLMChain"),
+    ] = "gpt-4",
+    root_dir: Annotated[
+        str, typer.Option("-d", "--root-dir", help="The root directory of the project")
+    ] = "./",
+    czignore_file: Annotated[
+        str, typer.Option("--czignore-file", help="The path to the .czignore file")
+    ] = "./.czignore",
+):
     # Set logging level
     logging.basicConfig(level=logging.WARNING)
-    if args.verbose:
+    if verbose:
         logging.basicConfig(level=logging.INFO)
 
-    model = ChatOpenAI(model_name=args.model_name)
-    llm = LLMChain(llm=model, prompt=prompt_template)
+    model = create_model(model_name=model_name)
 
-    project_files_paths = get_project_files_paths(args.root_dir)
-    czignore_patterns = load_ignore_file(args.ignore_file)
-    project_files_paths = (
-        filter_files(project_files_paths, czignore_patterns)
-        if czignore_patterns
-        else project_files_paths
+    relevant_filepaths = get_relevant_filepaths(
+        root_dirpath=Path(root_dir), czignore_filepath=Path(czignore_file)
     )
 
-    docs = load_files_to_langchain_documents(args.root_dir, project_files_paths)
-    context_string = build_context_string(docs)
+    context_string = build_context_string(Path(root_dir), relevant_filepaths)
 
-    logging.info(
-        f"Loaded {len(docs)} documents, total of {sum([len(doc.page_content) for doc in docs])} characters"
-    )
+    if estimate:
+        token_count = model.get_num_tokens(context_string)
+
+        print("Total number of request tokens:")
+        print(token_count)
+        print()
+
+        print("Included files:")
+        print("\n".join([str(p) for p in relevant_filepaths]))
+    else:
+        llm = LLMChain(llm=model, prompt=prompt_template)
+
+        with get_openai_callback() as cb:
+            result = llm.run(
+                file_context=context_string, issue_description=issue_description
+            )
 
-    with get_openai_callback() as cb:
-        result = llm.run(
-            file_context=context_string, issue_description=args.issue_description
-        )
-
-    print()
-    print("Answer:")
-    print(result)
-
-    print()
-    print("OpenAI stats:")
-    print(cb)
+        print()
+        print("Answer:")
+        print(result)
+
+        print()
+        print("OpenAI stats:")
+        print(cb)
```

### Comparing `codezen-0.3.0/codezen/ignore_files.py` & `codezen-0.4.0/codezen/ignore_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from pathlib import Path
 from typing import List, Optional
+import subprocess
 
 import pathspec
 
 
-def load_ignore_file(path: str) -> Optional[pathspec.PathSpec]:
+def get_filepaths_not_gitignored(root_dirpath: Path) -> List[Path]:
+    result = subprocess.run(
+        ["git", "ls-files"], cwd=root_dirpath, capture_output=True, text=True
+    ).stdout
+    file_paths_strings = result.splitlines()
+    file_paths = [root_dirpath / Path(fp) for fp in file_paths_strings]
+    return file_paths
+
+
+def load_ignore_file(path: Path) -> Optional[pathspec.PathSpec]:
     try:
         with open(path, "r") as file:
             lines = file.read().splitlines()
             spec = pathspec.GitIgnoreSpec.from_lines(lines)
             return spec
     except FileNotFoundError:
         return None
```

### Comparing `codezen-0.3.0/pyproject.toml` & `codezen-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "codezen"
-version = "0.3.0"
+version = "0.4.0"
 description = "Your indispensable partner in programming"
 authors = ["Maor Cohen <me@maorcohen.net>"]
 homepage = "https://github.com/mmaorc/codezen"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 langchain = "^0.0.177"
 openai = "^0.27.7"
 binaryornot = "^0.4.4"
 pathspec = "^0.11.1"
+typer = "^0.9.0"
+tiktoken = "^0.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `codezen-0.3.0/PKG-INFO` & `codezen-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: codezen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Your indispensable partner in programming
 Home-page: https://github.com/mmaorc/codezen
 Author: Maor Cohen
 Author-email: me@maorcohen.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: binaryornot (>=0.4.4,<0.5.0)
 Requires-Dist: langchain (>=0.0.177,<0.0.178)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pathspec (>=0.11.1,<0.12.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # CodeZen
 
 ## Description
 
 CodeZen is a CLI utility that uses LLMs to help you debug and evolve your codebase based on your requests.
@@ -27,15 +29,15 @@
 ```
 
 The differences from Github Copilot:
 * This is a CLI tool, meaning it can be used regardless of your chosen IDE.
 * This provides the LLM with the entire codebase, so it can do things that require a more holistic view of your project.
 
 Current limitations:
-* Only works for small codebases- currently it sends the entire codebase on each request. 😆
+* Only works for small codebases- currently it sends the entire codebase on each request (except the ignored files). 😆
 * It can't change files autonomously, it only offers a solution.
 * It uses gitignore file to know which files to ignore, so you must run this in a git repo and you can't currently ignore files that don't appear there.
 
 
 ## Installation
 ### Using PyPi
 You can install the application using `pip` or `pipx`:
@@ -75,14 +77,22 @@
 
 ```bash
 codezen <issue_description>
 ```
 
 `<issue_description>`: Describe the issue you are facing with your code
 
+If you want to ignore additional files without adding them to your `.gitignore`, You can create a `.czignore` file at the project's root and add them there.
+
+If you want to estimate the number of used tokens and show the files that are included in the prompt you can use:
+
+``` bash
+codezen <issue_description> --estimate
+```
+
 
 ## Contributing
 
 If you would like to contribute to this project, please feel free to fork the repository, create a feature branch, and submit a pull request.
 
 ## License
```

