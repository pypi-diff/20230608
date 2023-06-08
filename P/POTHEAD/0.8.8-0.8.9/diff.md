# Comparing `tmp/POTHEAD-0.8.8.tar.gz` & `tmp/POTHEAD-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "POTHEAD-0.8.8.tar", last modified: Thu Jun  1 08:16:53 2023, max compression
+gzip compressed data, was "POTHEAD-0.8.9.tar", last modified: Wed Jun  7 09:28:04 2023, max compression
```

## Comparing `POTHEAD-0.8.8.tar` & `POTHEAD-0.8.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.8/LICENSE
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/PKG-INFO
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-01 08:16:53.872469 POTHEAD-0.8.8/POTHEAD.egg-info/
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/PKG-INFO
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/SOURCES.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/dependency_links.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       76 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/requires.txt
--rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-06-01 08:16:53.000000 POTHEAD-0.8.8/POTHEAD.egg-info/top_level.txt
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.8/README.md
-drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/pothead/
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/__init__.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.8/pothead/cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.8/pothead/gating.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8196 2023-05-31 15:04:17.000000 POTHEAD-0.8.8/pothead/oob_response.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/resource_balancer.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/server.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    11721 2023-06-01 07:59:46.000000 POTHEAD-0.8.8/pothead/subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.8/pothead/test_cgroups.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.8/pothead/test_resource_balancer.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    15931 2023-06-01 07:59:46.000000 POTHEAD-0.8.8/pothead/test_subprocess_middleware.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    10257 2023-05-31 15:30:55.000000 POTHEAD-0.8.8/pothead/test_worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1173 2023-02-09 14:53:08.000000 POTHEAD-0.8.8/pothead/util.py
--rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    17037 2023-06-01 07:59:46.000000 POTHEAD-0.8.8/pothead/worker.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.8/pothead/wsgi_typing.py
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-06-01 08:16:53.876469 POTHEAD-0.8.8/setup.cfg
--rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      876 2023-06-01 08:10:50.000000 POTHEAD-0.8.8/setup.py
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-07 09:28:04.001194 POTHEAD-0.8.9/
+-rw-r--r--   0 ulrikm    (1000) ulrikm    (1000)    10174 2019-07-16 19:09:21.000000 POTHEAD-0.8.9/LICENSE
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-07 09:28:03.997194 POTHEAD-0.8.9/PKG-INFO
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-07 09:28:03.993193 POTHEAD-0.8.9/POTHEAD.egg-info/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     4177 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/PKG-INFO
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      517 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)        1 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      114 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/requires.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)        8 2023-06-07 09:28:03.000000 POTHEAD-0.8.9/POTHEAD.egg-info/top_level.txt
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3700 2021-06-10 19:44:43.000000 POTHEAD-0.8.9/README.md
+drwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)        0 2023-06-07 09:28:03.997194 POTHEAD-0.8.9/pothead/
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       17 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/__init__.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2934 2023-03-15 11:01:30.000000 POTHEAD-0.8.9/pothead/cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     7298 2023-03-15 10:50:06.000000 POTHEAD-0.8.9/pothead/gating.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     8134 2023-06-01 23:10:54.000000 POTHEAD-0.8.9/pothead/oob_response.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2451 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/resource_balancer.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)     2494 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/server.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    12045 2023-06-02 15:32:39.000000 POTHEAD-0.8.9/pothead/subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2282 2023-03-15 11:07:34.000000 POTHEAD-0.8.9/pothead/test_cgroups.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     2569 2021-06-10 15:08:55.000000 POTHEAD-0.8.9/pothead/test_resource_balancer.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    16421 2023-06-02 16:27:07.000000 POTHEAD-0.8.9/pothead/test_subprocess_middleware.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)    13439 2023-06-07 08:39:25.000000 POTHEAD-0.8.9/pothead/test_worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     3784 2023-06-01 23:07:19.000000 POTHEAD-0.8.9/pothead/util.py
+-rwxrwxr-x   0 ulrikm    (1000) ulrikm    (1000)    14816 2023-06-02 16:27:07.000000 POTHEAD-0.8.9/pothead/worker.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)     1239 2021-06-10 19:40:00.000000 POTHEAD-0.8.9/pothead/wsgi_typing.py
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)       38 2023-06-07 09:28:04.001194 POTHEAD-0.8.9/setup.cfg
+-rw-rw-r--   0 ulrikm    (1000) ulrikm    (1000)      914 2023-06-07 09:25:29.000000 POTHEAD-0.8.9/setup.py
```

### Comparing `POTHEAD-0.8.8/LICENSE` & `POTHEAD-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/PKG-INFO` & `POTHEAD-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.8
+Version: 0.8.9
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.8/POTHEAD.egg-info/PKG-INFO` & `POTHEAD-0.8.9/POTHEAD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: POTHEAD
-Version: 0.8.8
+Version: 0.8.9
 Summary: A reverse-http proxy implementation for non-concurrent requests
 Home-page: https://gitlab.com/rawler/pothead
 Author: Ulrik Mikaelsson
 Author-email: ulrik.mikaelsson@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `POTHEAD-0.8.8/POTHEAD.egg-info/SOURCES.txt` & `POTHEAD-0.8.9/POTHEAD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/README.md` & `POTHEAD-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/cgroups.py` & `POTHEAD-0.8.9/pothead/cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/gating.py` & `POTHEAD-0.8.9/pothead/gating.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/oob_response.py` & `POTHEAD-0.8.9/pothead/oob_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,35 @@
-from collections import deque
 from logging import getLogger
 from os import environ, urandom
 from threading import Lock, Thread, Timer
 from time import monotonic, sleep
-from typing import Any, Dict, Optional, Sequence, Tuple, Generic, TypeVar, Callable
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterator,
+    Optional,
+    Sequence,
+    Tuple,
+    Generic,
+    TypeVar,
+    Callable,
+)
 from warnings import warn
 
 from werkzeug.serving import make_server
 
 from .wsgi_typing import (
     Environ,
     ExcInfo,
     ResponseStream,
     StartResponse,
     WsgiApplication,
 )
-from .util import ThreadsTracker
+from .util import SocketCheckingWSGIHandler, ThreadsTracker
 
 # Interval of how often to attempt cleanup of unclaimed jobs
 CLEANUP_INTERVAL_SECONDS = float(environ.get("OOB_CLEANUP_INTERVAL_SECONDS", "5"))
 
 # Maximum time a process is allowed to remain unclaimed before attempting to clean it up
 ITEM_EXPIRY_SECONDS = float(environ.get("OOB_ITEM_EXPIRY_SECONDS", "20"))
 
@@ -102,37 +112,14 @@
                 if expires_at > now:
                     new_dict[key] = (expires_at, job)
                 elif hasattr(job, "close"):
                     job.close()
             self._dict = new_dict
 
 
-class PeekableIterator(object):
-    def __init__(self, inner):
-        self._inner = iter(inner)
-        self._cache = deque()
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        if len(self._cache):
-            return self._cache.popleft()
-        else:
-            return next(self._inner)
-
-    def peek_next(self):
-        if not len(self._cache):
-            return self._cache.append(next(self._inner))
-        return self._cache[0]
-
-    def close(self):
-        getattr(self._inner, "close", lambda: None)()
-
-
 AtomicReferenceT = TypeVar("AtomicReferenceT")
 
 
 class AtomicReference(Generic[AtomicReferenceT]):
     def __init__(self):
         self._lock = Lock()
 
@@ -145,14 +132,33 @@
             self.data = data
 
     def get(self) -> AtomicReferenceT:
         with self._lock:
             return self.data
 
 
+def take_until(
+    iterator: Iterator[bytes], condition: Callable[[], bool]
+) -> Generator[bytes, None, Iterator[bytes]]:
+    """Yields chunks until the first one after which condition is true. That chunk, and all the remaining chunks, are
+    returned via generator-return, as a new generator"""
+
+    def trimmed_generator(first_value):
+        yield first_value
+        yield from iterator
+
+    for chunk in iterator:
+        if condition():
+            return trimmed_generator(chunk)
+        else:
+            yield chunk
+
+    return iter(())
+
+
 class OutOfBandResponder:
     def __init__(
         self,
         wrapped_app: WsgiApplication,
         port=0,
         cleanup_interval_seconds: Optional[float] = None,
         item_expiry_seconds: Optional[float] = None,
@@ -164,15 +170,21 @@
 
         self._job_transfer = KeyedTransfer(
             cleanup_interval_seconds, item_expiry_seconds
         )
         self.wrapped_app = wrapped_app
 
         wsgi_app = self._content_response_wsgi
-        self._server = make_server("0.0.0.0", port=port, app=wsgi_app, threaded=True)
+        self._server = make_server(
+            "0.0.0.0",
+            port=port,
+            app=wsgi_app,
+            threaded=True,
+            request_handler=SocketCheckingWSGIHandler,
+        )
         responder_service = Thread(target=self._server.serve_forever)
         responder_service.daemon = True
         responder_service.start()
         self._worker_tracker = ThreadsTracker()
         self._service_port = self._server.port
 
     def _content_response_wsgi(self, environ, start_response):
@@ -223,40 +235,32 @@
             exc_info: Optional[ExcInfo] = None,
         ):
             if start_response_called.is_set():
                 warn("start_response called more than once")
             else:
                 start_response_called.set((status, headers, exc_info))
 
-        response = PeekableIterator(self.wrapped_app(environ, my_start_response))
-
-        while not start_response_called.is_set():
-            try:
-                response.peek_next()
-            except StopIteration:
-                if start_response_called.is_set():
-                    break
-                else:
-                    msg = "Application Terminated Without Response"
-                    LOGGER.error(msg)
-                    start_response("500 Internal Error", (), None)
-                    return [msg.encode()]
+        response_chunks = yield from take_until(
+            self.wrapped_app(environ, my_start_response), start_response_called.is_set
+        )
+        if not start_response_called:
+            msg = "Application Terminated Without Response"
+            LOGGER.error(msg)
+            return
 
         (status, headers, exc_info) = start_response_called.get()
-
         if not exc_info and status.startswith("200 "):
             on_done = assume_cleanup()
-            key = self._job_transfer.push(Response(headers, response, on_done))
+            key = self._job_transfer.push(Response(headers, response_chunks, on_done))
             start_response(
                 "303 See Other",
                 (
                     (
                         "Location",
                         f"http://{environ['SERVER_NAME']}:{self._service_port}/{key}",
                     ),
                 ),
                 None,
             )
-            return []
         else:
             start_response(status, headers, exc_info)
-            return response
+            yield from response_chunks
```

