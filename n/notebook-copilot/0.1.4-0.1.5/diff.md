# Comparing `tmp/notebook_copilot-0.1.4.tar.gz` & `tmp/notebook_copilot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_copilot-0.1.4.tar", last modified: Tue Jun  6 21:22:02 2023, max compression
+gzip compressed data, was "notebook_copilot-0.1.5.tar", last modified: Thu Jun  8 01:44:52 2023, max compression
```

## Comparing `notebook_copilot-0.1.4.tar` & `notebook_copilot-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.907738 notebook_copilot-0.1.4/
--rw-r--r--   0 tp         (501) staff       (20)     1059 2023-06-05 01:38:02.000000 notebook_copilot-0.1.4/LICENSE
--rw-r--r--   0 tp         (501) staff       (20)     4068 2023-06-06 21:22:02.907618 notebook_copilot-0.1.4/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)     3529 2023-06-05 02:20:23.000000 notebook_copilot-0.1.4/README.md
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.906180 notebook_copilot-0.1.4/notebook_copilot/
--rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1.4/notebook_copilot/__init__.py
--rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1.4/notebook_copilot/agents.py
--rw-r--r--   0 tp         (501) staff       (20)     1296 2023-06-05 01:04:00.000000 notebook_copilot-0.1.4/notebook_copilot/chains.py
--rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1.4/notebook_copilot/context.py
--rw-r--r--   0 tp         (501) staff       (20)     4554 2023-06-03 23:28:59.000000 notebook_copilot-0.1.4/notebook_copilot/notebook_copilot.py
--rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1.4/notebook_copilot/output.py
--rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1.4/notebook_copilot/prompts.py
--rw-r--r--   0 tp         (501) staff       (20)     2328 2023-06-05 01:34:26.000000 notebook_copilot-0.1.4/notebook_copilot/tools.py
--rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1.4/notebook_copilot/utils.py
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.907111 notebook_copilot-0.1.4/notebook_copilot.egg-info/
--rw-r--r--   0 tp         (501) staff       (20)     4068 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)      520 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 tp         (501) staff       (20)      118 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/requires.txt
--rw-r--r--   0 tp         (501) staff       (20)       23 2023-06-06 21:22:02.000000 notebook_copilot-0.1.4/notebook_copilot.egg-info/top_level.txt
--rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-06 21:22:02.907776 notebook_copilot-0.1.4/setup.cfg
--rw-r--r--   0 tp         (501) staff       (20)      927 2023-06-06 21:21:59.000000 notebook_copilot-0.1.4/setup.py
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-06 21:22:02.907396 notebook_copilot-0.1.4/tests/
--rw-r--r--   0 tp         (501) staff       (20)        0 2023-06-05 00:27:43.000000 notebook_copilot-0.1.4/tests/__init__.py
--rw-r--r--   0 tp         (501) staff       (20)     2129 2023-06-05 01:15:45.000000 notebook_copilot-0.1.4/tests/test_copilot.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.985686 notebook_copilot-0.1.5/
+-rw-r--r--   0 tp         (501) staff       (20)     1059 2023-06-05 01:38:02.000000 notebook_copilot-0.1.5/LICENSE
+-rw-r--r--   0 tp         (501) staff       (20)     4640 2023-06-08 01:44:52.985546 notebook_copilot-0.1.5/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)     3529 2023-06-05 02:20:23.000000 notebook_copilot-0.1.5/README.md
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.984162 notebook_copilot-0.1.5/notebook_copilot/
+-rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1.5/notebook_copilot/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1.5/notebook_copilot/agents.py
+-rw-r--r--   0 tp         (501) staff       (20)     1296 2023-06-05 01:04:00.000000 notebook_copilot-0.1.5/notebook_copilot/chains.py
+-rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1.5/notebook_copilot/context.py
+-rw-r--r--   0 tp         (501) staff       (20)     4573 2023-06-07 23:57:18.000000 notebook_copilot-0.1.5/notebook_copilot/notebook_copilot.py
+-rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1.5/notebook_copilot/output.py
+-rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1.5/notebook_copilot/prompts.py
+-rw-r--r--   0 tp         (501) staff       (20)     2328 2023-06-05 01:34:26.000000 notebook_copilot-0.1.5/notebook_copilot/tools.py
+-rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1.5/notebook_copilot/utils.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.984871 notebook_copilot-0.1.5/notebook_copilot.egg-info/
+-rw-r--r--   0 tp         (501) staff       (20)     4640 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)      520 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 tp         (501) staff       (20)      118 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/requires.txt
+-rw-r--r--   0 tp         (501) staff       (20)       23 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/top_level.txt
+-rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-08 01:44:52.985734 notebook_copilot-0.1.5/setup.cfg
+-rw-r--r--   0 tp         (501) staff       (20)     1488 2023-06-08 01:44:20.000000 notebook_copilot-0.1.5/setup.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.985157 notebook_copilot-0.1.5/tests/
+-rw-r--r--   0 tp         (501) staff       (20)        0 2023-06-05 00:27:43.000000 notebook_copilot-0.1.5/tests/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     2129 2023-06-05 01:15:45.000000 notebook_copilot-0.1.5/tests/test_copilot.py
```

### Comparing `notebook_copilot-0.1.4/LICENSE` & `notebook_copilot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/PKG-INFO` & `notebook_copilot-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: notebook_copilot
-Version: 0.1.4
-Summary: The Bridge from Thoughts to Well-Crafted Jupyter Notebook
-Home-page: https://github.com/talperetz/notebook_copilot
-Author: Tal Peretz
-Author-email: tp@aihumanlabs.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7.1, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🚀 Notebook Copilot: From Thoughts to Well-Crafted Notebook at Record-Speed. 
 
 Welcome to Notebook Copilot, your next-generation tool for Jupyter Notebooks. Inspired by GitHub Copilot, Notebook
 Copilot is designed to help engineers and data scientists in developing professional, high-quality notebooks. It's like
 having your personal AI-powered assistant that helps you navigate through the Jupyter universe, seamlessly
 generating code and markdown cells based on your inputs.
