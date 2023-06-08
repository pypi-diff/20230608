# Comparing `tmp/py-centrometal-web-boiler-0.0.52.tar.gz` & `tmp/py-centrometal-web-boiler-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-centrometal-web-boiler-0.0.52.tar", last modified: Tue Mar  7 10:50:11 2023, max compression
+gzip compressed data, was "py-centrometal-web-boiler-0.0.53.tar", last modified: Thu Jun  8 19:41:22 2023, max compression
```

## Comparing `py-centrometal-web-boiler-0.0.52.tar` & `py-centrometal-web-boiler-0.0.53.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.664235 py-centrometal-web-boiler-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-07 10:50:11.664235 py-centrometal-web-boiler-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-07 10:50:11.668235 py-centrometal-web-boiler-0.0.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.656235 py-centrometal-web-boiler-0.0.52/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.660235 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/HttpClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/HttpHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/WebBoilerClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/WebBoilerDeviceCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/WebBoilerWsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.660235 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.660235 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/exceptions/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/exceptions/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.664235 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/models/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/models/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.664235 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/utils/typing_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.664235 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/wsprotocols/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/wsprotocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/wsprotocols/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-07 10:49:59.000000 py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/wsprotocols/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 10:50:11.664235 py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-07 10:50:11.000000 py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-07 10:50:11.000000 py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 10:50:11.000000 py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-07 10:50:11.000000 py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-07 10:50:11.000000 py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.106117 py-centrometal-web-boiler-0.0.53/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.106117 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/HttpClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/HttpHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/WebBoilerClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/WebBoilerDeviceCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/WebBoilerWsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.106117 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.106117 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/exceptions/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/exceptions/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/models/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/utils/typing_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/wsprotocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/wsprotocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/wsprotocols/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 19:41:10.000000 py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/wsprotocols/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:41:22.110117 py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 19:41:22.000000 py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-08 19:41:22.000000 py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:41:22.000000 py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 19:41:22.000000 py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 19:41:22.000000 py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/top_level.txt
```

### Comparing `py-centrometal-web-boiler-0.0.52/LICENSE` & `py-centrometal-web-boiler-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/PKG-INFO` & `py-centrometal-web-boiler-0.0.53/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-centrometal-web-boiler
-Version: 0.0.52
+Version: 0.0.53
 Summary: Python library to interact with Centrometal Boiler System.
 Home-page: https://github.com/9a4gl/py-centrometal-web-boiler
 Author: Tihomir Heidelberg
 Author-email: tihomir.heidelberg@lite.hr
 Project-URL: Bug Tracker, https://github.com/9a4gl/py-centrometal-web-boiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `py-centrometal-web-boiler-0.0.52/README.md` & `py-centrometal-web-boiler-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/setup.cfg` & `py-centrometal-web-boiler-0.0.53/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-centrometal-web-boiler
-version = 0.0.52
+version = 0.0.53
 author = Tihomir Heidelberg
 author_email = tihomir.heidelberg@lite.hr
 description = Python library to interact with Centrometal Boiler System.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/9a4gl/py-centrometal-web-boiler
 project_urls =
```

### Comparing `py-centrometal-web-boiler-0.0.52/setup.py` & `py-centrometal-web-boiler-0.0.53/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
    name='py-centrometal-web-boiler',
-   version='0.0.52',
+   version='0.0.53',
    description='Python library to interact with Centrometal Boiler System.',
    author='Tihomir Heidelberg',
    author_email='tihomir.heidelberg@lite.hr',
    packages=['centrometal_web_boiler', 'centrometal_web_boiler.ws', 'centrometal_web_boiler.ws.exceptions', 'centrometal_web_boiler.ws.models', 'centrometal_web_boiler.ws.utils', 'centrometal_web_boiler.ws.wsprotocols'],
    url="https://github.com/9a4gl/py-centrometal-web-boiler",
    install_requires=[ "lxml>=4.9.1", "websockets>=10.3", "stomper>=0.4.3",
                       "aiohttp>=3.8.1", "faust-cchardet>=2.1.8", "aiodns>=3.0.0"]
