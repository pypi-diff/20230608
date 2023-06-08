# Comparing `tmp/ango-1.0.8.tar.gz` & `tmp/ango-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.8.tar", last modified: Thu Jun  1 11:05:04 2023, max compression
+gzip compressed data, was "ango-1.0.9.tar", last modified: Fri Jun  2 07:41:27 2023, max compression
```

## Comparing `ango-1.0.8.tar` & `ango-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-01 11:05:04.213060 ango-1.0.8/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.8/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.8/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.8/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.8/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-05-30 11:15:47.000000 ango-1.0.8/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.8/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5036 2023-06-01 09:29:39.000000 ango-1.0.8/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14428 2023-05-31 06:31:57.000000 ango-1.0.8/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-01 11:05:04.213060 ango-1.0.8/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-01 11:05:04.000000 ango-1.0.8/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-01 11:05:04.213060 ango-1.0.8/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-06-01 11:04:59.000000 ango-1.0.8/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-02 07:41:27.094165 ango-1.0.9/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.9/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.9/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.9/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.9/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5452 2023-05-30 11:15:47.000000 ango-1.0.9/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.9/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5446 2023-06-02 07:39:18.000000 ango-1.0.9/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14429 2023-06-01 20:58:42.000000 ango-1.0.9/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-06-02 07:41:27.094165 ango-1.0.9/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-06-02 07:41:26.000000 ango-1.0.9/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-06-02 07:41:27.000000 ango-1.0.9/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-06-02 07:41:26.000000 ango-1.0.9/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-06-02 07:41:27.000000 ango-1.0.9/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-06-02 07:41:27.000000 ango-1.0.9/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-06-02 07:41:27.094165 ango-1.0.9/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-06-02 07:22:27.000000 ango-1.0.9/setup.py
```

### Comparing `ango-1.0.8/PKG-INFO` & `ango-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.8/README.md` & `ango-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.8/ango/models/label_category.py` & `ango-1.0.9/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.8/ango/plugin_logger.py` & `ango-1.0.9/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.8/ango/plugins.py` & `ango-1.0.9/ango/plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import logging
 from io import BytesIO
 from typing import Callable, Tuple
-
+import queue
 import requests
 import socketio
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from ango.plugin_logger import PluginLogger
 from ango.sdk import SDK
 
@@ -50,14 +50,17 @@
     def _get_logger(self, data):
         org_id = data.get("orgId", "")
         run_by = data.get("runBy", "")
         session = data.get("session", "")
         logger = PluginLogger("logger", self.id, org_id, run_by, session, self)
         return logger
 
+    def start(self):
+        asyncio.get_event_loop().run_forever()
+
 
 class ExportPlugin(Plugin):
 
     def __init__(self, id: str, secret: str, callback: Callable[[str, dict], Tuple[str, BytesIO]],
                  host="https://imeritapi.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
@@ -95,29 +98,40 @@
             "response": upload_url.split("?")[0],
             "session": data.get("session", "")
         }
         self.emit('response', response)
 
 
 class ModelPlugin(Plugin):
-    def __init__(self, id: str, secret: str, callback: Callable, host="https://imeritapi.ango.ai"):
+    def __init__(self, id: str, secret: str, callback: Callable, host="https://imeritapi.ango.ai", concurrency=1):
         super().__init__(id, secret, callback)
         self.host = host
+        self.concurrency = concurrency
+        self.queue = queue.Queue()
+
+    async def work(self):
+        while True:
+            data = self.queue.get()
+            data["batches"] = data.get('tags', [])
+            api_key = data.get('apiKey')
+            task_id = data.get('taskId')
+            sdk = SDK(api_key=api_key, host=self.host)
+            answer = self.callback(**data)
+            sdk._annotate(task_id, answer.get("answer"))
 
     def on_plugin(self, data):
         workflow = data.get('workflow')
         if not workflow:
             return super().on_plugin(data)
-        #data["logger"] = self._get_logger(data)
-        data["batches"] = data.get('tags', [])
-        api_key = data.get('apiKey')
-        task_id = data.get('taskId')
-        sdk = SDK(api_key=api_key, host=self.host)
-        answer = self.callback(**data)
-        return sdk._annotate(task_id, answer.get("answer"));
+        self.queue.put(data)
+
+    def start(self):
+        tasks = [self.work() for i in range(self.concurrency)]
+        future = asyncio.gather(*tasks)
+        asyncio.get_event_loop().run_until_complete(future)
 
 class FileExplorerPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
 class BatchModelPlugin(Plugin):
@@ -136,10 +150,10 @@
 
 
 def run(plugin, host="https://plugin.imerit.ango.ai"):
     sio = socketio.Client()
     sio.register_namespace(plugin)
     sio.connect(host, namespaces=["/plugin"], wait_timeout=100)
     try:
-        asyncio.get_event_loop().run_forever()
+        plugin.start()
     except (KeyboardInterrupt, SystemExit):
         logging.getLogger().warning("Plugin Stopped")
```

### Comparing `ango-1.0.8/ango/sdk.py` & `ango-1.0.9/ango/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         return response.json()
 
     def get_assets(self, project_id, asset_id=None, external_id=None, page=1, limit=10):
         url = "%s/v2/project/%s/assets?page=%s&limit=%s" % (self.host, project_id, page, limit)
         if asset_id:
             url += "&_id=%s" % asset_id
         if external_id:
-            url += "&xternalId=%s" % external_id
+            url += "&externalId=%s" % external_id
 
         headers = {
             'apikey': self.api_key
         }
         response = self.session.get(url, headers=headers)
         return response.json()
```

### Comparing `ango-1.0.8/ango.egg-info/PKG-INFO` & `ango-1.0.9/ango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.8/setup.py` & `ango-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.8",
+    version="1.0.9",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

