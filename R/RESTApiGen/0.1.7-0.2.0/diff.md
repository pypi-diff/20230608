# Comparing `tmp/RESTApiGen-0.1.7.tar.gz` & `tmp/RESTApiGen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RESTApiGen-0.1.7.tar", last modified: Thu Mar 16 06:39:37 2023, max compression
+gzip compressed data, was "RESTApiGen-0.2.0.tar", last modified: Thu Jun  8 14:19:30 2023, max compression
```

## Comparing `RESTApiGen-0.1.7.tar` & `RESTApiGen-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-03-16 06:39:37.947791 RESTApiGen-0.1.7/
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     1065 2022-12-05 11:12:33.000000 RESTApiGen-0.1.7/LICENSE
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4153 2023-03-16 06:39:37.947791 RESTApiGen-0.1.7/PKG-INFO
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     3894 2023-03-16 06:38:14.000000 RESTApiGen-0.1.7/README.md
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       38 2023-03-16 06:39:37.947791 RESTApiGen-0.1.7/setup.cfg
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      837 2023-03-16 06:39:20.000000 RESTApiGen-0.1.7/setup.py
-drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-03-16 06:39:37.947791 RESTApiGen-0.1.7/src/
-drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-03-16 06:39:37.947791 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4153 2023-03-16 06:39:37.000000 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/PKG-INFO
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      274 2023-03-16 06:39:37.000000 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/SOURCES.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)        1 2023-03-16 06:39:37.000000 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/dependency_links.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       47 2023-03-16 06:39:37.000000 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/entry_points.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      130 2023-03-16 06:39:37.000000 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/requires.txt
--rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       11 2023-03-16 06:39:37.000000 RESTApiGen-0.1.7/src/RESTApiGen.egg-info/top_level.txt
--rwxrwxr-x   0 saiyam    (1000) saiyam    (1000)    16364 2023-03-03 16:21:27.000000 RESTApiGen-0.1.7/src/RESTApiGen.py
+drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     1065 2022-12-05 11:12:33.000000 RESTApiGen-0.2.0/LICENSE
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4780 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/PKG-INFO
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4544 2023-06-08 14:17:26.000000 RESTApiGen-0.2.0/README.md
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       38 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/setup.cfg
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      878 2023-06-08 14:17:17.000000 RESTApiGen-0.2.0/setup.py
+drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/src/
+drwxrwxr-x   0 saiyam    (1000) saiyam    (1000)        0 2023-06-08 14:19:30.888755 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)     4780 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/PKG-INFO
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      274 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/SOURCES.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)        1 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/dependency_links.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       47 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/entry_points.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)      130 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/requires.txt
+-rw-rw-r--   0 saiyam    (1000) saiyam    (1000)       11 2023-06-08 14:19:30.000000 RESTApiGen-0.2.0/src/RESTApiGen.egg-info/top_level.txt
+-rwxrwxr-x   0 saiyam    (1000) saiyam    (1000)    27076 2023-06-08 14:10:02.000000 RESTApiGen-0.2.0/src/RESTApiGen.py
```

### Comparing `RESTApiGen-0.1.7/LICENSE` & `RESTApiGen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RESTApiGen-0.1.7/PKG-INFO` & `RESTApiGen-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: RESTApiGen
-Version: 0.1.7
+Version: 0.2.0
 Summary: REST API auto-generator.
 Home-page: https://github.com/Saiyam-J/RESTApiGen
 Author: Saiyam Jain
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Project Description
-RESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it harnesses the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
+ESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
+harnessing the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
 
 # Features
 
 * Makes Models and REST files for each table so its easier to modulate and customize as per the needs.
 * Integrates flask-blueprints and auto registers the models.
 * Accepts requests in the form of application/json and also responds in JSON.
 * Auto-detects one-to-one, one-to-many and many-to-many relationships and creates an application level soft link, even if the SQL tables are not hard indexed.
 * Responds with an entire set of Collection based on the detected relationship, performs a JOIN wherever required, automatically.
+* Supports all data-typed Primary Keys. Your primary keys don't necessarily have to be an integer 'id'.
 * Makes the following REST APIs for each table
   * `GET` LIST : Retrieve all records from a table
   * `POST` COLLECTION : Insert a record into the table
   * `GET` GET : Retrieve a row or an entire Collection from a table
   * `PATCH` PUT : Update a row with newer data in a table
   * `DELETE` PURGE : Performs a delete operation of a row or a collection in a table
 
@@ -53,14 +54,22 @@
 | Argument   | Abbreviation | Usage                            |
 |------------|--------------|----------------------------------|
 | -\-user     | -u           | Enter the username               |
 | -\-password | -p           | Enter the password               |
 | -\-database | -d           | Enter the database name          |
 | -\-host     | -ho          | (Optional) Enter the hostname    |
 | -\-port     | -po          | (Optional) Enter the port number |
+----------------------------
+## List of flags
+| Argument              | Usage                            |
+|-----------------------|----------------------------------|
+| -\-use\-blueprints  |  Makes the back-end files using flask-blueprints and flask-marshmallow        |
+| -\-disbale-foreignkey |  Disables Foreign Key checker and doesnt make relations |
+| -\-only-models |  Just makes the Models, nothing more
+
 --------------------------------------
 
 ## Security Warning
 
 - Commands entered in the terminal can be viewed, in most cases it preserves the history.
 - It is highly recommended that you store the password as an environment variable and only call the environment variable.
 - Since the API Generator cannot access environment variable or identify whether you entered an environment variable name or an actual password, it will consider the literal input as a password.
