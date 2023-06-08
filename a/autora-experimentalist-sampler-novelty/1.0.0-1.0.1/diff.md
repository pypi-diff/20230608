# Comparing `tmp/autora-experimentalist-sampler-novelty-1.0.0.tar.gz` & `tmp/autora-experimentalist-sampler-novelty-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-novelty-1.0.0.tar", last modified: Wed May 31 12:18:17 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-novelty-1.0.1.tar", last modified: Thu Jun  8 17:11:27 2023, max compression
```

## Comparing `autora-experimentalist-sampler-novelty-1.0.0.tar` & `autora-experimentalist-sampler-novelty-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.143584 autora-experimentalist-sampler-novelty-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.143584 autora-experimentalist-sampler-novelty-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.143584 autora-experimentalist-sampler-novelty-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.143584 autora-experimentalist-sampler-novelty-1.0.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.143584 autora-experimentalist-sampler-novelty-1.0.0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.143584 autora-experimentalist-sampler-novelty-1.0.0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/src/autora/experimentalist/sampler/novelty/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/src/autora/experimentalist/sampler/novelty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-31 12:18:17.000000 autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 12:18:17.000000 autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:18:17.000000 autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-31 12:18:17.000000 autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 12:18:17.000000 autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.147584 autora-experimentalist-sampler-novelty-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-31 12:18:01.000000 autora-experimentalist-sampler-novelty-1.0.0/tests/test_exp_novelty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.508856 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/novelty/
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/novelty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:11:27.000000 autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:27.512856 autora-experimentalist-sampler-novelty-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-08 17:11:14.000000 autora-experimentalist-sampler-novelty-1.0.1/tests/test_exp_novelty_sampler.py
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-novelty-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/.gitignore` & `autora-experimentalist-sampler-novelty-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/.pre-commit-config.yaml` & `autora-experimentalist-sampler-novelty-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/PKG-INFO` & `autora-experimentalist-sampler-novelty-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-novelty
-Version: 1.0.0
+Version: 1.0.1
 Summary: AutoRA Novelty Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-novelty
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8.10
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/README.md` & `autora-experimentalist-sampler-novelty-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/docs/Basic Usage.ipynb` & `autora-experimentalist-sampler-novelty-1.0.1/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/docs/index.md` & `autora-experimentalist-sampler-novelty-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/mkdocs/base.yml` & `autora-experimentalist-sampler-novelty-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/pyproject.toml` & `autora-experimentalist-sampler-novelty-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/src/autora/experimentalist/sampler/novelty/__init__.py` & `autora-experimentalist-sampler-novelty-1.0.1/src/autora/experimentalist/sampler/novelty/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 from typing import Iterable, Literal, Optional
 
 import numpy as np
 from sklearn.metrics import DistanceMetric
 from sklearn.preprocessing import StandardScaler
 
+from autora.utils.deprecation import deprecated_alias
+
 AllowedMetrics = Literal[
     "euclidean",
     "manhattan",
     "chebyshev",
     "minkowski",
     "wminkowski",
     "seuclidean",
@@ -59,15 +61,15 @@
     """
 
     new_conditions, distance_scores = novelty_score_sampler(condition_pool, reference_conditions, num_samples, metric, integration)
 
     return new_conditions
 
 
-def novelty_score_sampler(
+def novelty_score_sample(
     condition_pool: np.ndarray,
     reference_conditions: np.ndarray,
     num_samples: Optional[int] = None,
     metric: AllowedMetrics = "euclidean",
     integration: str = "sum",
 ) -> np.ndarray:
     """
@@ -140,7 +142,9 @@
     score = scaler.fit_transform(integrated_distance.reshape(-1, 1)).flatten()
 
     # order rows in Y from highest to lowest
     sorted_condition_pool = condition_pool[np.argsort(integrated_distance)[::-1]]
     sorted_score = score[np.argsort(score)[::-1]]
 
     return sorted_condition_pool[:num_samples], sorted_score[:num_samples]
+
+novelty_score_sampler = deprecated_alias(novelty_score_sample, "novelty_score_sampler")
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO` & `autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-novelty
-Version: 1.0.0
+Version: 1.0.1
 Summary: AutoRA Novelty Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-novelty
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8.10
```

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-novelty-1.0.1/src/autora_experimentalist_sampler_novelty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-novelty-1.0.0/tests/test_exp_novelty_sampler.py` & `autora-experimentalist-sampler-novelty-1.0.1/tests/test_exp_novelty_sampler.py`

 * *Files identical despite different names*

