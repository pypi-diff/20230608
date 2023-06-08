# Comparing `tmp/RESTApiGen-0.2.0.tar.gz` & `tmp/RESTApiGen-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RESTApiGen-0.2.0.tar", last modified: Thu Jun  8 14:19:30 2023, max compression
+gzip compressed data, was "RESTApiGen-0.2.0.1.tar", last modified: Thu Jun  8 14:21:30 2023, max compression
```

## Comparing `RESTApiGen-0.2.0.tar` & `RESTApiGen-0.2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     1065 2022-12-05 11:12:33.000000 RESTApiGen-0.2.0/LICENSE
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4780 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/PKG-INFO
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4544 2023-06-08 14:17:26.000000 RESTApiGen-0.2.0/README.md
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       38 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/setup.cfg
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      878 2023-06-08 14:17:17.000000 RESTApiGen-0.2.0/setup.py
-drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/src/
-drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4780 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/PKG-INFO
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      274 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/SOURCES.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)        1 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/dependency_links.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       47 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/entry_points.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      130 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/requires.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       11 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/top_level.txt
--rwxrwxr-x   0 saiyam    (1000) saiyam    (1000)    27076 2023-06-08 14:10:02.000000 RESTApiGen-0.2.0/src/RESTApiGen.py
+drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:21:30.164564 RESTApiGen-0.2.0.1/
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     1065 2022-12-05 11:12:33.000000 RESTApiGen-0.2.0.1/LICENSE
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4783 2023-06-08 14:21:30.164564 RESTApiGen-0.2.0.1/PKG-INFO
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4544 2023-06-08 14:17:26.000000 RESTApiGen-0.2.0.1/README.md
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       38 2023-06-08 14:21:30.164564 RESTApiGen-0.2.0.1/setup.cfg
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      880 2023-06-08 14:20:58.000000 RESTApiGen-0.2.0.1/setup.py
+drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:21:30.164564 RESTApiGen-0.2.0.1/src/
+drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:21:30.164564 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4783 2023-06-08 14:21:30.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/PKG-INFO
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      274 2023-06-08 14:21:30.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/SOURCES.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)        1 2023-06-08 14:21:30.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/dependency_links.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       47 2023-06-08 14:21:30.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/entry_points.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      130 2023-06-08 14:21:30.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/requires.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       11 2023-06-08 14:21:30.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/top_level.txt
+-rwxrwxr-x   0 saiyam    (1000) saiyam    (1000)    27076 2023-06-08 14:10:02.000000 RESTApiGen-0.2.0.1/src/RESTApiGen.py
```

### Comparing `RESTApiGen-0.2.0/LICENSE` & `RESTApiGen-0.2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RESTApiGen-0.2.0/PKG-INFO` & `RESTApiGen-0.2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: RESTApiGen
-Version: 0.2.0
+Version: 0.2.0.1
 Summary: REST API auto-generator.
 Home-page: https://github.com/Saiyam-J/RESTApiGen
 Author: Saiyam Jain
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-ESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
+RESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
 harnessing the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
 
 # Features
 
 * Makes Models and REST files for each table so its easier to modulate and customize as per the needs.
 * Integrates flask-blueprints and auto registers the models.
 * Accepts requests in the form of application/json and also responds in JSON.
```

### Comparing `RESTApiGen-0.2.0/README.md` & `RESTApiGen-0.2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `RESTApiGen-0.2.0/setup.py` & `RESTApiGen-0.2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
-long_description = long_description[23:]
+long_description = long_description[22:]
 setup(
     name="RESTApiGen",
-    version="0.2.0",
+    version="0.2.0.1",
     description="REST API auto-generator.",
     url="https://github.com/Saiyam-J/RESTApiGen",
     author="Saiyam Jain",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
```

### Comparing `RESTApiGen-0.2.0/src/RESTApiGen.egg-info/PKG-INFO` & `RESTApiGen-0.2.0.1/src/RESTApiGen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: RESTApiGen
-Version: 0.2.0
+Version: 0.2.0.1
 Summary: REST API auto-generator.
 Home-page: https://github.com/Saiyam-J/RESTApiGen
 Author: Saiyam Jain
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-ESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
+RESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
 harnessing the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
 
 # Features
 
 * Makes Models and REST files for each table so its easier to modulate and customize as per the needs.
 * Integrates flask-blueprints and auto registers the models.
 * Accepts requests in the form of application/json and also responds in JSON.
```

### Comparing `RESTApiGen-0.2.0/src/RESTApiGen.py` & `RESTApiGen-0.2.0.1/src/RESTApiGen.py`

 * *Files identical despite different names*