```

### Comparing `RESTApiGen-0.1.7/README.md` & `RESTApiGen-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Project Description
-RESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it harnesses the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
+RESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
+harnessing the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
 
 # Features
 
 * Makes Models and REST files for each table so its easier to modulate and customize as per the needs.
 * Integrates flask-blueprints and auto registers the models.
 * Accepts requests in the form of application/json and also responds in JSON.
 * Auto-detects one-to-one, one-to-many and many-to-many relationships and creates an application level soft link, even if the SQL tables are not hard indexed.
 * Responds with an entire set of Collection based on the detected relationship, performs a JOIN wherever required, automatically.
+* Supports all data-typed Primary Keys. Your primary keys don't necessarily have to be an integer 'id'.
 * Makes the following REST APIs for each table
   * `GET` LIST : Retrieve all records from a table
   * `POST` COLLECTION : Insert a record into the table
   * `GET` GET : Retrieve a row or an entire Collection from a table
   * `PATCH` PUT : Update a row with newer data in a table
   * `DELETE` PURGE : Performs a delete operation of a row or a collection in a table
 
@@ -42,14 +44,22 @@
 | Argument   | Abbreviation | Usage                            |
 |------------|--------------|----------------------------------|
 | -\-user     | -u           | Enter the username               |
 | -\-password | -p           | Enter the password               |
 | -\-database | -d           | Enter the database name          |
 | -\-host     | -ho          | (Optional) Enter the hostname    |
 | -\-port     | -po          | (Optional) Enter the port number |
+----------------------------
+## List of flags
+| Argument              | Usage                            |
+|-----------------------|----------------------------------|
+| -\-use\-blueprints  |  Makes the back-end files using flask-blueprints and flask-marshmallow        |
+| -\-disbale-foreignkey |  Disables Foreign Key checker and doesnt make relations |
+| -\-only-models |  Just makes the Models, nothing more
+
 --------------------------------------
 
 ## Security Warning
 
 - Commands entered in the terminal can be viewed, in most cases it preserves the history.
 - It is highly recommended that you store the password as an environment variable and only call the environment variable.
 - Since the API Generator cannot access environment variable or identify whether you entered an environment variable name or an actual password, it will consider the literal input as a password.
```

### Comparing `RESTApiGen-0.1.7/setup.py` & `RESTApiGen-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
+long_description = long_description[23:]
 setup(
     name="RESTApiGen",
-    version="0.1.7",
+    version="0.2.0",
     description="REST API auto-generator.",
     url="https://github.com/Saiyam-J/RESTApiGen",
     author="Saiyam Jain",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
```

### Comparing `RESTApiGen-0.1.7/src/RESTApiGen.egg-info/PKG-INFO` & `RESTApiGen-0.2.0/src/RESTApiGen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: RESTApiGen
-Version: 0.1.7
+Version: 0.2.0
 Summary: REST API auto-generator.
 Home-page: https://github.com/Saiyam-J/RESTApiGen
 Author: Saiyam Jain
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Project Description
-RESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it harnesses the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
+ESTAPIGen is a tool that works with an existing SQL database and autogenerates back-end files based on the structure of the SQL. It creates Models that auto-detects the field type. Further, after creating the Models, it makes API routes for each table using the pre-generated Models. It can also use blueprints to make more modulated back-end files by
+harnessing the combined power of flask-blueprint and flask-marshmallow to create APIs around the pre-generated Models. The final result is a fully-working RESTFul API which is ready to be customized. Statistically, 100% of the developers were able to create a kick-starter boilerplate API which saved several days of monotonous coding.
 
 # Features
 
 * Makes Models and REST files for each table so its easier to modulate and customize as per the needs.
 * Integrates flask-blueprints and auto registers the models.
 * Accepts requests in the form of application/json and also responds in JSON.
 * Auto-detects one-to-one, one-to-many and many-to-many relationships and creates an application level soft link, even if the SQL tables are not hard indexed.
 * Responds with an entire set of Collection based on the detected relationship, performs a JOIN wherever required, automatically.
+* Supports all data-typed Primary Keys. Your primary keys don't necessarily have to be an integer 'id'.
 * Makes the following REST APIs for each table
   * `GET` LIST : Retrieve all records from a table
   * `POST` COLLECTION : Insert a record into the table
   * `GET` GET : Retrieve a row or an entire Collection from a table
   * `PATCH` PUT : Update a row with newer data in a table
   * `DELETE` PURGE : Performs a delete operation of a row or a collection in a table
 
@@ -53,14 +54,22 @@
 | Argument   | Abbreviation | Usage                            |
 |------------|--------------|----------------------------------|
 | -\-user     | -u           | Enter the username               |
 | -\-password | -p           | Enter the password               |
 | -\-database | -d           | Enter the database name          |
 | -\-host     | -ho          | (Optional) Enter the hostname    |
 | -\-port     | -po          | (Optional) Enter the port number |
+----------------------------
+## List of flags
+| Argument              | Usage                            |
+|-----------------------|----------------------------------|
+| -\-use\-blueprints  |  Makes the back-end files using flask-blueprints and flask-marshmallow        |
+| -\-disbale-foreignkey |  Disables Foreign Key checker and doesnt make relations |
+| -\-only-models |  Just makes the Models, nothing more
+
 --------------------------------------
 
 ## Security Warning
 
 - Commands entered in the terminal can be viewed, in most cases it preserves the history.
 - It is highly recommended that you store the password as an environment variable and only call the environment variable.
 - Since the API Generator cannot access environment variable or identify whether you entered an environment variable name or an actual password, it will consider the literal input as a password.
```

