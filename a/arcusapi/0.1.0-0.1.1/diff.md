# Comparing `tmp/arcusapi-0.1.0.tar.gz` & `tmp/arcusapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcusapi-0.1.0.tar", last modified: Wed Apr 26 02:47:53 2023, max compression
+gzip compressed data, was "arcusapi-0.1.1.tar", last modified: Wed Jun  7 23:04:44 2023, max compression
```

## Comparing `arcusapi-0.1.0.tar` & `arcusapi-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.072070 arcusapi-0.1.0/
--rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.0/LICENSE
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-04-26 02:47:53.071889 arcusapi-0.1.0/PKG-INFO
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-04-26 02:14:25.000000 arcusapi-0.1.0/README.md
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.060102 arcusapi-0.1.0/arcus/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3263 2023-04-18 15:39:42.000000 arcusapi-0.1.0/arcus/api_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      957 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/config.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1435 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/constants.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.060556 arcusapi-0.1.0/arcus/model/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      687 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.064714 arcusapi-0.1.0/arcus/model/shared/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/shared/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1707 2023-04-19 17:39:01.000000 arcusapi-0.1.0/arcus/model/shared/config.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/shared/data.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     5669 2023-04-24 21:56:28.000000 arcusapi-0.1.0/arcus/model/shared/metrics.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     9379 2023-04-24 21:56:45.000000 arcusapi-0.1.0/arcus/model/shared/trial.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.065981 arcusapi-0.1.0/arcus/model/torch/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1228 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/__init__.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.067707 arcusapi-0.1.0/arcus/model/torch/data/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/data_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/data_loader.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/torch/data/data_types.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/model/torch/data/dataset.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/data/lightning_utils.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2867 2023-04-24 21:57:55.000000 arcusapi-0.1.0/arcus/model/torch/data/tensor.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3196 2023-04-24 21:58:58.000000 arcusapi-0.1.0/arcus/model/torch/metrics.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.068965 arcusapi-0.1.0/arcus/model/torch/model/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/torch/model/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/torch/model/embedding_getter.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.0/arcus/model/torch/model/model_types.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-04-19 17:39:01.000000 arcusapi-0.1.0/arcus/model/torch/model/module.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-14 04:36:28.000000 arcusapi-0.1.0/arcus/model/torch/model/utils.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)    11284 2023-04-18 15:39:42.000000 arcusapi-0.1.0/arcus/model/torch/trainer.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3860 2023-04-18 10:17:50.000000 arcusapi-0.1.0/arcus/model/torch/utils.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.069346 arcusapi-0.1.0/arcus/prompt/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/__init.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.069792 arcusapi-0.1.0/arcus/prompt/text/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1006 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/config.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.070346 arcusapi-0.1.0/arcus/prompt/text/llms/
--rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/llms/__init__.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/llms/llm.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3706 2023-04-03 00:47:45.000000 arcusapi-0.1.0/arcus/prompt/text/llms/openai.py
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.071049 arcusapi-0.1.0/arcusapi.egg-info/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/PKG-INFO
--rw-r--r--   0 ardasahiner   (501) staff       (20)     1219 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/SOURCES.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/dependency_links.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)       87 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/requires.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-04-26 02:47:53.000000 arcusapi-0.1.0/arcusapi.egg-info/top_level.txt
--rw-r--r--   0 ardasahiner   (501) staff       (20)      725 2023-04-24 03:38:46.000000 arcusapi-0.1.0/pyproject.toml
--rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-04-26 02:47:53.072116 arcusapi-0.1.0/setup.cfg
-drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-04-26 02:47:53.071467 arcusapi-0.1.0/tests/
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3472 2023-04-18 15:39:42.000000 arcusapi-0.1.0/tests/test_api_client.py
--rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.0/tests/test_constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.006601 arcusapi-0.1.1/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11344 2023-03-04 18:52:55.000000 arcusapi-0.1.1/LICENSE
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-06-07 23:04:44.006445 arcusapi-0.1.1/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1222 2023-05-04 02:08:54.000000 arcusapi-0.1.1/README.md
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.996507 arcusapi-0.1.1/arcus/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      857 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4497 2023-05-25 18:25:11.000000 arcusapi-0.1.1/arcus/api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1514 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1463 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/constants.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.996735 arcusapi-0.1.1/arcus/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      687 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.998211 arcusapi-0.1.1/arcus/model/shared/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      889 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/model/shared/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1703 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/model/shared/config.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2716 2023-05-04 22:51:20.000000 arcusapi-0.1.1/arcus/model/shared/data.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     5894 2023-05-18 19:12:04.000000 arcusapi-0.1.1/arcus/model/shared/metrics.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    10126 2023-05-25 18:25:11.000000 arcusapi-0.1.1/arcus/model/shared/trial.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:43.999704 arcusapi-0.1.1/arcus/model/torch/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1223 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.001292 arcusapi-0.1.1/arcus/model/torch/data/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1143 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     4745 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/data_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     6588 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/data_loader.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      990 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/model/torch/data/data_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1936 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/model/torch/data/dataset.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     7924 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/data/lightning_utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2868 2023-05-04 22:31:56.000000 arcusapi-0.1.1/arcus/model/torch/data/tensor.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3391 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/metrics.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.002564 arcusapi-0.1.1/arcus/model/torch/model/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      787 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/torch/model/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     2129 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/torch/model/embedding_getter.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      706 2023-04-04 21:01:24.000000 arcusapi-0.1.1/arcus/model/torch/model/model_types.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    12970 2023-05-04 02:08:54.000000 arcusapi-0.1.1/arcus/model/torch/model/module.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1186 2023-04-27 17:14:10.000000 arcusapi-0.1.1/arcus/model/torch/model/utils.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    11404 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/trainer.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3839 2023-06-03 20:38:00.000000 arcusapi-0.1.1/arcus/model/torch/utils.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.003013 arcusapi-0.1.1/arcus/prompt/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      610 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/__init.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.003435 arcusapi-0.1.1/arcus/prompt/text/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      673 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/text/__init__.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.004189 arcusapi-0.1.1/arcus/prompt/text/chains/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      615 2023-06-04 07:01:05.000000 arcusapi-0.1.1/arcus/prompt/text/chains/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)    10988 2023-06-04 07:01:05.000000 arcusapi-0.1.1/arcus/prompt/text/chains/retrieval_qa.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1087 2023-05-18 19:12:04.000000 arcusapi-0.1.1/arcus/prompt/text/config.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.004996 arcusapi-0.1.1/arcus/prompt/text/llms/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      664 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/text/llms/__init__.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1591 2023-04-03 00:47:45.000000 arcusapi-0.1.1/arcus/prompt/text/llms/llm.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3898 2023-06-03 00:30:26.000000 arcusapi-0.1.1/arcus/prompt/text/llms/openai.py
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.005828 arcusapi-0.1.1/arcusapi.egg-info/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1749 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/PKG-INFO
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     1297 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        1 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      104 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/requires.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)        6 2023-06-07 23:04:43.000000 arcusapi-0.1.1/arcusapi.egg-info/top_level.txt
+-rw-r--r--   0 ardasahiner   (501) staff       (20)      747 2023-06-07 22:48:56.000000 arcusapi-0.1.1/pyproject.toml
+-rw-r--r--   0 ardasahiner   (501) staff       (20)       38 2023-06-07 23:04:44.006641 arcusapi-0.1.1/setup.cfg
+drwxr-xr-x   0 ardasahiner   (501) staff       (20)        0 2023-06-07 23:04:44.006244 arcusapi-0.1.1/tests/
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3516 2023-05-04 22:31:56.000000 arcusapi-0.1.1/tests/test_api_client.py
+-rw-r--r--   0 ardasahiner   (501) staff       (20)     3613 2023-04-03 00:47:45.000000 arcusapi-0.1.1/tests/test_constants.py
```

### Comparing `arcusapi-0.1.0/LICENSE` & `arcusapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/PKG-INFO` & `arcusapi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcusapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Arcus Data Exchange Client SDK.
 Author-email: "Arcus Inc." <sdk@arcus.co>
 Project-URL: Homepage, https://www.arcus.co
 Project-URL: Documentation, https://app.arcus.co/docs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `arcusapi-0.1.0/README.md` & `arcusapi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/__init__.py` & `arcusapi-0.1.1/arcus/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/api_client.py` & `arcusapi-0.1.1/arcus/api_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,45 +9,77 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import logging
 import warnings
 from typing import Dict, Optional
 
 import requests