```

### Comparing `notebook_copilot-0.1.4/notebook_copilot/agents.py` & `notebook_copilot-0.1.5/notebook_copilot/agents.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/notebook_copilot/chains.py` & `notebook_copilot-0.1.5/notebook_copilot/chains.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/notebook_copilot/context.py` & `notebook_copilot-0.1.5/notebook_copilot/context.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/notebook_copilot/notebook_copilot.py` & `notebook_copilot-0.1.5/notebook_copilot/notebook_copilot.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 from IPython.core.magic import Magics, magics_class, line_magic, cell_magic
 from langchain.document_loaders import NotebookLoader
 
 from notebook_copilot.agents import get_cot_notebook_agent, AgentStrategy, agent_strategy_type, \
     get_plan_execute_notebook_agent
-from notebook_copilot.chains import get_llm, get_cells_completion, explain_cell_completion
+from notebook_copilot.chains import get_cells_completion, explain_cell_completion
 from notebook_copilot.context import get_ipython_run_history, compress_notebook_context
 from notebook_copilot.output import generate_notebook_cells, reset_first_cell_index, generate_notebook_cell_above
 from notebook_copilot.prompts import CellCompletion, COPILOT_PERSONA, COPILOT_TASK, COPILOT_DIRECTIONS
 from notebook_copilot.utils import stringify_docs
 
 
 @magics_class
@@ -27,34 +27,35 @@
             parser.add_argument('-m', '--model', default='gpt-3.5-turbo',
                                 help='Model name to use.  e.g gpt-3.5-turbo')
             parser.add_argument('-k', '--api-key', default=None,
                                 help='API key to use. If not provided, OPENAI_API_KEY environment variable will be used.')
             valid_agent_strategies = ", ".join([strategy.name for strategy in AgentStrategy])
             parser.add_argument('-s', '--strategy', type=agent_strategy_type, default=AgentStrategy.COT,
                                 help=f'The strategy to use. one of: {valid_agent_strategies}')
-            parser.add_argument('-n', '--notebook-path', default=None,
-                                help='the current notebook path e.g /home/user/notebooks/this_notebook.ipynb')
+            parser.add_argument('-n', '--notebook-name', default=None,
+                                help='the current name e.g -n Untitled')
             parser.add_argument('-i', '--ignore-notebook', default=None,
                                 help='run copilot without the notebook context')
 
             # Parse the line input
             args = parser.parse_args(line.split())
 
             # Check if the API key is provided in the arguments
             api_key = os.getenv('OPENAI_API_KEY') if args.api_key is None else args.api_key
             if api_key is None:
                 raise ValueError('API key not provided and OPENAI_API_KEY environment variable is not set.')
 
-            if args.notebook_path is None:
+            if args.notebook_name is None:
                 raise ValueError(
-                    'Notebook path must be set. e.g %copilot_init -n /home/user/notebooks/this_notebook.ipynb')
+                    'Notebook name must be set. e.g %copilot_init -n notebook_copilot_example')
 
-            self.llm = get_llm(key=api_key, model_name=args.model)
+            # self.llm = get_llm(key=api_key, model_name=args.model)
             self.agent_strategy = args.strategy
-            notebook = NotebookLoader(args.notebook_path,
+            notebook_path = os.path.join(os.getcwd(), f"{args.notebook_name}.ipynb")
+            notebook = NotebookLoader(notebook_path,
                                       remove_newline=True).load()
             self.notebook_docs = compress_notebook_context(notebook)
 
     @cell_magic
     def generate(self, line, cell):
         with contextlib.suppress(KeyboardInterrupt):
             run_history = get_ipython_run_history()
```

### Comparing `notebook_copilot-0.1.4/notebook_copilot/output.py` & `notebook_copilot-0.1.5/notebook_copilot/output.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/notebook_copilot/prompts.py` & `notebook_copilot-0.1.5/notebook_copilot/prompts.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/notebook_copilot/tools.py` & `notebook_copilot-0.1.5/notebook_copilot/tools.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/notebook_copilot.egg-info/PKG-INFO` & `notebook_copilot-0.1.5/notebook_copilot.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 Metadata-Version: 2.1
 Name: notebook-copilot
-Version: 0.1.4
+Version: 0.1.5
 Summary: The Bridge from Thoughts to Well-Crafted Jupyter Notebook
 Home-page: https://github.com/talperetz/notebook_copilot
 Author: Tal Peretz
 Author-email: tp@aihumanlabs.com
 License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Jupyter
+Classifier: Natural Language :: English
 Requires-Python: >=3.7.1, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🚀 Notebook Copilot: From Thoughts to Well-Crafted Notebook at Record-Speed. 
 
 Welcome to Notebook Copilot, your next-generation tool for Jupyter Notebooks. Inspired by GitHub Copilot, Notebook
```

### Comparing `notebook_copilot-0.1.4/notebook_copilot.egg-info/SOURCES.txt` & `notebook_copilot-0.1.5/notebook_copilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.4/tests/test_copilot.py` & `notebook_copilot-0.1.5/tests/test_copilot.py`

 * *Files identical despite different names*

