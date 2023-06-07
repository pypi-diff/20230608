# Comparing `tmp/d20-securityLayer-2.0.0a2.tar.gz` & `tmp/d20-securityLayer-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-yw1pxvlb\d20-securityLayer-2.0.0a2.tar", last modified: Fri May 26 23:56:24 2023, max compression
+gzip compressed data, was "D:\d20\tools\libs\security_layer_python_arangodb\dist\.tmp-qc5pez9_\d20-securityLayer-2.0.0a4.tar", last modified: Wed Jun  7 23:55:29 2023, max compression
```

## Comparing `d20-securityLayer-2.0.0a2.tar` & `d20-securityLayer-2.0.0a4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.889098 d20-securityLayer-2.0.0a2/
--rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a2/LICENSE
--rw-rw-rw-   0        0        0      677 2023-05-26 23:56:24.886084 d20-securityLayer-2.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a2/README.md
--rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 23:56:24.890108 d20-securityLayer-2.0.0a2/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-05-26 23:55:43.000000 d20-securityLayer-2.0.0a2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.689836 d20-securityLayer-2.0.0a2/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.719309 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/
--rw-rw-rw-   0        0        0      677 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 23:56:24.000000 d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 23:56:24.882087 d20-securityLayer-2.0.0a2/src/securityLayer/
--rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a2/src/securityLayer/AccessControl.py
--rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a2/src/securityLayer/AuthAnswer.py
--rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a2/src/securityLayer/Error.py
--rw-rw-rw-   0        0        0    16923 2023-05-16 03:11:04.000000 d20-securityLayer-2.0.0a2/src/securityLayer/SSO.py
--rw-rw-rw-   0        0        0    15241 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a2/src/securityLayer/SecurityLayer.py
--rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a2/src/securityLayer/__init__.py
--rw-rw-rw-   0        0        0      156 2023-05-12 02:57:34.000000 d20-securityLayer-2.0.0a2/src/securityLayer/__version__.py
--rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a2/src/securityLayer/default.py
+drwxrwxrwx   0        0        0        0 2023-06-07 23:55:29.838205 d20-securityLayer-2.0.0a4/
+-rw-rw-rw-   0        0        0     1064 2021-09-22 23:30:22.000000 d20-securityLayer-2.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0      677 2023-06-07 23:55:29.835694 d20-securityLayer-2.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2021-06-18 21:41:10.000000 d20-securityLayer-2.0.0a4/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-22 23:14:25.000000 d20-securityLayer-2.0.0a4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 23:55:29.838205 d20-securityLayer-2.0.0a4/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-06-07 23:54:53.000000 d20-securityLayer-2.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 23:55:29.604007 d20-securityLayer-2.0.0a4/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 23:55:29.691354 d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/
+-rw-rw-rw-   0        0        0      677 2023-06-07 23:55:29.000000 d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-06-07 23:55:29.000000 d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 23:55:29.000000 d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-07 23:55:29.000000 d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 23:55:29.000000 d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 23:55:29.834694 d20-securityLayer-2.0.0a4/src/securityLayer/
+-rw-rw-rw-   0        0        0    10081 2023-05-12 01:22:57.000000 d20-securityLayer-2.0.0a4/src/securityLayer/AccessControl.py
+-rw-rw-rw-   0        0        0      233 2023-05-16 00:25:53.000000 d20-securityLayer-2.0.0a4/src/securityLayer/AuthAnswer.py
+-rw-rw-rw-   0        0        0     9697 2023-05-16 02:42:02.000000 d20-securityLayer-2.0.0a4/src/securityLayer/Error.py
+-rw-rw-rw-   0        0        0    16797 2023-06-07 23:54:37.000000 d20-securityLayer-2.0.0a4/src/securityLayer/SSO.py
+-rw-rw-rw-   0        0        0    15243 2023-05-27 00:03:51.000000 d20-securityLayer-2.0.0a4/src/securityLayer/SecurityLayer.py
+-rw-rw-rw-   0        0        0      125 2023-01-02 23:20:55.000000 d20-securityLayer-2.0.0a4/src/securityLayer/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-06-07 23:54:59.000000 d20-securityLayer-2.0.0a4/src/securityLayer/__version__.py
+-rw-rw-rw-   0        0        0       55 2021-09-23 23:27:01.000000 d20-securityLayer-2.0.0a4/src/securityLayer/default.py
```

### Comparing `d20-securityLayer-2.0.0a2/LICENSE` & `d20-securityLayer-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a2/PKG-INFO` & `d20-securityLayer-2.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a2
+Version: 2.0.0a4
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a2/setup.py` & `d20-securityLayer-2.0.0a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="d20-securityLayer",
-    version="2.0.0a2",
+    version="2.0.0a4",
     author="Alex Sánchez Vega",
     author_email="alex@d20.services",
     description="A simple access manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/d20services/security_layer_python_arangodb",
     project_urls={
```

### Comparing `d20-securityLayer-2.0.0a2/src/d20_securityLayer.egg-info/PKG-INFO` & `d20-securityLayer-2.0.0a4/src/d20_securityLayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d20-securityLayer
-Version: 2.0.0a2
+Version: 2.0.0a4
 Summary: A simple access manager
 Home-page: https://github.com/d20services/security_layer_python_arangodb
 Author: Alex Sánchez Vega
 Author-email: alex@d20.services
 Project-URL: Bug Tracker, https://github.com/d20services/security_layer_python_arangodb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `d20-securityLayer-2.0.0a2/src/securityLayer/AccessControl.py` & `d20-securityLayer-2.0.0a4/src/securityLayer/AccessControl.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a2/src/securityLayer/Error.py` & `d20-securityLayer-2.0.0a4/src/securityLayer/Error.py`

 * *Files identical despite different names*

### Comparing `d20-securityLayer-2.0.0a2/src/securityLayer/SSO.py` & `d20-securityLayer-2.0.0a4/src/securityLayer/SSO.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from .SecurityLayer import SecurityLayer
 from .AccessControl import *
 from .Error import *
-from dtwentyORM import Metadata
-from dtwentyCommunications import Communications
-from flask import request, redirect, url_for
 from .AuthAnswer import AuthAnswer
 import json
 import datetime
 from .default import crypt as D20_SL_CRYPTOKEY
 
 
 def sso_authorize(user_id='', auth_token='',token={},grant_type='',state='',scopes='',redirect_uri='', code='', refresh_token='',mode='', lifespawn=10):
```

### Comparing `d20-securityLayer-2.0.0a2/src/securityLayer/SecurityLayer.py` & `d20-securityLayer-2.0.0a4/src/securityLayer/SecurityLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import json
 
 def sl_dbname():
     return f'{os.environ.get("DBPREFIX", "")}security_layer'
 
 class SecurityLayer():
 
-    def __init__(self, conf={}):
+    def __init__(self, conf=None):
         graphname = ''
         collections = ['UserCredentials', 'APICredentials', 'UserTokens', 'APITokens', 'OTP', 'PasswordRecoveryTokens']
         edgeDefinitions={}
         db_name = sl_dbname()
         factory = GraphClassFactory.ClassFactory(graphname, db_name, collections = collections, edgeDefinitions=edgeDefinitions, conf=conf)
 
         print(factory, " - OK")
```