+from requests.adapters import HTTPAdapter, Retry
 
-from arcus.config import BaseConfig
-from arcus.constants import ARCUS_API_URL, BEARER_PREFIX
+from arcus.config import MODE, BaseConfig
+from arcus.constants import ARCUS_API_URL, ARCUS_MODULE_NAME, BEARER_PREFIX
+
+logger = logging.getLogger(ARCUS_MODULE_NAME)
+
+logger = logging.getLogger(__name__)
+
+BACKOFF_TIME = 0.5
+DISALLOWED_STATUS_CODES = [
+    status for status in requests.status_codes._codes if status >= 400
+]
+RETRIABLE_METHODS = frozenset(
+    ["HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE", "POST"]
+)
 
 
 class ArcusResponse:
     """
     Wrapper around the response from an Arcus API call. Encodes whether status
     code was okay and the data returned.
     """
 
     data: Optional[dict]
     status_ok: bool
 
-    def __init__(self, data: Optional[dict], status_ok: bool):
+    def __init__(self, status_ok: bool, data: Optional[dict] = None):
         self.data = data
         self.status_ok = status_ok
 
 
 class APIClient:
     """
     Base class for API clients. Provides a common interface for making
     requests to the Arcus API.
     """
 
-    def __init__(self, config: BaseConfig):
+    def __init__(self, config: BaseConfig, num_retries: int = 5):
         self.config = config
