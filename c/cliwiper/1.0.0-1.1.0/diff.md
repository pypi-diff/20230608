# Comparing `tmp/cliwiper-1.0.0.tar.gz` & `tmp/cliwiper-1.1.0.tar.gz`

## Comparing `cliwiper-1.0.0.tar` & `cliwiper-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cliwiper-1.0.0/cliwiper/__init__.py
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 cliwiper-1.0.0/cliwiper/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 cliwiper-1.0.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cliwiper-1.0.0/LICENSE
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 cliwiper-1.0.0/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cliwiper-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cliwiper-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cliwiper-1.1.0/cliwiper/__init__.py
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 cliwiper-1.1.0/cliwiper/cliwiper.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 cliwiper-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cliwiper-1.1.0/LICENSE
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 cliwiper-1.1.0/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cliwiper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 cliwiper-1.1.0/PKG-INFO
```

### Comparing `cliwiper-1.0.0/.gitignore` & `cliwiper-1.1.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+cliwiper-build/
```

### Comparing `cliwiper-1.0.0/LICENSE` & `cliwiper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliwiper-1.0.0/pyproject.toml` & `cliwiper-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "cliwiper"
 authors = [
   { name="Shall Mcfield", email="xhall.mc@protonmail.com" },
 ]
 description = "clear the cli"
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "MIT License"}
+license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
     "Operating System :: OS Independent",
     "Intended Audience :: Information Technology",
     "Topic :: Internet",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `cliwiper-1.0.0/PKG-INFO` & `cliwiper-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cliwiper
-Version: 1.0.0
+Version: 1.1.0
 Summary: clear the cli
 Project-URL: Homepage, https://github.com/SirX7/cliwiper
 Project-URL: Bug Tracker, https://github.com/SirX7/cliwiper/issues
 Author-email: Shall Mcfield <xhall.mc@protonmail.com>
-License: MIT License
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

