# Comparing `tmp/bn_testing-0.8.1.tar.gz` & `tmp/bn_testing-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bn_testing-0.8.1.tar", last modified: Sun Oct 23 18:34:10 2022, max compression
+gzip compressed data, was "bn_testing-0.9.0.tar", last modified: Tue Oct 25 20:26:55 2022, max compression
```

## Comparing `bn_testing-0.8.1.tar` & `bn_testing-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 18:34:10.713574 bn_testing-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-23 18:33:35.000000 bn_testing-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-10-23 18:34:10.713574 bn_testing-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-10-23 18:33:35.000000 bn_testing-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 18:34:10.713574 bn_testing-0.8.1/bn_testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 18:33:35.000000 bn_testing-0.8.1/bn_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-10-23 18:33:35.000000 bn_testing-0.8.1/bn_testing/conditionals.py
--rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-10-23 18:33:35.000000 bn_testing-0.8.1/bn_testing/dags.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-23 18:33:35.000000 bn_testing-0.8.1/bn_testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     9176 2022-10-23 18:33:35.000000 bn_testing-0.8.1/bn_testing/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5876 2022-10-23 18:33:35.000000 bn_testing-0.8.1/bn_testing/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 18:34:10.713574 bn_testing-0.8.1/bn_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-10-23 18:34:10.000000 bn_testing-0.8.1/bn_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-10-23 18:34:10.000000 bn_testing-0.8.1/bn_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 18:34:10.000000 bn_testing-0.8.1/bn_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-23 18:34:10.000000 bn_testing-0.8.1/bn_testing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-23 18:34:10.000000 bn_testing-0.8.1/bn_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-23 18:34:10.717574 bn_testing-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-10-23 18:33:35.000000 bn_testing-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:26:55.535705 bn_testing-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-25 20:26:20.000000 bn_testing-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-10-25 20:26:55.535705 bn_testing-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-10-25 20:26:20.000000 bn_testing-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:26:55.535705 bn_testing-0.9.0/bn_testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 20:26:20.000000 bn_testing-0.9.0/bn_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-10-25 20:26:20.000000 bn_testing-0.9.0/bn_testing/conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-10-25 20:26:20.000000 bn_testing-0.9.0/bn_testing/dags.py
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-10-25 20:26:20.000000 bn_testing-0.9.0/bn_testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9913 2022-10-25 20:26:20.000000 bn_testing-0.9.0/bn_testing/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5894 2022-10-25 20:26:20.000000 bn_testing-0.9.0/bn_testing/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:26:55.535705 bn_testing-0.9.0/bn_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-10-25 20:26:55.000000 bn_testing-0.9.0/bn_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-10-25 20:26:55.000000 bn_testing-0.9.0/bn_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 20:26:55.000000 bn_testing-0.9.0/bn_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-25 20:26:55.000000 bn_testing-0.9.0/bn_testing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-25 20:26:55.000000 bn_testing-0.9.0/bn_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-10-25 20:26:55.535705 bn_testing-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-10-25 20:26:20.000000 bn_testing-0.9.0/setup.py
```

### Comparing `bn_testing-0.8.1/LICENSE` & `bn_testing-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bn_testing-0.8.1/PKG-INFO` & `bn_testing-0.9.0/bn_testing.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: bn_testing
-Version: 0.8.1
+Name: bn-testing
+Version: 0.9.0
 Summary: A test bench to benchmark learn algorithms for graphical models
 Home-page: https://github.com/windisch/bn_testing
 Author: Tobias Windisch
 Author-email: tobias.windisch@posteo.de
 License: GNU GPL3
 Keywords: graphical models
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BN testing
 