+        self.num_retries = num_retries
+        self.session = requests.Session()
+        retry = Retry(
+            total=self.num_retries,
+            backoff_factor=BACKOFF_TIME,
+            raise_on_redirect=False,
+            raise_on_status=False,
+            status_forcelist=DISALLOWED_STATUS_CODES,
+            allowed_methods=RETRIABLE_METHODS,
+        )
+        self.session.mount(
+            "https://",
+            HTTPAdapter(max_retries=retry),
+        )
+        self.session.mount(
+            "http://",
+            HTTPAdapter(max_retries=retry),
+        )
 
     def _create_auth_headers(self) -> Dict:
         return {
             "Authorization": BEARER_PREFIX + self.config.get_api_key(),
         }
 
     def _append_auth_header(self, headers: Optional[Dict] = None) -> Dict:
@@ -80,26 +112,34 @@
             headers: Headers to pass to the request.
         Returns:
             ArcusResponse object containing the response data and whether the
             status code was okay.
         """
 
         headers = self._append_auth_header(headers)
-        response = requests.request(
+
+        response = self.session.request(
             method,
             f"{ARCUS_API_URL}/{path}",
             params=params,
             json=json,
             headers=headers,
         )
 
+        if self.config.mode == MODE.DEBUG:
+            logger.debug(
+                f"Request to {path} with parameters {params} took: "
+                + f"{response.elapsed.total_seconds()}s."
+            )
+
         if not response.ok:
             warnings.warn(
-                f"Request {method} {ARCUS_API_URL}/{path} failed with status"
-                + f"code {response.status_code} and message {response.text}."
+                f"Request {method} {ARCUS_API_URL}/{path} failed with"
+                + f"status code {response.status_code} and message"
+                + f"{response.text}."
             )
 
         # API client passes along whether status is okay to downstream
         # libraries to process as needed.
         return ArcusResponse(
             data=response.json() if response.ok else response.text,
             status_ok=response.ok,
```

### Comparing `arcusapi-0.1.0/arcus/config.py` & `arcusapi-0.1.1/arcus/prompt/text/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,25 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-class BaseConfig:
+from typing import Optional
+
+from arcus.config import BaseConfig
+
+
+class Config(BaseConfig):
+    """
+    Configuration for using Arcus Prompt (Text).
+    """
+
     def __init__(
-        self,
-        api_key: str,
-        project_id: str,
+        self, api_key: str, project_id: str, llm_api_key: Optional[str] = None
     ):
-        """
-        Configuration for a generic Arcus project.
-        """
-
-        self.api_key = api_key
-        self.project_id = project_id
+        super().__init__(api_key, project_id)
+        self.llm_api_key = llm_api_key
 
-    def get_api_key(self) -> str:
-        return self.api_key
+    def get_llm_api_key(self) -> Optional[str]:
+        return self.llm_api_key
 
-    def get_project_id(self) -> str:
-        return self.project_id
+    def set_llm_api_key(self, api_key: str):
+        self.llm_api_key = api_key
```

### Comparing `arcusapi-0.1.0/arcus/constants.py` & `arcusapi-0.1.1/arcus/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 import enum
 import os
 
 BEARER_PREFIX = "Bearer "
 ARCUS_ENV_VAR = "ARCUS_ENVIRONMENT"
+ARCUS_MODULE_NAME = "arcus"
 
 
 class Environment(enum.Enum):
     LOCAL = "LOCAL"
     DEV = "DEV"
     PROD = "PROD"
```

### Comparing `arcusapi-0.1.0/arcus/model/__init__.py` & `arcusapi-0.1.1/arcus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/shared/__init__.py` & `arcusapi-0.1.1/arcus/model/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/shared/config.py` & `arcusapi-0.1.1/arcus/model/shared/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
         return self.input_dim
 
     def get_output_dim(self) -> Optional[int]:
         return self.output_dim
 
     def get_column_headers(self) -> List[str]:
         return self.column_headers
-    
+
     def set_column_headers(self, column_headers: List[str]):
         self.column_headers = column_headers
```

### Comparing `arcusapi-0.1.0/arcus/model/shared/data.py` & `arcusapi-0.1.1/arcus/model/shared/data.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/shared/metrics.py` & `arcusapi-0.1.1/arcus/model/shared/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 import logging
 import time
 from enum import Enum
 from typing import Dict, List
 
 from arcus.api_client import APIClient, ArcusResponse
+from arcus.constants import ARCUS_MODULE_NAME
 from arcus.model.shared.config import Config
 from arcus.model.shared.data import CandidateMetadata
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger(ARCUS_MODULE_NAME)
 
 
 class MetricType(Enum):
     """
     Enum for the types of metrics. These are what you can log in your model
     to report important metrics to Arcus. This enum is used to enumerate the
     types of metrics that Arcus can track.
