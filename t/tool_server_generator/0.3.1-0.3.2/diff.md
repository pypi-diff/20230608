# Comparing `tmp/tool_server_generator-0.3.1.tar.gz` & `tmp/tool_server_generator-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_server_generator-0.3.1.tar", last modified: Thu Jun  8 16:04:37 2023, max compression
+gzip compressed data, was "tool_server_generator-0.3.2.tar", last modified: Thu Jun  8 16:05:44 2023, max compression
```

## Comparing `tool_server_generator-0.3.1.tar` & `tool_server_generator-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.3.1/LICENSE
--rwxr-xr-x   0        0        0      669 2023-06-07 18:45:05.137872 tool_server_generator-0.3.1/config_server.txt
--rwxr-xr-x   0        0        0      529 2023-06-08 16:03:12.030301 tool_server_generator-0.3.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-05 17:15:32.717658 tool_server_generator-0.3.1/readme.md
--rwxr-xr-x   0        0        0     2022 2023-06-08 16:04:34.281751 tool_server_generator-0.3.1/tool_server_generator/__init__.py
--rwxr-xr-x   0        0        0      669 2023-06-07 18:37:38.465184 tool_server_generator-0.3.1/tool_server_generator/config_server.txt
--rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.3.1/tool_server_generator/model/app.js
--rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.3.1/tool_server_generator/model/bin/www
--rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.3.1/tool_server_generator/model/package-lock.json
--rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.3.1/tool_server_generator/model/package.json
--rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.3.1/tool_server_generator/model/public/stylesheets/w3.css
--rwxr-xr-x   0        0        0     1993 2023-06-08 15:45:53.356074 tool_server_generator-0.3.1/tool_server_generator/model/routes/index.js
--rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.3.1/tool_server_generator/model/views/error.pug
--rwxr-xr-x   0        0        0       66 2023-06-05 14:49:43.488782 tool_server_generator-0.3.1/tool_server_generator/model/views/index.pug
--rwxr-xr-x   0        0        0      129 2023-06-05 19:35:26.231973 tool_server_generator-0.3.1/tool_server_generator/model/views/layout.pug
--rwxr-xr-x   0        0        0     1147 2023-06-07 21:08:08.603638 tool_server_generator-0.3.1/tool_server_generator/model/views/requests.pug
--rwxr-xr-x   0        0        0     1312 2023-06-08 15:55:11.225309 tool_server_generator-0.3.1/tool_server_generator/model/workers/process_command.js
--rwxr-xr-x   0        0        0     3708 2023-06-07 21:21:17.735915 tool_server_generator-0.3.1/tool_server_generator/model/workers/request_listener.js
--rwxr-xr-x   0        0        0    11115 2023-06-07 21:26:24.637323 tool_server_generator-0.3.1/tool_server_generator/utils/config_parser.py
--rwxr-xr-x   0        0        0     8320 2023-06-07 22:10:31.767136 tool_server_generator-0.3.1/tool_server_generator/utils/config_server.py
--rwxr-xr-x   0        0        0      679 2023-06-06 13:27:05.444944 tool_server_generator-0.3.1/tool_server_generator/utils/utils.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 tool_server_generator-0.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.3.2/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-06-07 18:45:05.137872 tool_server_generator-0.3.2/config_server.txt
+-rwxr-xr-x   0        0        0      516 2023-06-08 16:05:35.967066 tool_server_generator-0.3.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-05 17:15:32.717658 tool_server_generator-0.3.2/readme.md
+-rwxr-xr-x   0        0        0     2022 2023-06-08 16:05:39.865792 tool_server_generator-0.3.2/tool_server_generator/__init__.py
+-rwxr-xr-x   0        0        0      669 2023-06-07 18:37:38.465184 tool_server_generator-0.3.2/tool_server_generator/config_server.txt
+-rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.3.2/tool_server_generator/model/app.js
+-rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.3.2/tool_server_generator/model/bin/www
+-rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.3.2/tool_server_generator/model/package-lock.json
+-rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.3.2/tool_server_generator/model/package.json
+-rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.3.2/tool_server_generator/model/public/stylesheets/w3.css
+-rwxr-xr-x   0        0        0     1993 2023-06-08 15:45:53.356074 tool_server_generator-0.3.2/tool_server_generator/model/routes/index.js
+-rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.3.2/tool_server_generator/model/views/error.pug
+-rwxr-xr-x   0        0        0       66 2023-06-05 14:49:43.488782 tool_server_generator-0.3.2/tool_server_generator/model/views/index.pug
+-rwxr-xr-x   0        0        0      129 2023-06-05 19:35:26.231973 tool_server_generator-0.3.2/tool_server_generator/model/views/layout.pug
+-rwxr-xr-x   0        0        0     1147 2023-06-07 21:08:08.603638 tool_server_generator-0.3.2/tool_server_generator/model/views/requests.pug
+-rwxr-xr-x   0        0        0     1312 2023-06-08 15:55:11.225309 tool_server_generator-0.3.2/tool_server_generator/model/workers/process_command.js
+-rwxr-xr-x   0        0        0     3708 2023-06-07 21:21:17.735915 tool_server_generator-0.3.2/tool_server_generator/model/workers/request_listener.js
+-rwxr-xr-x   0        0        0    11115 2023-06-07 21:26:24.637323 tool_server_generator-0.3.2/tool_server_generator/utils/config_parser.py
+-rwxr-xr-x   0        0        0     8320 2023-06-07 22:10:31.767136 tool_server_generator-0.3.2/tool_server_generator/utils/config_server.py
+-rwxr-xr-x   0        0        0      679 2023-06-06 13:27:05.444944 tool_server_generator-0.3.2/tool_server_generator/utils/utils.py
+-rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 tool_server_generator-0.3.2/PKG-INFO
```

### Comparing `tool_server_generator-0.3.1/LICENSE` & `tool_server_generator-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/config_server.txt` & `tool_server_generator-0.3.2/config_server.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/pyproject.toml` & `tool_server_generator-0.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 
 [project]
 name = "tool_server_generator"
 authors = [{name = "brazafonso", email = "a93178@uminho.pt"},{name = "Tiago Silva", email = "a93277@uminho.pt"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
-dependencies = ["lark","argparse","subprocess"]
+dependencies = ["lark","argparse"]
 readme = "readme.md"
 
 
 [project.scripts]
 ts = "tool_server_generator:tool_server"
```

### Comparing `tool_server_generator-0.3.1/tool_server_generator/__init__.py` & `tool_server_generator-0.3.2/tool_server_generator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 import argparse
 import sys
 from .utils.utils import *
 from .utils.config_parser import *
 from .utils.config_server import *
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 project_dir = os.path.dirname(os.path.realpath(__file__))
 model_server = f'{project_dir}/model'
 
 
 def start_server(server_dir,config):
     '''Inicia o servidor'''
     server_path = f'{os.getcwd()}/{server_dir}'
```

### Comparing `tool_server_generator-0.3.1/tool_server_generator/config_server.txt` & `tool_server_generator-0.3.2/tool_server_generator/config_server.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/app.js` & `tool_server_generator-0.3.2/tool_server_generator/model/app.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/bin/www` & `tool_server_generator-0.3.2/tool_server_generator/model/bin/www`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/package-lock.json` & `tool_server_generator-0.3.2/tool_server_generator/model/package-lock.json`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/public/stylesheets/w3.css` & `tool_server_generator-0.3.2/tool_server_generator/model/public/stylesheets/w3.css`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/routes/index.js` & `tool_server_generator-0.3.2/tool_server_generator/model/routes/index.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/views/requests.pug` & `tool_server_generator-0.3.2/tool_server_generator/model/views/requests.pug`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/workers/process_command.js` & `tool_server_generator-0.3.2/tool_server_generator/model/workers/process_command.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/model/workers/request_listener.js` & `tool_server_generator-0.3.2/tool_server_generator/model/workers/request_listener.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/utils/config_parser.py` & `tool_server_generator-0.3.2/tool_server_generator/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/utils/config_server.py` & `tool_server_generator-0.3.2/tool_server_generator/utils/config_server.py`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.3.1/tool_server_generator/utils/utils.py` & `tool_server_generator-0.3.2/tool_server_generator/utils/utils.py`

 * *Files identical despite different names*

