# Comparing `tmp/python_code_outline-0.1.3.tar.gz` & `tmp/python_code_outline-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_code_outline-0.1.3.tar", max compression
+gzip compressed data, was "python_code_outline-0.1.4.tar", max compression
```

## Comparing `python_code_outline-0.1.3.tar` & `python_code_outline-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.3/LICENSE
--rw-r--r--   0        0        0     5714 2023-06-05 05:57:35.083931 python_code_outline-0.1.3/README.md
--rw-r--r--   0        0        0      540 2023-06-05 06:35:50.296065 python_code_outline-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      135 2023-06-05 06:35:45.789411 python_code_outline-0.1.3/python_code_outline/__init__.py
--rw-r--r--   0        0        0     5494 2023-06-05 06:20:39.362103 python_code_outline-0.1.3/python_code_outline/python_report_generator.py
--rw-r--r--   0        0        0     6336 1970-01-01 00:00:00.000000 python_code_outline-0.1.3/setup.py
--rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 python_code_outline-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5875 2023-06-08 08:08:25.199602 python_code_outline-0.1.4/README.md
+-rw-r--r--   0        0        0      540 2023-06-08 07:29:04.499995 python_code_outline-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-06-05 06:37:21.617890 python_code_outline-0.1.4/python_code_outline/__init__.py
+-rw-r--r--   0        0        0     5500 2023-06-08 08:02:04.030411 python_code_outline-0.1.4/python_code_outline/python_report_generator.py
+-rw-r--r--   0        0        0     6498 1970-01-01 00:00:00.000000 python_code_outline-0.1.4/setup.py
+-rw-r--r--   0        0        0     6162 1970-01-01 00:00:00.000000 python_code_outline-0.1.4/PKG-INFO
```

### Comparing `python_code_outline-0.1.3/LICENSE` & `python_code_outline-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_code_outline-0.1.3/README.md` & `python_code_outline-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,32 @@
 ```
 
 ## Usage as a pip module
 
 After installing the package via pip, you can import and use the functionality in your own code as well. For example:
 
 ```python
+""" Generate a report of the python code outline of a folder. """
 from python_code_outline import python_report_generator
 
 # Define the root folder
-root_folder = "/path/to/folder"
+ROOT_FOLDER = "/path/to/folder"
 
 # Specify the report and ignore file paths (optional)
-report_file_path = "custom_report.txt"
-ignore_file_path = "/path/to/folder/.gitignore"
+REPORT_FILE_PATH = "custom_report.txt"
+IGNORE_FILE_PATH = "/path/to/folder/.gitignore"
 
 # Generate the report
-report = python_report_generator.get_report(root_folder, ignore_file_path)
+REPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)
 
 # Write the report to a file
-with open(report_file_path, "w", encoding="utf-8") as file:
-    file.write(report)
+with open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:
+    file.write(REPORT)
 
-print(f"Report generated successfully to {report_file_path}.")
+print(f"Report generated successfully to {REPORT_FILE_PATH}.")
 ```
 
 Please replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.
 
 ## Output
 
 The script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.
@@ -73,17 +74,21 @@
 
 You can install this module using pip:
 
 ```bash
 pip install python-code-outline
 ```
 
-This command will download the package from PyPI and install it in your current Python environment.
+or with poetry
 
-Absolutely, I can update the installation instructions. Here is the updated `readme.md`:
+```bash
+poetry add python-code-outline
+```
+
+This command will download the package from PyPI and install it in your current Python environment.
 
 ## Running Tests
 
 This project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:
 
 ```bash
 poetry shell
@@ -95,20 +100,28 @@
 pytest
 ```
 
 ## Checking Test Coverage
 
 This project uses the `coverage` package to generate test coverage reports. Here's how to use it:
 
-1. First, you need to install the `coverage` package if it's not already installed. You can do so by running the following command:
+1. First, you need to install the `coverage` package if it's not already installed.
 
 ```bash
 pip install coverage
 ```
 
+or
+
+```bash
+poetry add coverage
+```
+
+If you're using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.
+
 2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
 
 ```bash
 coverage run -m pytest
 ```
 
 This command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.
```

