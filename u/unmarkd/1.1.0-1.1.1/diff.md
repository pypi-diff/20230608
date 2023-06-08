# Comparing `tmp/unmarkd-1.1.0.tar.gz` & `tmp/unmarkd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unmarkd-1.1.0.tar", max compression
+gzip compressed data, was "unmarkd-1.1.1.tar", max compression
```

## Comparing `unmarkd-1.1.0.tar` & `unmarkd-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-06-07 03:58:44.466970 unmarkd-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     9411 2023-06-08 04:20:50.629547 unmarkd-1.1.0/README.md
--rw-r--r--   0        0        0     2878 2023-06-08 04:52:10.623482 unmarkd-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      319 2023-06-08 04:50:40.779162 unmarkd-1.1.0/unmarkd/__init__.py
--rw-r--r--   0        0        0    12126 2023-06-08 04:53:46.775663 unmarkd-1.1.0/unmarkd/unmarkers.py
--rw-r--r--   0        0        0    10579 1970-01-01 00:00:00.000000 unmarkd-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 03:58:44.466970 unmarkd-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0     9411 2023-06-08 04:20:50.629547 unmarkd-1.1.1/README.md
+-rw-r--r--   0        0        0     2878 2023-06-08 05:07:08.174888 unmarkd-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      319 2023-06-08 05:07:03.426951 unmarkd-1.1.1/unmarkd/__init__.py
+-rw-r--r--   0        0        0    12247 2023-06-08 05:06:41.426133 unmarkd-1.1.1/unmarkd/unmarkers.py
+-rw-r--r--   0        0        0    10579 1970-01-01 00:00:00.000000 unmarkd-1.1.1/PKG-INFO
```

### Comparing `unmarkd-1.1.0/LICENSE.md` & `unmarkd-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unmarkd-1.1.0/README.md` & `unmarkd-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unmarkd-1.1.0/pyproject.toml` & `unmarkd-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "unmarkd"
 description = "A markdown reverser"
 authors = ["Bryan Hu <bryan.hu.2020@gmail.com>"]
-version = "1.1.0"
+version = "1.1.1"
 
 readme = "README.md"
 license = "GPL-3.0-or-later"
 classifiers = [
     # Get the list of trove classifiers here: https://pypi.org/classifiers/
     "Programming Language :: Python :: Implementation :: CPython",
     "Operating System :: OS Independent",
```

### Comparing `unmarkd-1.1.0/unmarkd/unmarkers.py` & `unmarkd-1.1.1/unmarkd/unmarkers.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,26 +133,29 @@
             snake_string = ""
             for i, char in enumerate(pascal_string):
                 if i > 0 and char.isupper():
                     snake_string += "_"
                 snake_string += char.lower()
             return snake_string
 
-        if isinstance(child, bs4.NavigableString):
+        if (
+            issubclass(type(child), bs4.NavigableString)
+            and type(child) is not bs4.NavigableString
+        ):
             try:
                 return getattr(  # type: ignore[no-any-return]
                     self,
                     f"handle_{pascal_to_snake(type(child).__name__)}",
                 )(
                     child,
                 )
             except AttributeError as error:
                 msg = "This should never happen"
-                raise AssertionError(msg) from error
-        if isinstance(child, str):
+                raise AssertionError(msg, type(child)) from error
+        if isinstance(child, (str, bs4.NavigableString)):
             return self.handle_string(child)
         return ""  # To indicate that it is a tag
 
     def __parse(
         self: "BaseUnmarker",
         html: SoupElement,
         escape: bool = False,
```

### Comparing `unmarkd-1.1.0/PKG-INFO` & `unmarkd-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmarkd
-Version: 1.1.0
+Version: 1.1.1
 Summary: A markdown reverser
 Home-page: https://github.com/ThatXliner/unmarkd
 License: GPL-3.0-or-later
 Author: Bryan Hu
 Author-email: bryan.hu.2020@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

