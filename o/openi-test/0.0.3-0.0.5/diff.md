# Comparing `tmp/openi-test-0.0.3.tar.gz` & `tmp/openi-test-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openi-test-0.0.3.tar", last modified: Thu Jun  8 10:04:59 2023, max compression
+gzip compressed data, was "dist\openi-test-0.0.5.tar", last modified: Thu Jun  8 10:08:47 2023, max compression
```

## Comparing `openi-test-0.0.3.tar` & `openi-test-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 10:04:59.818999 openi-test-0.0.3/
--rw-rw-rw-   0        0        0     1994 2023-06-08 10:04:59.818000 openi-test-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 10:04:59.818999 openi-test-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-06-08 10:04:53.000000 openi-test-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:04:59.754000 openi-test-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 10:04:59.762997 openi-test-0.0.3/src/openi/
--rw-rw-rw-   0        0        0       48 2023-06-08 07:26:17.000000 openi-test-0.0.3/src/openi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:04:59.769997 openi-test-0.0.3/src/openi/dataset/
--rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.3/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.3/src/openi/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:04:59.797013 openi-test-0.0.3/src/openi/utils/
--rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.3/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.3/src/openi/utils/helper.py
--rw-rw-rw-   0        0        0     1440 2023-06-08 08:41:21.000000 openi-test-0.0.3/src/openi/utils/minio.py
--rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.3/src/openi/utils/modelarts.py
--rw-rw-rw-   0        0        0     2359 2023-06-08 08:42:20.000000 openi-test-0.0.3/src/openi/utils/obs.py
--rw-rw-rw-   0        0        0     2117 2023-06-08 08:35:24.000000 openi-test-0.0.3/src/openi/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:04:59.814008 openi-test-0.0.3/src/openi_test.egg-info/
--rw-rw-rw-   0        0        0     1994 2023-06-08 10:04:59.000000 openi-test-0.0.3/src/openi_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-08 10:04:59.000000 openi-test-0.0.3/src/openi_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:04:59.000000 openi-test-0.0.3/src/openi_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-08 10:04:59.000000 openi-test-0.0.3/src/openi_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 10:04:59.000000 openi-test-0.0.3/src/openi_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 10:08:47.959912 openi-test-0.0.5/
+-rw-rw-rw-   0        0        0     1994 2023-06-08 10:08:47.957888 openi-test-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-06-08 09:05:33.000000 openi-test-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:08:47.960899 openi-test-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-06-08 10:08:42.000000 openi-test-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:08:47.897890 openi-test-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 10:08:47.906909 openi-test-0.0.5/src/openi/
+-rw-rw-rw-   0        0        0       44 2023-06-08 10:08:34.000000 openi-test-0.0.5/src/openi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:08:47.913893 openi-test-0.0.5/src/openi/dataset/
+-rw-rw-rw-   0        0        0       22 2023-06-08 07:26:17.000000 openi-test-0.0.5/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0    10925 2023-06-08 07:26:17.000000 openi-test-0.0.5/src/openi/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:08:47.937927 openi-test-0.0.5/src/openi/utils/
+-rw-rw-rw-   0        0        0       88 2023-06-08 08:03:34.000000 openi-test-0.0.5/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     4822 2023-06-08 08:19:40.000000 openi-test-0.0.5/src/openi/utils/helper.py
+-rw-rw-rw-   0        0        0     1440 2023-06-08 08:41:21.000000 openi-test-0.0.5/src/openi/utils/minio.py
+-rw-rw-rw-   0        0        0     1718 2023-06-08 07:56:06.000000 openi-test-0.0.5/src/openi/utils/modelarts.py
+-rw-rw-rw-   0        0        0     2359 2023-06-08 08:42:20.000000 openi-test-0.0.5/src/openi/utils/obs.py
+-rw-rw-rw-   0        0        0     2117 2023-06-08 08:35:24.000000 openi-test-0.0.5/src/openi/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:08:47.955903 openi-test-0.0.5/src/openi_test.egg-info/
+-rw-rw-rw-   0        0        0     1994 2023-06-08 10:08:47.000000 openi-test-0.0.5/src/openi_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-08 10:08:47.000000 openi-test-0.0.5/src/openi_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:08:47.000000 openi-test-0.0.5/src/openi_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-08 10:08:47.000000 openi-test-0.0.5/src/openi_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 10:08:47.000000 openi-test-0.0.5/src/openi_test.egg-info/top_level.txt
```

### Comparing `openi-test-0.0.3/PKG-INFO` & `openi-test-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.0.3
+Version: 0.0.5
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # This is a test package for OpenI PyPi
```

### Comparing `openi-test-0.0.3/README.md` & `openi-test-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/setup.py` & `openi-test-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-test',
-    version='0.0.3',
+    version='0.0.5',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/liuzx/openi-pypi-test',
     author='chenzh05,liuzx',
```

### Comparing `openi-test-0.0.3/src/openi/dataset/dataset.py` & `openi-test-0.0.5/src/openi/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/src/openi/utils/helper.py` & `openi-test-0.0.5/src/openi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/src/openi/utils/minio.py` & `openi-test-0.0.5/src/openi/utils/minio.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/src/openi/utils/modelarts.py` & `openi-test-0.0.5/src/openi/utils/modelarts.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/src/openi/utils/obs.py` & `openi-test-0.0.5/src/openi/utils/obs.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/src/openi/utils/utils.py` & `openi-test-0.0.5/src/openi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openi-test-0.0.3/src/openi_test.egg-info/PKG-INFO` & `openi-test-0.0.5/src/openi_test.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-test
-Version: 0.0.3
+Version: 0.0.5
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/liuzx/openi-pypi-test
 Author: chenzh05,liuzx
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Description: # This is a test package for OpenI PyPi
```