### Comparing `POTHEAD-0.8.8/pothead/resource_balancer.py` & `POTHEAD-0.8.9/pothead/resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/server.py` & `POTHEAD-0.8.9/pothead/server.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/subprocess_middleware.py` & `POTHEAD-0.8.9/pothead/subprocess_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 """
 
 import io
 import multiprocessing
 import psutil
 from logging import Logger
 from multiprocessing.connection import Connection
+from re import compile
+from setproctitle import setproctitle
 from tblib import pickling_support
 from threading import Thread
 import werkzeug
 
 from typing import (
     cast,
     Any,
@@ -35,14 +37,15 @@
     WsgiApplication,
 )
 
 # So that exception tracebacks can be moved across process boundaries
 pickling_support.install()
 
 INTERRUPTIBLE_INTERVAL_S = 0.5
+NAME_FILTER = compile(r"[^\w\.\-]")
 
 
 class MsgStartResponse(NamedTuple):
     """
     Sent when the wrapped WSGI app has invoked the `start_response` callback.
     """
 
@@ -99,25 +102,22 @@
 
 
 class SubprocessMiddleware:
     def __init__(
         self,
         logger: Logger,
         wrapped_app: WsgiApplication,
-        *,
-        process_name: str = "WSGI request subprocess",
     ):
         """
         wrapped_app: WsgiApplication
             The underlying WSGI app, which will have each of its requests called
             in a separate subprocess.
         """
         self.logger = logger
         self.wrapped_app = wrapped_app
