# Comparing `tmp/lts-mpsmqutils-2.0.2a16.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a16.tar", last modified: Thu Jun  8 16:32:39 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a17.tar", last modified: Thu Jun  8 16:52:04 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a16.tar` & `lts-mpsmqutils-2.0.2a17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.194702 lts-mpsmqutils-2.0.2a16/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:32:39.194423 lts-mpsmqutils-2.0.2a16/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.189529 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.192261 lts-mpsmqutils-2.0.2a16/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)      784 2023-06-08 14:50:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/log_wrapper.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    27044 2023-06-08 16:32:22.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.193500 lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 16:32:39.194794 lts-mpsmqutils-2.0.2a16/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 16:31:58.000000 lts-mpsmqutils-2.0.2a16/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.351858 lts-mpsmqutils-2.0.2a17/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:52:04.351182 lts-mpsmqutils-2.0.2a17/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.343789 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.347140 lts-mpsmqutils-2.0.2a17/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     1004 2023-06-08 16:51:45.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    27237 2023-06-08 16:50:15.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.349248 lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 16:52:04.352072 lts-mpsmqutils-2.0.2a17/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 16:51:57.000000 lts-mpsmqutils-2.0.2a17/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a16/PKG-INFO` & `lts-mpsmqutils-2.0.2a17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a16
+Version: 2.0.2a17
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a16/README.md` & `lts-mpsmqutils-2.0.2a17/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/PKG-INFO` & `lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a16
+Version: 2.0.2a17
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a16/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a17/mpsmqutils/messagehandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,21 +38,14 @@
 NOTIFY_QUEUE = os.getenv('MQ_NOTIFY_QUEUE', '/queue/iiif_notify')
 DLQ_QUEUE = os.getenv('MQ_DLQ_QUEUE', '/queue/ActiveMQ.DLQ')
 
 # Email SMTP host for use in notify
 NOTIFY_MAIL_RELAY=os.getenv('MQ_NOTIFY_MAIL_RELAY', None)
 NOTIFY_DEFAULT_EMAIL=os.getenv('MQ_NOTIFY_DEFAULT_EMAIL', None)
 
