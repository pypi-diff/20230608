# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.1.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.1.tar", last modified: Thu Jun  8 03:40:36 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.2.tar", last modified: Thu Jun  8 04:03:04 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.1.tar` & `hyutils-hyutil-hoyun-lab-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 03:40:36.553621 hyutils-hyutil-hoyun-lab-0.0.1/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      598 2023-06-08 03:40:36.551602 hyutils-hyutil-hoyun-lab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.1/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 03:40:36.553988 hyutils-hyutil-hoyun-lab-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      850 2023-06-08 03:40:08.000000 hyutils-hyutil-hoyun-lab-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:40:36.518488 hyutils-hyutil-hoyun-lab-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 03:40:36.540490 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      205 2023-06-07 01:36:26.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0      860 2023-06-07 07:24:26.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0      529 2023-06-01 07:38:08.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/xmlutil.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:40:36.548996 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      598 2023-06-08 03:40:36.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-08 03:40:36.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 03:40:36.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 03:40:36.000000 hyutils-hyutil-hoyun-lab-0.0.1/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 04:03:04.924577 hyutils-hyutil-hoyun-lab-0.0.2/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      598 2023-06-08 04:03:04.923577 hyutils-hyutil-hoyun-lab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.2/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 04:03:04.925076 hyutils-hyutil-hoyun-lab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      850 2023-06-08 03:59:23.000000 hyutils-hyutil-hoyun-lab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 04:03:04.896580 hyutils-hyutil-hoyun-lab-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 04:03:04.915077 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      205 2023-06-07 01:36:26.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0      860 2023-06-07 07:24:26.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0     3842 2023-06-08 04:01:29.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/xmlutil.py
+drwxrwxrwx   0        0        0        0 2023-06-08 04:03:04.922077 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-06-08 04:03:04.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-08 04:03:04.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 04:03:04.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-08 04:03:04.000000 hyutils-hyutil-hoyun-lab-0.0.2/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.1/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.1/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.1",
+    version="0.0.2",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.1/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.2/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.1/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.2/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

