# Comparing `tmp/enalog-0.2.0.tar.gz` & `tmp/enalog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enalog-0.2.0.tar", max compression
+gzip compressed data, was "enalog-0.2.1.tar", max compression
```

## Comparing `enalog-0.2.0.tar` & `enalog-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      390 2023-06-07 08:42:38.480467 enalog-0.2.0/README.md
--rw-r--r--   0        0        0     3768 2023-06-07 08:42:38.480467 enalog-0.2.0/enalog/__init__.py
--rw-r--r--   0        0        0      444 2023-06-07 08:42:38.480467 enalog-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 enalog-0.2.0/setup.py
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 enalog-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      390 2023-06-08 21:02:01.394841 enalog-0.2.1/README.md
+-rw-r--r--   0        0        0     4070 2023-06-08 21:02:01.394841 enalog-0.2.1/enalog/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-08 21:02:01.398841 enalog-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 enalog-0.2.1/setup.py
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 enalog-0.2.1/PKG-INFO
```

### Comparing `enalog-0.2.0/enalog/__init__.py` & `enalog-0.2.1/enalog/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import Dict, Union
 from os import environ
+import logging
+
 import requests
 from requests.exceptions import HTTPError, RequestException
 
+logger = logging.getLogger()
+logger.setLevel(logging.INFO)
+
 
 class MissingRequiredData(Exception):
     """Thrown when required keys are missing from the data object"""
 
     pass
 
 
@@ -83,17 +88,19 @@
 
             if res.status_code == 200:
                 return {
                     "status_code": 200,
                     "message": "Event succesfully sent to EnaLog",
                 }
         except requests.exceptions.HTTPError as ex:
-            raise HTTPError(ex)
+            logger.error("EnaLog: Failed to send send event")
+            return
         except requests.exceptions.RequestException as ex:
-            raise RequestException(ex)
+            logger.error("EnaLog: Failed to send send event")
+            return
 
     def check_feature(self, feature: str, user_id: str) -> Union[bool, str]:
         try:
             res = requests.post(
                 "https://api.enalog.app/v1/feature-flags",
                 json={"name": feature, "user_id": user_id},
                 headers={"Authorization": f"Bearer {self.api_token}"},
@@ -106,10 +113,12 @@
 
                 if data["flag_type"] == "Boolean":
                     if data["variant"] == "a-variant":
                         return True
                     else:
                         return False
         except requests.exceptions.HTTPError as ex:
-            raise HTTPError(ex)
+            logger.error("EnaLog: Failed to get evaluation for feature flag")
+            return False
         except requests.exceptions.RequestException as ex:
-            raise RequestException(ex)
+            logger.error("EnaLog: Failed to get evaluation for feature flag")
+            return False
```

### Comparing `enalog-0.2.0/setup.py` & `enalog-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'enalog',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Python package for sending events to EnaLog',
     'long_description': "# enalog-py\n\nEnaLog Python SDK\n\n### Usage\n\n```python\nfrom enalog import push\n\npush_event(api_token='dummy_api_token', event={\n    'project': 'enalog'\n    'name': 'user-subscribed',\n    'description': 'User has subscribed to EnaLog',\n    'push': False,\n    'icon': '💰',\n    'tags': ['app': 'EnaLog'],\n    'meta': {'user_id': 123},\n    'channels': {'slack': '<slack-channel-name>'}\n})\n```\n",
     'author': 'Sam Newby',
     'author_email': 'sam.newby19@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `enalog-0.2.0/PKG-INFO` & `enalog-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enalog
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for sending events to EnaLog
 Author: Sam Newby
 Author-email: sam.newby19@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

