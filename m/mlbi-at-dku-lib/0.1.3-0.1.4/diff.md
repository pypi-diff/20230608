# Comparing `tmp/mlbi_at_dku_lib-0.1.3.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.3.tar", last modified: Tue May 23 08:25:54 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.4.tar", last modified: Thu Jun  8 06:54:08 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.3.tar` & `mlbi_at_dku_lib-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 08:25:54.567681 mlbi_at_dku_lib-0.1.3/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.3/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.3/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-05-23 08:25:54.567681 mlbi_at_dku_lib-0.1.3/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.3/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 08:25:54.567681 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    32659 2023-05-23 08:25:18.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 08:25:54.567681 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-05-23 08:25:54.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      422 2023-05-23 08:25:54.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 08:25:54.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-05-23 01:46:40.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-05-23 08:25:54.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-05-23 08:25:54.000000 mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-05-23 08:25:54.567681 mlbi_at_dku_lib-0.1.3/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-05-23 08:25:08.000000 mlbi_at_dku_lib-0.1.3/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-05-23 08:25:54.567681 mlbi_at_dku_lib-0.1.3/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.3/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.4/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.4/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.4/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9379 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     5445 2023-06-08 06:50:28.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    32659 2023-05-23 08:25:18.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-08 06:51:51.000000 mlbi_at_dku_lib-0.1.4/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-08 06:54:08.909526 mlbi_at_dku_lib-0.1.4/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.4/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.3/LICENSE` & `mlbi_at_dku_lib-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.3/PKG-INFO` & `mlbi_at_dku_lib-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.3/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.4/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.3/setup.py` & `mlbi_at_dku_lib-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.3',
+    version             = '0.1.4',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