+
+[![Test Package](https://github.com/windisch/bn_testing/actions/workflows/test_package.yml/badge.svg)](https://github.com/windisch/bn_testing/actions/workflows/test_package.yml)
 [![Documentation Status](https://readthedocs.org/projects/bn_testing/badge/?version=latest)](https://bn_testing.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/bn_testing)](https://pypi.org/project/bn_testing/)
 
 A test framework to evaluate methods that learn Bayesian Networks from
 high-dimensional observed data.
 
 
@@ -26,17 +28,17 @@
 ```python
 from bn_testing.models import BayesianNetwork
 from bn_testing.dags import ErdosReny
 from bn_testing.conditionals import PolynomialConditional
 
 
 model = BayesianNetwork(
-   n_nodes=100,
-   dag=ErdosReny(p=0.01),
+   dag=ErdosReny(p=0.01, n_nodes=100),
    conditionals=PolynomialConditional(max_terms=5)
 )
 
-df = model.sample(10000)
+df = model.sample(10000, normalize=True)
 ```
+
 The observations are stored in a `pandas.DataFrame` where the columns
 are the nodes of the DAG and each row is an observation. The
 underlying DAG of the graphical model can be accessed with `model.dag`
```

### Comparing `bn_testing-0.8.1/README.md` & `bn_testing-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # BN testing
 
+
+[![Test Package](https://github.com/windisch/bn_testing/actions/workflows/test_package.yml/badge.svg)](https://github.com/windisch/bn_testing/actions/workflows/test_package.yml)
 [![Documentation Status](https://readthedocs.org/projects/bn_testing/badge/?version=latest)](https://bn_testing.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/bn_testing)](https://pypi.org/project/bn_testing/)
 
 A test framework to evaluate methods that learn Bayesian Networks from
 high-dimensional observed data.
 
 
@@ -13,17 +15,17 @@
 ```python
 from bn_testing.models import BayesianNetwork
 from bn_testing.dags import ErdosReny
 from bn_testing.conditionals import PolynomialConditional
 
 
 model = BayesianNetwork(
-   n_nodes=100,
-   dag=ErdosReny(p=0.01),
+   dag=ErdosReny(p=0.01, n_nodes=100),
    conditionals=PolynomialConditional(max_terms=5)
 )
 
-df = model.sample(10000)
+df = model.sample(10000, normalize=True)
 ```
+
 The observations are stored in a `pandas.DataFrame` where the columns
 are the nodes of the DAG and each row is an observation. The
 underlying DAG of the graphical model can be accessed with `model.dag`
```

### Comparing `bn_testing-0.8.1/bn_testing/conditionals.py` & `bn_testing-0.9.0/bn_testing/conditionals.py`

 * *Files identical despite different names*

### Comparing `bn_testing-0.8.1/bn_testing/dags.py` & `bn_testing-0.9.0/bn_testing/dags.py`

 * *Files identical despite different names*

### Comparing `bn_testing-0.8.1/bn_testing/models.py` & `bn_testing-0.9.0/bn_testing/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import numpy as np
+import pickle
+import cloudpickle
 import pandas as pd
 import logging
 import networkx as nx
 import pymc as pm
-from itertools import combinations
 
+from itertools import combinations
 from abc import ABCMeta
 
 from bn_testing.conditionals import ConstantConditional
 
 logger = logging.getLogger(__name__)
 
 
 class BayesianNetwork(metaclass=ABCMeta):
     """
 
-    Note:
-        We assume that the order of the nodes is a topological ordering of the resulting graph.
-
     :param bn_testing.dags.DAG dag: A DAG generation method
     :param bn_testing.conditionals.Conditionals conditionals: A conditional type
     :param int random_state: A random state
     """
 
     def __init__(self, dag=None, conditionals=None, random_state=None):
         self.random_state = random_state
@@ -266,22 +265,50 @@
         else:
             logger.warning('Hidden nodes will be included in the result!')
 
         logger.info('Build variables')
         variables = self._build_variables()
 
         logger.info('Start sampling')
-        data = pm.draw([variables[n] for n in nodes], draws=n)
+        data = pm.draw([variables[n] for n in nodes], draws=n, random_seed=self.random)
         df = pd.DataFrame(
             data=np.array(data).T,
             columns=nodes
         )
 
         if normalize:
             df = df/df.std()
         return df
 
     def show(self):
         """
         Visualizes the generated DAG.
         """
         self.dag_gen.show(self.dag)
+
+    def save(self, filepath):
+        """
+        Saves the model to the specified file
+
+        :param str filepath: Path to a file where model should be written to
+        """
+
+        model_pickled = cloudpickle.dumps(self)
+
+        with open(filepath, 'wb') as f:
+            pickle.dump(model_pickled, f)
+
+    @staticmethod
+    def load(filepath):
+        """
+        Loads the model from a file.
+
+        :param str filepath: Path to a file where model has been written to with
+            :py:func:`~bn_testing.models.BayesianNetwork.save`
+
+        :returns: The loaded model
+        :rtype: bn_testing.models.BayesianNetwork
+        """
+
+        with open(filepath, 'rb') as f:
+            model_pickled = cloudpickle.loads(f.read())
+        return pickle.loads(model_pickled)
```

### Comparing `bn_testing-0.8.1/bn_testing/terms.py` & `bn_testing-0.9.0/bn_testing/terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
 
     def __init__(self, parents, term_fn=None, disp=""):
         self.parents = parents
         self.disp = disp
 
         if term_fn is None:
-            self.term_fn = lambda x: 0
+            self.term_fn = lambda x: pm.math.constant(0)
         else:
             self.term_fn = term_fn
 
     def get_vars_from_dict(self, parent_dict):
         """
         Flattens the dict of parents to a list with order specified in the constructor.
```

### Comparing `bn_testing-0.8.1/bn_testing.egg-info/PKG-INFO` & `bn_testing-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: bn-testing
-Version: 0.8.1
+Name: bn_testing
+Version: 0.9.0
 Summary: A test bench to benchmark learn algorithms for graphical models
 Home-page: https://github.com/windisch/bn_testing
 Author: Tobias Windisch
 Author-email: tobias.windisch@posteo.de
 License: GNU GPL3
 Keywords: graphical models
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BN testing
 
+
+[![Test Package](https://github.com/windisch/bn_testing/actions/workflows/test_package.yml/badge.svg)](https://github.com/windisch/bn_testing/actions/workflows/test_package.yml)
 [![Documentation Status](https://readthedocs.org/projects/bn_testing/badge/?version=latest)](https://bn_testing.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/bn_testing)](https://pypi.org/project/bn_testing/)
 
 A test framework to evaluate methods that learn Bayesian Networks from
 high-dimensional observed data.
 
 
@@ -26,17 +28,17 @@
 ```python
 from bn_testing.models import BayesianNetwork
 from bn_testing.dags import ErdosReny
 from bn_testing.conditionals import PolynomialConditional
 
 
 model = BayesianNetwork(
-   n_nodes=100,
-   dag=ErdosReny(p=0.01),
+   dag=ErdosReny(p=0.01, n_nodes=100),
    conditionals=PolynomialConditional(max_terms=5)
 )
 
-df = model.sample(10000)
+df = model.sample(10000, normalize=True)
 ```
+
 The observations are stored in a `pandas.DataFrame` where the columns
 are the nodes of the DAG and each row is an observation. The
 underlying DAG of the graphical model can be accessed with `model.dag`
```

### Comparing `bn_testing-0.8.1/setup.py` & `bn_testing-0.9.0/setup.py`

 * *Files identical despite different names*

