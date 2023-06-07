# Comparing `tmp/pipd-0.1.5.tar.gz` & `tmp/pipd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.1.5.tar", last modified: Wed Jun  7 17:04:06 2023, max compression
+gzip compressed data, was "pipd-0.1.6.tar", last modified: Wed Jun  7 23:46:06 2023, max compression
```

## Comparing `pipd-0.1.5.tar` & `pipd-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:04:06.703185 pipd-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 17:04:06.703185 pipd-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-07 17:03:52.000000 pipd-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:04:06.699185 pipd-0.1.5/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:04:06.703185 pipd-0.1.5/pipd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/filter_cached.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/read_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/unbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/functions/write_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:04:06.703185 pipd-0.1.5/pipd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-07 17:03:52.000000 pipd-0.1.5/pipd/tests/test_pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:04:06.699185 pipd-0.1.5/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 17:04:06.000000 pipd-0.1.5/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 17:04:06.000000 pipd-0.1.5/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:04:06.000000 pipd-0.1.5/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 17:04:06.000000 pipd-0.1.5/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:04:06.703185 pipd-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 17:03:52.000000 pipd-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.445006 pipd-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 23:46:06.445006 pipd-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-07 23:45:54.000000 pipd-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.433007 pipd-0.1.6/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.441007 pipd-0.1.6/pipd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/functions/write_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.441007 pipd-0.1.6/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-07 23:45:54.000000 pipd-0.1.6/pipd/tests/test_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:06.433007 pipd-0.1.6/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 23:46:06.000000 pipd-0.1.6/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 23:46:06.445006 pipd-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 23:45:54.000000 pipd-0.1.6/setup.py
```

### Comparing `pipd-0.1.5/README.md` & `pipd-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 ```py
 for item in pipe:
     # do something with item
 ```
 
 _Iterate over the pipeline one item at a time_
 ```py
-next(pipe)
+it = iter(pipe)
+next(it)
+next(it)
 ```
 
 _Use a meta pipeline (i.e. functional only)_
 ```py
 pipe = Pipe.map(lambda x: x + 1)
 
 pipe([1, 2, 3, 4, 5]).list() == [2, 3, 4, 5, 6]
@@ -36,81 +38,68 @@
 
 
 ### `map`
 ```py
 from pipd import Pipe
 
 pipe = Pipe(1, 2, 3).map(lambda x: x * 2)
-
-print(next(pipe))
-print(next(pipe))
-print(next(pipe))
+print(list(pipe))
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
-2
-4
-6
+[2, 4, 6]
 ```
 
 </details>
 
 _Map items to parallel workers_
 ```py
 from pipd import Pipe
 
 pipe = Pipe(1, 2, 3).map(lambda x: x * 2, num_workers=2) # parallel map (note: order is not guaranteed)
-
-print(next(pipe))
-print(next(pipe))
-print(next(pipe))
+print(list(pipe))
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
-4
-2
-6
+[2, 4, 6]
 ```
 
 </details>
 
 ### `filter`
 
 ```py
 from pipd import Pipe
 
 pipe = Pipe(1, 2, 3).filter(lambda x: x != 1)
-
-print(next(pipe))
-print(next(pipe))
+print(list(pipe))
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
-2
-3
+[2, 3]
 ```
 
 </details>
 
 ### `side`
 
 Applies a function on each item in the pipeline without changing the item, useful for logging, saving state, etc.
 ```py
 from pipd import Pipe
 
 pipe = Pipe(1, 2, 3).side(lambda x: print('side', x))
-
-print(next(pipe))
-print(next(pipe))
+it = iter(pipe)
+print(next(it))
+print(next(it))
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
 side 1
 1
@@ -121,18 +110,18 @@
 </details>
 
 ### `batch`
 ```py
 from pipd import Pipe
 
 pipe = Pipe(1, 2, 3, 4, 5).batch(2)
-
-print(next(pipe))
-print(next(pipe))
-print(next(pipe))
+it = iter(pipe)
+print(next(it))
+print(next(it))
+print(next(it))
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
 [1, 2]
 [3, 4]
@@ -143,41 +132,32 @@
 
 ### `unbatch`
 
 ```py
 from pipd import Pipe
 
 pipe = Pipe([1, 2], [3], [4, 5]).unbatch()
-
-print(next(pipe))
-print(next(pipe))
-print(next(pipe))
-print(next(pipe))
-print(next(pipe))
+print(list(pipe))
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
-1
-2
-3
-4
-5
+[1, 2, 3, 4, 5]
 ```
 
 </details>
 
 ### `log`
 
 ```py
 from pipd import Pipe
 
 pipe = Pipe(range(10)).log()
-pipe() # run the pipeline
+list(pipe) # runs the pipeline
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
 0
 1
