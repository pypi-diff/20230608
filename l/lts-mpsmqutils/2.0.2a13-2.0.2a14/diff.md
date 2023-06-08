# Comparing `tmp/lts-mpsmqutils-2.0.2a13.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a13.tar", last modified: Fri Jun  2 16:46:06 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a14.tar", last modified: Thu Jun  8 15:41:54 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a13.tar` & `lts-mpsmqutils-2.0.2a14.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.780110 lts-mpsmqutils-2.0.2a13/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-02 16:46:06.779665 lts-mpsmqutils-2.0.2a13/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.776831 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      343 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-02 16:46:06.000000 lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.778009 lts-mpsmqutils-2.0.2a13/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    27140 2023-06-02 15:32:14.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7160 2023-06-02 15:06:59.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-02 16:46:06.779060 lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-02 16:46:06.780264 lts-mpsmqutils-2.0.2a13/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-02 16:46:00.000000 lts-mpsmqutils-2.0.2a13/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 15:41:54.895191 lts-mpsmqutils-2.0.2a14/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 15:41:54.894887 lts-mpsmqutils-2.0.2a14/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a14/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 15:41:54.891849 lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 15:41:54.000000 lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 15:41:54.000000 lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 15:41:54.000000 lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 15:41:54.000000 lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 15:41:54.000000 lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 15:41:54.893528 lts-mpsmqutils-2.0.2a14/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a14/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)      784 2023-06-08 14:50:09.000000 lts-mpsmqutils-2.0.2a14/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    27023 2023-06-08 15:18:02.000000 lts-mpsmqutils-2.0.2a14/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7250 2023-06-08 15:22:46.000000 lts-mpsmqutils-2.0.2a14/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 15:41:54.894295 lts-mpsmqutils-2.0.2a14/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a14/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a14/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 15:41:54.895285 lts-mpsmqutils-2.0.2a14/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 15:41:46.000000 lts-mpsmqutils-2.0.2a14/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a13/PKG-INFO` & `lts-mpsmqutils-2.0.2a14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a13
+Version: 2.0.2a14
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a13/README.md` & `lts-mpsmqutils-2.0.2a14/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a13/lts_mpsmqutils.egg-info/PKG-INFO` & `lts-mpsmqutils-2.0.2a14/lts_mpsmqutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a13
+Version: 2.0.2a14
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a13/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a14/mpsmqutils/messagehandler.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 import mpsjobtracker.trackers.jobtracker as jobtracker
 job_tracker = jobtracker.JobTracker()
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
+from .log_wrapper import LogWrapper
+logger = LogWrapper()
+
 retry_strategy = Retry(
     total=3,
     status_forcelist=[429, 500, 502, 503, 504],
     backoff_factor=1
 )
 adapter = HTTPAdapter(max_retries=retry_strategy)
 http_client = requests.Session()
@@ -43,117 +46,117 @@
 #import logging as logger
 #logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'DEBUG'))
 # https://stackoverflow.com/questions/15727420/using-logging-in-multiple-modules
 #logger = logging.getLogger(__name__)
 #app_name = __name__
 
 def call_worker_do_task(task_name, job_ticket_id = None, parent_job_ticket_id = None, worker_url_endpoint = 'do_task', worker_url = os.getenv('WORKER_API_URL'), add_params=None):
