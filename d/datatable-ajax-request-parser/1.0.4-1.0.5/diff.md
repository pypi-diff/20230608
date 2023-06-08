# Comparing `tmp/datatable-ajax-request-parser-1.0.4.tar.gz` & `tmp/datatable-ajax-request-parser-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-ajax-request-parser-1.0.4.tar", last modified: Mon May 29 15:30:56 2023, max compression
+gzip compressed data, was "datatable-ajax-request-parser-1.0.5.tar", last modified: Thu Jun  8 02:43:16 2023, max compression
```

## Comparing `datatable-ajax-request-parser-1.0.4.tar` & `datatable-ajax-request-parser-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 15:30:56.366571 datatable-ajax-request-parser-1.0.4/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.4/LICENCE
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 15:30:56.366624 datatable-ajax-request-parser-1.0.4/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.4/README.md
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 15:30:56.365864 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/
--rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/__init__.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1096 2023-05-29 15:27:44.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/dataclasses.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     3591 2023-05-29 15:29:54.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6043 2023-05-29 15:29:06.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 14:28:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/utils.py
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 15:30:56.366463 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/SOURCES.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/dependency_links.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/requires.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/top_level.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 15:30:56.366887 datatable-ajax-request-parser-1.0.4/setup.cfg
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-05-29 15:30:37.000000 datatable-ajax-request-parser-1.0.4/setup.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-06-08 02:43:16.216885 datatable-ajax-request-parser-1.0.5/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.5/LICENCE
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-06-08 02:43:16.216959 datatable-ajax-request-parser-1.0.5/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.5/README.md
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-06-08 02:43:16.215845 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/__init__.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1106 2023-06-08 02:42:15.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/dataclasses.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     3582 2023-06-08 02:42:15.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6043 2023-05-29 15:29:06.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/test_django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/test_parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 14:28:56.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/utils.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-06-08 02:43:16.216753 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-06-08 02:43:16.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-06-08 02:43:16.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-06-08 02:43:16.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-06-08 02:43:16.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/requires.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-06-08 02:43:16.000000 datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/top_level.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-06-08 02:43:16.217262 datatable-ajax-request-parser-1.0.5/setup.cfg
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-06-08 02:43:09.000000 datatable-ajax-request-parser-1.0.5/setup.py
```

### Comparing `datatable-ajax-request-parser-1.0.4/LICENCE` & `datatable-ajax-request-parser-1.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/PKG-INFO` & `datatable-ajax-request-parser-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.4
+Version: 1.0.5
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datatable-ajax-request-parser-1.0.4/README.md` & `datatable-ajax-request-parser-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/dataclasses.py` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import asdict, dataclass
-from typing import List
+from typing import Any, List
 
 
 @dataclass
 class DictHelperMixin:
     def to_dict(self):
         return asdict(self)
 
@@ -49,9 +49,9 @@
 
 
 @dataclass
 class DTResponse(DictHelperMixin):
     draw: int
     records_total: int
     records_filtered: int
-    data: dict
+    data: List[Any]
     error: str
```

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/django_extension.py` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/django_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass
+from typing import Callable, Type
 
-from django.db.models import Q, Model, QuerySet
+from django.db.models import Model, Q, QuerySet
 
 from datatable_ajax_request_parser.dataclasses import DTRequest, DTResponse
 from datatable_ajax_request_parser.parser import add_typings_to_dict, parse_datatable_raw_request_query
 
-from typing import Callable, Type
-
 
 @dataclass
 class DjangoDTRequest(DTRequest):
 
     def __init__(self, *args, **kwargs):
         raw_request = kwargs.pop('raw_request', None)
         if raw_request:
```

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/parser.py` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/parser.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_django_extension.py` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/test_django_extension.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_parser.py` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/utils.py` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser/utils.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/PKG-INFO` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.4
+Version: 1.0.5
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/SOURCES.txt` & `datatable-ajax-request-parser-1.0.5/datatable_ajax_request_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.4/setup.py` & `datatable-ajax-request-parser-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datatable-ajax-request-parser",
-    version="1.0.4",
+    version="1.0.5",
     description="Helper function to parse ajax datatable request into usable dictionary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yap ZhiHon",
     author_email="y.zhihon@gmail.com",
     url="https://github.com/ziiiio/datatable_ajax_request_parser.git",
     classifiers=[
```

