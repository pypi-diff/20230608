# Comparing `tmp/maap_jupyter_server_extension-1.0.1.tar.gz` & `tmp/maap_jupyter_server_extension-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maap_jupyter_server_extension-1.0.1.tar", last modified: Mon Jun  5 22:16:31 2023, max compression
+gzip compressed data, was "maap_jupyter_server_extension-1.1.0.tar", last modified: Thu Jun  8 15:57:37 2023, max compression
```

## Comparing `maap_jupyter_server_extension-1.0.1.tar` & `maap_jupyter_server_extension-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.376349 maap_jupyter_server_extension-1.0.1/
--rw-r--r--   0 mlucas     (502) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/CHANGELOG.md
--rw-r--r--   0 mlucas     (502) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.0.1/LICENSE
--rw-r--r--   0 mlucas     (502) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.0.1/MANIFEST.in
--rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-05 22:16:31.376021 maap_jupyter_server_extension-1.0.1/PKG-INFO
--rw-r--r--   0 mlucas     (502) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.0.1/README.md
--rw-r--r--   0 mlucas     (502) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.0.1/conftest.py
--rw-r--r--   0 mlucas     (502) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.0.1/install.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.347484 maap_jupyter_server_extension-1.0.1/jupyter-config/
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.355713 maap_jupyter_server_extension-1.0.1/jupyter-config/nb-config/
--rw-r--r--   0 mlucas     (502) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.0.1/jupyter-config/nb-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.356643 maap_jupyter_server_extension-1.0.1/jupyter-config/server-config/
--rw-r--r--   0 mlucas     (502) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.0.1/jupyter-config/server-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.359655 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/
--rw-r--r--   0 mlucas     (502) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/__init__.py
--rw-r--r--   0 mlucas     (502) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/_version.py
--rw-r--r--   0 mlucas     (502) staff       (20)    22639 2023-06-05 20:49:32.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/handlers.py
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.361130 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/
--rw-r--r--   0 mlucas     (502) staff       (20)     2885 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/package.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.369512 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/
--rw-r--r--   0 mlucas     (502) staff       (20)     3524 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/747.4ce08d0080c49e3989d8.js
--rw-r--r--   0 mlucas     (502) staff       (20)      904 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/763.c8afe390b9ba053ca78e.js
--rw-r--r--   0 mlucas     (502) staff       (20)     6490 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/remoteEntry.fbf9e31991f55b086f94.js
--rw-r--r--   0 mlucas     (502) staff       (20)      167 2023-06-05 22:08:15.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/style.js
--rw-r--r--   0 mlucas     (502) staff       (20)     2452 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.372658 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/
--rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/PKG-INFO
--rw-r--r--   0 mlucas     (502) staff       (20)     1154 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/SOURCES.txt
--rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/dependency_links.txt
--rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-05 22:16:30.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/not-zip-safe
--rw-r--r--   0 mlucas     (502) staff       (20)       88 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/requires.txt
--rw-r--r--   0 mlucas     (502) staff       (20)       25 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/top_level.txt
--rw-r--r--   0 mlucas     (502) staff       (20)     2748 2023-06-05 22:12:27.000000 maap_jupyter_server_extension-1.0.1/package.json
--rw-r--r--   0 mlucas     (502) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.0.1/pyproject.toml
--rw-r--r--   0 mlucas     (502) staff       (20)       38 2023-06-05 22:16:31.376452 maap_jupyter_server_extension-1.0.1/setup.cfg
--rw-r--r--   0 mlucas     (502) staff       (20)     3431 2023-06-05 22:15:51.000000 maap_jupyter_server_extension-1.0.1/setup.py
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.373703 maap_jupyter_server_extension-1.0.1/src/
--rw-r--r--   0 mlucas     (502) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.0.1/src/handler.ts
--rw-r--r--   0 mlucas     (502) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.0.1/src/index.ts
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.375504 maap_jupyter_server_extension-1.0.1/style/
--rw-r--r--   0 mlucas     (502) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/style/base.css
--rw-r--r--   0 mlucas     (502) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/style/index.css
--rw-r--r--   0 mlucas     (502) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/style/index.js
--rw-r--r--   0 mlucas     (502) staff       (20)      669 2023-06-05 20:12:23.000000 maap_jupyter_server_extension-1.0.1/tsconfig.json
--rw-r--r--   0 mlucas     (502) staff       (20)   223606 2023-06-05 22:07:59.000000 maap_jupyter_server_extension-1.0.1/yarn.lock
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:37.000452 maap_jupyter_server_extension-1.1.0/
+-rw-r--r--   0 mlucas     (502) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/CHANGELOG.md
+-rw-r--r--   0 mlucas     (502) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.1.0/LICENSE
+-rw-r--r--   0 mlucas     (502) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.1.0/MANIFEST.in
+-rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-08 15:57:36.999711 maap_jupyter_server_extension-1.1.0/PKG-INFO
+-rw-r--r--   0 mlucas     (502) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.1.0/README.md
+-rw-r--r--   0 mlucas     (502) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.1.0/conftest.py
+-rw-r--r--   0 mlucas     (502) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.1.0/install.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.969290 maap_jupyter_server_extension-1.1.0/jupyter-config/
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.976730 maap_jupyter_server_extension-1.1.0/jupyter-config/nb-config/
+-rw-r--r--   0 mlucas     (502) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.1.0/jupyter-config/nb-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.977435 maap_jupyter_server_extension-1.1.0/jupyter-config/server-config/
+-rw-r--r--   0 mlucas     (502) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.1.0/jupyter-config/server-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.980002 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/
+-rw-r--r--   0 mlucas     (502) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/__init__.py
+-rw-r--r--   0 mlucas     (502) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/_version.py
+-rw-r--r--   0 mlucas     (502) staff       (20)    23457 2023-06-07 23:49:22.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/handlers.py
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.982735 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/
+-rw-r--r--   0 mlucas     (502) staff       (20)    21024 2023-06-08 15:54:52.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/build_log.json
+-rw-r--r--   0 mlucas     (502) staff       (20)     2890 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/package.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.992518 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/
+-rw-r--r--   0 mlucas     (502) staff       (20)     3775 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     2459 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/lib_index_js.f3563370867954312194.js.map
+-rw-r--r--   0 mlucas     (502) staff       (20)    28001 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/remoteEntry.38858848937d208638ab.js
+-rw-r--r--   0 mlucas     (502) staff       (20)    26958 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/remoteEntry.38858848937d208638ab.js.map
+-rw-r--r--   0 mlucas     (502) staff       (20)      172 2023-06-08 15:54:52.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/style.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     4630 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     1832 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/style_index_js.985542941dd18f4568ee.js.map
+-rw-r--r--   0 mlucas     (502) staff       (20)    12088 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js
+-rw-r--r--   0 mlucas     (502) staff       (20)    13835 2023-06-08 15:54:53.000000 maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.265412ff30d319ce76fc.js.map
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.995221 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/
+-rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/PKG-INFO
+-rw-r--r--   0 mlucas     (502) staff       (20)     1749 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-08 15:53:58.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/not-zip-safe
+-rw-r--r--   0 mlucas     (502) staff       (20)       88 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/requires.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)       25 2023-06-08 15:57:36.000000 maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/top_level.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)     2748 2023-06-08 15:52:14.000000 maap_jupyter_server_extension-1.1.0/package.json
+-rw-r--r--   0 mlucas     (502) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.1.0/pyproject.toml
+-rw-r--r--   0 mlucas     (502) staff       (20)       38 2023-06-08 15:57:37.000623 maap_jupyter_server_extension-1.1.0/setup.cfg
+-rw-r--r--   0 mlucas     (502) staff       (20)     3431 2023-06-05 22:15:51.000000 maap_jupyter_server_extension-1.1.0/setup.py
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.996418 maap_jupyter_server_extension-1.1.0/src/
+-rw-r--r--   0 mlucas     (502) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.1.0/src/handler.ts
+-rw-r--r--   0 mlucas     (502) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.1.0/src/index.ts
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-08 15:57:36.998636 maap_jupyter_server_extension-1.1.0/style/
+-rw-r--r--   0 mlucas     (502) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/style/base.css
+-rw-r--r--   0 mlucas     (502) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/style/index.css
+-rw-r--r--   0 mlucas     (502) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.1.0/style/index.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      669 2023-06-05 20:12:23.000000 maap_jupyter_server_extension-1.1.0/tsconfig.json
```

### Comparing `maap_jupyter_server_extension-1.0.1/LICENSE` & `maap_jupyter_server_extension-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/MANIFEST.in` & `maap_jupyter_server_extension-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/PKG-INFO` & `maap_jupyter_server_extension-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap_jupyter_server_extension
-Version: 1.0.1
+Version: 1.1.0
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `maap_jupyter_server_extension-1.0.1/README.md` & `maap_jupyter_server_extension-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/__init__.py` & `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/_version.py` & `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/_version.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/handlers.py` & `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import functools
 import os
 import xml.etree.ElementTree as ET
 import xmltodict
 import logging
 import requests
 import yaml
+import time
 
 logging.basicConfig(format='%(asctime)s %(message)s')
 
 @functools.lru_cache(maxsize=128)
 def get_maap_config(host):
     print(os.environ)
     path_to_json = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', os.environ['ENVIRONMENTS_FILE_PATH'])
@@ -238,14 +239,31 @@
             print(r)
             self.finish({"status_code": r.status_code, "response": json.dumps(o)})
         except:
             print("Failed job result query.")
             self.finish()
 
 
+class RegisterWithFileHandler(IPythonHandler):
+    def get(self):
+        #maap = MAAP(not_self_signed=False)
+        maap = MAAP(maap_host=maap_api(self.request.host))
+
+        try:
+            config_file = self.get_argument("file")
+            r = maap.register_algorithm_from_yaml_file(config_file)
+            r.raise_for_status()
+            print(r.text)
+            self.finish({"status_code": r.status_code, "response": r.text})
+        except:
+            print("Failed to register.")
+
+
+
+
 
 class GetJobMetricsHandler(IPythonHandler):
     def get(self):
         #maap = MAAP(not_self_signed=False)
         maap = MAAP(maap_host=maap_api(self.request.host))
 
         try:
@@ -552,21 +570,24 @@
 class CreateFileHandler(IPythonHandler):
     def get(self):
 
         file_name = self.get_argument("fileName")
         data = self.get_argument("data")
 
         algo = json.loads(data)
-        print(algo)
 
         try:
             print("Attempting to create file.")
             with open(file_name, 'w') as f:
                 yaml.dump(algo, f)
-                # f.write(yaml.dump(data))
+                file_path = os.getcwd() + '/' + file_name
+                print(file_path)
+                while not os.path.exists(file_path):
+                    time.sleep(1)
+                self.finish({"file": file_path})
         except:
             print("Failed to create file.")
             self.finish()
 
 
 def setup_handlers(web_app):
     host_pattern = ".*$"
@@ -583,14 +604,16 @@
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getCMRCollections"), GetCMRCollectionsHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "listUserJobs"), ListUserJobsHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "submitJob"), SubmitJobHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getJobStatus"), GetJobStatusHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getJobResult"), GetJobResultHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getJobMetrics"), GetJobMetricsHandler)])
 
+    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "registerUsingFile"), RegisterWithFileHandler)])
+
     # USER WORKSPACE MANAGEMENT
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "test"), RouteTestHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "injectPublicKey"), InjectKeyHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "getSSHInfo"), GetSSHInfoHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "getSignedS3Url"), Presigneds3UrlHandler)])
 
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "createFile"), CreateFileHandler)])
```