-        self.process_name = process_name
 
         # Use a forkserver with the app's module preloaded, to make the
         # spawning of subprocesses for each request faster.
         self.forkserver_context = multiprocessing.get_context("forkserver")
         preload_module_names = [wrapped_app.__module__]
         self.forkserver_context.set_forkserver_preload(preload_module_names)
 
@@ -162,15 +162,14 @@
             args=(self.logger, environ, wsgi_input_writer),
         )
 
         # Setup up the subprocess for running the wrapped WSGI app
         (msg_reader, msg_writer) = self.forkserver_context.Pipe(duplex=False)
         subprocess = self.forkserver_context.Process(
             target=subprocess_main,
-            name=self.process_name,
             args=(
                 self.wrapped_app,
                 new_environ,
                 msg_writer,
                 wsgi_input_reader,
                 reset_cpu_reservation is not None,
             ),
@@ -213,16 +212,19 @@
                 elif isinstance(msg, MsgDone):
                     break
                 else:
                     assert (
                         False
                     ), f"Got unknown message type from WSGI subprocess: {msg}"
         finally:
-            _kill_process_and_its_descendants(subprocess)
-            request_sender_thread.join()
+            if subprocess.pid is None:
+                self.logger.info("Process failed startup, not killing")
+            else:
+                _kill_process_and_its_descendants(subprocess)
+                request_sender_thread.join()
 
     @staticmethod
     def send_request_data(logger: Logger, environ: Environ, writer: Connection):
         try:
             with writer:
                 request_data = werkzeug.Request(
                     cast(Dict[str, Any], environ)
@@ -251,14 +253,19 @@
     environ: Environ,
     msg_writer: Connection,
     wsgi_input_reader: Connection,
     has_reset_cpu_reservation_callback,
 ):
     with msg_writer, wsgi_input_reader:
         try:
+            request_id = NAME_FILTER.sub("", environ.get("HTTP_X_REQUEST_ID", ""))
+            if request_id:
+                setproctitle(f"ph-worker:{request_id}")
+            else:
+                setproctitle("ph-worker (anon)")
 
             def wrapped_start_response(
                 http_status: str,
                 headers: Sequence[Tuple[str, str]],
                 exc_info: Optional[ExcInfo] = None,
             ) -> WriteCallable:
                 """Implements the "start response callback" WSGI interface"""
```

### Comparing `POTHEAD-0.8.8/pothead/test_cgroups.py` & `POTHEAD-0.8.9/pothead/test_cgroups.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/test_resource_balancer.py` & `POTHEAD-0.8.9/pothead/test_resource_balancer.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/pothead/test_subprocess_middleware.py` & `POTHEAD-0.8.9/pothead/test_subprocess_middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import io
 import os
 import subprocess
 from logging import getLogger
 from uuid import uuid4
-from psutil import Process, process_iter
+from psutil import Process, process_iter, Error as PsError
 from threading import Thread
 import pytest
 import signal
 import sys
-import time
 import timeout_decorator
+from time import sleep, monotonic
 import traceback
 from typing import (
     Any,
     Callable,
     cast,
     Dict,
     Iterable,
@@ -112,23 +112,23 @@
             os.kill(os.getpid(), signal.SIGKILL)
         elif request.path == "/test_globals_not_reinitialized_for_each_request":
             start_response("200 OK", [], None)
             yield f"TEST_GLOBAL_VAR: {TEST_GLOBAL_VAR}".encode("utf-8")
         elif request.path == "/hang_forever":
             start_response("200 OK", [], None)
             while True:
-                time.sleep(60)
+                sleep(60)
         elif request.path in [
             "/test_successful_subprocess_is_shut_down",
             "/test_failing_subprocess_is_shut_down",
         ]:
 
             def sleep_forever():
                 while True:
-                    time.sleep(1)
+                    sleep(1)
 
             # This thread will prevent the subprocess from exiting normally
             t = Thread(target=sleep_forever, daemon=False)
             t.start()
 
             # This subprocess represents something that the app might spawn, that doesn't automatically exit on its own
             subprocess.Popen(
@@ -380,22 +380,41 @@
             assert next(response.response) == b""  # And keep yielding
         finally:
             mw.INTERRUPTIBLE_INTERVAL_S = orig_INTERRUPTIBLE_INTERVAL_S
 
     def test_closed_response_kills_subprocess(
         self,
     ) -> Optional[Exception]:
-        worker_name = str(uuid4())
-        client = Client(
-            SubprocessMiddleware(LOGGER, wrapped_app, process_name=worker_name)
-        )
+        request_id = str(uuid4())
+        client = Client(SubprocessMiddleware(LOGGER, wrapped_app))
 
-        response = client.post("/hang_forever", data=b"")
+        response = client.post(
+            "/hang_forever", data=b"", headers=[("x-request-id", request_id)]
+        )
+        wait_for(lambda: worker_running(request_id), timeout=100)
 
         assert response.status == "200 OK"
         response.response.close()
 
-        for _ in range(10):
-            if not any(filter(lambda p: worker_name in p.name(), process_iter())):
-                return
-            time.sleep(0.1)
-        raise AssertionError("Process left hanging after request-cancellation")
+        wait_for(lambda: not worker_running(request_id))
+
+
+def wait_for(condition: Callable[[], bool], *, interval=0.01, timeout=10):
+    start = monotonic()
+    while (monotonic() - start) < timeout:
+        if condition():
+            return
+        sleep(interval)
+    assert False, f"Timeout hit before {condition} matched"
+
+
+def worker_running(request_id):
+    def get_name(p):
+        try:
+            return p.name()
+        except PsError:
+            return "-"
+
+    try:
+        return any(filter(lambda p: request_id in get_name(p), process_iter()))
+    except PsError:
+        return worker_running(request_id)
```

### Comparing `POTHEAD-0.8.8/pothead/test_worker.py` & `POTHEAD-0.8.9/pothead/test_worker.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 from threading import Thread
 from time import sleep, monotonic
 from typing import Optional
 from unittest import TestCase
 from unittest.mock import MagicMock
 from urllib.request import urlopen
 from logging import INFO
+from uuid import uuid4
 
 from pytest import fixture
 
+from pothead.test_subprocess_middleware import wait_for, worker_running
+
 OOB_CLEANUP_INTERVAL_SECONDS = 0.05
 OOB_ITEM_EXPIRY_SECONDS = 0.5
 REQUEST_ID = "im-quite-unique!"
 
 from pothead.gating import wait_for_idle_cpus  # noqa: E402 override environ first
 
 from .util import ObjectProxy  # noqa: E402
@@ -26,59 +29,83 @@
     def set(self):
         self.v = True
 
     def is_set(self) -> bool:
         return self.v
 
 
-def make_demo_app(is_terminated: Flag):
-    def demo_app(environ, start_response):
-        path = environ.get("PATH_INFO")
+def demo_app(environ, start_response):
+    path = environ.get("PATH_INFO")
+    if path == "/":
+        start_response("200 OK", ())
+        yield b"Hello World!"
+    elif path == "/crash":
+        raise Exception("Nope nope nope")
+    elif path == "/slow_loris":
+        sleep(0.05)
+        start_response("200 OK", ())
+        for byte in b"This might take a while...":
+            sleep(0.1)
+            yield byte
+    elif path == "/hang_forever":
+        do_yield = environ.get("HTTP_YIELD", "").lower() == "true"
+        if environ.get("HTTP_START_RESPONSE", "").lower() == "true":
+            start_response("200 OK", ())
+        while True:
+            if do_yield:
+                yield b""
+            sleep(0.01)
+    else:
+        start_response("404 Not Found", ())
+
+
+def tracked_demo_app(is_terminated: Flag):
+    def app(environ, start_response):
         try:
-            if path == "/":
-                start_response("200 OK", ())
-                yield b"Hello World!"
-            elif path == "/crash":
-                raise Exception("Nope nope nope")
-            elif path == "/slow_loris":
-                sleep(0.05)
-                start_response("200 OK", ())
-                for byte in b"This might take a while...":
-                    sleep(0.1)
-                    yield byte
-            elif path == "/hang_forever":
-                start_response("200 OK", ())
-                while True:
-                    yield b""
-                    sleep(0.01)
-            else:
-                start_response("404 Not Found", ())
+            demo_app(environ, start_response)
         finally:
             is_terminated.set()
 
-    return demo_app
+    return app
 
 
 class WorkerConnection:
     def __init__(self, sock: socket):
         self.sock = sock
 
-    def send_request(self, path="/"):
-        self.sock.sendall(
-            f"GET {path} HTTP/1.1\r\nx-request-id: {REQUEST_ID}\r\n\r\n".encode("ascii")
-        )
+    def send_request(self, path="/", headers={}):
+        if "x-request-id" not in headers:
+            headers["x-request-id"] = REQUEST_ID
+        self.sock.sendall(f"GET {path} HTTP/1.1\r\n".encode("ascii"))
+        for k, v in headers.items():
+            self.sock.send(f"{k}: {v}\r\n".encode("ascii"))
+        self.sock.sendall(b"\r\n")
 
     def read_response(self):
         buf = b""
         read = True
         while read:
             read = self.sock.recv(1024)
             buf += read
         return buf
 
+    def parse_response(self):
+        response = self.read_response()
+        response_lines = iter(response.split(b"\r\n"))
+        (_http_version, status, *_) = next(response_lines).split()
+        headers = {}
+        for line in response_lines:
+            if line == b"":
+                break
+            (name, value) = line.split(b":", maxsplit=1)
+            headers[name.strip().lower().decode("ascii")] = str(
+                value.strip().decode("ascii")
+            )
+        return int(status), headers
+
     def disconnect(self):
         self.sock.shutdown(SHUT_RDWR)
         self.sock.close()
 
 
 class DummyBroker:
     def __init__(self):
@@ -105,15 +132,15 @@
 
     return MockBalancer
 
 
 class WorkerTest(TestCase):
     def test_load_balancing(self):
         broker_a, broker_b = (DummyBroker() for _ in range(2))
-        app = ObjectProxy(make_demo_app(Flag()))
+        app = ObjectProxy(demo_app)
         app.wait_for_slot = wait_for_idle_cpus(0, max_concurrent=10)
 
         worker = Server(
             ("", 0),
             app,
             load_balancer=mock_balancer(map(DummyBroker.addr, (broker_a, broker_b))),
         )
@@ -131,26 +158,26 @@
         connection_a.send_request()
         assert broker_a.accept(0.2) is not None
 
     def test_cancel_hung_request(self):
         broker = DummyBroker()
         request_finished = Flag()
 
-        app = ObjectProxy(make_demo_app(request_finished))
+        app = ObjectProxy(tracked_demo_app(request_finished))
         app.wait_for_slot = wait_for_idle_cpus(0, max_concurrent=10)
 
         server = Server(
             ("", 0),
             app,
             load_balancer=mock_balancer([broker.addr()]),
         )
         Thread(target=server.poll_loop, daemon=True).start()
         connection = broker.accept(0.1)
 
-        connection.send_request("/hang_forever")
+        connection.send_request("/hang_forever", {"yield": True})
         sleep(0.1)
         connection.disconnect()
 
         sleep(0.1)
 
         assert request_finished.is_set()
 
@@ -167,25 +194,25 @@
         else:
             from time import sleep
 
             while not halt():
                 sleep(0.05)
 
 
-class RedirectWorkerTest(TestCase):
+class OutOfBandResponseTest(TestCase):
     @fixture(autouse=True)
     def use_caplog(self, caplog):
         caplog.set_level(INFO)
         self.caplog = caplog
 
     def setUp(self):
         broker = DummyBroker()
         self.callbacks = MagicMock()
 
-        app = ObjectProxy(make_demo_app(Flag()))
+        app = ObjectProxy(demo_app)
         app.wait_for_slot = WaitForFirstSlot(self.callbacks)
 
         self.server = Server(
             ("", 0),
             app,
             load_balancer=mock_balancer([broker.addr()]),
             redirect_port=0,
@@ -196,23 +223,20 @@
         self.connection = broker.accept(0.1)
 
     def tearDown(self):
         self.server.shutdown()
 
     def test_response_redirect(self):
         self.connection.send_request()
-        resp = self.connection.read_response().split(b"\r\n")
+        status, headers = self.connection.parse_response()
+        assert status == 303
 
-        assert resp[0] == b"HTTP/1.1 303 See Other"
-        location = (
-            [x for x in resp if x.startswith(b"Location: ")][0].split()[1].decode()
-        )
-        real_response = urlopen(location)
-        assert real_response.status == 200
-        assert real_response.read().startswith(b"Hello World!")
+        with urlopen(headers.get("location")) as real_response:
+            assert real_response.status == 200
+            assert real_response.read().startswith(b"Hello World!")
 
     def test_reject_no_redirect(self):
         self.connection.send_request("/nonexisting")
         resp = self.connection.read_response().split(b"\r\n")
 
         assert resp[0] == b"HTTP/1.1 404 Not Found"
         assert b"Location" not in [x.split(b":") for x in resp]
@@ -222,24 +246,22 @@
         resp = self.connection.read_response().split(b"\r\n")
 
         assert resp[0] == b"HTTP/1.1 500 INTERNAL SERVER ERROR"
         assert b"Location" not in [x.split(b":") for x in resp]
 
     def test_ondone_deferred(self):
         self.connection.send_request()
-        resp = self.connection.read_response().split(b"\r\n")
+        status, headers = self.connection.parse_response()
+        assert status == 303
 
         self.callbacks.done.assert_not_called()
 
-        location = (
-            [x for x in resp if x.startswith(b"Location: ")][0].split()[1].decode()
-        )
-        real_response = urlopen(location)
-        assert real_response.status == 200
-        assert real_response.read().startswith(b"Hello World!")
+        with urlopen(headers.get("location")) as real_response:
+            assert real_response.status == 200
+            assert real_response.read().startswith(b"Hello World!")
 
         self.callbacks.done.assert_called()
 
     def test_ondone_called_for_crash(self):
         self.connection.send_request("/crash")
         self.connection.read_response()
 
@@ -282,14 +304,81 @@
         self.connection.disconnect()
 
         sleep(0.2)
 
         assert f"[{REQUEST_ID}] Elapsed: " in self.caplog.text
 
 
+class OutOfBandResponseWithSubprocessTest(TestCase):
+    def setUp(self):
+        broker = DummyBroker()
+        self.on_done = MagicMock()
+
+        self.server = Server(
+            ("", 0),
+            demo_app,
+            load_balancer=mock_balancer([broker.addr()]),
+            redirect_port=0,
+            use_request_subprocess=True,
+            oob_cleanup_interval_seconds=OOB_CLEANUP_INTERVAL_SECONDS,
+            oob_item_expiry_seconds=OOB_ITEM_EXPIRY_SECONDS,
+        )
+        Thread(
+            target=self.server._fetch_and_run_one_job,
+            kwargs={
+                "addr": broker.addr(),
+            },
+            daemon=True,
+        ).start()
+        self.connection = broker.accept(0.1)
+        self.request_id = str(uuid4())
+
+    def tearDown(self):
+        self.server.shutdown()
+
+    def test_abandoned_request_is_aborted_before_responding(self):
+        self.connection.send_request(
+            "/hang_forever",
+            {"yield": False, "start-response": False, "x-request-id": self.request_id},
+        )
+        wait_for(lambda: worker_running(self.request_id))
+
+        self.connection.disconnect()
+        wait_for(lambda: not worker_running(self.request_id), timeout=2)
+
+    def test_abandoned_request_is_aborted_when_oob_not_requested(self):
+        self.connection.send_request(
+            "/hang_forever",
+            {"yield": False, "start-response": True, "x-request-id": self.request_id},
+        )
+        status, _headers = self.connection.parse_response()
+        assert status == 303
+
+        # We never connect to read the response. Request should
+        # be aborted after OOB_CLEANUP_INTERVAL_SECONDS and
+        # OOB_ITEM_EXPIRY_SECONDS
+        wait_for(
+            lambda: not worker_running(self.request_id),
+            timeout=1 + OOB_CLEANUP_INTERVAL_SECONDS + OOB_ITEM_EXPIRY_SECONDS,
+        )
+
+    def test_abandoned_request_is_aborted_after_started_response(self):
+        self.connection.send_request(
+            "/hang_forever",
+            {"yield": False, "start-response": True, "x-request-id": self.request_id},
+        )
+        status, headers = self.connection.parse_response()
+        assert status == 303
+        with urlopen(headers.get("location")):
+            pass
+
+        # We connected, but abandoned the response before reading. Request should be aborted momentarily
+        wait_for(lambda: not worker_running(self.request_id), timeout=2)
+
+
 class TestShutdown(TestCase):
     DELAY_START_RESPONSE = 0.3
     DELAY_FINISH_RESPONSE = 0.8
 
     def setUp(self):
         broker = DummyBroker()
         self.callbacks = MagicMock()
@@ -326,21 +415,20 @@
         self.connection.read_response()
         st = self.shutdown_time()
         self.assertGreaterEqual(st, OOB_ITEM_EXPIRY_SECONDS)
         self.assertLessEqual(st, self.DELAY_FINISH_RESPONSE)
 
     def test_oob_finish_before_shutdown(self):
         self.connection.send_request()
-        resp = self.connection.read_response().split(b"\r\n")
+        status, headers = self.connection.parse_response()
+        assert status == 303
 
-        location = (
-            [x for x in resp if x.startswith(b"Location: ")][0].split()[1].decode()
-        )
-        real_response = urlopen(location)
-        assert real_response.status == 200
+        with urlopen(headers.get("location")) as real_response:
+            assert real_response.status == 200
 
-        self.assertGreaterEqual(self.shutdown_time(), self.DELAY_FINISH_RESPONSE)
+            # Still running the request, we expect it to be finished before shutdown
+            self.assertGreaterEqual(self.shutdown_time(), self.DELAY_FINISH_RESPONSE)
 
     def shutdown_time(self):
         start = monotonic()
         self.server.shutdown()
         return monotonic() - start
```

### Comparing `POTHEAD-0.8.8/pothead/worker.py` & `POTHEAD-0.8.9/pothead/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 #!/usr/bin/env python3
 
-from errno import EAGAIN
 from http import HTTPStatus
 from logging import getLogger
 from signal import SIGTERM, signal
 from socket import (
     AF_INET,
     IPPROTO_TCP,
-    MSG_DONTWAIT,
-    MSG_PEEK,
     SHUT_RDWR,
     SO_KEEPALIVE,
     SOCK_STREAM,
     SOL_SOCKET,
     TCP_KEEPCNT,
     TCP_KEEPIDLE,
     TCP_KEEPINTVL,
     getaddrinfo,
     socket,
-    error as SocketError,
 )
 from threading import Condition, Thread, Timer
 from time import monotonic, sleep
 from typing import Dict, Optional, Set
 from uuid import uuid4
 from wsgiref import simple_server
 
-from werkzeug.serving import WSGIRequestHandler, BaseWSGIServer, make_server
+from werkzeug.serving import BaseWSGIServer, make_server
 
 from .gating import wait_for_idle_cpus
 from .oob_response import OutOfBandResponder
 from .resource_balancer import BoundedResourceBalancer, ResourceLoan
 from .subprocess_middleware import SubprocessMiddleware
-from .util import ObjectProxy, ThreadsTracker
+from .util import ObjectProxy, SocketCheckingWSGIHandler, ThreadsTracker
 from .wsgi_typing import (
     WsgiApplication,
 )
 
 LOGGER = getLogger("pothead.worker")
 BROKER_CONNECT_RETRY_INTERVAL = 2
 
@@ -72,75 +68,32 @@
             self._cond.notify_all()
 
     def wait(self, timeout: float):
         with self._cond:
             self._cond.wait_for(lambda: self._set, timeout)
 
 
-class Handler(WSGIRequestHandler):
+class Handler(SocketCheckingWSGIHandler):
     protocol_version = "HTTP/1.1"
 
     def __init__(
         self, socket, address, server, cb_request_received, cb_processing_done
     ):
         self.cb_request_received = cb_request_received
         self.env = None
         self.request_id = None
         self.request_received_at = None
 
         with DeferrableCleanup(cb_processing_done) as c:
-            app = server.app
-            if isinstance(app, OutOfBandResponder):
-                app = self._oob_wrapped_app(app, c.assume)
+            if isinstance(server.app, OutOfBandResponder):
+                server = ObjectProxy(server)
+                server.app = self._oob_wrapped_app(server.app, c.assume)
 
-            app = self._socket_checking_app(app)
-
-            server = ObjectProxy(server)
-            server.app = app
             super().__init__(socket, address, server)
 
-    def _socket_checking_app(self, app) -> WsgiApplication:
-        def application(environ, start_response):
-            response_started = [False]
-
-            def wrapped_start_response(*args, **kwargs):
-                response_started[0] = True
-                return start_response(*args, **kwargs)
-
-            for chunk in app(environ, wrapped_start_response):
-                if len(chunk) == 0:
-                    # Non-empty chunks will fail by themselves when sending to client.
-                    # Empty chunks OTOH, will give us a chance to abort if client is no longer connected
-
-                    try:
-                        if len(self.request.recv(1, MSG_DONTWAIT | MSG_PEEK)) == 0:
-                            # recv() returns empty slice if client shutdown it's writing side
-                            #
-                            # Considering "closed for reading" as a sign of abandoned request is not supported by the
-                            # HTTP specification, (https://datatracker.ietf.org/doc/html/rfc9112#section-9.6).
-                            # However, it _is_ the default behavior of hyper, and we can probably get away with it
-                            # https://docs.rs/hyper/0.14.26/hyper/server/struct.Builder.html#method.http1_half_close
-                            raise ConnectionError(
-                                "Connection closed during response from server"
-                            )
-                    except SocketError as e:
-                        if e.errno != EAGAIN:
-                            raise ConnectionError(
-                                "Connection closed during response from server"
-                            ) from e
-                # By allowing empty chunks to be yielded before `start_response`, we enable early abort. But, werkzeug
-                # doesn't support even empty chunks to be yielded before `start_response` is called, so we suppress
-                # those
-                if not response_started[0] and len(chunk) == 0:
-                    continue
-
-                yield chunk
-
-        return application
-
     @staticmethod
     def _oob_wrapped_app(app, assume_cleanup) -> WsgiApplication:
         def application(environ, start_response):
             return app(environ, start_response, assume_cleanup)
 
         return application
 
@@ -266,16 +219,17 @@
 
         if inspection_port is not None:
             self.inspection_server = make_server(
                 "", inspection_port, self.inspect, threaded=True
             )
             Thread(target=self.inspection_server.serve_forever, daemon=True).start()
 
-        self.wait_for_slot = app.wait_for_slot
-        del app.wait_for_slot
+        self.wait_for_slot = getattr(app, "wait_for_slot", None)
+        if self.wait_for_slot:
+            del app.wait_for_slot
         self.app = app
         self.app = (
             SubprocessMiddleware(LOGGER, self.app)
             if use_request_subprocess
             else self.app
         )
         self.app = (
```

### Comparing `POTHEAD-0.8.8/pothead/wsgi_typing.py` & `POTHEAD-0.8.9/pothead/wsgi_typing.py`

 * *Files identical despite different names*

### Comparing `POTHEAD-0.8.8/setup.py` & `POTHEAD-0.8.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-test_deps = ["aiohttp", "werkzeug", "tblib", "timeout-decorator"]
+common_deps = ["psutil", "werkzeug>=2.1", "tblib", "setproctitle"]
+test_deps = [*common_deps, "aiohttp", "timeout-decorator"]
 
 setuptools.setup(
     name="POTHEAD",
-    version="0.8.8",
+    version="0.8.9",
     author="Ulrik Mikaelsson",
     author_email="ulrik.mikaelsson@gmail.com",
     description="A reverse-http proxy implementation for non-concurrent requests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/rawler/pothead",
     packages=setuptools.find_packages(),
-    install_requires=["psutil", "werkzeug>=2.1", "tblib"],
+    install_requires=[*common_deps],
     tests_require=test_deps,
     extras_require={
         "test": test_deps,
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
```

