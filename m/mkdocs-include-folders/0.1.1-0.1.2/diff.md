# Comparing `tmp/mkdocs-include-folders-0.1.1.tar.gz` & `tmp/mkdocs-include-folders-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-include-folders-0.1.1.tar", last modified: Thu Jun  8 10:37:24 2023, max compression
+gzip compressed data, was "mkdocs-include-folders-0.1.2.tar", last modified: Thu Jun  8 10:46:10 2023, max compression
```

## Comparing `mkdocs-include-folders-0.1.1.tar` & `mkdocs-include-folders-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:37:24.297508 mkdocs-include-folders-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 10:37:14.000000 mkdocs-include-folders-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 10:37:24.297508 mkdocs-include-folders-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-08 10:37:14.000000 mkdocs-include-folders-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:37:24.297508 mkdocs-include-folders-0.1.1/mkdocs_include_folders/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 10:37:14.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-08 10:37:14.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:37:24.297508 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 10:37:24.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 10:37:24.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:37:24.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 10:37:24.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 10:37:24.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 10:37:24.000000 mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:37:24.297508 mkdocs-include-folders-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-08 10:37:14.000000 mkdocs-include-folders-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:10.218268 mkdocs-include-folders-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 10:45:48.000000 mkdocs-include-folders-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 10:46:10.218268 mkdocs-include-folders-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-08 10:45:48.000000 mkdocs-include-folders-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:10.218268 mkdocs-include-folders-0.1.2/mkdocs_include_folders/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 10:45:48.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-08 10:45:48.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:10.218268 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-08 10:46:10.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 10:46:10.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:46:10.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 10:46:10.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 10:46:10.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 10:46:10.000000 mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:46:10.218268 mkdocs-include-folders-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 10:45:48.000000 mkdocs-include-folders-0.1.2/setup.py
```

### Comparing `mkdocs-include-folders-0.1.1/LICENSE` & `mkdocs-include-folders-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-include-folders-0.1.1/PKG-INFO` & `mkdocs-include-folders-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-include-folders
-Version: 0.1.1
+Version: 0.1.2
 Summary: A mkdocs plugin that lets you include subfolder of a top level tree.
 Home-page: https://github.com/hhdale/mkdocs-include-folders
 Author: Håkon Haugholt-Dale
 Author-email: hakon.dale@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs-include-folders-0.1.1/README.md` & `mkdocs-include-folders-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-include-folders-0.1.1/mkdocs_include_folders/plugin.py` & `mkdocs-include-folders-0.1.2/mkdocs_include_folders/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-include-folders-0.1.1/mkdocs_include_folders.egg-info/PKG-INFO` & `mkdocs-include-folders-0.1.2/mkdocs_include_folders.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-include-folders
-Version: 0.1.1
+Version: 0.1.2
 Summary: A mkdocs plugin that lets you include subfolder of a top level tree.
 Home-page: https://github.com/hhdale/mkdocs-include-folders
 Author: Håkon Haugholt-Dale
 Author-email: hakon.dale@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mkdocs-include-folders-0.1.1/setup.py` & `mkdocs-include-folders-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def read(name):
     mydir = os.path.abspath(os.path.dirname(__file__))
     return open(os.path.join(mydir, name)).read()
 
 
 setuptools.setup(
     name='mkdocs-include-folders',
-    version='0.1.1',
+    version='0.1.2',
     packages=['mkdocs_include_folders'],
     url='https://github.com/hhdale/mkdocs-include-folders',
     license='Apache',
     author='Håkon Haugholt-Dale',
     author_email='hakon.dale@gmail.com',
     description='A mkdocs plugin that lets you include subfolder of a top level tree.',
     long_description=read('README.md'),
@@ -21,11 +21,11 @@
     install_requires=['mkdocs'],
 
     # The following rows are important to register your plugin.
     # The format is "(plugin name) = (plugin folder):(class name)"
     # Without them, mkdocs will not be able to recognize it.
     entry_points={
         'mkdocs.plugins': [
-            'include = mkdocs_include_folders:IncludeFolders',
+            'include-folders = mkdocs_include_folders:IncludeFolders',
         ]
     },
 )
```

