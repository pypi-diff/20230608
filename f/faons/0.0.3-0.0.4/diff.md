# Comparing `tmp/faons-0.0.3.tar.gz` & `tmp/faons-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faons-0.0.3.tar", last modified: Wed Jun  7 07:58:07 2023, max compression
+gzip compressed data, was "faons-0.0.4.tar", last modified: Thu Jun  8 11:54:06 2023, max compression
```

## Comparing `faons-0.0.3.tar` & `faons-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 07:58:07.591930 faons-0.0.3/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     1716 2023-06-07 07:58:07.588931 faons-0.0.3/PKG-INFO
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     1609 2023-06-07 07:50:27.000000 faons-0.0.3/README.md
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 07:58:07.352971 faons-0.0.3/faons/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:06.000000 faons-0.0.3/faons/__init__.py
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     5748 2023-06-07 07:57:58.000000 faons-0.0.3/faons/cli.py
-drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 07:58:07.560032 faons-0.0.3/faons.egg-info/
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)     1716 2023-06-07 07:58:06.000000 faons-0.0.3/faons.egg-info/PKG-INFO
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      225 2023-06-07 07:58:07.000000 faons-0.0.3/faons.egg-info/SOURCES.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        1 2023-06-07 07:58:06.000000 faons-0.0.3/faons.egg-info/dependency_links.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       42 2023-06-07 07:58:06.000000 faons-0.0.3/faons.egg-info/entry_points.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       61 2023-06-07 07:58:06.000000 faons-0.0.3/faons.egg-info/requires.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)        6 2023-06-07 07:58:06.000000 faons-0.0.3/faons.egg-info/top_level.txt
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)       38 2023-06-07 07:58:07.592929 faons-0.0.3/setup.cfg
--rwxrwxrwx   0 anandu    (1000) anandu    (1000)      585 2023-06-07 07:57:45.000000 faons-0.0.3/setup.py
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-08 11:54:06.122762 faons-0.0.4/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2113 2023-06-08 11:54:06.120790 faons-0.0.4/PKG-INFO
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2009 2023-06-08 11:53:54.000000 faons-0.0.4/README.md
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-08 11:54:05.920441 faons-0.0.4/faons/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-07 04:50:06.000000 faons-0.0.4/faons/__init__.py
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)    10899 2023-06-08 11:48:24.000000 faons-0.0.4/faons/cli.py
+drwxrwxrwx   0 anandu    (1000) anandu    (1000)        0 2023-06-08 11:54:06.098754 faons-0.0.4/faons.egg-info/
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)     2113 2023-06-08 11:54:05.000000 faons-0.0.4/faons.egg-info/PKG-INFO
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      225 2023-06-08 11:54:05.000000 faons-0.0.4/faons.egg-info/SOURCES.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        1 2023-06-08 11:54:05.000000 faons-0.0.4/faons.egg-info/dependency_links.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       42 2023-06-08 11:54:05.000000 faons-0.0.4/faons.egg-info/entry_points.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       61 2023-06-08 11:54:05.000000 faons-0.0.4/faons.egg-info/requires.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)        6 2023-06-08 11:54:05.000000 faons-0.0.4/faons.egg-info/top_level.txt
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)       38 2023-06-08 11:54:06.125349 faons-0.0.4/setup.cfg
+-rwxrwxrwx   0 anandu    (1000) anandu    (1000)      585 2023-06-08 10:36:29.000000 faons-0.0.4/setup.py
```

### Comparing `faons-0.0.3/PKG-INFO` & `faons-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-Metadata-Version: 2.1
-Name: faons
-Version: 0.0.3
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Welcome to Fast API on Steroids(FAONS)!
-
-Hi! we have created faons to help those who are struggling to setup a base project for fast api with swagger ui. My team used to either copy paste or create manually the files and folders necessary for fast api. But with this package anyone can easily start a fast api project.
-
-
-## Installing
-
-Use the command `pip install faons` to install the latest version of faons in your environment.
-
-## Creating your first project
-
-Once the package has been installed you can create your first project using the command `faons intializeproject <project_name>`.
-
-## File structure
-
-All your files and folders are created as per the below representation
-```markdown
-├── src
-│   ├── config
-│   │   ├── config.py
-|   |   └── constants.py
-│   ├── core
-│   ├── logger
-├── conf
-│   ├── __init__.py
-│   ├── env.conf
-├── utils.py
-├── settings.py
-├── main.py 
-└── README.md
-```
-
-The `main.py` file will be responsible for running your application. The `settings.py` file will be used for including the settings (eg: database connections) for the application. The `utils.py` contains the necessary utilities to run the application.
-
-## Creating you first app for your project
-
-FAONS inherit the idea of creating apps from Django. We will be creating different apps to separate different modules in our application. We can create apps by using the command `faons startapp <app_name>` . Once done the app folder will be created inside the `src/core` folder.
-
-
+# Welcome to Fast API on Steroids(FAONS)!
+
+Hi! we have created faons to help those who are struggling to setup a base project for fast api with swagger ui. My team used to either copy paste or create manually the files and folders necessary for fast api. But with this package anyone can easily start a fast api project.
+
+
+## Installing
+
+Use the command `pip install faons` to install the latest version of faons in your environment.
+
+## Creating your first project
+
+Once the package has been installed you can create your first project using the command `faons intializeproject <project_name>`.
+
+## File structure
+
+All your files and folders are created as per the below representation
+```markdown
+├── src
+│   ├── config
+│   │   ├── config.py
+|   |   └── constants.py
+│   ├── core
+│   ├── logger
+├── conf
+│   ├── __init__.py
+│   ├── env.conf
+├── utils.py
+├── settings.py
+├── main.py 
+└── README.md
+```
+
+The `main.py` file will be responsible for running your application. The `settings.py` file will be used for including the settings (eg: database connections) for the application. The `utils.py` contains the necessary utilities to run the application.
+
+## Creating you first app for your project
+
+FAONS inherit the idea of creating apps from Django. We will be creating different apps to separate different modules in our application. We can create apps by using the command `faons startapp <app_name>` . Once done the app folder will be created inside the `src/core` folder.
+
+## Updating your schema to the DB
+
+One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps.
```

### Comparing `faons-0.0.3/faons.egg-info/PKG-INFO` & `faons-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faons
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Welcome to Fast API on Steroids(FAONS)!
 
@@ -40,8 +40,11 @@
 
 The `main.py` file will be responsible for running your application. The `settings.py` file will be used for including the settings (eg: database connections) for the application. The `utils.py` contains the necessary utilities to run the application.
 
 ## Creating you first app for your project
 
 FAONS inherit the idea of creating apps from Django. We will be creating different apps to separate different modules in our application. We can create apps by using the command `faons startapp <app_name>` . Once done the app folder will be created inside the `src/core` folder.
 
+## Updating your schema to the DB
+
+One useful feature that we missed while coming from django to fastapi was that it lacked the feature to migrate the schema to its db easily. With faons v 0.0.4 we included a function do exactly the same thing. You can use the command `faons updateschema` which will create, alter or drop tables based on the changes that you make to the `schema.py` in the apps.
```

### Comparing `faons-0.0.3/setup.py` & `faons-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faons',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'faons = faons.cli:faons'
         ]
```

