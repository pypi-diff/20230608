# Comparing `tmp/teamsgraphapi-0.0.1.tar.gz` & `tmp/teamsgraphapi-0.0.2.tar.gz`

## Comparing `teamsgraphapi-0.0.1.tar` & `teamsgraphapi-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/src/graphapi/__init__.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/src/graphapi/auth.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/src/graphapi/graph.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/LICENCE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/graphapi/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/graphapi/auth.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/graphapi/graph.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/LICENCE
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/README.md
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 teamsgraphapi-0.0.2/PKG-INFO
```

### Comparing `teamsgraphapi-0.0.1/src/graphapi/graph.py` & `teamsgraphapi-0.0.2/graphapi/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pprint import pprint
-from auth import authentication_headers, base_url
+from .auth import authentication_headers, base_url
 import requests
 
 
 class GraphAPI():
     """
     Graph Api class provides multiple
     usefull methods for different team
```

### Comparing `teamsgraphapi-0.0.1/LICENCE` & `teamsgraphapi-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `teamsgraphapi-0.0.1/pyproject.toml` & `teamsgraphapi-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
-requires = ["hatchling", "requests"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "TeamsGraphApi"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ajay Vishwakarma", email="ajay.vishwakarma@codiant.com" },
 ]
-description = "wrapper for teams graph api's"
+description = "wrapper for micorsoft teams graph api's"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+      "requests==2.31.0"
+]
+
 [project.urls]
 "Homepage" = "https://github.com/Ajay7415/graphapi"
 "Bug Tracker" = "https://github.com/Ajay7415/graphapi/issues"
```

