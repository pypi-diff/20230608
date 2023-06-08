# Comparing `tmp/velovi-0.2.0.tar.gz` & `tmp/velovi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velovi-0.2.0.tar", max compression
+gzip compressed data, was "velovi-0.3.0.tar", max compression
```

## Comparing `velovi-0.2.0.tar` & `velovi-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1517 2023-03-03 07:24:37.603948 velovi-0.2.0/LICENSE
--rw-r--r--   0        0        0     2129 2023-03-03 07:24:37.603948 velovi-0.2.0/README.md
--rw-r--r--   0        0        0     4429 2023-03-03 07:24:37.611948 velovi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1145 2023-03-03 07:24:37.611948 velovi-0.2.0/velovi/__init__.py
--rw-r--r--   0        0        0      149 2023-03-03 07:24:37.611948 velovi-0.2.0/velovi/_constants.py
--rw-r--r--   0        0        0    42966 2023-03-03 07:24:37.611948 velovi-0.2.0/velovi/_model.py
--rw-r--r--   0        0        0    22310 2023-03-03 07:24:37.611948 velovi-0.2.0/velovi/_module.py
--rw-r--r--   0        0        0     2128 2023-03-03 07:24:37.611948 velovi-0.2.0/velovi/_utils.py
--rw-r--r--   0        0        0     3569 2023-03-03 07:24:47.598106 velovi-0.2.0/setup.py
--rw-r--r--   0        0        0     4251 2023-03-03 07:24:47.598561 velovi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-06-08 04:42:18.546300 velovi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2129 2023-06-08 04:42:18.546300 velovi-0.3.0/README.md
+-rw-r--r--   0        0        0     4399 2023-06-08 04:42:18.550300 velovi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1145 2023-06-08 04:42:18.550300 velovi-0.3.0/velovi/__init__.py
+-rw-r--r--   0        0        0      149 2023-06-08 04:42:18.550300 velovi-0.3.0/velovi/_constants.py
+-rw-r--r--   0        0        0    42937 2023-06-08 04:42:18.550300 velovi-0.3.0/velovi/_model.py
+-rw-r--r--   0        0        0    22328 2023-06-08 04:42:18.550300 velovi-0.3.0/velovi/_module.py
+-rw-r--r--   0        0        0     2128 2023-06-08 04:42:18.550300 velovi-0.3.0/velovi/_utils.py
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 velovi-0.3.0/PKG-INFO
```

### Comparing `velovi-0.2.0/LICENSE` & `velovi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velovi-0.2.0/README.md` & `velovi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `velovi-0.2.0/pyproject.toml` & `velovi-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 [tool.poetry]
 authors = ["Adam Gayoso <adamgayoso@berkeley.edu>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Science/Research",
   "Natural Language :: English",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX :: Linux",
   "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 description = "Estimation of RNA velocity with variational inference."
 documentation = "https://scvi-tools.org"
 homepage = "https://github.com/YosefLab/velovi"
 license = "BSD-3-Clause"
 name = "velovi"
 packages = [
   {include = "velovi"},
 ]
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 anndata = ">=0.7.5"
 black = {version = ">=20.8b1", optional = true}
 codecov = {version = ">=2.0.8", optional = true}
 ruff = {version = "*", optional = true}
 importlib-metadata = {version = "^1.0", python = "<3.8"}
@@ -39,33 +39,32 @@
 sphinx-book-theme = {version = ">=1.0.0", optional = true}
 myst-nb = {version = "*", optional = true}
 sphinx-copybutton = {version = "*", optional = true}
 sphinxcontrib-bibtex = {version = "*", optional = true}
 ipykernel = {version = "*", optional = true}
 pytest = {version = ">=4.4", optional = true}
 pytest-cov = {version = "*", optional = true}
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 python-igraph = {version = "*", optional = true}
 scanpy = {version = ">=1.6", optional = true}
 scanpydoc = {version = ">=0.5", optional = true}
 scvelo = ">=0.2.5"
-scvi-tools = ">=0.20.1"
+scvi-tools = ">=1.0.0"
 scikit-learn = ">=0.21.2"
 sphinx = {version = ">=4.1", optional = true}
 sphinx-autodoc-typehints = {version = "*", optional = true}
 
 [tool.poetry.extras]
 dev = ["black", "pytest", "pytest-cov", "ruff", "codecov", "scanpy", "loompy", "jupyter", "pre-commit"]
 docs = [
   "sphinx",
   "scanpydoc",
   "ipython",
   "myst-nb",
   "sphinx-book-theme",
-  "sphinx-autodoc-typehints",
   "sphinx-copybutton",
   "sphinxcontrib-bibtex",
   "ipykernel",
   "ipython",
 ]
 tutorials = ["scanpy"]
```