-    print("************************ PRINT MQUTILS MQLISTENER - CALL WORKER DO TASK *******************************")
+    logger.debug("************************ MQUTILS MQLISTENER - CALL WORKER DO TASK *******************************")
     '''Call the worker task class do task method and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
       'message': None
     }
     job_ticket_id_str = f" job_ticket_id: {job_ticket_id}" if job_ticket_id else ""
     parent_job_ticket_id_str = f" parent_job_ticket_id: {parent_job_ticket_id}" if parent_job_ticket_id else ""
-    print(f'mqlistener call_worker_do_task START{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
+    logger.info(f'mqlistener call_worker_do_task START{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
 
     """
       Call worker task class do task method
     """
     try:
         message_data = { 'task_name': task_name }
         if add_params:
             message_data = {**json_params, **add_params}
         if job_ticket_id:
             message_data['job_ticket_id'] = job_ticket_id
         if parent_job_ticket_id:
             message_data['parent_job_ticket_id'] = parent_job_ticket_id
-        print(message_data)
+        logger.info(message_data)
         wt = worker_task.WorkerTask()
         response_json = wt.do_task(message_data)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise Exception(e)
 
-    print(f'mqlistener call_worker_do_task COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
+    logger.debug(f'mqlistener call_worker_do_task COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
 
-    print(response_json)
+    logger.info(response_json)
 
     success = False if not response_json.get('success') else True
-    print("success:")
-    print(success)
+    logger.info("mqlistener call_worker_do_task success:")
+    logger.info(success)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
 
     return result
 
 def call_worker_api(task_name, job_ticket_id = None, parent_job_ticket_id = None, worker_url_endpoint = 'do_task', worker_url = os.getenv('WORKER_API_URL'), add_params=None):
-    print("************************ MQUTILS MQLISTENER - CALL WORKER API *******************************")
+    logger.debug("************************ MQUTILS MQLISTENER - CALL WORKER API *******************************")
     '''Call the worker API and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
       'message': None
     }
     job_ticket_id_str = f" job_ticket_id: {job_ticket_id}" if job_ticket_id else ""
     parent_job_ticket_id_str = f" parent_job_ticket_id: {parent_job_ticket_id}" if parent_job_ticket_id else ""