@@ -47,14 +48,15 @@
     VALIDATE = "validate"
     TEST = "test"
     PREDICT = "predict"
 
 
 # The list of the names of metrics that can be logged to Arcus.
 SUPPORTED_METRICS: List[str] = [e.value for e in MetricType]
+LOG_EVERY_N_STEPS = 5
 
 
 class StepMetrics:
     def __init__(
         self,
         metrics_map: Dict[MetricType, float],
     ):
@@ -132,15 +134,21 @@
                     + " metrics to ensure they are logged to Arcus."
                 )
                 self.empty_warning_disabled = True
 
             return
 
         self.metrics.append(StepMetrics(report_dict))
-        should_stop = self._post_metrics()
+
+        should_stop = False
+        if (
+            len(self.metrics) == 1
+            or len(self.metrics) % LOG_EVERY_N_STEPS == 0
+        ):
+            should_stop = self.post_metrics()
         return should_stop
 
     def get(self) -> List[StepMetrics]:
         return self.metrics
 
     def get_string(self) -> List[Dict[str, float]]:
         return [m.get_metrics_string() for m in self.metrics]
@@ -153,15 +161,15 @@
 
     def get_config(self) -> Config:
         return self.config
 
     def get_candidate_metadata(self) -> CandidateMetadata:
         return self.candidate_metadata
 
-    def _post_metrics(self) -> bool:
+    def post_metrics(self) -> bool:
         """
         Post the metrics to Arcus. Returns True if the model training should be
         early-stopped, False otherwise.
         """
         should_early_stop = False
 
         response: ArcusResponse = self.api_client.request(
```

### Comparing `arcusapi-0.1.0/arcus/model/shared/trial.py` & `arcusapi-0.1.1/arcus/model/shared/trial.py`

 * *Files 6% similar despite different names*

```diff
@@ -281,7 +281,31 @@
         )
 
         # return metrics table with a link to visualize results
         return (
             f"{metrics_table}\n"
             + f"\n{VISUALIZE_RESULTS_TEXT} {visualize_results_link}."
         )