```

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/HttpClient.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/HttpClient.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/HttpHelper.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/HttpHelper.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/WebBoilerClient.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/WebBoilerClient.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/WebBoilerDeviceCollection.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/WebBoilerDeviceCollection.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/WebBoilerWsClient.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/WebBoilerWsClient.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/__init__.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/base.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/base.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/client.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,79 +4,129 @@
 from websockets import ConnectionClosedError
 
 from .base import BaseSocket
 from .models import Message, Object
 from .wsprotocols import WSCProtocol
 from .collector import EventCollector
 
+
 class ClientSocket(BaseSocket):
     def __init__(self):
         super().__init__()
-        self.listeners['message'].append(self.on_message)
-        self.listeners['connect'].append(self.on_connect)
-        self.listeners['disconnect'].append(self.on_disconnect)
+        self.listeners["message"].append(self.on_message)
+        self.listeners["connect"].append(self.on_connect)
+        self.listeners["disconnect"].append(self.on_disconnect)
         self.listeners.close.append(self.on_close)
         self.connection = None
         self.disconnection = None
+
     def connect(self, uri: str, **kwargs):
         kwargs.pop("create_protocol", None)
         self.loop.run_until_complete(self.__main(uri, **kwargs))
         self.loop.run_forever()
+
     async def on_message(self, message):
         pass
+
     async def __message_consumer(self):
         try:
             async for message in self.connection:
                 try:
                     data = json.loads(message)
                 except JSONDecodeError:
                     data = message
-                message_cls: Message = Message(data=data, websocket=self.connection, created_at=datetime.utcnow())
-                self.loop.create_task(asyncio.wait(
-                    [coro(message_cls) for coro in self.listeners['message']]+[self.__collector_verifier(futures, 'message', message_cls) 
-                     for futures in self.listeners.message_collector
-                    ]
-                ))
+                message_cls: Message = Message(
+                    data=data, websocket=self.connection, created_at=datetime.utcnow()
+                )
+                async with asyncio.TaskGroup() as tg:
+                    for coro in self.listeners["message"]:
+                        tg.create_task(coro(message_cls))
+                    for futures in self.listeners.message_collector:
+                        tg.create_task(
+                            self.__collector_verifier(futures, "message", message_cls)
+                        )
         except ConnectionClosedError as e:
-            self.disconnection = Object({'code': e.code, 'reason': e.reason, 'disconnected': True})
-            self.loop.create_task(asyncio.wait([coro(e.code, e.reason) for coro in self.listeners.disconnect]+[
-                     self.__collector_verifier(futures, 'disconnect', e.code, e.reason) 
-                     for futures in self.listeners.disconnect_collector
+            self.disconnection = Object(
+                {"code": e.code, "reason": e.reason, "disconnected": True}
+            )
+            self.loop.create_task(
+                asyncio.wait(
+                    [coro(e.code, e.reason) for coro in self.listeners.disconnect]
+                    + [
+                        self.__collector_verifier(
+                            futures, "disconnect", e.code, e.reason
+                        )
+                        for futures in self.listeners.disconnect_collector
                     ]
-            ))
+                )
+            )
             return e
+
     async def __on_connect(self):
-        await asyncio.wait([coro() for coro in self.listeners['connect']])
+        async with asyncio.TaskGroup() as tg:
+            for coro in self.listeners["connect"]:
+                tg.create_task(coro())
+
     async def on_connect(self):
         pass
+
     async def on_disconnect(self, code, reason):
         pass
+
     async def on_close(self, code, reason):
         pass
+
     async def __collector_verifier(self, futures, event, *event_data):
         if futures[1](*event_data):
             try:
-                futures[0].set_result(event_data[0] if len(event_data) == 1 else event_data)
+                futures[0].set_result(
+                    event_data[0] if len(event_data) == 1 else event_data
+                )
                 self.listeners[f"{event}_collector"].remove(futures)
             except asyncio.exceptions.InvalidStateError:
                 try:
                     self.listeners[f"{event}_collector"].remove(futures)
                 except ValueError:
                     pass
             except ValueError:
                 pass
+
     def collector(self, time: float):
         return EventCollector(websocket=self, time=time)
+
     async def __main(self, uri, **kwargs):
-        self.connection = await websockets.connect(uri, create_protocol=WSCProtocol, **kwargs)
-        self.loop.create_task(self.__on_connect())
-        done, pending = await asyncio.wait([self.__message_consumer()], return_when=asyncio.ALL_COMPLETED)
-        if ConnectionClosedError in [type(ret.result()) for ret in done]: return
-        self.disconnection = Object({'code': self.connection.close_code, 'reason': self.connection.close_reason, 'disconnected': True})
-        await asyncio.wait([coro(self.connection.close_code, self.connection.close_reason) for coro in self.listeners.close]+[
-                     self.__collector_verifier(futures, 'close', self.connection.close_code, self.connection.close_reason) 
-                     for futures in self.listeners.close_collector
-                    ])
+        self.connection = await websockets.connect(
+            uri, create_protocol=WSCProtocol, **kwargs
+        )
+        async with asyncio.TaskGroup() as tg:
+            tg.create_task(self.__on_connect())
+        done, pending = await asyncio.wait_for(self.__message_consumer(), timeout=None)
+        if ConnectionClosedError in [type(ret.result()) for ret in done]:
+            return
+        self.disconnection = Object(
+            {
+                "code": self.connection.close_code,
+                "reason": self.connection.close_reason,
+                "disconnected": True,
+            }
+        )
+        await asyncio.wait(
+            [
+                coro(self.connection.close_code, self.connection.close_reason)
+                for coro in self.listeners.close
+            ]
+            + [
+                self.__collector_verifier(
+                    futures,
+                    "close",
+                    self.connection.close_code,
+                    self.connection.close_reason,
+                )
+                for futures in self.listeners.close_collector
+            ]
+        )
+
     async def send(self, content: typing.Any = None, *, data: dict = None):
         await self.connection.send(content=content, data=data)
-    async def close(self, code: int = 1000, reason: str = ''):
+
+    async def close(self, code: int = 1000, reason: str = ""):
         await self.connection.close(code=code, reason=reason)
```

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/collector.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/collector.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/models/data.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/models/data.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/models/message.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/models/message.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/server.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/server.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/utils/typing_checking.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/utils/typing_checking.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/wsprotocols/client.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/wsprotocols/client.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/centrometal_web_boiler/ws/wsprotocols/server.py` & `py-centrometal-web-boiler-0.0.53/src/centrometal_web_boiler/ws/wsprotocols/server.py`

 * *Files identical despite different names*

### Comparing `py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/PKG-INFO` & `py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-centrometal-web-boiler
-Version: 0.0.52
+Version: 0.0.53
 Summary: Python library to interact with Centrometal Boiler System.
 Home-page: https://github.com/9a4gl/py-centrometal-web-boiler
 Author: Tihomir Heidelberg
 Author-email: tihomir.heidelberg@lite.hr
 Project-URL: Bug Tracker, https://github.com/9a4gl/py-centrometal-web-boiler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `py-centrometal-web-boiler-0.0.52/src/py_centrometal_web_boiler.egg-info/SOURCES.txt` & `py-centrometal-web-boiler-0.0.53/src/py_centrometal_web_boiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