@@ -194,15 +174,15 @@
 </details>
 
 ### `limit`
 ```py
 from pipd import Pipe
 
 pipe = Pipe(range(10)).limit(5).log()
-pipe() # run the pipeline
+list(pipe) # runs the pipeline
 ```
 
 <details> <summary> Show output </summary>
 
 ```py
 0
 1
```

### Comparing `pipd-0.1.5/pipd/functions/batch.py` & `pipd-0.1.6/pipd/functions/batch.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/filter.py` & `pipd-0.1.6/pipd/functions/filter.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/filter_cached.py` & `pipd-0.1.6/pipd/functions/filter_cached.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/map.py` & `pipd-0.1.6/pipd/functions/map.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,28 @@
     FIRST_COMPLETED,
     ProcessPoolExecutor,
     ThreadPoolExecutor,
     wait,
 )
 from typing import Callable, Iterable, Iterator, Optional, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Function, Pipe, log_traceback_and_continue
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-def log_and_continue(exception: Exception):
-    print(repr(exception))
-
-
 class Map(Function):
     def __init__(
         self,
         fn: Callable[[T], U],
         num_workers: int = 0,
         buffer: Optional[int] = None,
         mode: str = "multithread",
-        handler: Callable = log_and_continue,
+        handler: Callable = log_traceback_and_continue,
     ) -> None:
         assert mode in ["multithread", "multiprocess"]
         self.fn = fn
         self.num_workers = num_workers
         self.buffer = buffer
         self.mode = mode
         self.handler = handler
```

### Comparing `pipd-0.1.5/pipd/functions/read_csv.py` & `pipd-0.1.6/pipd/functions/read_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/read_files.py` & `pipd-0.1.6/pipd/functions/read_files.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/read_lines.py` & `pipd-0.1.6/pipd/functions/read_lines.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/shuffle.py` & `pipd-0.1.6/pipd/functions/shuffle.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/side.py` & `pipd-0.1.6/pipd/functions/side.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from typing import Callable, Iterable, Iterator, TypeVar
 
-from pipd import Function, Pipe
+from pipd import Function, Pipe, log_traceback_and_continue
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
-def log_and_continue(exception: Exception):
-    print(repr(exception))
-
-
 class Side(Function):
     def __init__(
         self,
         fn: Callable[[T], U],
         num_workers: int = 0,
         mode: str = "multithread",
-        handler: Callable = log_and_continue,
+        handler: Callable = log_traceback_and_continue,
     ) -> None:
         assert mode in ["multithread", "multiprocess"]
         self.fn = fn
         self.num_workers = num_workers
         self.mode = mode
         self.handler = handler
```

### Comparing `pipd-0.1.5/pipd/functions/tqdm.py` & `pipd-0.1.6/pipd/functions/tqdm.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/functions/write_csv.py` & `pipd-0.1.6/pipd/functions/write_csv.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/tests/test_functions.py` & `pipd-0.1.6/pipd/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pipd-0.1.5/pipd/tests/test_pipe.py` & `pipd-0.1.6/pipd/tests/test_pipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     assert list(pipe) == [0, 1, 2, 3]
 
     class ClassWithGetItem:
         def __getitem__(self, key):
             return key
 
     pipe = Pipe(ClassWithGetItem())
-    assert next(pipe) == 0
-    assert next(pipe) == 1
-    assert next(pipe) == 2
+    it = iter(pipe)
+    assert next(it) == 0
+    assert next(it) == 1
+    assert next(it) == 2
 
     pipe = Pipe(0, 1, 2, 3)
 
     def gen():
         yield from pipe
 
     assert list(gen()) == [0, 1, 2, 3]
@@ -32,12 +33,12 @@
     pipe = Pipe
     assert list(pipe(0, 1, 2, 3)) == [0, 1, 2, 3]
 
     pipe = Pipe.map(lambda x: x + 1)
     assert list(pipe(0, 1, 2, 3)) == [1, 2, 3, 4]
 
 
-def test_merge():
-    pipe0 = Pipe(0, 0, 0, 0, 0, 0)
-    pipe1 = Pipe(1, 1, 1, 1, 1, 1)
-    pipe = Pipe.merge(pipe0, pipe1, weights=[3, 1])
-    print(list(pipe))
+# def test_merge():
+#     pipe0 = Pipe(0, 0, 0, 0, 0, 0)
+#     pipe1 = Pipe(1, 1, 1, 1, 1, 1)
+#     pipe = Pipe.merge(pipe0, pipe1, weights=[3, 1])
+#     print(list(pipe))
```

### Comparing `pipd-0.1.5/pipd.egg-info/SOURCES.txt` & `pipd-0.1.6/pipd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

