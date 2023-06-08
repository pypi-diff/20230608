# Comparing `tmp/lts-mpsmqutils-2.0.2a19.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a19.tar", last modified: Thu Jun  8 17:21:43 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a20.tar", last modified: Thu Jun  8 17:48:55 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a19.tar` & `lts-mpsmqutils-2.0.2a20.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:21:43.166410 lts-mpsmqutils-2.0.2a19/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 17:21:43.165957 lts-mpsmqutils-2.0.2a19/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a19/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:21:43.161136 lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 17:21:43.000000 lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 17:21:43.000000 lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 17:21:43.000000 lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 17:21:43.000000 lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 17:21:43.000000 lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:21:43.164187 lts-mpsmqutils-2.0.2a19/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a19/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)      836 2023-06-08 17:20:10.000000 lts-mpsmqutils-2.0.2a19/mpsmqutils/log_wrapper.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    27069 2023-06-08 17:20:03.000000 lts-mpsmqutils-2.0.2a19/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a19/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:21:43.165305 lts-mpsmqutils-2.0.2a19/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a19/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a19/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 17:21:43.166550 lts-mpsmqutils-2.0.2a19/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 17:21:35.000000 lts-mpsmqutils-2.0.2a19/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:48:55.830163 lts-mpsmqutils-2.0.2a20/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 17:48:55.829746 lts-mpsmqutils-2.0.2a20/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a20/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:48:55.825008 lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 17:48:55.000000 lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 17:48:55.000000 lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 17:48:55.000000 lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 17:48:55.000000 lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 17:48:55.000000 lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:48:55.827490 lts-mpsmqutils-2.0.2a20/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a20/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)      868 2023-06-08 17:48:36.000000 lts-mpsmqutils-2.0.2a20/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    27071 2023-06-08 17:32:31.000000 lts-mpsmqutils-2.0.2a20/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a20/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:48:55.828723 lts-mpsmqutils-2.0.2a20/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a20/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a20/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 17:48:55.830316 lts-mpsmqutils-2.0.2a20/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 17:48:53.000000 lts-mpsmqutils-2.0.2a20/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a19/PKG-INFO` & `lts-mpsmqutils-2.0.2a20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a19
+Version: 2.0.2a20
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a19/README.md` & `lts-mpsmqutils-2.0.2a20/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a19/lts_mpsmqutils.egg-info/PKG-INFO` & `lts-mpsmqutils-2.0.2a20/lts_mpsmqutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a19
+Version: 2.0.2a20
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a19/mpsmqutils/log_wrapper.py` & `lts-mpsmqutils-2.0.2a20/mpsmqutils/log_wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 		else:
 			# if configured wrong, we default to info
 			print("log level configured incorrectly, defaulting to INFO")
 			self.log_level = 1
 
 	def debug(self, message):
 		if self.log_level <= 0:
-			print(message, flush=True)
+			print(message, end='', flush=True)
 
 	def info(self, message):
 		if self.log_level <= 1:
-			print(message, flush=True)
+			print(message, end='', flush=True)
 
 	def warning(self, message):
 		if self.log_level <= 2:
-			print(message, flush=True)
+			print(message, end='', flush=True)
 
 	def error(self, message):
 		if self.log_level <= 3:
-			print(message, flush=True)
+			print(message, end='', flush=True)
```

### Comparing `lts-mpsmqutils-2.0.2a19/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a20/mpsmqutils/messagehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         try:
             job_tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
         except Exception as e:
             import traceback
             self.logger.error("Exception trying to get tracker_document: " + traceback.format_exc())
             job_tracker_doc = None
 
-        self.logger.info('job_tracker_doc {}'.format(job_tracker_doc))
+        self.logger.debug('job_tracker_doc {}'.format(job_tracker_doc))
         status = job_tracker_doc['job_management']['job_status']
         if status in completed_statuses:
             self.logger.info(f'Status {status} counts as completed, assuming job is complete')
             #Assume if the tracker is completed or not there, that this job is no longer running
             return
 
         self.logger.info(f"Dispatching based on category: {category}")
@@ -342,15 +342,15 @@
                 tracker_doc["job_management"]["numberOfTries"] = 0
                 tracker_doc["job_management"]["current_step"] = json_message["current_step"]
                 tracker_doc["job_management"]["job_status"] = "queued"
                 tracker_doc["job_management"]["previous_step_status"] = json_message["previous_step_status"]
                 try:
                     self.logger.debug('******** UPDATE TRACKER FILE ********')
                     updated_tracker_doc = job_tracker.replace_tracker_doc(tracker_doc)
-                    self.logger.info('updated_tracker_doc {}'.format(updated_tracker_doc))
+                    self.logger.debug('updated_tracker_doc {}'.format(updated_tracker_doc))
                 except Exception as e:
                     #TODO what to do here - what does this mean if the tracker retrieval fails?
                     self.logger.error("TRACKER RETRIEVAL FAILED")
                     self.logger.error(e)
                     raise e
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[nextmessage], kwargs={}, queue=queue)
         self.logger.info('task_success for __ingest_message_handler:')
```

### Comparing `lts-mpsmqutils-2.0.2a19/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a20/mpsmqutils/mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a19/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a20/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a19/setup.py` & `lts-mpsmqutils-2.0.2a20/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a19",
+    version="2.0.2a20",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

