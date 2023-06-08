# Comparing `tmp/cliwiper-1.1.3.tar.gz` & `tmp/cliwiper-1.1.4.tar.gz`

## Comparing `cliwiper-1.1.3.tar` & `cliwiper-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cliwiper-1.1.3/cliwiper/__init__.py
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 cliwiper-1.1.3/cliwiper/cliwiper.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 cliwiper-1.1.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cliwiper-1.1.3/LICENSE
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 cliwiper-1.1.3/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cliwiper-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 cliwiper-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cliwiper-1.1.4/cliwiper/__init__.py
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 cliwiper-1.1.4/cliwiper/cliwiper.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 cliwiper-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cliwiper-1.1.4/LICENSE
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 cliwiper-1.1.4/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cliwiper-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 cliwiper-1.1.4/PKG-INFO
```

### Comparing `cliwiper-1.1.3/.gitignore` & `cliwiper-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cliwiper-1.1.3/LICENSE` & `cliwiper-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cliwiper-1.1.3/pyproject.toml` & `cliwiper-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliwiper-1.1.3/PKG-INFO` & `cliwiper-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliwiper
-Version: 1.1.3
+Version: 1.1.4
 Summary: clear the cli
 Project-URL: Homepage, https://github.com/SirX7/cliwiper
 Project-URL: Bug Tracker, https://github.com/SirX7/cliwiper/issues
 Author-email: Shall Mcfield <xhall.mc@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,16 +26,23 @@
 
 `pip install cliwiper`  
 `pipx install cliwiper`  
 
 # Usages  
 
 ```
-from cliwiper import wiper  
+from cliwiper import cliwiper  
 ```
+```
+cliwiper.wiper()  
+```
+or  
 
 ```
+from cliwiper.cliwiper import wiper  
+```
+```
 wiper()  
 ```
 
 # License  
 This project is licensed under the terms of the [MIT license](#LICENSE).
```