-    print(f'mqlistener call_worker_api START{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
+    logger.info(f'mqlistener call_worker_api START{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name}')
 
     """
       Call worker API internally to perform the task
       This API call is calling the worker task in the same container and must use the internal container port
     """
     try:
 
         if not worker_url:
             error_msg = 'Missing configuration WORKER_API_URL'
-            print(error_msg, flush=True)
+            logger.error(error_msg, flush=True)
             raise Exception(error_msg)
         url = worker_url + '/' + worker_url_endpoint
-        print('mqlistener call_worker_api url {}'.format(url), flush=True)
+        logger.debug('mqlistener call_worker_api url {}'.format(url), flush=True)
         json_params = { 'task_name': task_name }
         if add_params:
             json_params = {**json_params, **add_params}
         if job_ticket_id:
             json_params['job_ticket_id'] = job_ticket_id
         if parent_job_ticket_id:
             json_params['parent_job_ticket_id'] = parent_job_ticket_id
-        print("json_params")
-        print(json_params)
+        logger.info("json_params")
+        logger.info(json_params)
         # The worker uses a self-signed certificate and it does not need to be verified since the listener makes a request to the worker inside the same container internally
         response = http_client.post(url, json = json_params, verify=False)
         response.raise_for_status()
-        print(response)
+        logger.info(response)
     except Exception as e:
-        print(e)
+        logger.error(e)
         if job_ticket_id:
             job_tracker.append_error(job_ticket_id, 'mqlistener call_worker_api API call failed', traceback.format_exc(), True)
         raise Exception(e)
 
-    print(f'mqlistener call_worker_api COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name} response.json() {response.json()}', flush=True)
+    logger.debug(f'mqlistener call_worker_api COMPLETE{job_ticket_id_str}{parent_job_ticket_id_str} task_name {task_name} response.json() {response.json()}', flush=True)
 
     response_json = response.json()
-    print(response_json)
+    logger.debug(response_json)
 
     success = False if not response_json.get('success') else True
-    print("success:")
-    print(success)
+    logger.info("mqlistener call_worker_api success:")
+    logger.info(success)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
 
     return result
 
 def call_generic_worker_api(message_data, worker_endpoint):
-    print("************************ MQUTILS MQLISTENER - CALL GENERIC WORKER API *******************************", flush=True)
+    logger.debug("************************ MQUTILS MQLISTENER - CALL GENERIC WORKER API *******************************", flush=True)
     '''Call the worker API and process the response in a standard format'''
 
     result = {
       'success': False,
       'error': None,
       'message': None,
       'next_queue': None
@@ -163,350 +166,332 @@
     """
       Call worker API internally to perform the task
       This API call is calling the worker task in the same container and must use the internal container port
     """
     try:
         if not worker_url:
             error_msg = 'Missing configuration WORKER_API_URL'
-            print(error_msg, flush=True)
+            logger.error(error_msg, flush=True)
             raise Exception(error_msg)
         url = worker_url
-        print('mqlistener call_generic_worker_api url {}'.format(url), flush=True)
+        logger.info('mqlistener call_generic_worker_api url {}'.format(url), flush=True)
         # The worker uses a self-signed certificate and it does not need to be verified since the listener makes a request to the worker inside the same container internally
         response = http_client.post(url, json = message_data, verify=False)
         response.raise_for_status()
-        print('response.raise_for_status', flush=True)
-        print(response, flush=True)
+        logger.info('response.raise_for_status', flush=True)
+        logger.info(response, flush=True)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise Exception(e)
 
     response_json = response.json()
-    print(response_json, flush=True)
+    logger.debug(response_json, flush=True)
 
     success = False if not response_json.get('success') else True
-    print("success:", flush=True)
-    print(success, flush=True)
+    logger.info("success for call_generic_worker_api:", flush=True)
+    logger.info(success, flush=True)
     result['success'] = success
     result['error'] = response_json.get('error', None)
     result['message'] = response_json.get('message', None)
     result['next_queue'] = response_json.get('next_queue', None)
 
     return result
 
 def handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id=None):
-    print("************************ MQUTILS MQLISTENER - HANDLE_WORKER_RESPONSE *******************************")
+    logger.debug("************************ MQUTILS MQLISTENER - HANDLE_WORKER_RESPONSE *******************************")
     """Handle the response from the worker API
     Capture any error messages returned in the json body
     Examples worker API responses:
     Response was successful: { success: true }
     Response had an error: { success: false, 'error': 'Example error', 'message': 'Example error message' }
     """
     task_success = True if worker_response.get('success') else False
-    print("task success")
-    print(task_success)
+    logger.info("task success for handle_worker_response")
+    logger.info(task_success)
     if not task_success:
         # Set job failed if the job is a child job
         set_job_failed = True if parent_job_ticket_id else False
         job_tracker.append_error(job_ticket_id, worker_response.get('error'), worker_response.get('message'), set_job_failed)
     return task_success
 
 completed_statuses = frozenset(['success', 'failed'])
 class MqMessageHandler():
     def __init__(self, message):
         self.message = message
 
     def handle_message(self):
-        print("************************ MQUTILS MQLISTENER - HANDLE_MESSAGE *******************************")
+        logger.debug("************************ MQUTILS MQLISTENER - HANDLE_MESSAGE *******************************")
         # headers, body = frame.headers, frame.body
-        print('handling message "%s"' % self.message)
+        logger.info('handling message "%s"' % self.message)
 
         category = self.message.get("category", "ingest")
+        # task_management
         task_success = False
         job_ticket_id = self.message.get('job_ticket_id')
-        print('job_ticket_id {}'.format(job_ticket_id))
+        logger.info('job_ticket_id {}'.format(job_ticket_id))
         try:
             job_tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
         except Exception as e:
             import traceback
-            print("Exception trying to get tracker_document: " + traceback.format_exc())
+            logger.error("Exception trying to get tracker_document: " + traceback.format_exc())
             job_tracker_doc = None
 
-        print('job_tracker_doc {}'.format(job_tracker_doc))
+        logger.info('job_tracker_doc {}'.format(job_tracker_doc))
         status = job_tracker_doc['job_management']['job_status']
         if status in completed_statuses:
-            print(f'Status {status} counts as completed, assuming job is complete')
+            logger.info(f'Status {status} counts as completed, assuming job is complete')
             #Assume if the tracker is completed or not there, that this job is no longer running
             return
 
-        print(f"Dispatching based on category: {category}", flush=True)
+        logger.info(f"Dispatching based on category: {category}", flush=True)
         if (category == "ingest"):
             task_success = self.__ingest_message_handler(self.message)
         elif (category == "task_management"):
             task_success = self.__task_management_message_handler(self.message)
         elif (category == "service"):
             task_success = self.__service_message_handler(self.message)
         elif (category == "cache_management"):
             task_success = self.__cache_management_message_handler(self.message)
 
-        #Sometimes the ack/nack might be sent in the handler
         if (task_success != None):
             if not task_success:
-                # TODO: ack is sent automatically after task completes
-                # TODO: unsure how nack works in the case of celery
                 job_tracker.set_job_status('failed', job_ticket_id, "failed")
-                print('Task unsuccessful')
-                # self.conn.nack(message_id, self._sub_id)
+                logger.error('Task unsuccessful')
 
-        #TODO- Handle
-        print('processed message for job id {}'.format(job_ticket_id))
+        logger.info('processed message for job id {}'.format(job_ticket_id))
 
     def __ingest_message_handler(self, message_data):
-        print("************************ MQUTILS MQLISTENER - INGEST_MESSAGE_HANDLER *******************************")
+        logger.debug("************************ MQUTILS MQLISTENER - INGEST_MESSAGE_HANDLER *******************************")
         job_ticket_id = message_data.get('job_ticket_id')
-        print('job_ticket_id {}'.format(job_ticket_id))
+        logger.info('__ingest_message_handler job_ticket_id {}'.format(job_ticket_id))
         parent_job_ticket_id = message_data.get('parent_job_ticket_id', None)
-        print('parent_job_ticket_id {}'.format(parent_job_ticket_id))
+        logger.info('parent_job_ticket_id {}'.format(parent_job_ticket_id))
         task_name = message_data.get('task_name')
-        print('task_name {}'.format(task_name))
+        logger.info('task_name {}'.format(task_name))
         previous_step_status = message_data.get('previous_step_status', 'success')
-        print('previous_step_status {}'.format(previous_step_status))
+        logger.info('previous_step_status {}'.format(previous_step_status))
         task_success = False
         worker_url_endpoint = "do_task"
 
         try:
-            print('set_job_status to running')
+            logger.info('set_job_status to running')
             job_tracker.set_job_status('running', job_ticket_id)
         except Exception as e:
-            print(e)
+            logger.error(e)
             return False
 
         #Send a message to the task manager queue as long as this isn't the task manager message
         tm_message = mqutils.create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id)
