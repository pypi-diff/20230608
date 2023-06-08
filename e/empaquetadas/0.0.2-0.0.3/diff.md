# Comparing `tmp/empaquetadas-0.0.2.tar.gz` & `tmp/empaquetadas-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empaquetadas-0.0.2.tar", last modified: Thu Jun  8 01:37:53 2023, max compression
+gzip compressed data, was "empaquetadas-0.0.3.tar", last modified: Thu Jun  8 03:09:09 2023, max compression
```

## Comparing `empaquetadas-0.0.2.tar` & `empaquetadas-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1071 2023-06-08 00:05:41.000000 empaquetadas-0.0.2/LICENSE
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1532 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       26 2023-06-08 00:05:13.000000 empaquetadas-0.0.2/README.md
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      406 2023-06-08 01:37:06.000000 empaquetadas-0.0.2/pyproject.toml
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/setup.cfg
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/src/
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/src/empaquetadas/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      704 2023-06-08 00:18:11.000000 empaquetadas-0.0.2/src/empaquetadas/__init__.py
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     2037 2023-06-08 00:21:31.000000 empaquetadas-0.0.2/src/empaquetadas/samples.py
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/src/empaquetadas.egg-info/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1532 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      249 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/SOURCES.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/dependency_links.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       13 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/top_level.txt
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1071 2023-06-08 00:05:41.000000 empaquetadas-0.0.3/LICENSE
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1575 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/PKG-INFO
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       26 2023-06-08 00:05:13.000000 empaquetadas-0.0.3/README.md
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1109 2023-06-08 03:07:48.000000 empaquetadas-0.0.3/pyproject.toml
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/setup.cfg
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/src/
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/src/empaquetadas/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      713 2023-06-08 02:57:10.000000 empaquetadas-0.0.3/src/empaquetadas/__init__.py
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      822 2023-06-08 03:02:01.000000 empaquetadas-0.0.3/src/empaquetadas/cli.py
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     2038 2023-06-08 02:29:07.000000 empaquetadas-0.0.3/src/empaquetadas/samples.py
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/src/empaquetadas.egg-info/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1575 2023-06-08 03:09:09.000000 empaquetadas-0.0.3/src/empaquetadas.egg-info/PKG-INFO
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      381 2023-06-08 03:09:09.000000 empaquetadas-0.0.3/src/empaquetadas.egg-info/SOURCES.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-08 03:09:09.000000 empaquetadas-0.0.3/src/empaquetadas.egg-info/dependency_links.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       61 2023-06-08 03:09:09.000000 empaquetadas-0.0.3/src/empaquetadas.egg-info/entry_points.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       30 2023-06-08 03:09:09.000000 empaquetadas-0.0.3/src/empaquetadas.egg-info/requires.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       13 2023-06-08 03:09:09.000000 empaquetadas-0.0.3/src/empaquetadas.egg-info/top_level.txt
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 03:09:09.124700 empaquetadas-0.0.3/tests/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      237 2023-06-08 01:52:23.000000 empaquetadas-0.0.3/tests/test_conversions.py
```

### Comparing `empaquetadas-0.0.2/LICENSE` & `empaquetadas-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `empaquetadas-0.0.2/PKG-INFO` & `empaquetadas-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empaquetadas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to calculate what would have happened if you had invested your pesos
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafael Sanabria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,11 +20,13 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Serpientes empaquetadas
```

### Comparing `empaquetadas-0.0.2/src/empaquetadas/__init__.py` & `empaquetadas-0.0.3/src/empaquetadas/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from typing import Union
-import empaquetadas.samples as samples
+import empaquetadas.samples as samples  # noqa
 
 
 @dataclass
 class Converter:
     records: dict[str, float]
 
     def change_factor(self, initial_record: str, final_record: str) -> float:
@@ -17,8 +17,8 @@
     final_record: str,
     converter: Union[Converter, list[Converter]],
 ) -> float:
     final_value = initial_value
     converter = [converter] if isinstance(converter, Converter) else converter
     for conv in converter:
         final_value *= conv.change_factor(initial_record, final_record)
-    return final_value
+    return final_value
```

### Comparing `empaquetadas-0.0.2/src/empaquetadas/samples.py` & `empaquetadas-0.0.3/src/empaquetadas/samples.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,8 @@
     "2022-12": 4076.57,
     "2023-01": 3824.14,
     "2023-02": 4119.21,
     "2023-03": 3951.39,
     "2023-04": 4124.51,
     "2023-05": 4167.87,
     "2023-06": 4221.02,
-}
+}
```

### Comparing `empaquetadas-0.0.2/src/empaquetadas.egg-info/PKG-INFO` & `empaquetadas-0.0.3/src/empaquetadas.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empaquetadas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to calculate what would have happened if you had invested your pesos
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafael Sanabria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,11 +20,13 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Serpientes empaquetadas
```

