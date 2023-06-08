# Comparing `tmp/autora-experimentalist-sampler-inequality-1.0.0.tar.gz` & `tmp/autora-experimentalist-sampler-inequality-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-inequality-1.0.0.tar", last modified: Wed May 31 19:30:47 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-inequality-1.0.1.tar", last modified: Thu Jun  8 17:08:35 2023, max compression
```

## Comparing `autora-experimentalist-sampler-inequality-1.0.0.tar` & `autora-experimentalist-sampler-inequality-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.836968 autora-experimentalist-sampler-inequality-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.828968 autora-experimentalist-sampler-inequality-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/build-code-reference.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/build-pages-from-toml.yml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/build-readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-31 19:30:47.836968 autora-experimentalist-sampler-inequality-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:30:47.836968 autora-experimentalist-sampler-inequality-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.832968 autora-experimentalist-sampler-inequality-1.0.0/src/autora/experimentalist/sampler/inequality/
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/src/autora/experimentalist/sampler/inequality/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.836968 autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-31 19:30:47.000000 autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-31 19:30:47.000000 autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:30:47.000000 autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 19:30:47.000000 autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:30:47.000000 autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:47.836968 autora-experimentalist-sampler-inequality-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:30:33.000000 autora-experimentalist-sampler-inequality-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.678851 autora-experimentalist-sampler-inequality-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/build-code-reference.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/build-pages-from-toml.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/build-readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.678851 autora-experimentalist-sampler-inequality-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.678851 autora-experimentalist-sampler-inequality-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.678851 autora-experimentalist-sampler-inequality-1.0.1/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.678851 autora-experimentalist-sampler-inequality-1.0.1/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/src/autora/experimentalist/sampler/inequality/
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/src/autora/experimentalist/sampler/inequality/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-08 17:08:35.000000 autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-08 17:08:35.000000 autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:08:35.000000 autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 17:08:35.000000 autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:08:35.000000 autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:35.682851 autora-experimentalist-sampler-inequality-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:08:25.000000 autora-experimentalist-sampler-inequality-1.0.1/tests/__init__.py
```

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/build-code-reference.yml` & `autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/build-code-reference.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/build-pages-from-toml.yml` & `autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/build-pages-from-toml.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/build-readme.yml` & `autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/build-readme.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-inequality-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/.gitignore` & `autora-experimentalist-sampler-inequality-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/.pre-commit-config.yaml` & `autora-experimentalist-sampler-inequality-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/PKG-INFO` & `autora-experimentalist-sampler-inequality-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-inequality
-Version: 1.0.0
+Version: 1.0.1
 Summary: AutoRA Inequality Sampler
 Author-email: "Chad C. Williams" <cwilliams.uca@gmail.com>, Younes Strittmatter <younes_strittmatter@brown.com>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-inequality
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/README.md` & `autora-experimentalist-sampler-inequality-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/docs/Basic Usage.ipynb` & `autora-experimentalist-sampler-inequality-1.0.1/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/mkdocs/base.yml` & `autora-experimentalist-sampler-inequality-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/pyproject.toml` & `autora-experimentalist-sampler-inequality-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/src/autora/experimentalist/sampler/inequality/__init__.py` & `autora-experimentalist-sampler-inequality-1.0.1/src/autora/experimentalist/sampler/inequality/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Iterable, Literal
 
 import numpy as np
 from sklearn.metrics import DistanceMetric
 
+from autora.utils.deprecation import deprecated_alias
+
 AllowedMetrics = Literal[
     "euclidean",
     "manhattan",
     "chebyshev",
     "minkowski",
     "wminkowski",
     "seuclidean",
@@ -23,15 +25,15 @@
     "russellrao",
     "sokalmichener",
     "sokalsneath",
     "yule",
 ]
 
 
-def summed_inequality_sampler(
+def summed_inequality_sample(
     condition_pool: np.ndarray,
     reference_conditions: np.ndarray,
     n: int = 1,
     equality_distance: float = 0,
     metric: str = "euclidean",
 ) -> np.ndarray:
     """
@@ -131,7 +133,9 @@
         condition_pool_res.append(condition_pool[0])
         # add the chosen value to reference_conditions
         reference_conditions = np.append(reference_conditions, [condition_pool[0]], axis=0)
         # remove the chosen value from condition_pool
         condition_pool = condition_pool[1:]
 
     return np.array(condition_pool_res[:n])
+
+summed_inequality_sampler = deprecated_alias(summed_inequality_sample, "summed_inequality_sampler")
```

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/PKG-INFO` & `autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-inequality
-Version: 1.0.0
+Version: 1.0.1
 Summary: AutoRA Inequality Sampler
 Author-email: "Chad C. Williams" <cwilliams.uca@gmail.com>, Younes Strittmatter <younes_strittmatter@brown.com>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-inequality
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/src/autora_experimentalist_sampler_inequality.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-inequality-1.0.1/src/autora_experimentalist_sampler_inequality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-inequality-1.0.0/tests/README.md` & `autora-experimentalist-sampler-inequality-1.0.1/tests/README.md`

 * *Files identical despite different names*

