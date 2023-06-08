# Comparing `tmp/specker-1.1.0.tar.gz` & `tmp/specker-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specker-1.1.0.tar", last modified: Fri Jun  2 06:42:16 2023, max compression
+gzip compressed data, was "specker-1.1.1.tar", last modified: Thu Jun  8 21:13:44 2023, max compression
```

## Comparing `specker-1.1.0.tar` & `specker-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-02 06:34:14.000000 specker-1.1.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.0/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.0/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.238685 specker-1.1.0/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.0/.vscode/extensions.json
--rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-02 06:24:00.000000 specker-1.1.0/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-02 06:42:16.242685 specker-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.0/build_requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.0/git-tags.sh
--rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.0/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-02 06:42:10.000000 specker-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 06:42:16.242685 specker-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.238685 specker-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/src/specker/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/content.py
--rw-rw-rw-   0 root         (0) root         (0)     5945 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/src/specker/specs/
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/specs/SPECFILES.md
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-06-02 06:24:00.000000 specker-1.1.0/src/specker/specs/specker.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:42:16.242685 specker-1.1.0/src/specker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 06:42:16.000000 specker-1.1.0/src/specker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-02 06:24:00.000000 specker-1.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-02 06:34:14.000000 specker-1.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-02 06:24:00.000000 specker-1.1.1/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    20971 2023-06-02 06:24:00.000000 specker-1.1.1/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-02 06:24:00.000000 specker-1.1.1/.vscode/extensions.json
+-rw-rw-rw-   0 root         (0) root         (0)   115210 2023-06-08 21:03:55.000000 specker-1.1.1/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-06-02 06:24:00.000000 specker-1.1.1/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-06-02 06:24:00.000000 specker-1.1.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-08 21:13:44.964403 specker-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-06-02 06:24:00.000000 specker-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-02 06:24:00.000000 specker-1.1.1/build_requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2586 2023-06-02 06:24:00.000000 specker-1.1.1/git-tags.sh
+-rwxrwxrwx   0 root         (0) root         (0)     7192 2023-06-02 06:24:00.000000 specker-1.1.1/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-08 21:13:38.000000 specker-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:13:44.964403 specker-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.960403 specker-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/src/specker/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-06-02 06:24:00.000000 specker-1.1.1/src/specker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-06-08 21:07:15.000000 specker-1.1.1/src/specker/content.py
+-rw-rw-rw-   0 root         (0) root         (0)     5945 2023-06-02 06:24:00.000000 specker-1.1.1/src/specker/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/src/specker/specs/
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-08 21:00:19.000000 specker-1.1.1/src/specker/specs/SPECFILES.md
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-08 21:00:19.000000 specker-1.1.1/src/specker/specs/specker.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:13:44.964403 specker-1.1.1/src/specker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 21:13:44.000000 specker-1.1.1/src/specker.egg-info/top_level.txt
```

### Comparing `specker-1.1.0/.gitlab-ci.yml` & `specker-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/.pylintrc` & `specker-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/.vscode/extensions.json` & `specker-1.1.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/Doxyfile` & `specker-1.1.1/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 PROJECT_NAME           = "Specker JSON Specification Validator"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.1.0"
+PROJECT_NUMBER = "1.1.1"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `specker-1.1.0/LICENSE.md` & `specker-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/Makefile` & `specker-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/PKG-INFO` & `specker-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `specker-1.1.0/README.md` & `specker-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/git-tags.sh` & `specker-1.1.1/git-tags.sh`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/icon.png` & `specker-1.1.1/icon.png`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/pyproject.toml` & `specker-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specker"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "Specker JSON Specification Validator"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `specker-1.1.0/src/specker/__init__.py` & `specker-1.1.1/src/specker/__init__.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/src/specker/content.py` & `specker-1.1.1/src/specker/content.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     __type_map:dict[str,object] = {
         "str": str,
         "int": int,
         "list": list,
         "dict": dict,
         "bool": bool,
-        "any": typing.Any
+        "any": typing.Any,
+        "float": float
     }
 
     @property
     def type(self) -> object:
         """Get Spec Value Type
         @retval type Type specified from Spec
         """
@@ -67,13 +68,20 @@
         if not hasattr(self,"_values"):
             self._values = []
 
     def __str__(self) -> str:
         """To String Generator
         @retval str Markdown Formatted Data about Spec
         """
+        default_str:str = ""
+        if self._default is not None:
+            default_str = f"\n - Default: {str(self._default)}"
+        values_str:str = ""
+        if len(self._values) > 0:
+            values_str = f"\n - Acceptable Values: {', '.join(self._values)}"
+        example_str:str = ""
+        if len(self._example) > 0:
+            example_str = f"\n - Example: {str(self._example)}"
         return f'''Option: `{self._name}` - {self._comment}
  - Type: {self._type}
- - Required: {str(self._required)}
- - Default: {str(self._default)}
- - Example: {str(self._example)}
+ - Required: {str(self._required)}{default_str}{values_str}{example_str}
 '''
```

### Comparing `specker-1.1.0/src/specker/loader.py` & `specker-1.1.1/src/specker/loader.py`

 * *Files identical despite different names*

### Comparing `specker-1.1.0/src/specker/specs/SPECFILES.md` & `specker-1.1.1/src/specker/specs/SPECFILES.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,38 +2,30 @@
 Auto generated from .spec files
 ## Spec for specker
 
 Option: `required` - Whether or not this Option is required
  - Type: bool
  - Required: False
  - Default: False
- - Example: 
 
 Option: `default` - Default Value if not required and not set
  - Type: any
  - Required: False
- - Default: None
- - Example: 
 
-Option: `type` - Type the Value must be. Must be one of: int, str, list, dict, bool, any
+Option: `type` - Type the Value must be.
  - Type: str
  - Required: True
  - Default: any
- - Example: 
+ - Acceptable Values: any, str, int, list, dict, float, bool
 
 Option: `comment` - Informational Comment about this Option and Value
  - Type: str
  - Required: False
- - Default: None
- - Example: 
 
 Option: `example` - Example Data for this Option and Value
  - Type: any
  - Required: False
- - Default: None
- - Example: 
 
 Option: `values` - List of Acceptable Values
  - Type: list
  - Required: False
- - Default: None
- - Example: 
+ - Example: [ "value1", "value2" ]
```

### Comparing `specker-1.1.0/src/specker/specs/specker.spec` & `specker-1.1.1/src/specker/specs/specker.spec`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'type'": "{'comment': 'Type the Value must be.', 'values': ['any', 'str', 'int', 'list', 'dict', "*

 * *           "'float', 'bool']}",*

 * * "'values'": '{\'example\': \'[ "value1", "value2" ]\'}'}*

```diff
@@ -17,18 +17,28 @@
     "required": {
         "comment": "Whether or not this Option is required",
         "default": false,
         "required": false,
         "type": "bool"
     },
     "type": {
-        "comment": "Type the Value must be. Must be one of: int, str, list, dict, bool, any",
+        "comment": "Type the Value must be.",
         "default": "any",
         "required": true,
-        "type": "str"
+        "type": "str",
+        "values": [
+            "any",
+            "str",
+            "int",
+            "list",
+            "dict",
+            "float",
+            "bool"
+        ]
     },
     "values": {
         "comment": "List of Acceptable Values",
+        "example": "[ \"value1\", \"value2\" ]",
         "required": false,
         "type": "list"
     }
 }
```

### Comparing `specker-1.1.0/src/specker.egg-info/PKG-INFO` & `specker-1.1.1/src/specker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Specker JSON Specification Validator
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-specker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

