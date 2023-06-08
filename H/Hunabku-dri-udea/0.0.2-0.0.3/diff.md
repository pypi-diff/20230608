# Comparing `tmp/Hunabku_dri_udea-0.0.2.tar.gz` & `tmp/Hunabku_dri_udea-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_dri_udea-0.0.2.tar", last modified: Tue May 30 21:55:47 2023, max compression
+gzip compressed data, was "Hunabku_dri_udea-0.0.3.tar", last modified: Thu Jun  8 19:28:05 2023, max compression
```

## Comparing `Hunabku_dri_udea-0.0.2.tar` & `Hunabku_dri_udea-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 21:55:47.000000 Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/hunabku_dri_udea/endpoints/dri_udea.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:55:47.253308 Hunabku_dri_udea-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 21:55:31.000000 Hunabku_dri_udea-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:05.707593 Hunabku_dri_udea-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:05.703593 Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 19:28:05.000000 Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 19:28:05.000000 Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:28:05.000000 Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:28:05.000000 Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 19:28:05.000000 Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 19:27:51.000000 Hunabku_dri_udea-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 19:28:05.707593 Hunabku_dri_udea-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 19:27:51.000000 Hunabku_dri_udea-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:05.703593 Hunabku_dri_udea-0.0.3/hunabku_dri_udea/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:27:51.000000 Hunabku_dri_udea-0.0.3/hunabku_dri_udea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 19:27:51.000000 Hunabku_dri_udea-0.0.3/hunabku_dri_udea/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:05.707593 Hunabku_dri_udea-0.0.3/hunabku_dri_udea/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-08 19:27:51.000000 Hunabku_dri_udea-0.0.3/hunabku_dri_udea/endpoints/dri_udea.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:28:05.707593 Hunabku_dri_udea-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-08 19:27:51.000000 Hunabku_dri_udea-0.0.3/setup.py
```

### Comparing `Hunabku_dri_udea-0.0.2/Hunabku_dri_udea.egg-info/PKG-INFO` & `Hunabku_dri_udea-0.0.3/Hunabku_dri_udea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-dri-udea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hunabku plugin from the International Affairs Office of the university of Antioquia
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_dri_udea-0.0.2/PKG-INFO` & `Hunabku_dri_udea-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_dri_udea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hunabku plugin from the International Affairs Office of the university of Antioquia
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_dri_udea-0.0.2/hunabku_dri_udea/endpoints/dri_udea.py` & `Hunabku_dri_udea-0.0.3/hunabku_dri_udea/endpoints/dri_udea.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,34 @@
 
     config += Param(mobility_collection_name="international_mobility",
                     doc="Mongo DB collection")
 
     config += Param(agreements_collection_name="agreements_raw",
                     doc="Mongo DB collection")
 
+    config += Param(apikey="colav",
+                    doc="Plugin API key")
+
     def __init__(self, hunabku):
         super().__init__(hunabku)
         self.dbclient = MongoClient(self.config.db_uri)
         self.db = self.dbclient[self.config.db_name]
         self.mobility_collection = self.db[self.config.mobility_collection_name]
         self.agreements_collection = self.db[self.config.agreements_collection_name]
+        self.apikey = self.config.apikey
+
+    def valid_apikey(self):
+        if self.request.method == 'POST':
+            apikey = self.request.form.get('apikey')
+        else:
+            apikey = self.request.args.get('apikey')
+        if self.apikey == apikey:
+            return True
+        else:
+            return False
 
     @endpoint('/agreements', methods=['GET'])
     def get_agreements(self):
         """
         @api {get} /agreements Agreements records
         @apiName Agreements
         @apiGroup DRI UdeA
```

### Comparing `Hunabku_dri_udea-0.0.2/setup.py` & `Hunabku_dri_udea-0.0.3/setup.py`

 * *Files identical despite different names*

