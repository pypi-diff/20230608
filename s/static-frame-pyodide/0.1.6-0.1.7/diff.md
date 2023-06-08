# Comparing `tmp/static-frame-pyodide-0.1.6.tar.gz` & `tmp/static-frame-pyodide-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-pyodide-0.1.6.tar", last modified: Wed Jun  7 23:01:40 2023, max compression
+gzip compressed data, was "static-frame-pyodide-0.1.7.tar", last modified: Thu Jun  8 17:13:30 2023, max compression
```

## Comparing `static-frame-pyodide-0.1.6.tar` & `static-frame-pyodide-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-07 23:01:40.633834 static-frame-pyodide-0.1.6/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.6/LICENSE
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-07 23:01:40.633834 static-frame-pyodide-0.1.6/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.6/README.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.6/pyproject.toml
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-07 23:01:40.633834 static-frame-pyodide-0.1.6/setup.cfg
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-07 23:01:40.629834 static-frame-pyodide-0.1.6/static_frame_pyodide/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2383 2023-06-07 22:59:44.000000 static-frame-pyodide-0.1.6/static_frame_pyodide/__init__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-07 23:01:40.629834 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-08 17:13:30.002188 static-frame-pyodide-0.1.7/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-05 17:12:03.000000 static-frame-pyodide-0.1.7/LICENSE
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-08 17:13:30.002188 static-frame-pyodide-0.1.7/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-05 17:12:03.000000 static-frame-pyodide-0.1.7/README.md
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-05 17:12:03.000000 static-frame-pyodide-0.1.7/pyproject.toml
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-08 17:13:30.002188 static-frame-pyodide-0.1.7/setup.cfg
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-08 17:13:30.002188 static-frame-pyodide-0.1.7/static_frame_pyodide/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1943 2023-06-08 17:12:16.000000 static-frame-pyodide-0.1.7/static_frame_pyodide/__init__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-08 17:13:30.002188 static-frame-pyodide-0.1.7/static_frame_pyodide.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-08 17:13:29.000000 static-frame-pyodide-0.1.7/static_frame_pyodide.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-08 17:13:29.000000 static-frame-pyodide-0.1.7/static_frame_pyodide.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-08 17:13:29.000000 static-frame-pyodide-0.1.7/static_frame_pyodide.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-08 17:13:29.000000 static-frame-pyodide-0.1.7/static_frame_pyodide.egg-info/top_level.txt
```

### Comparing `static-frame-pyodide-0.1.6/LICENSE` & `static-frame-pyodide-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.6/PKG-INFO` & `static-frame-pyodide-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.6
+Version: 0.1.7
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `static-frame-pyodide-0.1.6/pyproject.toml` & `static-frame-pyodide-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.6/static_frame_pyodide/__init__.py` & `static-frame-pyodide-0.1.7/static_frame_pyodide/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,75 @@
 import sys
 import asyncio
 
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 
 _SF = '1.4.5'
 _AK = '0.4.8'
 _AM = '0.1.9'
 
 _EMS = '3_1_32' # emscripten version
 _URL = 'https://flexatone.s3.us-west-1.amazonaws.com/packages/'
 
 _MODULE = sys.modules[__name__]
 
 async def _micropip_and_import() -> bool:
-    print('micropiping start')
+
     micropip = __import__('micropip')
 
     await micropip.install([
         'sqlite3',
         f'{_URL}arraymap-{_AM}-cp311-cp311-emscripten_{_EMS}_wasm32.whl',
         f'{_URL}arraykit-{_AK}-cp311-cp311-emscripten_{_EMS}_wasm32.whl',
         f'static-frame=={_SF}',
         ])
 
-    print('micropiping complete')
-
-    # sf = __import__('static_frame')
-
-    # for name in dir(sf):
-    #     if not name.startswith('_'):
-    #         setattr(_MODULE, name, getattr(sf, name))
-    #         print('set', name)
-    # await asyncio.sleep(0)
-
-# async def _schedule_and_await(loop):
-#     task = loop.create_task(_micropip_and_import())
-#     await task
-
-# async def _schedule_and_await(loop):
-#     await asyncio.wait_for(_micropip_and_import(), None)
-#     print('post wait-for')
-
-# async def _schedule_and_await(loop):
-#     await loop.run_in_executor(None, _micropip_and_import())
+    try:
+        sf = __import__('static_frame')
+    except ModuleNotFoundError:
+        print("Cannot import statc-frame into this namespace, try `import static_frame as sf`")
+        sf = None
+
+    if sf:
+        for name in dir(sf):
+            if not name.startswith('_'):
+                setattr(_MODULE, name, getattr(sf, name))
 
 #-------------------------------------------------------------------------------
 if sys.platform != 'emscripten':
     raise RuntimeError('This package is only for use in emscripten environments')
 
 try:
     loop = asyncio.get_running_loop()
 except RuntimeError:
     loop = None
 
 if loop and loop.is_running():
-    print('loop already running')
     loop.create_task(asyncio.wait_for(_micropip_and_import(), None))
-
-    # new_loop = asyncio.new_event_loop()
-    # new_loop.run_until_complete(_micropip_and_import())
-
-    # loop.create_task(_schedule_and_await(loop))
-
-    # for coro in asyncio.as_completed((_micropip_and_import(),)):
-    #     # loop.create_task(coro)
-    #     print(coro)
-
-    # def finished(_):
-    #     print('finished')
-    # future = asyncio.run_coroutine_threadsafe(_micropip_and_import(), loop)
-    # future.add_done_callback(finished)
-    # assert future.result(20) == True
-
-    # loop.call_soon(_micropip_and_import())
-
-    # import threading
-    # def target():
-    #     return asyncio.run(_micropip_and_import())
-    # t = threading.Thread(target=target)
-    # t.start()
-    # t.join()
-
 else:
-    print('starting new event loop')
     asyncio.run(_micropip_and_import())
 
 
 
+# new_loop = asyncio.new_event_loop()
+# new_loop.run_until_complete(_micropip_and_import())
+
+# loop.create_task(_schedule_and_await(loop))
+
+# for coro in asyncio.as_completed((_micropip_and_import(),)):
+#     # loop.create_task(coro)
+#     print(coro)
+
+# def finished(_):
+#     print('finished')
+# future = asyncio.run_coroutine_threadsafe(_micropip_and_import(), loop)
+# future.add_done_callback(finished)
+# assert future.result(20) == True
+
+# loop.call_soon(_micropip_and_import())
+
+# import threading
+# def target():
+#     return asyncio.run(_micropip_and_import())
+# t = threading.Thread(target=target)
+# t.start()
+# t.join()
```

### Comparing `static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/PKG-INFO` & `static-frame-pyodide-0.1.7/static_frame_pyodide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.6
+Version: 0.1.7
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

