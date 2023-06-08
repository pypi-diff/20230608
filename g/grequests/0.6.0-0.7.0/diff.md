# Comparing `tmp/grequests-0.6.0.tar.gz` & `tmp/grequests-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grequests-0.6.0.tar", last modified: Sun Apr  5 14:27:35 2020, max compression
+gzip compressed data, was "grequests-0.7.0.tar", last modified: Thu Jun  8 00:04:21 2023, max compression
```

## Comparing `grequests-0.6.0.tar` & `grequests-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-05 14:27:35.000000 grequests-0.6.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2020-04-05 14:27:13.000000 grequests-0.6.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1484 2020-04-05 14:27:35.000000 grequests-0.6.0/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5522 2020-04-05 14:27:13.000000 grequests-0.6.0/grequests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-05 14:27:35.000000 grequests-0.6.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1484 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-04-05 14:27:35.000000 grequests-0.6.0/grequests.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1283 2020-04-05 14:27:13.000000 grequests-0.6.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2224 2020-04-05 14:27:13.000000 grequests-0.6.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1599 2020-04-05 14:27:13.000000 grequests-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:04:21.157163 grequests-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-08 00:04:16.000000 grequests-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-08 00:04:16.000000 grequests-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 00:04:16.000000 grequests-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-08 00:04:21.157163 grequests-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-08 00:04:16.000000 grequests-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:04:21.153163 grequests-0.7.0/grequests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-08 00:04:21.000000 grequests-0.7.0/grequests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 00:04:21.000000 grequests-0.7.0/grequests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:04:21.000000 grequests-0.7.0/grequests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:04:21.000000 grequests-0.7.0/grequests.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 00:04:21.000000 grequests-0.7.0/grequests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 00:04:21.000000 grequests-0.7.0/grequests.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7442 2023-06-08 00:04:16.000000 grequests-0.7.0/grequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:04:21.157163 grequests-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-08 00:04:16.000000 grequests-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grequests-0.6.0/PKG-INFO` & `grequests-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grequests
-Version: 0.6.0
+Version: 0.7.0
 Summary: Requests + Gevent
-Home-page: https://github.com/kennethreitz/grequests
+Home-page: https://github.com/spyoungtech/grequests
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: BSD
-Description: 
-        GRequests allows you to use Requests with Gevent to make asynchronous HTTP
-        Requests easily.
-        
-        Usage
-        -----
-        
-        Usage is simple::
-        
-            import grequests
-        
-            urls = [
-                'http://www.heroku.com',
-                'http://tablib.org',
-                'http://httpbin.org',
-                'http://python-requests.org',
-                'http://kennethreitz.com'
-            ]
-        
-        Create a set of unsent Requests::
-        
-            >>> rs = (grequests.get(u) for u in urls)
-        
-        Send them all at the same time::
-        
-            >>> grequests.map(rs)
-            [<Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>]
-        
-        
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+
+GRequests allows you to use Requests with Gevent to make asynchronous HTTP
+Requests easily.
+
+Usage
+-----
+
+Usage is simple::
+
+    import grequests
+
+    urls = [
+        'http://www.heroku.com',
+        'http://tablib.org',
+        'http://httpbin.org',
+        'http://python-requests.org',
+        'http://kennethreitz.com'
+    ]
+
+Create a set of unsent Requests::
+
+    >>> rs = (grequests.get(u) for u in urls)
+
+Send them all at the same time::
+
+    >>> grequests.map(rs)
+    [<Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>]
+
+
+
```

### Comparing `grequests-0.6.0/grequests.py` & `grequests-0.7.0/grequests.py`

 * *Files 25% similar despite different names*

```diff
@@ -159,7 +159,55 @@
             yield request.response
         elif exception_handler:
             ex_result = exception_handler(request, request.exception)
             if ex_result is not None:
                 yield ex_result
 
     pool.join()
