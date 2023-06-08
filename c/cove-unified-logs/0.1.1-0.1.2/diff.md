# Comparing `tmp/cove_unified_logs-0.1.1.tar.gz` & `tmp/cove_unified_logs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cove_unified_logs-0.1.1.tar", last modified: Thu Jun  8 18:34:51 2023, max compression
+gzip compressed data, was "cove_unified_logs-0.1.2.tar", last modified: Thu Jun  8 18:47:16 2023, max compression
```

## Comparing `cove_unified_logs-0.1.1.tar` & `cove_unified_logs-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:34:51.294646 cove_unified_logs-0.1.1/
--rw-r--r--   0 sarvpriye   (502) staff       (20)      783 2023-06-08 18:20:43.000000 cove_unified_logs-0.1.1/LICENSE
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5322 2023-06-08 18:34:51.294544 cove_unified_logs-0.1.1/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)     4517 2023-06-08 18:22:32.000000 cove_unified_logs-0.1.1/README.md
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:34:51.293732 cove_unified_logs-0.1.1/cove_unified_logs/
--rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 10:41:05.000000 cove_unified_logs-0.1.1/cove_unified_logs/__init__.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5938 2023-06-08 17:20:34.000000 cove_unified_logs-0.1.1/cove_unified_logs/cloud_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      785 2023-06-08 16:58:09.000000 cove_unified_logs-0.1.1/cove_unified_logs/console_logger.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1799 2023-06-08 17:30:29.000000 cove_unified_logs-0.1.1/cove_unified_logs/log_consumer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1656 2023-06-08 16:39:23.000000 cove_unified_logs-0.1.1/cove_unified_logs/log_producer.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.1/cove_unified_logs/middleware.py
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1570 2023-06-08 17:10:22.000000 cove_unified_logs-0.1.1/cove_unified_logs/unified_logger.py
-drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:34:51.294385 cove_unified_logs-0.1.1/cove_unified_logs.egg-info/
--rw-r--r--   0 sarvpriye   (502) staff       (20)     5322 2023-06-08 18:34:51.000000 cove_unified_logs-0.1.1/cove_unified_logs.egg-info/PKG-INFO
--rw-r--r--   0 sarvpriye   (502) staff       (20)      466 2023-06-08 18:34:51.000000 cove_unified_logs-0.1.1/cove_unified_logs.egg-info/SOURCES.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 18:34:51.000000 cove_unified_logs-0.1.1/cove_unified_logs.egg-info/dependency_links.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 18:34:51.000000 cove_unified_logs-0.1.1/cove_unified_logs.egg-info/requires.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 18:34:51.000000 cove_unified_logs-0.1.1/cove_unified_logs.egg-info/top_level.txt
--rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 18:34:51.294683 cove_unified_logs-0.1.1/setup.cfg
--rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 18:34:42.000000 cove_unified_logs-0.1.1/setup.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:47:16.286107 cove_unified_logs-0.1.2/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      783 2023-06-08 18:20:43.000000 cove_unified_logs-0.1.2/LICENSE
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     5322 2023-06-08 18:47:16.285965 cove_unified_logs-0.1.2/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     4517 2023-06-08 18:22:32.000000 cove_unified_logs-0.1.2/README.md
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:47:16.278715 cove_unified_logs-0.1.2/cove_unified_logs/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       72 2023-06-08 10:41:05.000000 cove_unified_logs-0.1.2/cove_unified_logs/__init__.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     5938 2023-06-08 17:20:34.000000 cove_unified_logs-0.1.2/cove_unified_logs/cloud_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      785 2023-06-08 16:58:09.000000 cove_unified_logs-0.1.2/cove_unified_logs/console_logger.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1799 2023-06-08 17:30:29.000000 cove_unified_logs-0.1.2/cove_unified_logs/log_consumer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1880 2023-06-08 18:44:58.000000 cove_unified_logs-0.1.2/cove_unified_logs/log_producer.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      865 2023-06-08 17:53:38.000000 cove_unified_logs-0.1.2/cove_unified_logs/middleware.py
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1570 2023-06-08 17:10:22.000000 cove_unified_logs-0.1.2/cove_unified_logs/unified_logger.py
+drwxr-xr-x   0 sarvpriye   (502) staff       (20)        0 2023-06-08 18:47:16.285758 cove_unified_logs-0.1.2/cove_unified_logs.egg-info/
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     5322 2023-06-08 18:47:16.000000 cove_unified_logs-0.1.2/cove_unified_logs.egg-info/PKG-INFO
+-rw-r--r--   0 sarvpriye   (502) staff       (20)      466 2023-06-08 18:47:16.000000 cove_unified_logs-0.1.2/cove_unified_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)        1 2023-06-08 18:47:16.000000 cove_unified_logs-0.1.2/cove_unified_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       31 2023-06-08 18:47:16.000000 cove_unified_logs-0.1.2/cove_unified_logs.egg-info/requires.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       18 2023-06-08 18:47:16.000000 cove_unified_logs-0.1.2/cove_unified_logs.egg-info/top_level.txt
+-rw-r--r--   0 sarvpriye   (502) staff       (20)       38 2023-06-08 18:47:16.286155 cove_unified_logs-0.1.2/setup.cfg
+-rw-r--r--   0 sarvpriye   (502) staff       (20)     1174 2023-06-08 18:44:58.000000 cove_unified_logs-0.1.2/setup.py
```

### Comparing `cove_unified_logs-0.1.1/LICENSE` & `cove_unified_logs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/PKG-INFO` & `cove_unified_logs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove_unified_logs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.1.1/README.md` & `cove_unified_logs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs/cloud_logger.py` & `cove_unified_logs-0.1.2/cove_unified_logs/cloud_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs/console_logger.py` & `cove_unified_logs-0.1.2/cove_unified_logs/console_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs/log_consumer.py` & `cove_unified_logs-0.1.2/cove_unified_logs/log_consumer.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs/log_producer.py` & `cove_unified_logs-0.1.2/cove_unified_logs/log_producer.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 import os
 
 
 class LogProducer:
     def __init__(self, channel='logs'):
         redis_host = os.getenv('REDIS_HOST', 'localhost')
         redis_port = os.getenv('REDIS_PORT', 6379)