-# Logging
-#import logging as logger
-#logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'DEBUG'))
-# https://stackoverflow.com/questions/15727420/using-logging-in-multiple-modules
-#logger = logging.getLogger(__name__)
-#app_name = __name__
-
 def call_worker_do_task(task_name, job_ticket_id = None, parent_job_ticket_id = None, worker_url_endpoint = 'do_task', worker_url = os.getenv('WORKER_API_URL'), add_params=None):
     logger.debug("************************ MQUTILS MQLISTENER - CALL WORKER DO TASK *******************************")
     '''Call the worker task class do task method and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
@@ -212,286 +205,288 @@
         set_job_failed = True if parent_job_ticket_id else False
         job_tracker.append_error(job_ticket_id, worker_response.get('error'), worker_response.get('message'), set_job_failed)
     return task_success
 
 completed_statuses = frozenset(['success', 'failed'])
 class MqMessageHandler():
     def __init__(self, message):
+        self.logger = log_wrapper.LogWrapper()
         self.message = message
 
     def handle_message(self):
-        logger.debug("************************ MQUTILS MQLISTENER - HANDLE_MESSAGE *******************************")
+        self.logger.debug("************************ MQUTILS MQLISTENER - HANDLE_MESSAGE *******************************")
         # headers, body = frame.headers, frame.body
-        logger.info('handling message "%s"' % self.message)
+        self.logger.info('handling message "%s"' % self.message)
 
         category = self.message.get("category", "ingest")
         # task_management
         task_success = False
         job_ticket_id = self.message.get('job_ticket_id')
-        logger.info('job_ticket_id {}'.format(job_ticket_id))
+        self.logger.info('job_ticket_id {}'.format(job_ticket_id))
         try:
             job_tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
         except Exception as e:
             import traceback
-            logger.error("Exception trying to get tracker_document: " + traceback.format_exc())
+            self.logger.error("Exception trying to get tracker_document: " + traceback.format_exc())
             job_tracker_doc = None
 
-        logger.info('job_tracker_doc {}'.format(job_tracker_doc))
+        self.logger.info('job_tracker_doc {}'.format(job_tracker_doc))
         status = job_tracker_doc['job_management']['job_status']
         if status in completed_statuses:
-            logger.info(f'Status {status} counts as completed, assuming job is complete')
+            self.logger.info(f'Status {status} counts as completed, assuming job is complete')
             #Assume if the tracker is completed or not there, that this job is no longer running
             return
 
-        logger.info(f"Dispatching based on category: {category}", flush=True)
+        self.logger.info(f"Dispatching based on category: {category}", flush=True)
         if (category == "ingest"):
             task_success = self.__ingest_message_handler(self.message)
         elif (category == "task_management"):
             task_success = self.__task_management_message_handler(self.message)
         elif (category == "service"):
             task_success = self.__service_message_handler(self.message)
         elif (category == "cache_management"):
             task_success = self.__cache_management_message_handler(self.message)
 
         if (task_success != None):
             if not task_success:
                 job_tracker.set_job_status('failed', job_ticket_id, "failed")
-                logger.error('Task unsuccessful')
+                self.logger.error('Task unsuccessful')
 
-        logger.info('processed message for job id {}'.format(job_ticket_id))
+        self.logger.info('processed message for job id {}'.format(job_ticket_id))
 
     def __ingest_message_handler(self, message_data):
-        logger.debug("************************ MQUTILS MQLISTENER - INGEST_MESSAGE_HANDLER *******************************")
+        self.logger.debug("************************ MQUTILS MQLISTENER - INGEST_MESSAGE_HANDLER *******************************")
         job_ticket_id = message_data.get('job_ticket_id')
-        logger.info('__ingest_message_handler job_ticket_id {}'.format(job_ticket_id))
+        self.logger.info('__ingest_message_handler job_ticket_id {}'.format(job_ticket_id))
         parent_job_ticket_id = message_data.get('parent_job_ticket_id', None)
-        logger.info('parent_job_ticket_id {}'.format(parent_job_ticket_id))
+        self.logger.info('parent_job_ticket_id {}'.format(parent_job_ticket_id))
         task_name = message_data.get('task_name')
-        logger.info('task_name {}'.format(task_name))
+        self.logger.info('task_name {}'.format(task_name))
         previous_step_status = message_data.get('previous_step_status', 'success')
-        logger.info('previous_step_status {}'.format(previous_step_status))
+        self.logger.info('previous_step_status {}'.format(previous_step_status))
         task_success = False
         worker_url_endpoint = "do_task"
 
         try:
-            logger.info('set_job_status to running')
+            self.logger.info('set_job_status to running')
             job_tracker.set_job_status('running', job_ticket_id)
         except Exception as e:
-            logger.error(e)
+            self.logger.error(e)
             return False
 
         #Send a message to the task manager queue as long as this isn't the task manager message
         tm_message = mqutils.create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id)
-        logger.info('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
+        self.logger.info('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
         celeryapp.execute.send_task("tasks.tasks.do_task", args=[tm_message], kwargs={}, queue=_tm_queue)
 
         # Run the service
         # Check if previous step status was successful
         if previous_step_status and 'fail' not in previous_step_status:
             # Update timestamp file before do task
-            logger.info('Calling do_task for job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
+            self.logger.info('Calling do_task for job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
 
             worker_url_endpoint = "do_task"
 
             nextmessage = mqutils.create_next_queue_message(job_ticket_id, parent_job_ticket_id)
-            logger.info('create_next_queue_message nextmessage {}'.format(nextmessage))
+            self.logger.info('create_next_queue_message nextmessage {}'.format(nextmessage))
 
         else:
             job_tracker.update_timestamp(job_ticket_id)
 
-            logger.info('Calling revert_task for job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
+            self.logger.info('Calling revert_task for job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
             worker_url_endpoint = "revert_task"
 
             # Create next queue message
             nextmessage = mqutils.create_revert_message(job_ticket_id, parent_job_ticket_id)
-            logger.info('create_revert_message nextmessage {}'.format(nextmessage))
+            self.logger.info('create_revert_message nextmessage {}'.format(nextmessage))
         try:
             #Update the timestamp
             job_tracker.update_timestamp(job_ticket_id)
-            logger.info("Successfully updated timestampf for job_ticket_id {} parent_job_ticket_id {}".format(job_ticket_id, parent_job_ticket_id))
+            self.logger.info("Successfully updated timestampf for job_ticket_id {} parent_job_ticket_id {}".format(job_ticket_id, parent_job_ticket_id))
         except Exception as e:
-            logger.error(e)
+            self.logger.error(e)
             return False
 
         # Call worker class do task method
         try:
             worker_response = call_worker_do_task(task_name, job_ticket_id, parent_job_ticket_id, worker_url_endpoint)
             task_success = handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id)
-            logger.info("SUCCESS IN WORKER RESPONSE TRY BLOCK")
+            self.logger.info("SUCCESS IN WORKER RESPONSE TRY BLOCK")
         except Exception as e:
-            logger.error(e)
+            self.logger.error(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
         if (task_success):
             # Update timestamp file after task is complete
-            logger.debug('AFTER TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
+            self.logger.debug('AFTER TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
             job_tracker.update_timestamp(job_ticket_id)
             if nextmessage is None:
                 job_tracker.set_job_status(previous_step_status, job_ticket_id)
-                logger.debug('******** LAST TASK COMPLETED ********')
-                logger.info('previous_step_status {} job_ticket_id {} parent_job_ticket_id {}'.format(previous_step_status, job_ticket_id, parent_job_ticket_id))
+                self.logger.debug('******** LAST TASK COMPLETED ********')
+                self.logger.info('previous_step_status {} job_ticket_id {} parent_job_ticket_id {}'.format(previous_step_status, job_ticket_id, parent_job_ticket_id))
             else:
                 try:
                     json_message = json.loads(nextmessage)
-                    logger.info(json_message)
+                    self.logger.info(json_message)
                 except ValueError as e:
-                    logger.error(e)
+                    self.logger.error(e)
                     job_tracker.append_error(job_ticket_id, 'Unable to get parse the next queue message',  traceback.format_exc(), False)
                     raise e
 
                 # Set the queue name to match the worker type
                 worker_type = json_message["event"]
                 queue = worker_type
-                logger.info('worker_type {}'.format(worker_type))
+                self.logger.info('worker_type {}'.format(worker_type))
                 tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
                 # Update the number of tries in the tracker file
                 tracker_doc["job_management"]["numberOfTries"] = 0
                 tracker_doc["job_management"]["current_step"] = json_message["current_step"]
                 tracker_doc["job_management"]["job_status"] = "queued"
                 tracker_doc["job_management"]["previous_step_status"] = json_message["previous_step_status"]
                 try:
-                    logger.debug('******** UPDATE TRACKER FILE ********')
+                    self.logger.debug('******** UPDATE TRACKER FILE ********')
                     updated_tracker_doc = job_tracker.replace_tracker_doc(tracker_doc)
-                    logger.info('updated_tracker_doc {}'.format(updated_tracker_doc))
+                    self.logger.info('updated_tracker_doc {}'.format(updated_tracker_doc))
                 except Exception as e:
                     #TODO what to do here - what does this mean if the tracker retrieval fails?
-                    logger.error("TRACKER RETRIEVAL FAILED")
-                    logger.error(e, flush=True)
+                    self.logger.error("TRACKER RETRIEVAL FAILED")
+                    self.logger.error(e, flush=True)
                     raise e
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[nextmessage], kwargs={}, queue=queue)
-        logger.info('task_success for __ingest_message_handler:')
-        logger.info(task_success)
+        self.logger.info('task_success for __ingest_message_handler:')
+        self.logger.info(task_success)
         return task_success
 
     def __task_management_message_handler(self, message_data):
-        logger.debug("************************ MQUTILS MQLISTENER - TASK MANAGEMENT MESSAGE HANDLER *******************************")
-        logger.info('__task_management_message_handler:')
+        self.logger.debug("************************ MQUTILS MQLISTENER - TASK MANAGEMENT MESSAGE HANDLER *******************************")
+        self.logger.info('__task_management_message_handler:')
         job_ticket_id = message_data.get('job_ticket_id')
         parent_job_ticket_id = message_data.get('parent_job_ticket_id', None)
         task_name = message_data.get('task_name')
-        logger.info(task_name)
+        self.logger.info(task_name)
         task_success = False
 
         #We want the task manager to watch the multi asset ingest jobs
         if (task_name == "multi_asset_ingest"):
             #Send a message to the task manager queue as long as this isn't the task manager message
-            logger.debug("MULTI ASSET INGEST TASK")
+            self.logger.debug("MULTI ASSET INGEST TASK")
             tm_message = mqutils.create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id)
-            logger.info('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
+            self.logger.info('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
             # BROKEN
             celeryapp.execute.send_task("tasks.tasks.do_task", args=[tm_message], kwargs={}, queue=_tm_queue)
 
         try:
             job_tracker.set_job_status('running', job_ticket_id)
             # Run the service
             # Update timestamp file before do task
-            logger.debug('BEFORE DO TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
+            self.logger.debug('BEFORE DO TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
             job_tracker.update_timestamp(job_ticket_id)
         except Exception as e:
-            logger.error(e)
+            self.logger.error(e)
             task_success = False
 
         # Call do task
-        logger.debug("******************* CALLING WORKER API DO TASK __task_management_message_handler *******************")
+        self.logger.debug("******************* CALLING WORKER API DO TASK __task_management_message_handler *******************")
         try:
-            logger.info("call_worker_api task_name {} job_ticket_id {} parent_job_ticket_id {} do_task")
+            self.logger.info("call_worker_api task_name {} job_ticket_id {} parent_job_ticket_id {} do_task")
             worker_response = call_worker_api(task_name, job_ticket_id, parent_job_ticket_id, 'do_task')
-            logger.info("worker_response")
-            logger.info(worker_response)
+            self.logger.info("worker_response")
+            self.logger.info(worker_response)
         except Exception as e:
-            logger.error("CALLING WORKER API DO TASK FAILED")
-            logger.error(e)
+            self.logger.error("CALLING WORKER API DO TASK FAILED")
+            self.logger.error(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
-        logger.debug("******************* HANDLE WORKER RESPONSE *******************")
+        self.logger.debug("******************* HANDLE WORKER RESPONSE *******************")
         try:
             task_success = handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id)
         except Exception as e:
-            logger.error("HANDLE WORKER RESPONSE FAILED")
-            logger.error(e)
+            self.logger.error("HANDLE WORKER RESPONSE FAILED")
+            self.logger.error(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
-        logger.info("task_success in __task_management_message_handler:")
-        logger.info(task_success)
+        self.logger.info("task_success in __task_management_message_handler:")
+        self.logger.info(task_success)
 
         #Ack message was already handled above
         if (task_name == "multi_asset_ingest"):
             try:
                 job_status = job_tracker.get_job_status(job_ticket_id)
                 if job_status == "failed":
-                    logger.error('JOB STATUS: FAILED')
+                    self.logger.error('JOB STATUS: FAILED')
                 # Successful parent jobs will be handled by the task_manager's job monitor which periodically checks in-progress
                 # jobs for stalled jobs or parent jobs where all children are complete. Upon successful completion of all child
                 # jobs, the parent will be marked by that process as successful
             except Exception as e:
                 job_tracker.append_error(job_ticket_id, f"Exception {str(e)} in job {job_ticket_id}", traceback.format_exc(), True)
 
             return None
         return task_success
 
 
     def __service_message_handler(self, message_data):
-        logger.info('services message')
+        self.logger.info('services message')
         return True
 
     def __cache_management_message_handler(self, message_data, message_id):
-        logger.info('cache management message')
+        self.logger.info('cache management message')
         try:
             worker_response = call_worker_api('update_cache')
         except Exception as e:
             import traceback;
-            logger.error('Failure in cache management handler')
-            logger.error(traceback.format_exc(), flush=True)
+            self.logger.error('Failure in cache management handler')
+            self.logger.error(traceback.format_exc(), flush=True)
             return False
         return True
 
 # Generalized listener based on MQListener for use with components that do not use jobtracker
 # If a next queue is returned from do_task, will place the same message it received on the specified queue
 class GenericMessageHandler():
     def __init__(self, message, worker_endpoint='do_task'):
         self.message = message
         self.worker_endpoint = worker_endpoint
+        self.logger = log_wrapper.LogWrapper()
 
     def handle_message(self):
-        logger.info('received a message headers "%s"' % self.message)
+        self.logger.info('received a message headers "%s"' % self.message)
         task_success = False
 
         task_success = self.__generic_message_handler(self.message, self.worker_endpoint)
 
         if (task_success != None):
             if not task_success:
-                logger.error('Task unsuccessful')
+                self.logger.error('Task unsuccessful')
 
     def __generic_message_handler(self, message_data, worker_endpoint):
-        logger.debug("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************")
+        self.logger.debug("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************")
         task_success = False
 
         # Call task
         try:
             worker_response = call_generic_worker_api(message_data, worker_endpoint)
             next_queue = os.getenv('NEXT_QUEUE')
             task_success = True if worker_response.get('success') else False
-            logger.info("SUCCESS IN WORKER RESPONSE TRY BLOCK")
+            self.logger.info("SUCCESS IN WORKER RESPONSE TRY BLOCK")
         except Exception as e:
-            logger.error(e)
+            self.logger.error(e)
             task_success = False
 
         if (task_success):
             # Update timestamp file after task is complete
             if next_queue is None:
                 #There are no more items to queue so the job is actually finished.
-                logger.info('******** LAST TASK COMPLETED ********')
+                self.logger.info('******** LAST TASK COMPLETED ********')
             else:
-                logger.info('******** TASK COMPLETED - GOING TO NEXT QUEUE ********')
+                self.logger.info('******** TASK COMPLETED - GOING TO NEXT QUEUE ********')
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[self.message], kwargs={}, queue=next_queue)
-        logger.info('task_success for __generic_message_handler')
-        logger.info(task_success)
+        self.logger.info('task_success for __generic_message_handler')
+        self.logger.info(task_success)
         return task_success
 
 # NOTIFY_SUB=2
 # DLQ_SUB=3
 # recipient_separators = re.compile(r'[,;]')
 # class NotificationListener(stomp.ConnectionListener):
 #     def __init__(self, conn):
```

### Comparing `lts-mpsmqutils-2.0.2a16/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a17/mpsmqutils/mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a16/setup.py` & `lts-mpsmqutils-2.0.2a17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a16",
+    version="2.0.2a17",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

