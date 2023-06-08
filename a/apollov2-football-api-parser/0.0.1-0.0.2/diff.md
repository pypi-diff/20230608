# Comparing `tmp/apollov2_football_api_parser-0.0.1.tar.gz` & `tmp/apollov2_football_api_parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollov2_football_api_parser-0.0.1.tar", last modified: Thu Jun  8 16:39:12 2023, max compression
+gzip compressed data, was "apollov2_football_api_parser-0.0.2.tar", last modified: Thu Jun  8 16:49:23 2023, max compression
```

## Comparing `apollov2_football_api_parser-0.0.1.tar` & `apollov2_football_api_parser-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:39:12.821295 apollov2_football_api_parser-0.0.1/
--rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:25:55.000000 apollov2_football_api_parser-0.0.1/LICENSE
--rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 16:39:12.821429 apollov2_football_api_parser-0.0.1/PKG-INFO
--rw-r--r--   0 jerrywang   (501) staff       (20)      528 2023-06-08 16:30:33.000000 apollov2_football_api_parser-0.0.1/README.md
--rw-r--r--   0 jerrywang   (501) staff       (20)      103 2023-06-08 16:27:29.000000 apollov2_football_api_parser-0.0.1/pyproject.toml
--rw-r--r--   0 jerrywang   (501) staff       (20)      508 2023-06-08 16:39:12.821869 apollov2_football_api_parser-0.0.1/setup.cfg
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:39:12.819151 apollov2_football_api_parser-0.0.1/src/
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:39:12.820522 apollov2_football_api_parser-0.0.1/src/apollov2_football_api_parser.egg-info/
--rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 16:39:12.000000 apollov2_football_api_parser-0.0.1/src/apollov2_football_api_parser.egg-info/PKG-INFO
--rw-r--r--   0 jerrywang   (501) staff       (20)      320 2023-06-08 16:39:12.000000 apollov2_football_api_parser-0.0.1/src/apollov2_football_api_parser.egg-info/SOURCES.txt
--rw-r--r--   0 jerrywang   (501) staff       (20)        1 2023-06-08 16:39:12.000000 apollov2_football_api_parser-0.0.1/src/apollov2_football_api_parser.egg-info/dependency_links.txt
--rw-r--r--   0 jerrywang   (501) staff       (20)       10 2023-06-08 16:39:12.000000 apollov2_football_api_parser-0.0.1/src/apollov2_football_api_parser.egg-info/top_level.txt
-drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:39:12.820833 apollov2_football_api_parser-0.0.1/src/mypackage/
--rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:30:28.000000 apollov2_football_api_parser-0.0.1/src/mypackage/__init__.py
--rw-r--r--   0 jerrywang   (501) staff       (20)    15911 2023-06-08 16:30:31.000000 apollov2_football_api_parser-0.0.1/src/mypackage/api_parser.py
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.425166 apollov2_football_api_parser-0.0.2/
+-rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:25:55.000000 apollov2_football_api_parser-0.0.2/LICENSE
+-rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 16:49:23.425255 apollov2_football_api_parser-0.0.2/PKG-INFO
+-rw-r--r--   0 jerrywang   (501) staff       (20)      528 2023-06-08 16:30:33.000000 apollov2_football_api_parser-0.0.2/README.md
+-rw-r--r--   0 jerrywang   (501) staff       (20)      103 2023-06-08 16:27:29.000000 apollov2_football_api_parser-0.0.2/pyproject.toml
+-rw-r--r--   0 jerrywang   (501) staff       (20)      508 2023-06-08 16:49:23.425615 apollov2_football_api_parser-0.0.2/setup.cfg
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.422825 apollov2_football_api_parser-0.0.2/src/
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.423714 apollov2_football_api_parser-0.0.2/src/apollov2/
+-rw-r--r--   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:48:32.000000 apollov2_football_api_parser-0.0.2/src/apollov2/__init__.py
+-rw-r--r--   0 jerrywang   (501) staff       (20)    15911 2023-06-08 16:30:31.000000 apollov2_football_api_parser-0.0.2/src/apollov2/api_parser.py
+drwxr-xr-x   0 jerrywang   (501) staff       (20)        0 2023-06-08 16:49:23.425010 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/
+-rw-r--r--   0 jerrywang   (501) staff       (20)      912 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/PKG-INFO
+-rw-r--r--   0 jerrywang   (501) staff       (20)      318 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 jerrywang   (501) staff       (20)        1 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 jerrywang   (501) staff       (20)        9 2023-06-08 16:49:23.000000 apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/top_level.txt
```

### Comparing `apollov2_football_api_parser-0.0.1/PKG-INFO` & `apollov2_football_api_parser-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollov2_football_api_parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: extract data from api and transform it into dataframe
 Author: zhe wang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `apollov2_football_api_parser-0.0.1/README.md` & `apollov2_football_api_parser-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `apollov2_football_api_parser-0.0.1/src/apollov2_football_api_parser.egg-info/PKG-INFO` & `apollov2_football_api_parser-0.0.2/src/apollov2_football_api_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollov2-football-api-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: extract data from api and transform it into dataframe
 Author: zhe wang
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `apollov2_football_api_parser-0.0.1/src/mypackage/api_parser.py` & `apollov2_football_api_parser-0.0.2/src/apollov2/api_parser.py`

 * *Files identical despite different names*

