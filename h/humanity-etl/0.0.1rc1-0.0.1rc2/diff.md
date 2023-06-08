# Comparing `tmp/humanity_etl-0.0.1rc1.tar.gz` & `tmp/humanity_etl-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanity_etl-0.0.1rc1.tar", last modified: Thu Jun  8 18:03:41 2023, max compression
+gzip compressed data, was "humanity_etl-0.0.1rc2.tar", last modified: Thu Jun  8 18:35:44 2023, max compression
```

## Comparing `humanity_etl-0.0.1rc1.tar` & `humanity_etl-0.0.1rc2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:03:41.790237 humanity_etl-0.0.1rc1/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc1/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-08 18:03:41.786237 humanity_etl-0.0.1rc1/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc1/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:03:41.786237 humanity_etl-0.0.1rc1/humanity_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc1/humanity_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc1/humanity_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc1/humanity_etl/humanity_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:03:41.786237 humanity_etl-0.0.1rc1/humanity_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc1/humanity_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4129 2023-06-08 18:00:43.000000 humanity_etl-0.0.1rc1/humanity_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc1/humanity_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-08 18:02:02.000000 humanity_etl-0.0.1rc1/humanity_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc1/humanity_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:03:41.786237 humanity_etl-0.0.1rc1/humanity_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc1/humanity_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4135 2023-06-08 18:00:43.000000 humanity_etl-0.0.1rc1/humanity_etl/tables/timeclocks.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:03:41.786237 humanity_etl-0.0.1rc1/humanity_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-08 18:03:41.000000 humanity_etl-0.0.1rc1/humanity_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-08 18:03:41.000000 humanity_etl-0.0.1rc1/humanity_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-08 18:03:41.000000 humanity_etl-0.0.1rc1/humanity_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       48 2023-06-08 18:03:41.000000 humanity_etl-0.0.1rc1/humanity_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-08 18:03:41.000000 humanity_etl-0.0.1rc1/humanity_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-08 18:03:41.790237 humanity_etl-0.0.1rc1/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      957 2023-06-08 16:57:41.000000 humanity_etl-0.0.1rc1/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:03:41.786237 humanity_etl-0.0.1rc1/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc1/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc2/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc2/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/humanity_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc2/humanity_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc2/humanity_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc2/humanity_etl/humanity_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/humanity_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc2/humanity_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4129 2023-06-08 18:00:43.000000 humanity_etl-0.0.1rc2/humanity_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc2/humanity_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-08 18:02:02.000000 humanity_etl-0.0.1rc2/humanity_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc2/humanity_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/humanity_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc2/humanity_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4135 2023-06-08 18:00:43.000000 humanity_etl-0.0.1rc2/humanity_etl/tables/timeclocks.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/humanity_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-08 18:35:44.000000 humanity_etl-0.0.1rc2/humanity_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-08 18:35:44.000000 humanity_etl-0.0.1rc2/humanity_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-08 18:35:44.000000 humanity_etl-0.0.1rc2/humanity_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       54 2023-06-08 18:35:44.000000 humanity_etl-0.0.1rc2/humanity_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-08 18:35:44.000000 humanity_etl-0.0.1rc2/humanity_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      963 2023-06-08 18:35:23.000000 humanity_etl-0.0.1rc2/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:35:44.767877 humanity_etl-0.0.1rc2/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc2/tests/__init__.py
```

### Comparing `humanity_etl-0.0.1rc1/PKG-INFO` & `humanity_etl-0.0.1rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity_etl
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.0.1rc1/README_PUBLIC.md` & `humanity_etl-0.0.1rc2/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/humanity_etl/libs/cnst.py` & `humanity_etl-0.0.1rc2/humanity_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/humanity_etl/libs/dbg.py` & `humanity_etl-0.0.1rc2/humanity_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/humanity_etl/libs/network.py` & `humanity_etl-0.0.1rc2/humanity_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/humanity_etl/libs/transform.py` & `humanity_etl-0.0.1rc2/humanity_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/humanity_etl/tables/timeclocks.py` & `humanity_etl-0.0.1rc2/humanity_etl/tables/timeclocks.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/humanity_etl.egg-info/PKG-INFO` & `humanity_etl-0.0.1rc2/humanity_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity-etl
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.0.1rc1/humanity_etl.egg-info/SOURCES.txt` & `humanity_etl-0.0.1rc2/humanity_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc1/setup.py` & `humanity_etl-0.0.1rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="humanity_etl",
-    version="0.0.1rc1",
+    version="0.0.1rc2",
     description="Replicate humanity data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
     license="UNLICENSED",
     packages=find_packages(include=["humanity_etl", "humanity_etl.*"]),
     url="https://github.com/neofinancial/humanity_etl",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["click", "pandas", "requests", "pyspark", "typing_extensions"],
+    install_requires=["click", "pandas>=1,<2", "requests", "pyspark", "typing_extensions"],
     tests_require=["pytest"],
 )
```

