# Comparing `tmp/prelude-cli-1.2.3.tar.gz` & `tmp/prelude-cli-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.2.3.tar", last modified: Wed Jun  7 21:04:54 2023, max compression
+gzip compressed data, was "prelude-cli-1.2.4.tar", last modified: Thu Jun  8 13:37:11 2023, max compression
```

## Comparing `prelude-cli-1.2.3.tar` & `prelude-cli-1.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.064973 prelude-cli-1.2.3/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-07 21:04:54.065024 prelude-cli-1.2.3/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.3/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.061793 prelude-cli-1.2.3/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.3/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.3/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.062585 prelude-cli-1.2.3/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.3/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.064779 prelude-cli-1.2.3/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4036 2023-06-06 22:22:58.000000 prelude-cli-1.2.3/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.3/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7960 2023-06-07 20:52:19.000000 prelude-cli-1.2.3/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3879 2023-06-07 20:52:19.000000 prelude-cli-1.2.3/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.3/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.3/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:04:54.062405 prelude-cli-1.2.3/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-07 21:04:54.000000 prelude-cli-1.2.3/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.3/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-07 21:04:54.065247 prelude-cli-1.2.3/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.401651 prelude-cli-1.2.4/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-08 13:37:11.401730 prelude-cli-1.2.4/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.2.4/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.398112 prelude-cli-1.2.4/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.2.4/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.2.4/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.398974 prelude-cli-1.2.4/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      249 2023-06-01 16:01:25.000000 prelude-cli-1.2.4/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.401430 prelude-cli-1.2.4/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     4036 2023-06-06 22:22:58.000000 prelude-cli-1.2.4/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.2.4/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     7960 2023-06-07 20:52:19.000000 prelude-cli-1.2.4/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3879 2023-06-07 20:52:19.000000 prelude-cli-1.2.4/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.2.4/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.2.4/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-08 13:37:11.398784 prelude-cli-1.2.4/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-08 13:37:11.000000 prelude-cli-1.2.4/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.2.4/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-08 13:37:11.401959 prelude-cli-1.2.4/setup.cfg
```

### Comparing `prelude-cli-1.2.3/LICENSE` & `prelude-cli-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/PKG-INFO` & `prelude-cli-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.3/prelude_cli/cli.py` & `prelude-cli-1.2.4/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli/views/build.py` & `prelude-cli-1.2.4/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli/views/configure.py` & `prelude-cli-1.2.4/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli/views/detect.py` & `prelude-cli-1.2.4/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli/views/iam.py` & `prelude-cli-1.2.4/prelude_cli/views/iam.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli/views/partner.py` & `prelude-cli-1.2.4/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli/views/shared.py` & `prelude-cli-1.2.4/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.2.4/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.2.3/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.2.4/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.2.3/setup.cfg` & `prelude-cli-1.2.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.2.3
+version = 1.2.4
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.2.3
+	prelude-sdk == 1.2.4
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