### Comparing `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/package.json` & `maap_jupyter_server_extension-1.1.0/jupyter_server_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9518849206349206%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.38858848937d208638ab.js'}}",*

 * * "'name'": "'maap-jupyter-server-extension'",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -40,15 +40,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fbf9e31991f55b086f94.js",
+            "load": "static/remoteEntry.38858848937d208638ab.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_server_extension"
                 },
@@ -63,15 +63,15 @@
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "Apache 2.0",
     "main": "lib/index.js",
-    "name": "jupyter-server-extension",
+    "name": "maap-jupyter-server-extension",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/MAAP-Project/jupyter-server-extension.git"
     },
@@ -93,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0"
 }
```

### Comparing `maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/PKG-INFO` & `maap_jupyter_server_extension-1.1.0/maap_jupyter_server_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap-jupyter-server-extension
-Version: 1.0.1
+Version: 1.1.0
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `maap_jupyter_server_extension-1.0.1/package.json` & `maap_jupyter_server_extension-1.1.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.1.0"
 }
```

### Comparing `maap_jupyter_server_extension-1.0.1/pyproject.toml` & `maap_jupyter_server_extension-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/setup.py` & `maap_jupyter_server_extension-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/src/handler.ts` & `maap_jupyter_server_extension-1.1.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/src/index.ts` & `maap_jupyter_server_extension-1.1.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.1/tsconfig.json` & `maap_jupyter_server_extension-1.1.0/tsconfig.json`

 * *Files identical despite different names*

