# Comparing `tmp/cove_unified_logs-0.1.4.tar.gz` & `tmp/cove_unified_logs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cove_unified_logs-0.1.4.tar", last modified: Thu Jun  8 19:55:34 2023, max compression
+gzip compressed data, was "cove_unified_logs-0.1.5.tar", last modified: Thu Jun  8 20:22:59 2023, max compression
```

## Comparing `cove_unified_logs-0.1.4.tar` & `cove_unified_logs-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 19:55:34.039493 cove_unified_logs-0.1.4/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.1.4/LICENSE
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 19:55:34.039378 cove_unified_logs-0.1.4/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.1.4/README.md
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 19:55:34.038494 cove_unified_logs-0.1.4/cove_unified_logs/
--rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 10:41:05.000000 cove_unified_logs-0.1.4/cove_unified_logs/__init__.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5938 2023-06-08 17:20:34.000000 cove_unified_logs-0.1.4/cove_unified_logs/cloud_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1397 2023-06-08 18:58:04.000000 cove_unified_logs-0.1.4/cove_unified_logs/console_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     2219 2023-06-08 19:37:52.000000 cove_unified_logs-0.1.4/cove_unified_logs/log_consumer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1880 2023-06-08 18:44:58.000000 cove_unified_logs-0.1.4/cove_unified_logs/log_producer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.4/cove_unified_logs/middleware.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1524 2023-06-08 19:03:18.000000 cove_unified_logs-0.1.4/cove_unified_logs/unified_logger.py
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 19:55:34.039206 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)      466 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/SOURCES.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/dependency_links.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/requires.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 19:55:34.000000 cove_unified_logs-0.1.4/cove_unified_logs.egg-info/top_level.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 19:55:34.039531 cove_unified_logs-0.1.4/setup.cfg
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 19:14:41.000000 cove_unified_logs-0.1.4/setup.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 20:22:59.217890 cove_unified_logs-0.1.5/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1076 2023-06-08 19:25:10.000000 cove_unified_logs-0.1.5/LICENSE
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 20:22:59.217779 cove_unified_logs-0.1.5/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     6452 2023-06-08 19:44:21.000000 cove_unified_logs-0.1.5/README.md
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 20:22:59.216979 cove_unified_logs-0.1.5/cove_unified_logs/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 10:41:05.000000 cove_unified_logs-0.1.5/cove_unified_logs/__init__.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     5938 2023-06-08 17:20:34.000000 cove_unified_logs-0.1.5/cove_unified_logs/cloud_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1585 2023-06-08 20:11:05.000000 cove_unified_logs-0.1.5/cove_unified_logs/console_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2219 2023-06-08 19:37:52.000000 cove_unified_logs-0.1.5/cove_unified_logs/log_consumer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     2112 2023-06-08 20:15:13.000000 cove_unified_logs-0.1.5/cove_unified_logs/log_producer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.5/cove_unified_logs/middleware.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1524 2023-06-08 20:11:39.000000 cove_unified_logs-0.1.5/cove_unified_logs/unified_logger.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 20:22:59.217604 cove_unified_logs-0.1.5/cove_unified_logs.egg-info/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     7257 2023-06-08 20:22:59.000000 cove_unified_logs-0.1.5/cove_unified_logs.egg-info/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      466 2023-06-08 20:22:59.000000 cove_unified_logs-0.1.5/cove_unified_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 20:22:59.000000 cove_unified_logs-0.1.5/cove_unified_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 20:22:59.000000 cove_unified_logs-0.1.5/cove_unified_logs.egg-info/requires.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 20:22:59.000000 cove_unified_logs-0.1.5/cove_unified_logs.egg-info/top_level.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 20:22:59.217926 cove_unified_logs-0.1.5/setup.cfg
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 20:22:58.000000 cove_unified_logs-0.1.5/setup.py
```

### Comparing `cove_unified_logs-0.1.4/LICENSE` & `cove_unified_logs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.4/PKG-INFO` & `cove_unified_logs-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove_unified_logs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.1.4/README.md` & `cove_unified_logs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs/cloud_logger.py` & `cove_unified_logs-0.1.5/cove_unified_logs/cloud_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs/console_logger.py` & `cove_unified_logs-0.1.5/cove_unified_logs/console_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,7 +31,11 @@
         self._put_log_event(logging.WARNING, message, **metadata)
 
     def error(self, message, **metadata):
         self._put_log_event(logging.ERROR, message, **metadata)
 
     def critical(self, message, **metadata):
         self._put_log_event(logging.CRITICAL, message, **metadata)
+
+    def exception(self, message, **metadata):
+        # Log the exception with a traceback
+        self.logger.exception(message, extra={'app_name': self.app_name, 'metadata': metadata})
```

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs/log_consumer.py` & `cove_unified_logs-0.1.5/cove_unified_logs/log_consumer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs/log_producer.py` & `cove_unified_logs-0.1.5/cove_unified_logs/log_producer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-# log_producer.py
 import json
 import time
 import redis
 import logging
 import os
 
 
 class LogProducer:
+    _instance = None
+    _redis_pool = None
+
+    def __new__(cls, *args, **kwargs):
+        if not isinstance(cls._instance, cls):
+            cls._instance = super(LogProducer, cls).__new__(cls, *args, **kwargs)
+            # Initialize Redis ConnectionPool
+            redis_host = os.getenv('REDIS_HOST', 'localhost')
+            redis_port = int(os.getenv('REDIS_PORT', 6379))
+            redis_password = os.getenv('REDIS_PASSWORD', None)
+            cls._redis_pool = redis.ConnectionPool(host=redis_host, port=redis_port, password=redis_password)
+        return cls._instance
+
     def __init__(self, channel='logs'):
-        redis_host = os.getenv('REDIS_HOST', 'localhost')
-        redis_port = os.getenv('REDIS_PORT', 6379)
-        redis_password = os.getenv('REDIS_PASSWORD', None)
         try:
-            if redis_password is not None:
-                self.redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password)
-            else:
-                self.redis = redis.Redis(host=redis_host, port=redis_port)
+            self.redis = redis.Redis(connection_pool=self._redis_pool)
             self.channel = channel
         except Exception as e:
             logging.error(f"Failed to initialize LogProducer: {str(e)}")
             raise
 
     def log(self, level, message, **metadata):
         try:
@@ -47,8 +53,7 @@
         self.log('warning', message, **metadata)
 
     def error(self, message, **metadata):
         self.log('error', message, **metadata)
 
     def critical(self, message, **metadata):
         self.log('critical', message, **metadata)
-
```

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs/middleware.py` & `cove_unified_logs-0.1.5/cove_unified_logs/middleware.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs/unified_logger.py` & `cove_unified_logs-0.1.5/cove_unified_logs/unified_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.4/cove_unified_logs.egg-info/PKG-INFO` & `cove_unified_logs-0.1.5/cove_unified_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove-unified-logs
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.1.4/setup.py` & `cove_unified_logs-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cove_unified_logs',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Coveidentity Tech Private Limited',
     author_email='sarvpriye.soni@coveidentity.com',
     url='https://github.com/Cove-Identity/cove-unified-logs',
     packages=['cove_unified_logs'],
```