### Comparing `velovi-0.2.0/velovi/__init__.py` & `velovi-0.3.0/velovi/__init__.py`

 * *Files identical despite different names*

### Comparing `velovi-0.2.0/velovi/_model.py` & `velovi-0.3.0/velovi/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,14 @@
         trainer_kwargs.update(user_train_kwargs)
 
         data_splitter = DataSplitter(
             self.adata_manager,
             train_size=train_size,
             validation_size=validation_size,
             batch_size=batch_size,
-            use_gpu=use_gpu,
         )
         training_plan = TrainingPlan(self.module, **plan_kwargs)
 
         es = "early_stopping"
         trainer_kwargs[es] = (
             early_stopping if es not in trainer_kwargs.keys() else trainer_kwargs[es]
         )
```

### Comparing `velovi-0.2.0/velovi/_module.py` & `velovi-0.3.0/velovi/_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         return px_pi, px_rho, px_tau
 
 
 # VAE model
 class VELOVAE(BaseModuleClass):
     """Variational auto-encoder model.
 
-    This is an implementation of the scVI model descibed in [Lopez18]_
+    This is an implementation of the veloVI model descibed in :cite:p:`GayosoWeiler2022`
 
     Parameters
     ----------
     n_input
         Number of input genes
     n_hidden
         Number of nodes per hidden layer
```

### Comparing `velovi-0.2.0/velovi/_utils.py` & `velovi-0.3.0/velovi/_utils.py`

 * *Files identical despite different names*

### Comparing `velovi-0.2.0/PKG-INFO` & `velovi-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: velovi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Estimation of RNA velocity with variational inference.
 Home-page: https://github.com/YosefLab/velovi
 License: BSD-3-Clause
 Author: Adam Gayoso
 Author-email: adamgayoso@berkeley.edu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tutorials
 Requires-Dist: anndata (>=0.7.5)
-Requires-Dist: black (>=20.8b1); extra == "dev"
-Requires-Dist: codecov (>=2.0.8); extra == "dev"
-Requires-Dist: importlib-metadata (>=1.0,<2.0); python_version < "3.8"
-Requires-Dist: ipykernel; extra == "docs"
-Requires-Dist: ipython (>=7.1.1); extra == "docs" or extra == "docs"
-Requires-Dist: jupyter (>=1.0); extra == "dev"
-Requires-Dist: myst-nb; extra == "docs"
-Requires-Dist: pre-commit (>=2.7.1); extra == "dev"
-Requires-Dist: pytest (>=4.4); extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: black (>=20.8b1) ; extra == "dev"
+Requires-Dist: codecov (>=2.0.8) ; extra == "dev"
+Requires-Dist: importlib-metadata (>=1.0,<2.0) ; python_version < "3.8"
+Requires-Dist: ipykernel ; extra == "docs"
+Requires-Dist: ipython (>=7.1.1) ; extra == "docs" or extra == "docs"
+Requires-Dist: jupyter (>=1.0) ; extra == "dev"
+Requires-Dist: myst-nb ; extra == "docs"
+Requires-Dist: pre-commit (>=2.7.1) ; extra == "dev"
+Requires-Dist: pytest (>=4.4) ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: python-igraph
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: scanpy (>=1.6); extra == "dev" or extra == "tutorials"
-Requires-Dist: scanpydoc (>=0.5); extra == "docs"
+Requires-Dist: ruff ; extra == "dev"
+Requires-Dist: scanpy (>=1.6) ; extra == "dev" or extra == "tutorials"
+Requires-Dist: scanpydoc (>=0.5) ; extra == "docs"
 Requires-Dist: scikit-learn (>=0.21.2)
 Requires-Dist: scvelo (>=0.2.5)
-Requires-Dist: scvi-tools (>=0.20.1)
-Requires-Dist: sphinx (>=4.1); extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
-Requires-Dist: sphinx-book-theme (>=1.0.0); extra == "docs"
-Requires-Dist: sphinx-copybutton; extra == "docs"
-Requires-Dist: sphinxcontrib-bibtex; extra == "docs"
+Requires-Dist: scvi-tools (>=1.0.0)
+Requires-Dist: sphinx (>=4.1) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints
+Requires-Dist: sphinx-book-theme (>=1.0.0) ; extra == "docs"
+Requires-Dist: sphinx-copybutton ; extra == "docs"
+Requires-Dist: sphinxcontrib-bibtex ; extra == "docs"
 Project-URL: Documentation, https://scvi-tools.org
 Description-Content-Type: text/markdown
 
 # velovi
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
```

