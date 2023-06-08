# Comparing `tmp/glocalx-0.0.2.tar.gz` & `tmp/glocalx-0.0.3.tar.gz`

## Comparing `glocalx-0.0.2.tar` & `glocalx-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/.gitignore
--rwxr-xr-x   0        0        0    11172 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/__init__.py
--rwxr-xr-x   0        0        0     9848 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/api.py
--rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/callbacks.py
--rwxr-xr-x   0        0        0    26406 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/evaluators.py
--rwxr-xr-x   0        0        0     8617 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/generators.py
--rwxr-xr-x   0        0        0    24739 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/glocalx.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/glocax_probabilistic.py
--rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/models.py
--rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/requirements.txt
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/serialization.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/data/dummy/dummy_dataset.csv
--rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/data/dummy/dummy_model.h5
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/data/dummy/dummy_rules.json
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/data/loaders/adult_info.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.2/src/glocalx/loaders/lore.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.2/LICENSE
--rwxr-xr-x   0        0        0    11172 2020-02-02 00:00:00.000000 glocalx-0.0.2/README.md
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 glocalx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 glocalx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/.gitignore
+-rwxr-xr-x   0        0        0    11172 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/__init__.py
+-rwxr-xr-x   0        0        0     9852 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/api.py
+-rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/callbacks.py
+-rwxr-xr-x   0        0        0    26407 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/evaluators.py
+-rwxr-xr-x   0        0        0     8618 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/generators.py
+-rwxr-xr-x   0        0        0    24742 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/glocalx.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/glocax_probabilistic.py
+-rwxr-xr-x   0        0        0    12664 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/models.py
+-rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/requirements.txt
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/serialization.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/data/dummy/dummy_dataset.csv
+-rw-r--r--   0        0        0    32544 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/data/dummy/dummy_model.h5
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/data/dummy/dummy_rules.json
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/data/loaders/adult_info.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 glocalx-0.0.3/src/glocalx/loaders/lore.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 glocalx-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0    11172 2020-02-02 00:00:00.000000 glocalx-0.0.3/README.md
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 glocalx-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 glocalx-0.0.3/PKG-INFO
```

### Comparing `glocalx-0.0.2/src/glocalx/.gitignore` & `glocalx-0.0.3/src/glocalx/.gitignore`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/README.md` & `glocalx-0.0.3/src/glocalx/README.md`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/api.py` & `glocalx-0.0.3/src/glocalx/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """API module for GLocalX."""
 import sys
 import os
 import time
 import pickle
 import json
 
-from callbacks import print_cb, full_cb, final_rule_dump_cb
-from glocalx import GLocalX
-from generators import TrePanGenerator, BudgedExhaustedException
+from .callbacks import print_cb, full_cb, final_rule_dump_cb
+from .glocalx import GLocalX
+from .generators import TrePanGenerator, BudgedExhaustedException
 
 # Shut up, tensorflow!
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
 import click
 import logzero
 import numpy as np
 from tensorflow.keras.models import load_model as load_tf_model
 
 from logzero import logger
 
-from models import Rule
+from .models import Rule
 
 
 @click.command()
 # Compulsory arguments: input rules, TR set, TS set, oracle
 @click.argument('rules', type=click.Path(exists=True))
 @click.argument('tr', type=click.Path(exists=True))
 @click.option('-o', '--oracle', type=click.Path(exists=True))
```

### Comparing `glocalx-0.0.2/src/glocalx/callbacks.py` & `glocalx-0.0.3/src/glocalx/callbacks.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/evaluators.py` & `glocalx-0.0.3/src/glocalx/evaluators.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import abstractmethod
 
 import numpy as np
 from scipy.spatial.distance import hamming
 
 from logzero import logger
 
-from models import Rule
+from .models import Rule
 
 
 def covers(rule, x):
     """Does `rule` cover c?
 
     Args:
         rule (Rule): The rule.
```

### Comparing `glocalx-0.0.2/src/glocalx/generators.py` & `glocalx-0.0.3/src/glocalx/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from numpy import hstack, unique, array, argwhere, concatenate
 
 # Stats
 from numpy.random import choice, random
 from sklearn.neighbors import KernelDensity
 
-from evaluators import MemEvaluator
+from .evaluators import MemEvaluator
 
 from logzero import logger
 
 
 class BudgedExhaustedException(Exception):
     """Exception raised when a given budget is exhausted."""
```

### Comparing `glocalx-0.0.2/src/glocalx/glocalx.py` & `glocalx-0.0.3/src/glocalx/glocalx.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 from logzero import logger
 
 from sklearn.model_selection import train_test_split
 import tensorflow as tf
 import numpy as np
 
-from evaluators import MemEvaluator
-from callbacks import final_rule_dump_cb as final_rule_dump_callback
-from models import Rule
+from .evaluators import MemEvaluator
+from .callbacks import final_rule_dump_cb as final_rule_dump_callback
+from .models import Rule
 
 
 class Predictor:
     """Interface to be implemented by black boxes."""
     @abstractmethod
     def predict(self, x):
         """
```

### Comparing `glocalx-0.0.2/src/glocalx/glocax_probabilistic.py` & `glocalx-0.0.3/src/glocalx/glocax_probabilistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from glocalx import GLocalX
+from .glocalx import GLocalX
 
 
 class ProbabilisticCutGLocalX(GLocalX):
 
     def _cut(self, conflicting_group, x, y, strict_cut=True):
         """
         Cut the provided `conflicting_groups`. Each conflicting group is
```

### Comparing `glocalx-0.0.2/src/glocalx/models.py` & `glocalx-0.0.3/src/glocalx/models.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/requirements.txt` & `glocalx-0.0.3/src/glocalx/requirements.txt`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/serialization.py` & `glocalx-0.0.3/src/glocalx/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from tensorflow.keras.models import load_model as load_tf_model
 import numpy as np
 
 import json
 import os
 
-from glocalx import GLocalX
-from models import Rule
+from .glocalx import GLocalX
+from .models import Rule
 
 
 def load_run(run_file):
     """
     The rules file output by GLocalX is slightly different than the input one loaded
     with models.Rule.from_json, as it contains additional information on the run, such as
     the input files paths, hyperparameters, etc.
```

### Comparing `glocalx-0.0.2/src/glocalx/data/dummy/dummy_model.h5` & `glocalx-0.0.3/src/glocalx/data/dummy/dummy_model.h5`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/data/loaders/adult_info.json` & `glocalx-0.0.3/src/glocalx/data/loaders/adult_info.json`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/src/glocalx/loaders/lore.py` & `glocalx-0.0.3/src/glocalx/loaders/lore.py`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/LICENSE` & `glocalx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/README.md` & `glocalx-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `glocalx-0.0.2/pyproject.toml` & `glocalx-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "glocalx"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Mattia Setzu", email="mattia.setzu@di.unipi.it" },
 ]
 description = "Generating global explanations from local ones."
 readme = "README.md"
 requires-python = ">=3.8, <3.9"
 classifiers = [
```

### Comparing `glocalx-0.0.2/PKG-INFO` & `glocalx-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glocalx
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generating global explanations from local ones.
 Project-URL: Homepage, https://github.com/msetzu/glocalx
 Project-URL: Bug Tracker, https://github.com/msetzu/glocalx/issues
 Author-email: Mattia Setzu <mattia.setzu@di.unipi.it>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

