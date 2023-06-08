# Comparing `tmp/openi-test-0.0.1.tar.gz` & `tmp/openi-test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi-test-0.0.1.tar", last modified: Thu Jun  8 09:32:19 2023, max compression
+gzip compressed data, was "dist\openi-test-0.0.2.tar", last modified: Thu Jun  8 10:00:00 2023, max compression
```

## Comparing `openi-test-0.0.1.tar` & `openi-test-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:32:19.684108 openi-test-0.0.1/
--rw-rw-rw-   0        0        0     1994 2023-06-08 09:32:19.683119 openi-test-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 09:32:19.685110 openi-test-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1099 2023-06-08 09:07:10.000000 openi-test-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:32:19.601050 openi-test-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 09:32:19.613048 openi-test-0.0.1/src/openi/
--rw-rw-rw-   0        0        0       48 2023-06-08 07:26:17.000000 openi-test-0.0.1/src/openi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:32:19.621052 openi-test-0.0.1/src/openi/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.1/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.1/src/openi/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:32:19.653107 openi-test-0.0.1/src/openi/utils/
--rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.1/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.1/src/openi/utils/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-08 08:41:21.000000 openi-test-0.0.1/src/openi/utils/minio.py
--rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.1/src/openi/utils/modelarts.py
--rw-rw-rw-   0        0        0     2359 2023-06-08 08:42:20.000000 openi-test-0.0.1/src/openi/utils/obs.py
--rw-rw-rw-   0        0        0     2117 2023-06-08 08:35:24.000000 openi-test-0.0.1/src/openi/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:32:19.678109 openi-test-0.0.1/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     1994 2023-06-08 09:32:19.000000 openi-test-0.0.1/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-08 09:32:19.000000 openi-test-0.0.1/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:32:19.000000 openi-test-0.0.1/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-08 09:32:19.000000 openi-test-0.0.1/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 09:32:19.000000 openi-test-0.0.1/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:00.947651 openi-test-0.0.2/
+-rw-rw-rw-   0        0        0     1994 2023-06-08 10:00:00.945645 openi-test-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:00:00.947651 openi-test-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-06-08 09:58:04.000000 openi-test-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:00.877930 openi-test-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:00.888644 openi-test-0.0.2/src/openi/
+-rw-rw-rw-   0        0        0       48 2023-06-08 07:26:17.000000 openi-test-0.0.2/src/openi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:00.894875 openi-test-0.0.2/src/openi/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.2/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.2/src/openi/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:00.920647 openi-test-0.0.2/src/openi/utils/
+-rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.2/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.2/src/openi/utils/helper.py
+-rw-rw-rw-   0        0        0     1440 2023-06-08 08:41:21.000000 openi-test-0.0.2/src/openi/utils/minio.py
+-rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.2/src/openi/utils/modelarts.py
+-rw-rw-rw-   0        0        0     2359 2023-06-08 08:42:20.000000 openi-test-0.0.2/src/openi/utils/obs.py
+-rw-rw-rw-   0        0        0     2117 2023-06-08 08:35:24.000000 openi-test-0.0.2/src/openi/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:00.941643 openi-test-0.0.2/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     1994 2023-06-08 10:00:00.000000 openi-test-0.0.2/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-08 10:00:00.000000 openi-test-0.0.2/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:00:00.000000 openi-test-0.0.2/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-08 10:00:00.000000 openi-test-0.0.2/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 10:00:00.000000 openi-test-0.0.2/src/openi_test.egg-info/top_level.txt
```

### Comparing `openi-test-0.0.1/PKG-INFO` & `openi-test-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # This is a test package for OpenI PyPi
```

### Comparing `openi-test-0.0.1/README.md` & `openi-test-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi/dataset/dataset.py` & `openi-test-0.0.2/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi/utils/helper.py` & `openi-test-0.0.2/src/openi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi/utils/minio.py` & `openi-test-0.0.2/src/openi/utils/minio.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi/utils/modelarts.py` & `openi-test-0.0.2/src/openi/utils/modelarts.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi/utils/obs.py` & `openi-test-0.0.2/src/openi/utils/obs.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi/utils/utils.py` & `openi-test-0.0.2/src/openi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.1/src/openi_test.egg-info/PKG-INFO` & `openi-test-0.0.2/src/openi_test.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # This is a test package for OpenI PyPi
```

