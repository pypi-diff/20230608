# Comparing `tmp/timeitpoj-0.1.5.tar.gz` & `tmp/timeitpoj-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeitpoj-0.1.5.tar", max compression
+gzip compressed data, was "timeitpoj-0.1.6.tar", max compression
```

## Comparing `timeitpoj-0.1.5.tar` & `timeitpoj-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1944 2023-06-06 07:05:21.764410 timeitpoj-0.1.5/README.md
--rwxr-xr-x   0        0        0      960 2023-06-07 12:11:04.464924 timeitpoj-0.1.5/pyproject.toml
--rwxr-xr-x   0        0        0       35 2023-06-06 06:50:58.047770 timeitpoj-0.1.5/timeitpoj/__init__.py
--rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.5/timeitpoj/task_report.py
--rwxr-xr-x   0        0        0     6038 2023-06-07 12:03:21.244263 timeitpoj-0.1.5/timeitpoj/timeit.py
--rwxr-xr-x   0        0        0        0 2023-06-07 12:01:50.735335 timeitpoj-0.1.5/timeitpoj/timer/__init__.py
--rwxr-xr-x   0        0        0      498 2023-06-07 12:00:38.457110 timeitpoj-0.1.5/timeitpoj/timer/internal_timer.py
--rwxr-xr-x   0        0        0     2973 2023-06-07 12:03:21.248146 timeitpoj-0.1.5/timeitpoj/timer/timer.py
--rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.5/timeitpoj/utils/__init__.py
--rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.5/timeitpoj/utils/constants.py
--rwxr-xr-x   0        0        0     1141 2023-06-05 12:28:55.956023 timeitpoj-0.1.5/timeitpoj/utils/misc.py
--rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 timeitpoj-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1944 2023-06-06 07:05:21.764410 timeitpoj-0.1.6/README.md
+-rwxr-xr-x   0        0        0      960 2023-06-08 06:56:25.804921 timeitpoj-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0       35 2023-06-06 06:50:58.047770 timeitpoj-0.1.6/timeitpoj/__init__.py
+-rwxr-xr-x   0        0        0     4534 2023-06-05 12:28:55.944886 timeitpoj-0.1.6/timeitpoj/task_report.py
+-rwxr-xr-x   0        0        0     6068 2023-06-08 06:56:21.058164 timeitpoj-0.1.6/timeitpoj/timeit.py
+-rwxr-xr-x   0        0        0        0 2023-06-07 12:01:50.735335 timeitpoj-0.1.6/timeitpoj/timer/__init__.py
+-rwxr-xr-x   0        0        0      498 2023-06-07 12:00:38.457110 timeitpoj-0.1.6/timeitpoj/timer/internal_timer.py
+-rwxr-xr-x   0        0        0     3061 2023-06-07 14:15:45.437874 timeitpoj-0.1.6/timeitpoj/timer/timer.py
+-rwxr-xr-x   0        0        0        0 2023-06-03 08:09:35.298405 timeitpoj-0.1.6/timeitpoj/utils/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-06-03 08:09:35.298519 timeitpoj-0.1.6/timeitpoj/utils/constants.py
+-rwxr-xr-x   0        0        0     1141 2023-06-07 14:03:02.786124 timeitpoj-0.1.6/timeitpoj/utils/misc.py
+-rw-r--r--   0        0        0     2894 1970-01-01 00:00:00.000000 timeitpoj-0.1.6/PKG-INFO
```

### Comparing `timeitpoj-0.1.5/README.md` & `timeitpoj-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.5/pyproject.toml` & `timeitpoj-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timeitpoj"
-version = "0.1.5"
+version = "0.1.6"
 description = "yet another random library for measuring python performance"
 authors = ["Jari Van Melckebeke <jarivanmelckebeke@gmail.com>"]
 maintainers = ["Jari Van Melckebeke <jarivanmelckebeke@gmail.com>"]
 repository = "https://github.com/jvanmelckebeke/timeitpoj"
 homepage = "https://github.com/jvanmelckebeke/timeitpoj"
```

### Comparing `timeitpoj-0.1.5/timeitpoj/task_report.py` & `timeitpoj-0.1.6/timeitpoj/task_report.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.5/timeitpoj/timeit.py` & `timeitpoj-0.1.6/timeitpoj/timeit.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import time
 from distutils.util import strtobool
 import os
 from functools import wraps
 
 from timeitpoj.timer.internal_timer import InternalTimer
 from timeitpoj.task_report import TaskReport
+from timeitpoj.timer.timer import Timer
 from timeitpoj.utils.misc import reformat_units, time_to_str
 
 
 class TimeIt:
     """
     Jari's infamous timeit class for all your performance measuring needs
 
@@ -53,29 +54,29 @@
 
             self.active = bool(strtobool(os.getenv("TIME_IT", "true")))
 
     def __enter__(self):
         with self.internal_timer:
             self.start_time = time.time()
             if self.timer is None:
-                self.timer = self.Timer(self.name, self.internal_timer, None)
+                self.timer = Timer(self.name, self.internal_timer, None)
             return self.timer.__enter__()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.end_time = time.time()
         self.__print_timeit_report()
         pass
 
     @property
     def elapsed_time(self):
         return self.end_time - self.start_time if self.end_time is not None else None
 
     def __call__(self, name, *args, **kwargs):
         if self.timer is None:
-            self.timer = self.Timer(name, self.internal_timer, None)
+            self.timer = Timer(name, self.internal_timer, None)
 
         return self.timer(name)
 
     def __print_timeit_report(self):
         def print_report_title_line():
             print(f"================= [{self.name}] TIMEIT REPORT =================")
```

### Comparing `timeitpoj-0.1.5/timeitpoj/timer/timer.py` & `timeitpoj-0.1.6/timeitpoj/timer/timer.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,21 +54,24 @@
                 "elapsed_time": self.end_time - self.start_time,
                 "task_timers": self.task_timers,
             })
             return
 
         elapsed_time = self.end_time - self.start_time
 
-        self.elapsed_time = elapsed_time
         self.report_object = {
             "name": self.name,
             "elapsed_time": elapsed_time,
             "task_timers": self.task_timers
         }
 
+    @property
+    def elapsed_time(self):
+        return self.end_time - self.start_time if self.end_time is not None else None
+
     def start_timer(self):
         self.start_time = time.time()
 
     def register_task_end(self, task_report):
         self.current_task = None
         self.task_timers.append(task_report)
```

### Comparing `timeitpoj-0.1.5/timeitpoj/utils/misc.py` & `timeitpoj-0.1.6/timeitpoj/utils/misc.py`

 * *Files identical despite different names*

### Comparing `timeitpoj-0.1.5/PKG-INFO` & `timeitpoj-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeitpoj
-Version: 0.1.5
+Version: 0.1.6
 Summary: yet another random library for measuring python performance
 Home-page: https://github.com/jvanmelckebeke/timeitpoj
 License: MIT
 Keywords: timeit,performance,benchmark,time,measure
 Author: Jari Van Melckebeke
 Author-email: jarivanmelckebeke@gmail.com
 Maintainer: Jari Van Melckebeke
```