-        print('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
+        logger.info('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
         celeryapp.execute.send_task("tasks.tasks.do_task", args=[tm_message], kwargs={}, queue=_tm_queue)
 
         # Run the service
         # Check if previous step status was successful
         if previous_step_status and 'fail' not in previous_step_status:
             # Update timestamp file before do task
-            print('BEFORE DO TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
-            print('CALLING DO TASK')
-            print('job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
+            logger.info('Calling do_task for job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
 
             worker_url_endpoint = "do_task"
 
             nextmessage = mqutils.create_next_queue_message(job_ticket_id, parent_job_ticket_id)
-            print('create_next_queue_message nextmessage {}'.format(nextmessage))
+            logger.info('create_next_queue_message nextmessage {}'.format(nextmessage))
 
         else:
-            # Update timestamp file before revert task
-            print('BEFORE REVERT TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
             job_tracker.update_timestamp(job_ticket_id)
 
-            print('CALLING REVERT TASK')
-            print('job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
+            logger.info('Calling revert_task for job_ticket_id {} task_name {}'.format(job_ticket_id, task_name))
             worker_url_endpoint = "revert_task"
 
             # Create next queue message
             nextmessage = mqutils.create_revert_message(job_ticket_id, parent_job_ticket_id)
-            print('create_revert_message nextmessage {}'.format(nextmessage))
+            logger.info('create_revert_message nextmessage {}'.format(nextmessage))
         try:
             #Update the timestamp
             job_tracker.update_timestamp(job_ticket_id)
-            print("SUCCESSFULLY UPDATED TIMESTAMP job_ticket_id {} parent_job_ticket_id {}".format(job_ticket_id, parent_job_ticket_id))
+            logger.info("Successfully updated timestampf for job_ticket_id {} parent_job_ticket_id {}".format(job_ticket_id, parent_job_ticket_id))
         except Exception as e:
-            print(e)
+            logger.error(e)
             return False
 
         # Call worker class do task method
         try:
             worker_response = call_worker_do_task(task_name, job_ticket_id, parent_job_ticket_id, worker_url_endpoint)
             task_success = handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id)
-            print("SUCCESS IN WORKER RESPONSE TRY BLOCK")
+            logger.info("SUCCESS IN WORKER RESPONSE TRY BLOCK")
         except Exception as e:
-            print(e)
+            logger.error(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
         if (task_success):
             # Update timestamp file after task is complete
-            print('AFTER TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
+            logger.debug('AFTER TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
             job_tracker.update_timestamp(job_ticket_id)
             if nextmessage is None:
                 job_tracker.set_job_status(previous_step_status, job_ticket_id)
-                #There are no more items to queue so the job is actually finished.
-                #TODO: LTSIIIF-499 Call manifest services at the end of the workflow
-                print('******** LAST TASK COMPLETED ********')
-                print('previous_step_status {} job_ticket_id {} parent_job_ticket_id {}'.format(previous_step_status, job_ticket_id, parent_job_ticket_id))
+                logger.debug('******** LAST TASK COMPLETED ********')
+                logger.info('previous_step_status {} job_ticket_id {} parent_job_ticket_id {}'.format(previous_step_status, job_ticket_id, parent_job_ticket_id))
             else:
                 try:
                     json_message = json.loads(nextmessage)
-                    print(json_message)
+                    logger.info(json_message)
                 except ValueError as e:
-                    print(e)
+                    logger.error(e)
                     job_tracker.append_error(job_ticket_id, 'Unable to get parse the next queue message',  traceback.format_exc(), False)
                     raise e
 
                 # Set the queue name to match the worker type
                 worker_type = json_message["event"]
                 queue = worker_type
-                print('worker_type {}'.format(worker_type))
+                logger.info('worker_type {}'.format(worker_type))
                 tracker_doc = job_tracker.get_tracker_document(job_ticket_id)
                 # Update the number of tries in the tracker file
                 tracker_doc["job_management"]["numberOfTries"] = 0
                 tracker_doc["job_management"]["current_step"] = json_message["current_step"]
                 tracker_doc["job_management"]["job_status"] = "queued"
                 tracker_doc["job_management"]["previous_step_status"] = json_message["previous_step_status"]
                 try:
-                    print('******** UPDATE TRACKER FILE ********')
+                    logger.debug('******** UPDATE TRACKER FILE ********')
                     updated_tracker_doc = job_tracker.replace_tracker_doc(tracker_doc)
-                    print('updated_tracker_doc {}'.format(updated_tracker_doc))
+                    logger.info('updated_tracker_doc {}'.format(updated_tracker_doc))
                 except Exception as e:
                     #TODO what to do here - what does this mean if the tracker retrieval fails?
-                    print("TRACKER RETRIEVAL FAILED")
-                    print(e, flush=True)
+                    logger.error("TRACKER RETRIEVAL FAILED")
+                    logger.error(e, flush=True)
                     raise e
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[nextmessage], kwargs={}, queue=queue)
-        print('task_success')
-        print(task_success)
+        logger.info('task_success for __ingest_message_handler:')
+        logger.info(task_success)
         return task_success
 
     def __task_management_message_handler(self, message_data):
-        print("************************ MQUTILS MQLISTENER - TASK MANAGEMENT MESSAGE HANDLER *******************************")
-        print('task management message')
+        logger.debug("************************ MQUTILS MQLISTENER - TASK MANAGEMENT MESSAGE HANDLER *******************************")
+        logger.info('__task_management_message_handler:')
         job_ticket_id = message_data.get('job_ticket_id')
         parent_job_ticket_id = message_data.get('parent_job_ticket_id', None)
         task_name = message_data.get('task_name')
-        print('TASK NAME:')
-        print(task_name)
+        logger.info(task_name)
         task_success = False
 
         #We want the task manager to watch the multi asset ingest jobs
         if (task_name == "multi_asset_ingest"):
             #Send a message to the task manager queue as long as this isn't the task manager message
-            print("MULTI ASSET INGEST TASK")
+            logger.debug("MULTI ASSET INGEST TASK")
             tm_message = mqutils.create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id)
-            print('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
+            logger.info('sending tm message {} to queue {}'.format(tm_message, _tm_queue))
             # BROKEN
             celeryapp.execute.send_task("tasks.tasks.do_task", args=[tm_message], kwargs={}, queue=_tm_queue)
 
         try:
             job_tracker.set_job_status('running', job_ticket_id)
             # Run the service
             # Update timestamp file before do task
-            print('BEFORE DO TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
+            logger.debug('BEFORE DO TASK UPDATING TIMESTAMP FILE job_ticket_id {}'.format(job_ticket_id))
             job_tracker.update_timestamp(job_ticket_id)
         except Exception as e:
-            print(e)
+            logger.error(e)
             task_success = False
 
         # Call do task
-        print("******************* CALLING WORKER API DO TASK __task_management_message_handler *******************")
+        logger.debug("******************* CALLING WORKER API DO TASK __task_management_message_handler *******************")
         try:
-            print("call_worker_api task_name {} job_ticket_id {} parent_job_ticket_id {} do_task")
+            logger.info("call_worker_api task_name {} job_ticket_id {} parent_job_ticket_id {} do_task")
             worker_response = call_worker_api(task_name, job_ticket_id, parent_job_ticket_id, 'do_task')
-            print("worker_response")
-            print(worker_response)
+            logger.info("worker_response")
+            logger.info(worker_response)
         except Exception as e:
-            print("CALLING WORKER API DO TASK FAILED")
-            print(e)
+            logger.error("CALLING WORKER API DO TASK FAILED")
+            logger.error(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
-        print("******************* HANDLE WORKER RESPONSE *******************")
+        logger.debug("******************* HANDLE WORKER RESPONSE *******************")
         try:
             task_success = handle_worker_response(job_ticket_id, worker_response, parent_job_ticket_id)
         except Exception as e:
-            print("HANDLE WORKER RESPONSE FAILED")
-            print(e)
+            logger.error("HANDLE WORKER RESPONSE FAILED")
+            logger.error(e)
             task_success = False
             job_tracker.append_error(job_ticket_id, str(e), traceback.format_exc(), True)
 
-        print("task_success")
-        print(task_success)
+        logger.info("task_success in __task_management_message_handler:")
+        logger.info(task_success)
 
         #Ack message was already handled above
         if (task_name == "multi_asset_ingest"):
             try:
-                print("MORE MULTI ASSET INGEST STUFF HERE")
                 job_status = job_tracker.get_job_status(job_ticket_id)
                 if job_status == "failed":
-                    print('JOB STATUS: FAILED')
+                    logger.error('JOB STATUS: FAILED')
                 # Successful parent jobs will be handled by the task_manager's job monitor which periodically checks in-progress
                 # jobs for stalled jobs or parent jobs where all children are complete. Upon successful completion of all child
                 # jobs, the parent will be marked by that process as successful
             except Exception as e:
                 job_tracker.append_error(job_ticket_id, f"Exception {str(e)} in job {job_ticket_id}", traceback.format_exc(), True)
 
             return None
         return task_success
 
 
     def __service_message_handler(self, message_data):
-        print('services message')
+        logger.info('services message')
         return True
 
     def __cache_management_message_handler(self, message_data, message_id):
-        print('cache management message')
+        logger.info('cache management message')
         try:
             worker_response = call_worker_api('update_cache')
         except Exception as e:
             import traceback;
-            print('Failure in cache management handler')
-            print(traceback.format_exc(), flush=True)
-            # print('Nack message_id {}'.format(message_id))
-            # self.conn.nack(message_id, self._sub_id)
-            # TODO: HOW DO WE NACK IN CELERY?
+            logger.error('Failure in cache management handler')
+            logger.error(traceback.format_exc(), flush=True)
             return False
         return True
 
 # Generalized listener based on MQListener for use with components that do not use jobtracker
 # If a next queue is returned from do_task, will place the same message it received on the specified queue
 class GenericMessageHandler():
     def __init__(self, message, worker_endpoint='do_task'):
         self.message = message
         self.worker_endpoint = worker_endpoint
 
     def handle_message(self):
-        print('received a message headers "%s"' % self.message)
+        logger.info('received a message headers "%s"' % self.message)
         task_success = False
 
         task_success = self.__generic_message_handler(self.message, self.worker_endpoint)
 
-        # #Sometimes the ack/nack might be sent in the handler
         if (task_success != None):
             if not task_success:
-                print('Task unsuccessful')
-                # TODO: HOW TO NACK A TASK?
+                logger.error('Task unsuccessful')
 
     def __generic_message_handler(self, message_data, worker_endpoint):
-        print("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************")
+        logger.debug("************************ MQUTILS MQLISTENER - GENERIC_MESSAGE_HANDLER *******************************")
         task_success = False
 
         # Call task
         try:
             worker_response = call_generic_worker_api(message_data, worker_endpoint)
             next_queue = os.getenv('NEXT_QUEUE')
             task_success = True if worker_response.get('success') else False
-            print("SUCCESS IN WORKER RESPONSE TRY BLOCK")
+            logger.info("SUCCESS IN WORKER RESPONSE TRY BLOCK")
         except Exception as e:
-            print(e)
+            logger.error(e)
             task_success = False
 
         if (task_success):
             # Update timestamp file after task is complete
             if next_queue is None:
                 #There are no more items to queue so the job is actually finished.
-                print('******** LAST TASK COMPLETED ********')
+                logger.info('******** LAST TASK COMPLETED ********')
             else:
-                print('******** TASK COMPLETED - GOING TO NEXT QUEUE ********')
+                logger.info('******** TASK COMPLETED - GOING TO NEXT QUEUE ********')
                 celeryapp.execute.send_task("tasks.tasks.do_task", args=[self.message], kwargs={}, queue=next_queue)
-        print('task_success')
-        print(task_success)
+        logger.info('task_success for __generic_message_handler')
+        logger.info(task_success)
         return task_success
 
 # NOTIFY_SUB=2
 # DLQ_SUB=3
 # recipient_separators = re.compile(r'[,;]')
 # class NotificationListener(stomp.ConnectionListener):
 #     def __init__(self, conn):
```

### Comparing `lts-mpsmqutils-2.0.2a13/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a14/mpsmqutils/mqutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os, json, time, datetime
 from contextlib import contextmanager
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from traceback import format_exc
 # Job tracker module
 import mpsjobtracker.trackers.jobtracker as jobtracker
 
+from .log_wrapper import LogWrapper
+logger = LogWrapper()
+
 jt = None
 def get_jt():
     global jt
     if not jt:
         jt = jobtracker.JobTracker()
     return jt
 
@@ -32,137 +35,135 @@
 # Logging
 #import logging
 #logging.basicConfig(level=os.environ.get('APP_LOG_LEVEL', 'INFO'))
 #logger = logging.getLogger(__name__)
 
 def create_initial_queue_message(job_ticket_id, parent_job_ticket_id = None):
     '''Creates a queue json message to be picked up by the worker'''
-    print("************************ MQUTILS - CREATE_INITIAL_QUEUE_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_INITIAL_QUEUE_MESSAGE *******************************")
     try:
         message = __create_ingest_message(job_ticket_id, 0, "success", parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_initial_queue_message")
-        print(message)
+        logger.info(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_next_queue_message(ticket_id, parent_job_ticket_id = None):
     '''Creates a message for the next task in the job'''
-    print("************************ MQUTILS - CREATE_NEXT_QUEUE_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_NEXT_QUEUE_MESSAGE *******************************")
     message = None
     try:
         message = __create_ingest_message(ticket_id, 1, "success", parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_next_queue_message")
-        print(message)
+        logger.info(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_requeue_message(ticket_id, parent_job_ticket_id = None):
     '''Creates a queue json message for the current task to be requeued'''
-    print("************************ MQUTILS - CREATE_REQUEUE_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_REQUEUE_MESSAGE *******************************")
     try:
         jt = get_jt()
         job_tracker_file = jt.get_tracker_document(ticket_id)
         job_management = job_tracker_file.get("job_management")
         if (job_management is None):
             raise Exception ('Tracker File is malformed, missing job_management')
         prev_step_status = job_management["previous_step_status"]
         message = __create_ingest_message(ticket_id, 0, prev_step_status, parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_requeue_message")
-        print(message)
+        logger.info(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_revert_message(ticket_id, parent_job_ticket_id = None):
-    print("************************ MQUTILS - CREATE_REVERT_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_REVERT_MESSAGE *******************************")
     '''Creates a queue json message to revert the previous task
          Returns None if there is no previous message'''
     message = None
     try:
         message = __create_ingest_message(ticket_id, -1, "failed", parent_job_ticket_id)
-        print("MESSAGE TO QUEUE create_revert_message")
-        print(message)
+        logger.info("MESSAGE TO QUEUE create_revert_message")
+        logger.info(message)
     except Exception as e:
-        print(e)
+        logger.error(e)
         raise(e)
     return message
 
 def create_task_manager_queue_message(job_ticket_id, parent_job_ticket_id = None):
-    print("************************ MQUTILS - CREATE_TASK_MANANGER_QUEUE_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_TASK_MANANGER_QUEUE_MESSAGE *******************************")
     json_message = {
         "job_ticket_id": job_ticket_id,
         "task_name": "task_manager_worker_inprocess",
         "previous_step_status" : "success",
         "category": "task_management"
     }
     if parent_job_ticket_id:
         json_message["parent_job_ticket_id"] = parent_job_ticket_id
     message = json.dumps(json_message)
-    print(message)
+    logger.info("create_task_manager_queue_message message:")
+    logger.info(message)
     return message
 
 NOTIFY_QUEUE = os.getenv('MQ_NOTIFY_QUEUE', '/queue/iiif_notify')
 def create_notification(sender, recipients, subject, message, method="email", **opts):
-    print("************************ MQUTILS - CREATE_NOTIFICATION *******************************")
+    logger.info("************************ MQUTILS - CREATE_NOTIFICATION *******************************")
     jt=get_jt()
     message = json.dumps({
         "from": sender,
         "to": recipients,
         "subject": subject,
         "message": message,
         "options": opts,
         "timestamp": jt.get_timestamp_utc_now(),
         "method": method
     })
-    print(message)
+    logger.info(message)
 
     with managed_mq_connect() as conn:
         conn.send(NOTIFY_QUEUE, message, headers = {"persistent": "true"})
 
 CACHE_MANAGER_QUEUE = os.getenv('MQ_CACHE_MANAGER_QUEUE', '/queue/mps-asset-db-cache')
 def create_cache_refresh_message(**opts):
-    print("************************ MQUTILS - CREATE_CACHE_REFRESH_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_CACHE_REFRESH_MESSAGE *******************************")
     jt = get_jt()
     message = json.dumps({
         "category": "cache_management",
         "timestamp": jt.get_timestamp_utc_now(),
         "options": opts
     })
-    print(message)
+    logger.info(message)
     with managed_mq_connect() as conn:
         conn.send(CACHE_MANAGER_QUEUE, message, headers = {"persistent": "true"})
 
 def create_multi_asset_ingest_queue_message(job_ticket_id):
-    print("************************ MQUTILS - CREATE_MULTI_ASSET_INGEST_QUEUE_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_MULTI_ASSET_INGEST_QUEUE_MESSAGE *******************************")
     json_message = {
         "job_ticket_id": job_ticket_id,
         "task_name": "multi_asset_ingest",
         "previous_step_status" : "success",
         "category": "task_management"
     }
-    print(json_message)
+    logger.info(json_message)
     message = json.dumps(json_message)
     return message
 
 def __create_ingest_message(ticket_id, step_number_increment, prev_step_status, parent_job_ticket_id = None):
-    print("************************ MQUTILS - CREATE_INGEST_MESSAGE *******************************")
+    logger.info("************************ MQUTILS - CREATE_INGEST_MESSAGE *******************************")
     '''Helper method for the create messages above'''
     jt = get_jt()
     job_tracker_file = jt.get_tracker_document(ticket_id)
 
     timestamp = jt.get_timestamp_utc_now()
 
     job_management = job_tracker_file.get("job_management")
     if (job_management is None):
-        print("Malformed Tracker File")
+        logger.error("Malformed Tracker File")
         raise Exception ('Tracker File is malformed, missing job_management.')
 
     current_step = int(job_management["current_step"])
     step_number = current_step + step_number_increment
     steps_list = job_management["steps"]
     # Get step by looking up the step by step number
     event = jt.filter_element_by_property(steps_list, "step_number", step_number)
@@ -179,10 +180,10 @@
         "current_step": step_number,
         "previous_step_status": prev_step_status,
         "category": "ingest"
     }
     if parent_job_ticket_id:
         msg_json["parent_job_ticket_id"] = parent_job_ticket_id
 
-    print(msg_json)
+    logger.info(msg_json)
     message = json.dumps(msg_json)
     return message
```

### Comparing `lts-mpsmqutils-2.0.2a13/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a14/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a13/setup.py` & `lts-mpsmqutils-2.0.2a14/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a13",
+    version="2.0.2a14",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