### Comparing `python_code_outline-0.1.3/pyproject.toml` & `python_code_outline-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-code-outline"
-version = "0.1.3"
+version = "0.1.4"
 description = "Takes a folder path and outputs a text outline of the code, supports ignore files."
 authors = ["Sean Dearnaley <SeanDearnaley@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `python_code_outline-0.1.3/python_code_outline/python_report_generator.py` & `python_code_outline-0.1.4/python_code_outline/python_report_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Generate a text-based report of the code structure for Python code in a folder."""
 import argparse
 import ast
 from pathlib import Path
 from typing import List, Optional
 
 
-def parse_ignore_patterns(ignorefile_path: Path) -> List[str]:
+def parse_ignore_patterns(ignorefile_path: str) -> List[str]:
     """Parse the patterns to ignore from a .gitignore file."""
-    with ignorefile_path.open(encoding="utf-8") as file:
+    with Path(ignorefile_path).open(encoding="utf-8") as file:
         return [
             line.strip() for line in file if line.strip() and not line.startswith("#")
         ]
 
 
 def is_ignored(entry: Path, ignored_patterns: List[str]) -> bool:
     """Check if a given entry should be ignored."""
     return entry.name == ".gitignore" or any(
         entry.match(pattern) for pattern in ignored_patterns
     )
 
 
-def list_entries(root: Path) -> List[Path]:
+def list_entries(root: str) -> List[Path]:
     """List all entries in a given folder, sorted by type and name."""
-    return sorted(root.iterdir(), key=lambda e: (e.is_file(), e.name.lower()))
+    return sorted(Path(root).iterdir(), key=lambda e: (e.is_file(), e.name.lower()))
 
 
 def process_import(item: ast.Import) -> str:
     """Process an import statement."""
     return f"imports {', '.join([alias.name for alias in item.names])}"
 
 
@@ -79,15 +79,15 @@
     return "\n".join(output)
 
 
 # ...
 
 
 def generate_report(
-    root: Path, root_folder: Path, ignored_patterns: Optional[List[str]] = None
+    root: str, root_folder: str, ignored_patterns: Optional[List[str]] = None
 ) -> str:
     """
     Generate a report of the code structure for all Python
     files in a given folder."""
 
     if ignored_patterns is None:
         ignored_patterns = []
@@ -138,31 +138,31 @@
 
     if not Path(root_folder).is_dir():
         raise ValueError(f"{root_folder} is not a valid directory")
 
     return args
 
 
-def get_report(root_folder: Path, ignore_file_path: Optional[Path] = None) -> str:
+def get_report(root_folder: str, ignore_file_path: Optional[str] = None) -> str:
     """Get the report of the code structure for all Python files in a given folder."""
     ignored_patterns = (
         parse_ignore_patterns(ignore_file_path)
-        if ignore_file_path and ignore_file_path.exists()
+        if ignore_file_path and Path(ignore_file_path).exists()
         else []
     )
 
     return generate_report(root_folder, root_folder, ignored_patterns)
 
 
 def main() -> None:
     """Main function."""
     args = parse_arguments()
     root_folder = Path(args.root_folder)
     report_file_path = args.report_file_path
-    ignore_file_path = Path(args.ignore_file_path) if args.ignore_file_path else None
+    ignore_file_path = args.ignore_file_path if args.ignore_file_path else None
 
     report = get_report(root_folder, ignore_file_path)
 
     with open(report_file_path, "w", encoding="utf-8") as file:
         file.write(report)
 
     print(f"Report generated successfully to {report_file_path}.")
```

### Comparing `python_code_outline-0.1.3/setup.py` & `python_code_outline-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['python_code_outline']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'python-code-outline',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Takes a folder path and outputs a text outline of the code, supports ignore files.',
-    'long_description': '# Python Code Structure Report Generator\n\n[![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)\n\n![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)\n\nThis Python script generates a text-based report of the code structure for all Python files in a given folder. It\'s useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.\n\n[Example Report](example_report.txt?raw=true)\n\n## Usage\n\nTo use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.\n\n```bash\npython python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore\n```\n\nIf the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.\n\n```bash\npython python_report_generator.py /path/to/folder\n```\n\n## Usage as a pip module\n\nAfter installing the package via pip, you can import and use the functionality in your own code as well. For example:\n\n```python\nfrom python_code_outline import python_report_generator\n\n# Define the root folder\nroot_folder = "/path/to/folder"\n\n# Specify the report and ignore file paths (optional)\nreport_file_path = "custom_report.txt"\nignore_file_path = "/path/to/folder/.gitignore"\n\n# Generate the report\nreport = python_report_generator.get_report(root_folder, ignore_file_path)\n\n# Write the report to a file\nwith open(report_file_path, "w", encoding="utf-8") as file:\n    file.write(report)\n\nprint(f"Report generated successfully to {report_file_path}.")\n```\n\nPlease replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.\n\n## Output\n\nThe script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.\n\n## Optional Parameters\n\n- `--report_file_path`: The name of the report file. Defaults to `report.txt` if not provided.\n- `--ignore_file_path`: The path to the ignore file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.\n\n## Requirements\n\nThis script requires Python 3.x to run.\n\n## Installation\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency management. To install the dependencies, first install Poetry by following the [official installation guide](https://python-poetry.org/docs/#installation), and then run the following command in the project directory:\n\n```bash\npoetry install\n```\n\nThis will create a virtual environment and install the required dependencies.\n\nYou can install this module using pip:\n\n```bash\npip install python-code-outline\n```\n\nThis command will download the package from PyPI and install it in your current Python environment.\n\nAbsolutely, I can update the installation instructions. Here is the updated `readme.md`:\n\n## Running Tests\n\nThis project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:\n\n```bash\npoetry shell\n```\n\nThen, run the tests using the following command:\n\n```bash\npytest\n```\n\n## Checking Test Coverage\n\nThis project uses the `coverage` package to generate test coverage reports. Here\'s how to use it:\n\n1. First, you need to install the `coverage` package if it\'s not already installed. You can do so by running the following command:\n\n```bash\npip install coverage\n```\n\n2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you\'re using `pytest` for testing, you can use the following command:\n\n```bash\ncoverage run -m pytest\n```\n\nThis command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.\n\n3. Once you\'ve collected coverage data, you can generate a report by running:\n\n```bash\ncoverage report\n```\n\nThis will print a coverage report to the terminal, showing the code coverage for each module in your project.\n\n4. If you want a more detailed view, you can generate an HTML report using:\n\n```bash\ncoverage html\n```\n\nThis will generate an `htmlcov` directory in your project directory. Inside this directory, you\'ll find an `index.html` file. You can open this file in a web browser to view a detailed coverage report that shows which lines of each file were covered by the tests.\n\n5. If you\'re finished checking coverage and want to clear the collected data, you can use the command:\n\n```bash\ncoverage erase\n```\n\nThis will delete the `.coverage` data file, clearing the collected coverage data.\n\nRemember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn\'t necessarily mean your testing is perfect. It\'s important to write meaningful tests and not just strive for high coverage percentages.',
+    'long_description': '# Python Code Structure Report Generator\n\n[![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)\n\n![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)\n\nThis Python script generates a text-based report of the code structure for all Python files in a given folder. It\'s useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.\n\n[Example Report](example_report.txt?raw=true)\n\n## Usage\n\nTo use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.\n\n```bash\npython python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore\n```\n\nIf the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.\n\n```bash\npython python_report_generator.py /path/to/folder\n```\n\n## Usage as a pip module\n\nAfter installing the package via pip, you can import and use the functionality in your own code as well. For example:\n\n```python\n""" Generate a report of the python code outline of a folder. """\nfrom python_code_outline import python_report_generator\n\n# Define the root folder\nROOT_FOLDER = "/path/to/folder"\n\n# Specify the report and ignore file paths (optional)\nREPORT_FILE_PATH = "custom_report.txt"\nIGNORE_FILE_PATH = "/path/to/folder/.gitignore"\n\n# Generate the report\nREPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)\n\n# Write the report to a file\nwith open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:\n    file.write(REPORT)\n\nprint(f"Report generated successfully to {REPORT_FILE_PATH}.")\n```\n\nPlease replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.\n\n## Output\n\nThe script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.\n\n## Optional Parameters\n\n- `--report_file_path`: The name of the report file. Defaults to `report.txt` if not provided.\n- `--ignore_file_path`: The path to the ignore file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.\n\n## Requirements\n\nThis script requires Python 3.x to run.\n\n## Installation\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency management. To install the dependencies, first install Poetry by following the [official installation guide](https://python-poetry.org/docs/#installation), and then run the following command in the project directory:\n\n```bash\npoetry install\n```\n\nThis will create a virtual environment and install the required dependencies.\n\nYou can install this module using pip:\n\n```bash\npip install python-code-outline\n```\n\nor with poetry\n\n```bash\npoetry add python-code-outline\n```\n\nThis command will download the package from PyPI and install it in your current Python environment.\n\n## Running Tests\n\nThis project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:\n\n```bash\npoetry shell\n```\n\nThen, run the tests using the following command:\n\n```bash\npytest\n```\n\n## Checking Test Coverage\n\nThis project uses the `coverage` package to generate test coverage reports. Here\'s how to use it:\n\n1. First, you need to install the `coverage` package if it\'s not already installed.\n\n```bash\npip install coverage\n```\n\nor\n\n```bash\npoetry add coverage\n```\n\nIf you\'re using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.\n\n2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you\'re using `pytest` for testing, you can use the following command:\n\n```bash\ncoverage run -m pytest\n```\n\nThis command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.\n\n3. Once you\'ve collected coverage data, you can generate a report by running:\n\n```bash\ncoverage report\n```\n\nThis will print a coverage report to the terminal, showing the code coverage for each module in your project.\n\n4. If you want a more detailed view, you can generate an HTML report using:\n\n```bash\ncoverage html\n```\n\nThis will generate an `htmlcov` directory in your project directory. Inside this directory, you\'ll find an `index.html` file. You can open this file in a web browser to view a detailed coverage report that shows which lines of each file were covered by the tests.\n\n5. If you\'re finished checking coverage and want to clear the collected data, you can use the command:\n\n```bash\ncoverage erase\n```\n\nThis will delete the `.coverage` data file, clearing the collected coverage data.\n\nRemember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn\'t necessarily mean your testing is perfect. It\'s important to write meaningful tests and not just strive for high coverage percentages.',
     'author': 'Sean Dearnaley',
     'author_email': 'SeanDearnaley@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `python_code_outline-0.1.3/PKG-INFO` & `python_code_outline-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-code-outline
-Version: 0.1.3
+Version: 0.1.4
 Summary: Takes a folder path and outputs a text outline of the code, supports ignore files.
 Author: Sean Dearnaley
 Author-email: SeanDearnaley@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,31 +35,32 @@
 ```
 
 ## Usage as a pip module
 
 After installing the package via pip, you can import and use the functionality in your own code as well. For example:
 
 ```python
+""" Generate a report of the python code outline of a folder. """
 from python_code_outline import python_report_generator
 
 # Define the root folder
-root_folder = "/path/to/folder"
+ROOT_FOLDER = "/path/to/folder"
 
 # Specify the report and ignore file paths (optional)
-report_file_path = "custom_report.txt"
-ignore_file_path = "/path/to/folder/.gitignore"
+REPORT_FILE_PATH = "custom_report.txt"
+IGNORE_FILE_PATH = "/path/to/folder/.gitignore"
 
 # Generate the report
-report = python_report_generator.get_report(root_folder, ignore_file_path)
+REPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)
 
 # Write the report to a file