+
+
+def imap_enumerated(requests, stream=False, size=2, exception_handler=None):
+    """
+    Like imap, but yields tuple of original request index and response object
+
+    Unlike imap, failed results and responses from exception handlers that return None are not ignored. Instead, a
+    tuple of (index, None) is yielded. Additionally, the ``requests`` parameter must be a sequence of Request objects
+    (generators or other non-sequence iterables are not allowed)
+
+    The index is merely the original index of the original request in the requests list and does NOT provide any
+    indication of the order in which requests or responses are sent or received. Responses are still in arbitrary order.
+
+    ::
+        >>> rs = [grequests.get(f'https://httpbin.org/status/{i}') for i in range(200, 206)]
+        >>> for index, response in grequests.imap_enumerated(rs, size=5):
+        ...     print(index, response)
+        1 <Response [201]>
+        0 <Response [200]>
+        4 <Response [204]>
+        2 <Response [202]>
+        5 <Response [205]>
+        3 <Response [203]>
+
+
+    :param requests: a sequence of Request objects.
+    :param stream: If True, the content will not be downloaded immediately.
+    :param size: Specifies the number of requests to make at a time. default is 2
+    :param exception_handler: Callback function, called when exception occurred. Params: Request, Exception
+    """
+
+    pool = Pool(size)
+
+    def send(r):
+        return r._index, r.send(stream=stream)
+
+    requests = list(requests)
+    for index, req in enumerate(requests):
+        req._index = index
+
+    for index, request in pool.imap_unordered(send, requests):
+        if request.response is not None:
+            yield index, request.response
+        elif exception_handler:
+            ex_result = exception_handler(request, request.exception)
+            yield index, ex_result
+        else:
+            yield index, None
```

### Comparing `grequests-0.6.0/grequests.egg-info/PKG-INFO` & `grequests-0.7.0/grequests.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: grequests
-Version: 0.6.0
+Version: 0.7.0
 Summary: Requests + Gevent
-Home-page: https://github.com/kennethreitz/grequests
+Home-page: https://github.com/spyoungtech/grequests
 Author: Kenneth Reitz
 Author-email: me@kennethreitz.com
 License: BSD
-Description: 
-        GRequests allows you to use Requests with Gevent to make asynchronous HTTP
-        Requests easily.
-        
-        Usage
-        -----
-        
-        Usage is simple::
-        
-            import grequests
-        
-            urls = [
-                'http://www.heroku.com',
-                'http://tablib.org',
-                'http://httpbin.org',
-                'http://python-requests.org',
-                'http://kennethreitz.com'
-            ]
-        
-        Create a set of unsent Requests::
-        
-            >>> rs = (grequests.get(u) for u in urls)
-        
-        Send them all at the same time::
-        
-            >>> grequests.map(rs)
-            [<Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>]
-        
-        
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+
+GRequests allows you to use Requests with Gevent to make asynchronous HTTP
+Requests easily.
+
+Usage
+-----
+
+Usage is simple::
+
+    import grequests
+
+    urls = [
+        'http://www.heroku.com',
+        'http://tablib.org',
+        'http://httpbin.org',
+        'http://python-requests.org',
+        'http://kennethreitz.com'
+    ]
+
+Create a set of unsent Requests::
+
+    >>> rs = (grequests.get(u) for u in urls)
+
+Send them all at the same time::
+
+    >>> grequests.map(rs)
+    [<Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>, <Response [200]>]
+
+
+
```

### Comparing `grequests-0.6.0/LICENSE` & `grequests-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grequests-0.6.0/setup.py` & `grequests-0.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 """
 
 from setuptools import setup
 
 setup(
     name='grequests',
-    version='0.6.0',
-    url='https://github.com/kennethreitz/grequests',
+    version='0.7.0',
+    url='https://github.com/spyoungtech/grequests',
     license='BSD',
     author='Kenneth Reitz',
     author_email='me@kennethreitz.com',
     description='Requests + Gevent',
     long_description=__doc__,
     install_requires=[
         'gevent',
```

