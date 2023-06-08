# Comparing `tmp/project.harpy-0.0.2.tar.gz` & `tmp/project.harpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project.harpy-0.0.2.tar", last modified: Tue Apr 18 02:10:59 2023, max compression
+gzip compressed data, was "project.harpy-0.0.3.tar", last modified: Thu Jun  8 09:47:00 2023, max compression
```

## Comparing `project.harpy-0.0.2.tar` & `project.harpy-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:10:59.454620 project.harpy-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-09 02:21:24.000000 project.harpy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      732 2023-04-18 02:10:59.452415 project.harpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-04-18 01:38:12.000000 project.harpy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 02:10:59.435391 project.harpy-0.0.2/harpy/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:08:24.000000 project.harpy-0.0.2/harpy/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-04-12 22:47:33.000000 project.harpy-0.0.2/harpy/__main__.py
--rw-rw-rw-   0        0        0       81 2023-04-18 02:04:19.000000 project.harpy-0.0.2/harpy/__version__.py
--rw-rw-rw-   0        0        0      514 2023-04-12 19:14:24.000000 project.harpy-0.0.2/harpy/argtypes.py
--rw-rw-rw-   0        0        0     2498 2023-04-13 03:59:56.000000 project.harpy-0.0.2/harpy/cli.py
--rw-rw-rw-   0        0        0      745 2023-04-12 22:21:39.000000 project.harpy-0.0.2/harpy/consts.py
--rw-rw-rw-   0        0        0  1150157 2023-04-09 02:21:24.000000 project.harpy-0.0.2/harpy/db.json
--rw-rw-rw-   0        0        0      584 2023-04-11 18:47:25.000000 project.harpy-0.0.2/harpy/globs.py
--rw-rw-rw-   0        0        0     1224 2023-04-12 21:39:45.000000 project.harpy-0.0.2/harpy/handlers.py
--rw-rw-rw-   0        0        0     5374 2023-04-13 04:06:23.000000 project.harpy-0.0.2/harpy/net.py
--rw-rw-rw-   0        0        0     1506 2023-04-12 21:49:05.000000 project.harpy-0.0.2/harpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:10:59.451392 project.harpy-0.0.2/project.harpy.egg-info/
--rw-rw-rw-   0        0        0      732 2023-04-18 02:10:59.000000 project.harpy-0.0.2/project.harpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-04-18 02:10:59.000000 project.harpy-0.0.2/project.harpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:10:59.000000 project.harpy-0.0.2/project.harpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-18 02:10:59.000000 project.harpy-0.0.2/project.harpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 02:10:58.000000 project.harpy-0.0.2/project.harpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-04-18 02:10:59.000000 project.harpy-0.0.2/project.harpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1037 2023-04-18 02:03:40.000000 project.harpy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 02:10:59.454620 project.harpy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 09:47:00.720914 project.harpy-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-09 02:21:24.000000 project.harpy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      732 2023-06-08 09:47:00.720914 project.harpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-04-18 01:38:12.000000 project.harpy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:47:00.711835 project.harpy-0.0.3/harpy/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:08:24.000000 project.harpy-0.0.3/harpy/__init__.py
+-rw-rw-rw-   0        0        0     2211 2023-05-15 20:34:04.000000 project.harpy-0.0.3/harpy/__main__.py
+-rw-rw-rw-   0        0        0       81 2023-06-08 09:42:33.000000 project.harpy-0.0.3/harpy/__version__.py
+-rw-rw-rw-   0        0        0      514 2023-04-12 19:14:24.000000 project.harpy-0.0.3/harpy/argtypes.py
+-rw-rw-rw-   0        0        0     2498 2023-04-13 03:59:56.000000 project.harpy-0.0.3/harpy/cli.py
+-rw-rw-rw-   0        0        0      745 2023-04-12 22:21:39.000000 project.harpy-0.0.3/harpy/consts.py
+-rw-rw-rw-   0        0        0  1150157 2023-04-09 02:21:24.000000 project.harpy-0.0.3/harpy/db.json
+-rw-rw-rw-   0        0        0      584 2023-04-11 18:47:25.000000 project.harpy-0.0.3/harpy/globs.py
+-rw-rw-rw-   0        0        0     1224 2023-04-12 21:39:45.000000 project.harpy-0.0.3/harpy/handlers.py
+-rw-rw-rw-   0        0        0     5419 2023-05-31 04:56:17.000000 project.harpy-0.0.3/harpy/net.py
+-rw-rw-rw-   0        0        0     1506 2023-04-12 21:49:05.000000 project.harpy-0.0.3/harpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:47:00.718356 project.harpy-0.0.3/project.harpy.egg-info/
+-rw-rw-rw-   0        0        0      732 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1037 2023-04-18 02:03:40.000000 project.harpy-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 09:47:00.720914 project.harpy-0.0.3/setup.cfg
```

### Comparing `project.harpy-0.0.2/LICENSE` & `project.harpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/PKG-INFO` & `project.harpy-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project.harpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Active/passive ARP discovery tool
 Author: Serhat Çelik
 License: MIT
 Keywords: harpy,arp,discovery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `project.harpy-0.0.2/harpy/__main__.py` & `project.harpy-0.0.3/harpy/__main__.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/argtypes.py` & `project.harpy-0.0.3/harpy/argtypes.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/cli.py` & `project.harpy-0.0.3/harpy/cli.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/consts.py` & `project.harpy-0.0.3/harpy/consts.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/db.json` & `project.harpy-0.0.3/harpy/db.json`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/globs.py` & `project.harpy-0.0.3/harpy/globs.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/handlers.py` & `project.harpy-0.0.3/harpy/handlers.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/harpy/net.py` & `project.harpy-0.0.3/harpy/net.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,16 @@
                 interrupts.append([self.name, err])
                 break
             else:
                 sent.set(spa + '->' + tpa)
                 try:
                     controller.wait(self.sleep)
                 except OverflowError:
-                    controller.wait(DEFAULT_SLEEP / 1000)
+                    self.sleep = DEFAULT_SLEEP / 1000
+                    controller.wait(self.sleep)
         else:
             sent.set('')
 
 
 @dataclasses.dataclass
 class Scent:
     """Sniff result fields."""
```

### Comparing `project.harpy-0.0.2/harpy/utils.py` & `project.harpy-0.0.3/harpy/utils.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.2/project.harpy.egg-info/PKG-INFO` & `project.harpy-0.0.3/project.harpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project.harpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Active/passive ARP discovery tool
 Author: Serhat Çelik
 License: MIT
 Keywords: harpy,arp,discovery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
```

### Comparing `project.harpy-0.0.2/pyproject.toml` & `project.harpy-0.0.3/pyproject.toml`

 * *Files identical despite different names*