+
+    def select(self, candidate_id: str) -> None:
+        """
+        Selects a candidate that was trialed for the project.
+        """
+        assert (
+            candidate_id in self.candidates_dict.keys()
+        ), f"Candidate ID {candidate_id} not found in candidates."
+
+        response: ArcusResponse = self.api_client.request(
+            "POST",
+            "model/selections",
+            params={
+                "project_id": self.config.get_project_id(),
+                "candidate_id": candidate_id,
+            },
+        )
+
+        if not response.status_ok:
+            raise Exception(
+                f"Failed to make selection for project: {response.data}."
+            )
+
+        print(f"Selected candidate {candidate_id}.")
```

### Comparing `arcusapi-0.1.0/arcus/model/torch/__init__.py` & `arcusapi-0.1.1/arcus/model/torch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     wrap_lightningmodule_loaders_vertical,
     wrap_module_and_trainer_dataloaders_vertical,
 )
 from .metrics import ArcusMetricsCallback  # noqa: F401
 from .model import EmbeddingType, HeadType, Model  # noqa: F401
 from .trainer import Trainer  # noqa: F401
 from .utils import configure_model_for_external  # noqa: F401
-from .utils import generate_selection_metadata, get_arcus_config
+from .utils import get_arcus_config, get_selection_metadata
```

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/__init__.py` & `arcusapi-0.1.1/arcus/model/torch/data/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/data_client.py` & `arcusapi-0.1.1/arcus/model/torch/data/data_client.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/data_loader.py` & `arcusapi-0.1.1/arcus/model/torch/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/data_types.py` & `arcusapi-0.1.1/arcus/model/torch/data/data_types.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/dataset.py` & `arcusapi-0.1.1/arcus/model/torch/data/dataset.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/lightning_utils.py` & `arcusapi-0.1.1/arcus/model/torch/data/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/data/tensor.py` & `arcusapi-0.1.1/arcus/model/torch/data/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     """
     Represents a tensor that is vertically augmented with external data
         from the Arcus Data Exchange.
     Args:
         first_party_data: The first party data.
         external_data: The external data.
     """
+
     def __init__(
         self,
         first_party_data: torch.Tensor,
         external_data: ExternalDataTensor,
     ):
         assert len(first_party_data) == len(
             external_data
```

### Comparing `arcusapi-0.1.0/arcus/model/torch/metrics.py` & `arcusapi-0.1.1/arcus/model/torch/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 
 
 import logging
 from typing import Dict, List, Optional
 
 from pytorch_lightning import Callback, LightningModule, Trainer
 
+from arcus.constants import ARCUS_MODULE_NAME
 from arcus.model.shared.config import Config
 from arcus.model.shared.metrics import (
     SUPPORTED_METRICS,
     MetricStore,
     Stage,
     StepMetrics,
 )
 from arcus.model.torch.utils import get_arcus_config
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger(ARCUS_MODULE_NAME)
 
 
 class ArcusMetricsCallback(Callback):
     def __init__(
         self,
         metric_names: List[str] = SUPPORTED_METRICS,
     ):
@@ -88,7 +89,12 @@
         if should_stop:
             logger.info("Arcus is stopping training early.")
 
     def get_metrics(self) -> Optional[List[StepMetrics]]:
         if self.metric_store is None:
             return None
         return self.metric_store.get()
+
+    def post_metrics(self) -> None:
+        if self.metric_store is None:
+            return None
+        self.metric_store.post_metrics()
```

### Comparing `arcusapi-0.1.0/arcus/model/torch/model/__init__.py` & `arcusapi-0.1.1/arcus/model/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/model/embedding_getter.py` & `arcusapi-0.1.1/arcus/model/torch/model/embedding_getter.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/model/model_types.py` & `arcusapi-0.1.1/arcus/model/torch/model/model_types.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/model/module.py` & `arcusapi-0.1.1/arcus/model/torch/model/module.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/model/utils.py` & `arcusapi-0.1.1/arcus/model/torch/model/utils.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/model/torch/trainer.py` & `arcusapi-0.1.1/arcus/model/torch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     TrainerDataLoaders,
     VerticalExternalDataClient,
     wrap_module_and_trainer_dataloaders_vertical,
 )
 from arcus.model.torch.metrics import ArcusMetricsCallback, Stage
 from arcus.model.torch.utils import (
     configure_model_for_external,
-    generate_selection_metadata,
     get_arcus_config,
+    get_selection_metadata,
 )
 
 __all__ = [
     "Trainer",
 ]
 
 
