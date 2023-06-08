# Comparing `tmp/zappa-packer-0.0.3.tar.gz` & `tmp/zappa-packer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zappa-packer-0.0.3.tar", last modified: Mon Jun  5 23:07:58 2023, max compression
+gzip compressed data, was "zappa-packer-0.0.4.tar", last modified: Thu Jun  8 15:53:54 2023, max compression
```

## Comparing `zappa-packer-0.0.3.tar` & `zappa-packer-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-05 23:07:58.030454 zappa-packer-0.0.3/
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     2402 2023-06-05 23:07:58.030120 zappa-packer-0.0.3/PKG-INFO
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1437 2023-06-05 23:06:00.000000 zappa-packer-0.0.3/README.md
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)       38 2023-06-05 23:07:58.030569 zappa-packer-0.0.3/setup.cfg
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1967 2023-06-05 22:13:23.000000 zappa-packer-0.0.3/setup.py
-drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-05 23:07:58.024851 zappa-packer-0.0.3/tests/
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1662 2023-06-05 22:10:33.000000 zappa-packer-0.0.3/tests/test.py
-drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-05 23:07:58.026820 zappa-packer-0.0.3/zappa_packer/
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1441 2023-06-05 23:07:26.000000 zappa-packer-0.0.3/zappa_packer/__init__.py
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)    32173 2023-06-05 22:31:42.000000 zappa-packer-0.0.3/zappa_packer/cli.py
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)    28584 2023-06-05 22:32:47.000000 zappa-packer-0.0.3/zappa_packer/handler.py
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)    30114 2023-06-05 20:57:30.000000 zappa-packer-0.0.3/zappa_packer/zappa.py
-drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-05 23:07:58.029617 zappa-packer-0.0.3/zappa_packer.egg-info/
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     2402 2023-06-05 23:07:57.000000 zappa-packer-0.0.3/zappa_packer.egg-info/PKG-INFO
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)      341 2023-06-05 23:07:57.000000 zappa-packer-0.0.3/zappa_packer.egg-info/SOURCES.txt
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)        1 2023-06-05 23:07:57.000000 zappa-packer-0.0.3/zappa_packer.egg-info/dependency_links.txt
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)       86 2023-06-05 23:07:57.000000 zappa-packer-0.0.3/zappa_packer.egg-info/entry_points.txt
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)      114 2023-06-05 23:07:57.000000 zappa-packer-0.0.3/zappa_packer.egg-info/requires.txt
--rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)       13 2023-06-05 23:07:57.000000 zappa-packer-0.0.3/zappa_packer.egg-info/top_level.txt
+drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-08 15:53:54.207353 zappa-packer-0.0.4/
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     2402 2023-06-08 15:53:54.207053 zappa-packer-0.0.4/PKG-INFO
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1437 2023-06-05 23:06:00.000000 zappa-packer-0.0.4/README.md
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)       38 2023-06-08 15:53:54.207502 zappa-packer-0.0.4/setup.cfg
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1967 2023-06-05 22:13:23.000000 zappa-packer-0.0.4/setup.py
+drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-08 15:53:54.201577 zappa-packer-0.0.4/tests/
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1662 2023-06-05 22:10:33.000000 zappa-packer-0.0.4/tests/test.py
+drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-08 15:53:54.204277 zappa-packer-0.0.4/zappa_packer/
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     1441 2023-06-08 15:52:58.000000 zappa-packer-0.0.4/zappa_packer/__init__.py
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)    32173 2023-06-05 22:31:42.000000 zappa-packer-0.0.4/zappa_packer/cli.py
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)    25419 2023-06-08 15:51:44.000000 zappa-packer-0.0.4/zappa_packer/handler.py
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     2071 2023-06-08 15:12:01.000000 zappa-packer-0.0.4/zappa_packer/middleware.py
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     4662 2023-06-08 15:50:40.000000 zappa-packer-0.0.4/zappa_packer/utilities.py
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     6789 2023-06-08 15:48:53.000000 zappa-packer-0.0.4/zappa_packer/wsgi.py
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)    30114 2023-06-05 20:57:30.000000 zappa-packer-0.0.4/zappa_packer/zappa.py
+drwxr-xr-x   0 marioalejandromixtegapacheco   (501) staff       (20)        0 2023-06-08 15:53:54.206607 zappa-packer-0.0.4/zappa_packer.egg-info/
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)     2402 2023-06-08 15:53:54.000000 zappa-packer-0.0.4/zappa_packer.egg-info/PKG-INFO
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)      415 2023-06-08 15:53:54.000000 zappa-packer-0.0.4/zappa_packer.egg-info/SOURCES.txt
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)        1 2023-06-08 15:53:54.000000 zappa-packer-0.0.4/zappa_packer.egg-info/dependency_links.txt
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)       86 2023-06-08 15:53:54.000000 zappa-packer-0.0.4/zappa_packer.egg-info/entry_points.txt
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)      114 2023-06-08 15:53:54.000000 zappa-packer-0.0.4/zappa_packer.egg-info/requires.txt
+-rw-r--r--   0 marioalejandromixtegapacheco   (501) staff       (20)       13 2023-06-08 15:53:54.000000 zappa-packer-0.0.4/zappa_packer.egg-info/top_level.txt
```

### Comparing `zappa-packer-0.0.3/PKG-INFO` & `zappa-packer-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zappa-packer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Server-less Python Web Services for AWS Lambda and API Gateway
 Home-page: https://github.com/mariowix/ZappaPacker
 Author: Mario Mixtega
 Author-email: mariomixtega@yahoo.com
 License: MIT License
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `zappa-packer-0.0.3/README.md` & `zappa-packer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zappa-packer-0.0.3/setup.py` & `zappa-packer-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `zappa-packer-0.0.3/tests/test.py` & `zappa-packer-0.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `zappa-packer-0.0.3/zappa_packer/__init__.py` & `zappa-packer-0.0.4/zappa_packer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
     # when running in docker enforce minimum version only
     err_msg = (
         f"This version of Python ({sys.version_info.major}.{sys.version_info.minor}) is not supported!\n"
         f"Zappa requires a minimum version of 3.{MINIMUM_SUPPORTED_MINOR_VERSION}"
     )
     raise RuntimeError(err_msg)
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `zappa-packer-0.0.3/zappa_packer/cli.py` & `zappa-packer-0.0.4/zappa_packer/cli.py`

 * *Files identical despite different names*

### Comparing `zappa-packer-0.0.3/zappa_packer/zappa.py` & `zappa-packer-0.0.4/zappa_packer/zappa.py`

 * *Files identical despite different names*

### Comparing `zappa-packer-0.0.3/zappa_packer.egg-info/PKG-INFO` & `zappa-packer-0.0.4/zappa_packer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zappa-packer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Server-less Python Web Services for AWS Lambda and API Gateway
 Home-page: https://github.com/mariowix/ZappaPacker
 Author: Mario Mixtega
 Author-email: mariomixtega@yahoo.com
 License: MIT License
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
```