+        redis_password = os.getenv('REDIS_PASSWORD', None)
         try:
-            self.redis = redis.Redis(host=redis_host, port=redis_port)
+            if redis_password is not None:
+                self.redis = redis.Redis(host=redis_host, port=redis_port, password=redis_password)
+            else:
+                self.redis = redis.Redis(host=redis_host, port=redis_port)
             self.channel = channel
         except Exception as e:
             logging.error(f"Failed to initialize LogProducer: {str(e)}")
             raise
 
     def log(self, level, message, **metadata):
         try:
```

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs/middleware.py` & `cove_unified_logs-0.1.2/cove_unified_logs/middleware.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs/unified_logger.py` & `cove_unified_logs-0.1.2/cove_unified_logs/unified_logger.py`

 * *Files identical despite different names*

### Comparing `cove_unified_logs-0.1.1/cove_unified_logs.egg-info/PKG-INFO` & `cove_unified_logs-0.1.2/cove_unified_logs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cove-unified-logs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.
 Home-page: https://github.com/Cove-Identity/cove-unified-logs
 Author: Coveidentity Tech Private Limited
 Author-email: sarvpriye.soni@coveidentity.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `cove_unified_logs-0.1.1/setup.py` & `cove_unified_logs-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cove_unified_logs',
-    version='0.1.1',
+    version='0.1.2',
     description='A Python logging library for unified logging across AWS Lambda, Django, and Google Cloud servers. Logs are asynchronously pushed to AWS CloudWatch.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Coveidentity Tech Private Limited',
     author_email='sarvpriye.soni@coveidentity.com',
     url='https://github.com/Cove-Identity/cove-unified-logs',
     packages=['cove_unified_logs'],
```