@@ -171,14 +171,18 @@
             )
 
             # Resets epoch to 0
             self.fit_loop.epoch_progress.current.reset()
             self.fit_loop.epoch_progress.total.reset()
             self.should_stop = False
 
+            # Ensures that the metrics from the final
+            # epoch are reported
+            self.get_reporting_callback().post_metrics()
+
             self.latest_trial.store_candidate_metrics(
                 candidate_candidate_id,
                 self.get_reporting_callback().get_metrics(),
             )
 
         self.latest_trial.complete()
 
@@ -240,15 +244,15 @@
         """
         Fits LightningModule using the given data loaders. Uses the Arcus model
         consumer service API to fetch external data.
         """
 
         self.stage = Stage.FIT
 
-        project_candidate_metadata = generate_selection_metadata(model)
+        project_candidate_metadata = get_selection_metadata(model)
         return self._train_val(
             model,
             train_dataloaders,
             val_dataloaders,
             datamodule,
             ckpt_path,
             project_candidate_metadata,
@@ -267,15 +271,15 @@
         """
         Runs validation using the given data loaders. Uses the Arcus model
         consumer service API to fetch external data.
         """
         self.stage = Stage.VALIDATE
         curr_dataloaders = TrainerDataLoaders(val_dataloaders=dataloaders)
 
-        project_candidate_metadata = generate_selection_metadata(model)
+        project_candidate_metadata = get_selection_metadata(model)
         wrapped_dataloaders = self._setup_arcus_loop(
             model,
             curr_dataloaders,
             project_candidate_metadata,
             datamodule,
         )
 
@@ -300,15 +304,15 @@
         """
         Runs test using the given data loaders. Uses the Arcus model
         consumer service API to fetch external data.
         """
         self.stage = Stage.TEST
         curr_dataloaders = TrainerDataLoaders(test_dataloaders=dataloaders)
 
-        project_candidate_metadata = generate_selection_metadata(model)
+        project_candidate_metadata = get_selection_metadata(model)
         wrapped_dataloaders = self._setup_arcus_loop(
             model,
             curr_dataloaders,
             project_candidate_metadata,
             datamodule,
         )
 
@@ -333,15 +337,15 @@
         """
         Runs prediction using the given data loaders. Uses the Arcus model
         consumer service API to fetch external data.
         """
         self.stage = Stage.PREDICT
         curr_dataloaders = TrainerDataLoaders(predict_dataloaders=dataloaders)
 
-        project_candidate_metadata = generate_selection_metadata(model)
+        project_candidate_metadata = get_selection_metadata(model)
         wrapped_dataloaders = self._setup_arcus_loop(
             model,
             curr_dataloaders,
             project_candidate_metadata,
             datamodule,
         )
```

### Comparing `arcusapi-0.1.0/arcus/model/torch/utils.py` & `arcusapi-0.1.1/arcus/model/torch/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 
 import logging
 from typing import Optional
 
 import pytorch_lightning as pl
 
 from arcus.api_client import APIClient, ArcusResponse
+from arcus.constants import ARCUS_MODULE_NAME
 from arcus.model.shared.config import Config
 from arcus.model.shared.data import (
     CandidateMetadata,
     ExternalFeatureType,
     ProjectCandidateMetadata,
 )
 from arcus.model.torch.data import VerticalExternalDataClient
 from arcus.model.torch.model import EmbeddingType, HeadType
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger(ARCUS_MODULE_NAME)
 
 __all__ = [
     "get_arcus_config",
-    "generate_selection_metadata",
+    "get_selection_metadata",
     "configure_model_for_external",
 ]
 
 
 def get_arcus_config(
     model: pl.LightningModule,
 ) -> Config:
@@ -45,37 +46,34 @@
     except AttributeError:
         assert False, (
             "LightningModule without model attribute does "
             + "not support external data"
         )
 
 
-def generate_selection_metadata(
+def get_selection_metadata(
     model: pl.LightningModule,
 ) -> Optional[ProjectCandidateMetadata]:
     """
-    Generates the Arcus metadata of the selction for the given model using the
+    Gets the Arcus metadata of the selction for the given model using the
     Arcus API.
     """
     config = get_arcus_config(model)
     api_client = APIClient(config)
 
     response: ArcusResponse = api_client.request(
-        "POST",
+        "GET",
         "model/selections/metadata",
         params={"project_id": config.get_project_id()},
-        json={
-            "column_headers": config.get_column_headers(),
-        },
     )
 
     if not response.status_ok:
-        logger.warning(
-            "Failed to retrieve data selection. Status code: "
-            + f"{response.status}."
+        raise RuntimeError(
+            "Failed to retrieve data selection. Make sure a selection has "
+            + "been made for this project."
         )
         return None
 
     response_data = response.data
 
     candidate_metadata = CandidateMetadata(
         candidate_id=response_data["candidate_id"],
```

### Comparing `arcusapi-0.1.0/arcus/prompt/__init.py` & `arcusapi-0.1.1/arcus/prompt/__init.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/prompt/text/__init__.py` & `arcusapi-0.1.1/arcus/prompt/text/__init__.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/prompt/text/config.py` & `arcusapi-0.1.1/arcus/prompt/text/llms/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,25 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Optional
-
-from arcus.config import BaseConfig
-
-
-class Config(BaseConfig):
-    """
-    Configuration for using Arcus Prompt (Text).
-    """
-
-    def __init__(
-        self, api_key: str, project_id: str, llm_api_key: Optional[str] = None
-    ):
-        super().__init__(api_key, project_id)
-        self.llm_api_key = llm_api_key
-
-    def get_llm_api_key(self) -> Optional[str]:
-        return self.llm_api_key
+from .llm import LLM, LLMOutput  # noqa: F401
+from .openai import OpenAI  # noqa: F401
```

### Comparing `arcusapi-0.1.0/arcus/prompt/text/llms/llm.py` & `arcusapi-0.1.1/arcus/prompt/text/llms/llm.py`

 * *Files identical despite different names*

### Comparing `arcusapi-0.1.0/arcus/prompt/text/llms/openai.py` & `arcusapi-0.1.1/arcus/prompt/text/llms/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import os
 from typing import Tuple
 
 import langchain
 
 from arcus.api_client import APIClient, ArcusResponse
 from arcus.prompt.text.config import Config
 from arcus.prompt.text.llms import LLM, LLMOutput
@@ -42,14 +43,16 @@
 ]
 
 OPENAI_MODEL_IDS = OPENAI_COMPLETION_MODEL_IDS + OPENAI_CHAT_MODEL_IDS
 HELPFUL_ASSISTANT_SYSTEM_MESSAGE = langchain.schema.SystemMessage(
     content="You are a helpful assistant."
 )
 
+OPENAI_API_KEY = "OPENAI_API_KEY"
+
 
 class OpenAI(LLM):
     def __init__(
         self,
         model_id: str,
         config: Config,
         **kwargs,
@@ -59,43 +62,46 @@
         assert model_id in OPENAI_MODEL_IDS, (
             "Invalid model_id for OpenAI: "
             + f"{model_id}. Valid model_ids are: {OPENAI_MODEL_IDS}."
         )
 
         self._is_chat = model_id in OPENAI_CHAT_MODEL_IDS
 
+        if self.config.get_llm_api_key() is None:
+            self.config.set_llm_api_key(os.environ.get(OPENAI_API_KEY, None))
+
         if self.is_chat():
             self.model = langchain.chat_models.ChatOpenAI(
                 model_name=model_id,
-                openai_api_key=config.get_llm_api_key(),
+                openai_api_key=self.config.get_llm_api_key(),
                 **kwargs,
             )
         else:
             self.model = langchain.llms.OpenAI(
                 model_name=model_id,
-                openai_api_key=config.get_llm_api_key(),
+                openai_api_key=self.config.get_llm_api_key(),
                 **kwargs,
             )
 
-        self.api_client = APIClient(config)
+        self.api_client = APIClient(self.config)
 
     def _augment_prompt_context(self, prompt: str) -> Tuple[str, str]:
         if not self.is_chat():
             max_tokens_remaining = self.model.max_tokens_for_prompt(prompt)
         else:
             max_tokens_remaining = None
 
         response: ArcusResponse = self.api_client.request(
             "POST",
             "/prompt/enrich",
             {
                 "project_id": self.config.get_project_id(),
-                "prompt": prompt,
                 "max_tokens_remaining": max_tokens_remaining,
             },
+            json={"prompt": prompt},
         )
 
         if not response.status_ok:
             raise Warning(
                 f"Failed to get additional context for prompt: {prompt}. "
                 + f"Response: {response}"
             )
```

### Comparing `arcusapi-0.1.0/arcusapi.egg-info/PKG-INFO` & `arcusapi-0.1.1/arcusapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcusapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Arcus Data Exchange Client SDK.
 Author-email: "Arcus Inc." <sdk@arcus.co>
 Project-URL: Homepage, https://www.arcus.co
 Project-URL: Documentation, https://app.arcus.co/docs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `arcusapi-0.1.0/arcusapi.egg-info/SOURCES.txt` & `arcusapi-0.1.1/arcusapi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 arcus/model/torch/model/embedding_getter.py
 arcus/model/torch/model/model_types.py
 arcus/model/torch/model/module.py
 arcus/model/torch/model/utils.py
 arcus/prompt/__init.py
 arcus/prompt/text/__init__.py
 arcus/prompt/text/config.py
+arcus/prompt/text/chains/__init__.py
+arcus/prompt/text/chains/retrieval_qa.py
 arcus/prompt/text/llms/__init__.py
 arcus/prompt/text/llms/llm.py
 arcus/prompt/text/llms/openai.py
 arcusapi.egg-info/PKG-INFO
 arcusapi.egg-info/SOURCES.txt
 arcusapi.egg-info/dependency_links.txt
 arcusapi.egg-info/requires.txt
```

### Comparing `arcusapi-0.1.0/pyproject.toml` & `arcusapi-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arcusapi"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Arcus Inc.", email="sdk@arcus.co" },
 ]
 description = "Arcus Data Exchange Client SDK."
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 dependencies = [
   "torch==1.13.1",
   "numpy==1.24.2",
   "pytorch-lightning==1.9.3",
-  "langchain==0.0.123",
+  "langchain==0.0.189",
   "openai==0.27.2",
+  "requests==2.31.0",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `arcusapi-0.1.0/tests/test_api_client.py` & `arcusapi-0.1.1/tests/test_api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,17 @@
                 "Authorization": "Bearer test",
                 "test": "test",
             },
         )
 
 
 class TestApiClient(unittest.TestCase):
-    @mock.patch("requests.request", side_effect=mocked_requests_request)
+    @mock.patch(
+        "requests.Session.request", side_effect=mocked_requests_request
+    )
     def test_create_arcus_request(self, mock_request):
         method = "GET"
         path = "test"
         config = MagicMock()
         config.get_api_key.return_value = "test"
         config.get_project_id.return_value = "test"
         params = {"test": "test"}
@@ -89,15 +91,17 @@
 
         api_client = APIClient(config)
 
         response = api_client.request(method, path, params, json, headers)
         self.assertEqual(response.data, {"key1": "value1"})
         self.assertEqual(response.status_ok, True)
 
-    @mock.patch("requests.request", side_effect=mocked_requests_request)
+    @mock.patch(
+        "requests.Session.request", side_effect=mocked_requests_request
+    )
     def test_create_arcus_request_fail(self, mock_request):
         method = "GET"
         path = "test2"
         config = MagicMock()
         config.get_api_key.return_value = "test"
         config.get_project_id.return_value = "test"
         params = {"test": "test"}
```

### Comparing `arcusapi-0.1.0/tests/test_constants.py` & `arcusapi-0.1.1/tests/test_constants.py`

 * *Files identical despite different names*

