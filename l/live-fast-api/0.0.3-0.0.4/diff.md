# Comparing `tmp/live-fast-api-0.0.3.tar.gz` & `tmp/live-fast-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live-fast-api-0.0.3.tar", last modified: Fri Apr 21 18:20:26 2023, max compression
+gzip compressed data, was "live-fast-api-0.0.4.tar", last modified: Thu Jun  8 10:00:52 2023, max compression
```

## Comparing `live-fast-api-0.0.3.tar` & `live-fast-api-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.293313 live-fast-api-0.0.3/
--rw-rw-rw-   0        0        0      215 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2054 2023-04-21 18:20:26.293313 live-fast-api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.3/build.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.245331 live-fast-api-0.0.3/live_api/
--rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.3/live_api/__init__.py
--rw-rw-rw-   0        0        0     8981 2023-03-09 10:59:33.000000 live-fast-api-0.0.3/live_api/base.py
--rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.3/live_api/document.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.259317 live-fast-api-0.0.3/live_api/endpoints/
--rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.3/live_api/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.3/live_api/endpoints/data.py
--rw-rw-rw-   0        0        0    10624 2023-04-15 12:51:23.000000 live-fast-api-0.0.3/live_api/endpoints/engine.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.3/live_api/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.3/live_api/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.271314 live-fast-api-0.0.3/live_api/service/
--rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.3/live_api/service/__init__.py
--rw-rw-rw-   0        0        0    17698 2023-04-15 12:53:17.000000 live-fast-api-0.0.3/live_api/service/rest.py
--rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.3/live_api/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.224308 live-fast-api-0.0.3/live_api/source/
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.224308 live-fast-api-0.0.3/live_api/source/assets/
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.277311 live-fast-api-0.0.3/live_api/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.3/live_api/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.3/live_api/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-04-21 18:20:26.292312 live-fast-api-0.0.3/live_fast_api.egg-info/
--rw-rw-rw-   0        0        0     2054 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/live_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/live_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/live_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/live_fast_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/live_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      172 2023-04-21 18:20:26.000000 live-fast-api-0.0.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       91 2023-04-21 18:18:24.000000 live-fast-api-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 18:20:26.293313 live-fast-api-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1580 2023-04-21 18:19:54.000000 live-fast-api-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:52.724998 live-fast-api-0.0.4/
+-rw-rw-rw-   0        0        0      215 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2054 2023-06-08 10:00:52.724998 live-fast-api-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-04-12 14:06:13.000000 live-fast-api-0.0.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 live-fast-api-0.0.4/build.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:52.340999 live-fast-api-0.0.4/live_api/
+-rw-rw-rw-   0        0        0      493 2023-03-09 10:59:51.000000 live-fast-api-0.0.4/live_api/__init__.py
+-rw-rw-rw-   0        0        0     8981 2023-06-07 10:02:06.000000 live-fast-api-0.0.4/live_api/base.py
+-rw-rw-rw-   0        0        0      281 2023-04-12 14:23:43.000000 live-fast-api-0.0.4/live_api/document.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:52.599002 live-fast-api-0.0.4/live_api/endpoints/
+-rw-rw-rw-   0        0        0      182 2023-04-12 14:16:43.000000 live-fast-api-0.0.4/live_api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-04-12 14:12:33.000000 live-fast-api-0.0.4/live_api/endpoints/data.py
+-rw-rw-rw-   0        0        0    10624 2023-04-15 12:51:23.000000 live-fast-api-0.0.4/live_api/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 live-fast-api-0.0.4/live_api/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1601 2023-04-12 14:15:29.000000 live-fast-api-0.0.4/live_api/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:52.611000 live-fast-api-0.0.4/live_api/service/
+-rw-rw-rw-   0        0        0       92 2023-04-12 14:22:24.000000 live-fast-api-0.0.4/live_api/service/__init__.py
+-rw-rw-rw-   0        0        0    17838 2023-06-08 09:59:10.000000 live-fast-api-0.0.4/live_api/service/rest.py
+-rw-rw-rw-   0        0        0     2991 2023-04-21 18:19:24.000000 live-fast-api-0.0.4/live_api/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:51.957000 live-fast-api-0.0.4/live_api/source/
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:51.958000 live-fast-api-0.0.4/live_api/source/assets/
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:52.619000 live-fast-api-0.0.4/live_api/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-02-04 16:41:18.000000 live-fast-api-0.0.4/live_api/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-02-04 16:40:24.000000 live-fast-api-0.0.4/live_api/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:52.723998 live-fast-api-0.0.4/live_fast_api.egg-info/
+-rw-rw-rw-   0        0        0     2054 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/live_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      641 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/live_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/live_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/live_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/live_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-06-08 10:00:51.000000 live-fast-api-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-04-21 18:21:15.000000 live-fast-api-0.0.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       91 2023-04-21 18:18:24.000000 live-fast-api-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:00:52.725998 live-fast-api-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-06-08 10:00:40.000000 live-fast-api-0.0.4/setup.py
```

### Comparing `live-fast-api-0.0.3/PKG-INFO` & `live-fast-api-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.3/README.md` & `live-fast-api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/build.py` & `live-fast-api-0.0.4/build.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/base.py` & `live-fast-api-0.0.4/live_api/base.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/endpoints/data.py` & `live-fast-api-0.0.4/live_api/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/endpoints/engine.py` & `live-fast-api-0.0.4/live_api/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/endpoints/exceptions.py` & `live-fast-api-0.0.4/live_api/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/endpoints/process.py` & `live-fast-api-0.0.4/live_api/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/service/rest.py` & `live-fast-api-0.0.4/live_api/service/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,44 +596,48 @@
     def terminate(self) -> None:
         """Pauses the process of service."""
 
         if not self.running():
             return
         # end if
 
-        terminate_thread(self.service_process)
+        if isinstance(self.service_process, threading.Thread):
+            terminate_thread(self.service_process)
+
+            self.service_process = None
+        # end if
     # end terminate
 
     def running(self) -> bool:
         """
         Checks if the service is currently running.
 
         :return: The boolean value.
         """
 
-        if self.service_process is None:
+        if self.created:
             return False
         # end if
 
         return self.service_process.is_alive()
     # end running
 
     def built(self) -> bool:
         """
         Checks if the service was built.
 
         :return: The value for the service being built.
         """
 
-        return self.app is not None
+        return isinstance(self.app, FastAPI)
     # end built
 
     def created(self) -> bool:
         """
         Checks if the service was created.
 
         :return: The value for the service being created.
         """
 
-        return self.service_process is not None
+        return isinstance(self.service_process, threading.Thread)
     # end created
 # end BaseService
```

### Comparing `live-fast-api-0.0.3/live_api/service/sockets.py` & `live-fast-api-0.0.4/live_api/service/sockets.py`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/source/assets/icon/icon.ico` & `live-fast-api-0.0.4/live_api/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_api/source/assets/icon/icon.png` & `live-fast-api-0.0.4/live_api/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/live_fast_api.egg-info/PKG-INFO` & `live-fast-api-0.0.4/live_fast_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: live-fast-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/live-api
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `live-fast-api-0.0.3/live_fast_api.egg-info/SOURCES.txt` & `live-fast-api-0.0.4/live_fast_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `live-fast-api-0.0.3/pyproject.toml` & `live-fast-api-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'live-fast-api'
-version = '0.0.3'
+version = '0.0.4'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `live-fast-api-0.0.3/setup.py` & `live-fast-api-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "live_api/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='live-fast-api',
-        version='0.0.3',
+        version='0.0.4',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

