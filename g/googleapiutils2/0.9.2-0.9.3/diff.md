# Comparing `tmp/googleapiutils2-0.9.2.tar.gz` & `tmp/googleapiutils2-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.9.2.tar", max compression
+gzip compressed data, was "googleapiutils2-0.9.3.tar", max compression
```

## Comparing `googleapiutils2-0.9.2.tar` & `googleapiutils2-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.2/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.2/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.2/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.2/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    21607 2023-06-07 18:11:07.739854 googleapiutils2-0.9.2/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.2/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.2/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.2/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.2/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.2/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.2/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    33736 2023-06-07 18:16:28.569445 googleapiutils2-0.9.2/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.2/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     9452 2023-06-07 18:45:50.330658 googleapiutils2-0.9.2/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1089 2023-06-07 18:44:02.915563 googleapiutils2-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.9.3/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.9.3/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.9.3/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    21607 2023-06-07 18:11:07.739854 googleapiutils2-0.9.3/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-06-07 16:12:16.848980 googleapiutils2-0.9.3/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.9.3/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.9.3/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.9.3/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.9.3/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.9.3/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    33736 2023-06-07 18:16:28.569445 googleapiutils2-0.9.3/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.9.3/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     9430 2023-06-07 18:49:59.814378 googleapiutils2-0.9.3/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1089 2023-06-07 18:50:56.789817 googleapiutils2-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.9.3/PKG-INFO
```

### Comparing `googleapiutils2-0.9.2/LICENSE` & `googleapiutils2-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/README.md` & `googleapiutils2-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/drive/drive.py` & `googleapiutils2-0.9.3/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.9.3/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.9.3/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.9.3/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.9.3/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.9.3/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.9.2/googleapiutils2/utils.py` & `googleapiutils2-0.9.3/googleapiutils2/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
     if len(hex_code) == 3 or len(hex_code) == 4:
         hex_code = "".join([2 * c for c in hex_code])
 
     rgb: Color = {
         "red": int(hex_code[:2], 16),
         "green": int(hex_code[2:4], 16),
         "blue": int(hex_code[4:6], 16),
-        "alpha": 1.0,
     }
 
     if len(hex_code) == 8:
         rgb["alpha"] = int(hex_code[6:8], 16)
     elif len(hex_code) != 6:
         raise ValueError("Invalid hex code")
```

### Comparing `googleapiutils2-0.9.2/pyproject.toml` & `googleapiutils2-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.9.2"
+version = "0.9.3"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.9.2/PKG-INFO` & `googleapiutils2-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.9.2
+Version: 0.9.3
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