-with open(report_file_path, "w", encoding="utf-8") as file:
-    file.write(report)
+with open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:
+    file.write(REPORT)
 
-print(f"Report generated successfully to {report_file_path}.")
+print(f"Report generated successfully to {REPORT_FILE_PATH}.")
 ```
 
 Please replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.
 
 ## Output
 
 The script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.
@@ -85,17 +86,21 @@
 
 You can install this module using pip:
 
 ```bash
 pip install python-code-outline
 ```
 
-This command will download the package from PyPI and install it in your current Python environment.
+or with poetry
 
-Absolutely, I can update the installation instructions. Here is the updated `readme.md`:
+```bash
+poetry add python-code-outline
+```
+
+This command will download the package from PyPI and install it in your current Python environment.
 
 ## Running Tests
 
 This project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:
 
 ```bash
 poetry shell
@@ -107,20 +112,28 @@
 pytest
 ```
 
 ## Checking Test Coverage
 
 This project uses the `coverage` package to generate test coverage reports. Here's how to use it:
 
-1. First, you need to install the `coverage` package if it's not already installed. You can do so by running the following command:
+1. First, you need to install the `coverage` package if it's not already installed.
 
 ```bash
 pip install coverage
 ```
 
+or
+
+```bash
+poetry add coverage
+```
+
+If you're using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.
+
 2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
 
 ```bash
 coverage run -m pytest
 ```
 
 This command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.
```

