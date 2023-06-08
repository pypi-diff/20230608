# Comparing `tmp/patio-0.1.1.tar.gz` & `tmp/patio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patio-0.1.1.tar", max compression
+gzip compressed data, was "patio-0.1.2.tar", max compression
```

## Comparing `patio-0.1.1.tar` & `patio-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    13343 2023-06-08 10:57:28.341047 patio-0.1.1/README.md
--rw-r--r--   0        0        0      580 2023-06-08 10:47:29.273489 patio-0.1.1/patio/__init__.py
--rw-r--r--   0        0        0      294 2023-06-08 10:47:29.274047 patio-0.1.1/patio/broker/__init__.py
--rw-r--r--   0        0        0     1845 2023-06-08 10:47:29.274688 patio-0.1.1/patio/broker/abc.py
--rw-r--r--   0        0        0      542 2023-06-08 10:47:29.275407 patio-0.1.1/patio/broker/memory.py
--rw-r--r--   0        0        0     1684 2023-06-08 10:47:29.276506 patio-0.1.1/patio/broker/serializer.py
--rw-r--r--   0        0        0      151 2023-06-08 10:47:29.277259 patio-0.1.1/patio/broker/tcp/__init__.py
--rw-r--r--   0        0        0    13207 2023-06-08 10:47:29.277917 patio-0.1.1/patio/broker/tcp/broker.py
--rw-r--r--   0        0        0     2765 2023-06-08 10:47:29.278972 patio-0.1.1/patio/broker/tcp/protocol.py
--rw-r--r--   0        0        0      674 2023-06-08 10:47:29.279837 patio-0.1.1/patio/compat.py
--rw-r--r--   0        0        0      329 2023-06-08 10:47:29.280419 patio-0.1.1/patio/executor/__init__.py
--rw-r--r--   0        0        0     2176 2023-06-08 10:47:29.281010 patio-0.1.1/patio/executor/asyncronous.py
--rw-r--r--   0        0        0     2663 2023-06-08 10:47:29.281647 patio-0.1.1/patio/executor/base.py
--rw-r--r--   0        0        0      547 2023-06-08 10:47:29.282312 patio-0.1.1/patio/executor/null.py
--rw-r--r--   0        0        0     1277 2023-06-08 10:47:29.282966 patio-0.1.1/patio/executor/process_pool.py
--rw-r--r--   0        0        0     1308 2023-06-08 10:47:29.283510 patio-0.1.1/patio/executor/thread_pool.py
--rw-r--r--   0        0        0        0 2023-06-08 10:47:29.283734 patio-0.1.1/patio/py.typed
--rw-r--r--   0        0        0     8769 2023-06-08 10:47:29.285807 patio-0.1.1/patio/registry.py
--rw-r--r--   0        0        0     2247 2023-06-08 10:57:48.879255 patio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14780 1970-01-01 00:00:00.000000 patio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13343 2023-06-08 10:57:28.341047 patio-0.1.2/README.md
+-rw-r--r--   0        0        0      580 2023-06-08 10:47:29.273489 patio-0.1.2/patio/__init__.py
+-rw-r--r--   0        0        0      294 2023-06-08 10:47:29.274047 patio-0.1.2/patio/broker/__init__.py
+-rw-r--r--   0        0        0     1845 2023-06-08 10:47:29.274688 patio-0.1.2/patio/broker/abc.py
+-rw-r--r--   0        0        0      542 2023-06-08 10:47:29.275407 patio-0.1.2/patio/broker/memory.py
+-rw-r--r--   0        0        0     1684 2023-06-08 10:47:29.276506 patio-0.1.2/patio/broker/serializer.py
+-rw-r--r--   0        0        0      151 2023-06-08 10:47:29.277259 patio-0.1.2/patio/broker/tcp/__init__.py
+-rw-r--r--   0        0        0    13207 2023-06-08 10:47:29.277917 patio-0.1.2/patio/broker/tcp/broker.py
+-rw-r--r--   0        0        0     2765 2023-06-08 10:47:29.278972 patio-0.1.2/patio/broker/tcp/protocol.py
+-rw-r--r--   0        0        0      674 2023-06-08 10:47:29.279837 patio-0.1.2/patio/compat.py
+-rw-r--r--   0        0        0      329 2023-06-08 10:47:29.280419 patio-0.1.2/patio/executor/__init__.py
+-rw-r--r--   0        0        0     2176 2023-06-08 10:47:29.281010 patio-0.1.2/patio/executor/asyncronous.py
+-rw-r--r--   0        0        0     2663 2023-06-08 10:47:29.281647 patio-0.1.2/patio/executor/base.py
+-rw-r--r--   0        0        0      547 2023-06-08 10:47:29.282312 patio-0.1.2/patio/executor/null.py
+-rw-r--r--   0        0        0     1277 2023-06-08 10:47:29.282966 patio-0.1.2/patio/executor/process_pool.py
+-rw-r--r--   0        0        0     1308 2023-06-08 10:47:29.283510 patio-0.1.2/patio/executor/thread_pool.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:47:29.283734 patio-0.1.2/patio/py.typed
+-rw-r--r--   0        0        0     8769 2023-06-08 10:47:29.285807 patio-0.1.2/patio/registry.py
+-rw-r--r--   0        0        0     2299 2023-06-08 11:00:12.674462 patio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14830 1970-01-01 00:00:00.000000 patio-0.1.2/PKG-INFO
```

### Comparing `patio-0.1.1/README.md` & `patio-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/__init__.py` & `patio-0.1.2/patio/__init__.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/broker/abc.py` & `patio-0.1.2/patio/broker/abc.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/broker/memory.py` & `patio-0.1.2/patio/broker/memory.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/broker/serializer.py` & `patio-0.1.2/patio/broker/serializer.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/broker/tcp/broker.py` & `patio-0.1.2/patio/broker/tcp/broker.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/broker/tcp/protocol.py` & `patio-0.1.2/patio/broker/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/compat.py` & `patio-0.1.2/patio/compat.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/executor/asyncronous.py` & `patio-0.1.2/patio/executor/asyncronous.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/executor/base.py` & `patio-0.1.2/patio/executor/base.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/executor/null.py` & `patio-0.1.2/patio/executor/null.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/executor/process_pool.py` & `patio-0.1.2/patio/executor/process_pool.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/executor/thread_pool.py` & `patio-0.1.2/patio/executor/thread_pool.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/patio/registry.py` & `patio-0.1.2/patio/registry.py`

 * *Files identical despite different names*

### Comparing `patio-0.1.1/pyproject.toml` & `patio-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "patio"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python Asynchronous Task for AsyncIO"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/patio-python/patio/"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
```

### Comparing `patio-0.1.1/PKG-INFO` & `patio-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: patio
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Asynchronous Task for AsyncIO
+Home-page: https://github.com/patio-python/patio/
 License: MIT
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

