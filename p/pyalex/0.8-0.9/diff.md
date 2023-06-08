# Comparing `tmp/pyalex-0.8.tar.gz` & `tmp/pyalex-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalex-0.8.tar", last modified: Sun Mar 19 09:38:56 2023, max compression
+gzip compressed data, was "pyalex-0.9.tar", last modified: Mon Mar 27 21:58:32 2023, max compression
```

## Comparing `pyalex-0.8.tar` & `pyalex-0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:38:56.498790 pyalex-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-19 09:38:42.000000 pyalex-0.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:38:56.498790 pyalex-0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:38:56.498790 pyalex-0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-19 09:38:42.000000 pyalex-0.8/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-19 09:38:42.000000 pyalex-0.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-19 09:38:42.000000 pyalex-0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-19 09:38:42.000000 pyalex-0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-19 09:38:42.000000 pyalex-0.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-19 09:38:42.000000 pyalex-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-03-19 09:38:56.498790 pyalex-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-03-19 09:38:42.000000 pyalex-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:38:56.498790 pyalex-0.8/pyalex/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-19 09:38:42.000000 pyalex-0.8/pyalex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-19 09:38:56.000000 pyalex-0.8/pyalex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-03-19 09:38:42.000000 pyalex-0.8/pyalex/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:38:56.498790 pyalex-0.8/pyalex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-03-19 09:38:56.000000 pyalex-0.8/pyalex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-19 09:38:56.000000 pyalex-0.8/pyalex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 09:38:56.000000 pyalex-0.8/pyalex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-19 09:38:56.000000 pyalex-0.8/pyalex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-19 09:38:56.000000 pyalex-0.8/pyalex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-03-19 09:38:42.000000 pyalex-0.8/pyalex_repocard.png
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-19 09:38:42.000000 pyalex-0.8/pyalex_repocard.svg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-19 09:38:42.000000 pyalex-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 09:38:56.498790 pyalex-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 09:38:56.498790 pyalex-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-03-19 09:38:42.000000 pyalex-0.8/tests/test_pyalex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:58:32.267570 pyalex-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-27 21:58:18.000000 pyalex-0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:58:32.263570 pyalex-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:58:32.263570 pyalex-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-27 21:58:18.000000 pyalex-0.9/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-27 21:58:18.000000 pyalex-0.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-27 21:58:18.000000 pyalex-0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-27 21:58:18.000000 pyalex-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-27 21:58:18.000000 pyalex-0.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-27 21:58:18.000000 pyalex-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-03-27 21:58:32.267570 pyalex-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-03-27 21:58:18.000000 pyalex-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:58:32.267570 pyalex-0.9/pyalex/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-27 21:58:18.000000 pyalex-0.9/pyalex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-27 21:58:32.000000 pyalex-0.9/pyalex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-03-27 21:58:18.000000 pyalex-0.9/pyalex/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:58:32.267570 pyalex-0.9/pyalex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-03-27 21:58:32.000000 pyalex-0.9/pyalex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-27 21:58:32.000000 pyalex-0.9/pyalex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 21:58:32.000000 pyalex-0.9/pyalex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-27 21:58:32.000000 pyalex-0.9/pyalex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 21:58:32.000000 pyalex-0.9/pyalex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-03-27 21:58:18.000000 pyalex-0.9/pyalex_repocard.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-27 21:58:18.000000 pyalex-0.9/pyalex_repocard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-27 21:58:18.000000 pyalex-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 21:58:32.267570 pyalex-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 21:58:32.267570 pyalex-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-03-27 21:58:18.000000 pyalex-0.9/tests/test_pyalex.py
```

### Comparing `pyalex-0.8/.github/workflows/python-package.yml` & `pyalex-0.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/.github/workflows/python-publish.yml` & `pyalex-0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/.gitignore` & `pyalex-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/LICENSE` & `pyalex-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/PKG-INFO` & `pyalex-0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalex
-Version: 0.8
+Version: 0.9
 Summary: One downloader for many scientific data and code repositories!
 Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -34,14 +34,16 @@
 The following features of OpenAlex are currently supported by PyAlex:
 
 - [x] Get single entities
 - [x] Filter entities
 - [x] Search entities
 - [x] Group entities
 - [x] Search filters
+- [x] Select fields
+- [x] Sample
 - [x] Pagination
 - [ ] [Autocomplete endpoint](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/autocomplete-entities)
 - [x] N-grams
 - [x] Authentication
 
 We aim to cover the entire API, and we are looking for help. We are welcoming Pull Requests.
 
@@ -60,15 +62,15 @@
 ```
 
 ## Getting started
 
 PyAlex offers support for all [Entity Objects](https://docs.openalex.org/api-entities/entities-overview): [Works](https://docs.openalex.org/api-entities/works), [Authors](https://docs.openalex.org/api-entities/authors), [Sources](https://docs.openalex.org/api-entities/sourcese), [Institutions](https://docs.openalex.org/api-entities/institutions), [Concepts](https://docs.openalex.org/api-entities/concepts), and [Publishers](https://docs.openalex.org/api-entities/publishers).
 
 ```python
-from pyalex import Works, Authors, Sources, Institutions, Concepts
+from pyalex import Works, Authors, Sources, Institutions, Concepts, Publishers
 ```
 
 ### The polite pool
 
 [The polite pool](https://docs.openalex.org/how-to-use-the-api/rate-limits-and-authentication#the-polite-pool) has much
 faster and more consistent response times. To get into the polite pool, you
 set your email:
@@ -208,14 +210,61 @@
 
 OpenAlex reference: [Sort entity lists](https://docs.openalex.org/api-entities/works/get-lists-of-works#page-and-sort-works).
 
 ```python
 Works().sort(cited_by_count="desc").get()
 ```
 
+#### Select
+
+OpenAlex reference: [Select fields](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/select-fields).
+
+```python
+Works().filter(publication_year=2020, is_oa=True).select(["id", "doi"]).get()
+```
+
+#### Sample
+
+OpenAlex reference: [Sample entity lists](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/sample-entity-lists).
+
+```python
+Works().sample(100, seed=535).get()
+```
+
+#### Logical expressions
+
+OpenAlex reference: [Logical expressions](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/filter-entity-lists#logical-expressions)
+
+Inequality:
+
+```python
+Sources().filter(works_count=">1000").get()
+```
+
+Negation (NOT):
+
+```python
+Institutions().filter(country_code="!us").get()
+```
+
+Intersection (AND):
+
+```python
+Works().filter(institutions={"country_code": ["fr", "gb"]}).get()
+
+# same
+Works().filter(institutions={"country_code": "fr"}).filter(institutions={"country_code": "gb"}).get()
+```
+
+Addition (OR):
+
+```python
+Works().filter(institutions={"country_code": "fr|gb"}).get()
+```
+
 #### Paging
 
 OpenAlex offers two methods for paging: [basic paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging#basic-paging) and [cursor paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging#cursor-paging). Both methods are supported by
 PyAlex, although cursor paging seems to be easier to implement and less error-prone.
 
 ##### Basic paging
```

### Comparing `pyalex-0.8/README.md` & `pyalex-0.9/pyalex.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pyalex
+Version: 0.9
+Summary: One downloader for many scientific data and code repositories!
+Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
+License-File: LICENSE
+
 <p align="center">
   <img alt="PyAlex - a Python wrapper for OpenAlex" src="https://github.com/J535D165/pyalex/raw/main/pyalex_repocard.svg">
 </p>
 
 # PyAlex
 
 ![PyPI](https://img.shields.io/pypi/v/pyalex) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
@@ -15,14 +34,16 @@
 The following features of OpenAlex are currently supported by PyAlex:
 
 - [x] Get single entities
 - [x] Filter entities
 - [x] Search entities
 - [x] Group entities
 - [x] Search filters
+- [x] Select fields
+- [x] Sample
 - [x] Pagination
 - [ ] [Autocomplete endpoint](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/autocomplete-entities)
 - [x] N-grams
 - [x] Authentication
 
 We aim to cover the entire API, and we are looking for help. We are welcoming Pull Requests.
 
@@ -41,15 +62,15 @@
 ```
 
 ## Getting started
 
 PyAlex offers support for all [Entity Objects](https://docs.openalex.org/api-entities/entities-overview): [Works](https://docs.openalex.org/api-entities/works), [Authors](https://docs.openalex.org/api-entities/authors), [Sources](https://docs.openalex.org/api-entities/sourcese), [Institutions](https://docs.openalex.org/api-entities/institutions), [Concepts](https://docs.openalex.org/api-entities/concepts), and [Publishers](https://docs.openalex.org/api-entities/publishers).
 
 ```python
-from pyalex import Works, Authors, Sources, Institutions, Concepts
+from pyalex import Works, Authors, Sources, Institutions, Concepts, Publishers
 ```
 
 ### The polite pool
 
 [The polite pool](https://docs.openalex.org/how-to-use-the-api/rate-limits-and-authentication#the-polite-pool) has much
 faster and more consistent response times. To get into the polite pool, you
 set your email:
@@ -189,14 +210,61 @@
 
 OpenAlex reference: [Sort entity lists](https://docs.openalex.org/api-entities/works/get-lists-of-works#page-and-sort-works).
 
 ```python
 Works().sort(cited_by_count="desc").get()
 ```
 
+#### Select
+
+OpenAlex reference: [Select fields](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/select-fields).
+
+```python
+Works().filter(publication_year=2020, is_oa=True).select(["id", "doi"]).get()
+```
+
+#### Sample
+
+OpenAlex reference: [Sample entity lists](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/sample-entity-lists).
+
+```python
+Works().sample(100, seed=535).get()
+```
+
+#### Logical expressions
+
+OpenAlex reference: [Logical expressions](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/filter-entity-lists#logical-expressions)
+
+Inequality:
+
+```python
+Sources().filter(works_count=">1000").get()
+```
+
+Negation (NOT):
+
+```python
+Institutions().filter(country_code="!us").get()
+```
+
+Intersection (AND):
+
+```python
+Works().filter(institutions={"country_code": ["fr", "gb"]}).get()
+
+# same
+Works().filter(institutions={"country_code": "fr"}).filter(institutions={"country_code": "gb"}).get()
+```
+
+Addition (OR):
+
+```python
+Works().filter(institutions={"country_code": "fr|gb"}).get()
+```
+
 #### Paging
 
 OpenAlex offers two methods for paging: [basic paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging#basic-paging) and [cursor paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging#cursor-paging). Both methods are supported by
 PyAlex, although cursor paging seems to be easier to implement and less error-prone.
 
 ##### Basic paging
```

### Comparing `pyalex-0.8/pyalex/__init__.py` & `pyalex-0.9/pyalex/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/pyalex/api.py` & `pyalex-0.9/pyalex/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,29 +17,63 @@
     def __setattr__(self, key, value):
         return super().__setitem__(key, value)
 
 
 config = AlexConfig(email=None, api_key=None, openalex_url="https://api.openalex.org")
 
 
-def _flatten_kv(k, v):
+def _flatten_kv(d, prefix=""):
 
-    if isinstance(v, dict):
+    if isinstance(d, dict):
 
-        if len(v.keys()) > 1:
-            raise ValueError()
+        t = []
+        for k, v in d.items():
+            if isinstance(v, list):
+                t.extend([f"{prefix}.{k}:{i}" for i in v])
+            else:
+                new_prefix = f"{prefix}.{k}" if prefix else f"{k}"
+                x = _flatten_kv(v, prefix=new_prefix)
+                t.append(x)
 
-        k_0 = list(v.keys())[0]
-        return str(k) + "." + _flatten_kv(k_0, v[k_0])
+        return ",".join(t)
     else:
 
         # workaround for bug https://groups.google.com/u/1/g/openalex-users/c/t46RWnzZaXc
-        v = str(v).lower() if isinstance(v, bool) else v
+        d = str(d).lower() if isinstance(d, bool) else d
+
+        return f"{prefix}:{d}"
+
 
-        return str(k) + ":" + str(v)
+def _params_merge(params, add_params):
+
+    for k, v in add_params.items():
+        if (
+            k in params
+            and isinstance(params[k], dict)
+            and isinstance(add_params[k], dict)
+        ):
+            _params_merge(params[k], add_params[k])
+        elif (
+            k in params
+            and not isinstance(params[k], list)
+            and isinstance(add_params[k], list)
+        ):
+            # example: params="a" and add_params=["b", "c"]
+            params[k] = [params[k]] + add_params[k]
+        elif (
+            k in params
+            and isinstance(params[k], list)
+            and not isinstance(add_params[k], list)
+        ):
+            # example: params=["b", "c"] and add_params="a"
+            params[k] = params[k] + [add_params[k]]
+        elif k in params:
+            params[k] = [params[k], add_params[k]]
+        else:
+            params[k] = add_params[k]
 
 
 def invert_abstract(inv_index):
 
     if inv_index is not None:
         l = [(w, p) for w, pos in inv_index.items() for p in pos]
         return " ".join(map(lambda x: x[0], sorted(l, key=lambda x: x[1])))
@@ -100,14 +134,15 @@
 
 class Publisher(OpenAlexEntity):
     pass
 
 
 # deprecated
 
+
 def Venue(*args, **kwargs):
 
     # warn about deprecation
     warnings.warn(
         "Venue is deprecated. Use Sources instead.",
         DeprecationWarning,
         stacklevel=2,
@@ -148,17 +183,15 @@
         return r
 
 
 class BaseOpenAlex(object):
 
     """Base class for OpenAlex objects."""
 
-    url = None
-
-    def __init__(self, params={}):
+    def __init__(self, params=None):
 
         self.params = params
 
     def _get_multi_items(self, record_list):
 
         return self.filter(openalex_id="|".join(record_list)).get()
 
@@ -178,56 +211,73 @@
         return getattr(self, key)
 
     def __getitem__(self, record_id):
 
         if isinstance(record_id, list):
             return self._get_multi_items(record_id)
 
-        url = self.url + "/" + record_id
+        url = self.url_collection + "/" + record_id
         params = {"api_key": config.api_key} if config.api_key else {}
         res = requests.get(
             url,
             headers={"User-Agent": "pyalex/" + __version__, "email": config.email},
-            params=params
+            params=params,
         )
         res.raise_for_status()
         res_json = res.json()
 
         return self.obj(res_json)
 
-    def get(self, return_meta=False, page=None, per_page=None, cursor=None):
-
-        if per_page is not None and (per_page < 1 or per_page > 200):
-            raise ValueError("per_page should be a number between 1 and 200.")
+    @property
+    def url(self):
 
-        self.params["per-page"] = per_page
-        self.params["page"] = page
-        self.params["cursor"] = cursor
+        if not self.params:
+            return self.url_collection
 
         l = []
         for k, v in self.params.items():
-            if k in ["filter", "sort"]:
-                l.append(k + "=" + ",".join(_flatten_kv(k, d) for k, d in v.items()))
-            elif v is None:
+
+            if v is None:
                 pass
+            elif isinstance(v, list):
+                v_quote = [quote_plus(q) for q in v]
+                l.append(k + "=" + ",".join(v_quote))
+            elif k in ["filter", "sort"]:
+                l.append(k + "=" + _flatten_kv(v))
             else:
                 l.append(k + "=" + quote_plus(str(v)))
 
-        url = self.url + "?" + "&".join(l)
+        if l:
+            return self.url_collection + "?" + "&".join(l)
+
+        return self.url_collection
+
+    def get(self, return_meta=False, page=None, per_page=None, cursor=None):
+
+        if per_page is not None and (per_page < 1 or per_page > 200):
+            raise ValueError("per_page should be a number between 1 and 200.")
+
+        self._add_params("per-page", per_page)
+        self._add_params("page", page)
+        self._add_params("cursor", cursor)
+
         params = {"api_key": config.api_key} if config.api_key else {}
         res = requests.get(
-            url,
+            self.url,
             headers={"User-Agent": "pyalex/" + __version__, "email": config.email},
-            params=params
+            params=params,
         )
 
         # handle query errors
         if res.status_code == 403:
             res_json = res.json()
-            if isinstance(res_json["error"], str) and "query parameters" in res_json["error"]:
+            if (
+                isinstance(res_json["error"], str)
+                and "query parameters" in res_json["error"]
+            ):
                 raise QueryError(res_json["message"])
         res.raise_for_status()
 
         res_json = res.json()
 
         # group-by or results page
         if "group-by" in self.params:
@@ -245,117 +295,101 @@
 
         return CursorPaginator(self, per_page=per_page, cursor=cursor, n_max=n_max)
 
     def random(self):
 
         return self.__getitem__("random")
 
-    def filter(self, **kwargs):
-
-        p = self.params.copy()
+    def _add_params(self, argument, new_params):
 
-        if "filter" in p:
-            p["filter"] = {**p["filter"], **kwargs}
+        if self.params is None:
+            self.params = {argument: new_params}
+        elif argument in self.params and isinstance(self.params[argument], dict):
+            _params_merge(self.params[argument], new_params)
         else:
-            p["filter"] = kwargs
+            self.params[argument] = new_params
 
-        self.params = p
-        logging.debug("Params updated:", p)
+        logging.debug("Params updated:", self.params)
+
+    def filter(self, **kwargs):
 
+        self._add_params("filter", kwargs)
         return self
 
     def search_filter(self, **kwargs):
 
-        search_kwargs = {f"{k}.search": v for k, v in kwargs.items()}
-
-        p = self.params.copy()
-
-        if "filter" in p:
-            p["filter"] = {**p["filter"], **search_kwargs}
-        else:
-            p["filter"] = search_kwargs
-
-        self.params = p
-        logging.debug("Params updated:", p)
-
+        self._add_params("filter", {f"{k}.search": v for k, v in kwargs.items()})
         return self
 
     def sort(self, **kwargs):
 
-        p = self.params.copy()
-
-        if "sort" in p:
-            p["sort"] = {**p["sort"], **kwargs}
-        else:
-            p["sort"] = kwargs
-
-        self.params = p
-        logging.debug("Params updated:", p)
-
+        self._add_params("sort", kwargs)
         return self
 
     def group_by(self, group_key):
 
-        p = self.params.copy()
-        p["group-by"] = group_key
-        self.params = p
+        self._add_params("group-by", group_key)
+        return self
 
-        logging.debug("Params updated:", p)
+    def search(self, s):
 
+        self._add_params("search", s)
         return self
 
-    def search(self, s):
+    def sample(self, n, seed=None):
 
-        p = self.params.copy()
-        p["search"] = s
-        self.params = p
+        self._add_params("sample", n)
+        self._add_params("seed", seed)
+        return self
 
-        logging.debug("Params updated:", p)
+    def select(self, s):
 
+        self._add_params("select", s)
         return self
 
 
 class Works(BaseOpenAlex):
 
-    url = config.openalex_url + "/works"
+    url_collection = config.openalex_url + "/works"
     obj = Work
 
 
 class Authors(BaseOpenAlex):
 
-    url = config.openalex_url + "/authors"
+    url_collection = config.openalex_url + "/authors"
     obj = Author
 
 
 class Sources(BaseOpenAlex):
 
-    url = config.openalex_url + "/sources"
+    url_collection = config.openalex_url + "/sources"
     obj = Source
 
 
 class Institutions(BaseOpenAlex):
 
-    url = config.openalex_url + "/institutions"
+    url_collection = config.openalex_url + "/institutions"
     obj = Institution
 
 
 class Concepts(BaseOpenAlex):
 
-    url = config.openalex_url + "/concepts"
+    url_collection = config.openalex_url + "/concepts"
     obj = Concept
 
 
 class Publishers(BaseOpenAlex):
 
-    url = config.openalex_url + "/publishers"
+    url_collection = config.openalex_url + "/publishers"
     obj = Publisher
 
 
 # deprecated
 
+
 def Venues(*args, **kwargs):
 
     # warn about deprecation
     warnings.warn(
         "Venues is deprecated. Use Sources instead.",
         DeprecationWarning,
         stacklevel=2,
```

### Comparing `pyalex-0.8/pyalex.egg-info/PKG-INFO` & `pyalex-0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pyalex
-Version: 0.8
-Summary: One downloader for many scientific data and code repositories!
-Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: test
-License-File: LICENSE
-
 <p align="center">
   <img alt="PyAlex - a Python wrapper for OpenAlex" src="https://github.com/J535D165/pyalex/raw/main/pyalex_repocard.svg">
 </p>
 
 # PyAlex
 
 ![PyPI](https://img.shields.io/pypi/v/pyalex) [![DOI](https://zenodo.org/badge/557541347.svg)](https://zenodo.org/badge/latestdoi/557541347)
@@ -34,14 +15,16 @@
 The following features of OpenAlex are currently supported by PyAlex:
 
 - [x] Get single entities
 - [x] Filter entities
 - [x] Search entities
 - [x] Group entities
 - [x] Search filters
+- [x] Select fields
+- [x] Sample
 - [x] Pagination
 - [ ] [Autocomplete endpoint](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/autocomplete-entities)
 - [x] N-grams
 - [x] Authentication
 
 We aim to cover the entire API, and we are looking for help. We are welcoming Pull Requests.
 
@@ -60,15 +43,15 @@
 ```
 
 ## Getting started
 
 PyAlex offers support for all [Entity Objects](https://docs.openalex.org/api-entities/entities-overview): [Works](https://docs.openalex.org/api-entities/works), [Authors](https://docs.openalex.org/api-entities/authors), [Sources](https://docs.openalex.org/api-entities/sourcese), [Institutions](https://docs.openalex.org/api-entities/institutions), [Concepts](https://docs.openalex.org/api-entities/concepts), and [Publishers](https://docs.openalex.org/api-entities/publishers).
 
 ```python
-from pyalex import Works, Authors, Sources, Institutions, Concepts
+from pyalex import Works, Authors, Sources, Institutions, Concepts, Publishers
 ```
 
 ### The polite pool
 
 [The polite pool](https://docs.openalex.org/how-to-use-the-api/rate-limits-and-authentication#the-polite-pool) has much
 faster and more consistent response times. To get into the polite pool, you
 set your email:
@@ -208,14 +191,61 @@
 
 OpenAlex reference: [Sort entity lists](https://docs.openalex.org/api-entities/works/get-lists-of-works#page-and-sort-works).
 
 ```python
 Works().sort(cited_by_count="desc").get()
 ```
 
+#### Select
+
+OpenAlex reference: [Select fields](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/select-fields).
+
+```python
+Works().filter(publication_year=2020, is_oa=True).select(["id", "doi"]).get()
+```
+
+#### Sample
+
+OpenAlex reference: [Sample entity lists](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/sample-entity-lists).
+
+```python
+Works().sample(100, seed=535).get()
+```
+
+#### Logical expressions
+
+OpenAlex reference: [Logical expressions](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/filter-entity-lists#logical-expressions)
+
+Inequality:
+
+```python
+Sources().filter(works_count=">1000").get()
+```
+
+Negation (NOT):
+
+```python
+Institutions().filter(country_code="!us").get()
+```
+
+Intersection (AND):
+
+```python
+Works().filter(institutions={"country_code": ["fr", "gb"]}).get()
+
+# same
+Works().filter(institutions={"country_code": "fr"}).filter(institutions={"country_code": "gb"}).get()
+```
+
+Addition (OR):
+
+```python
+Works().filter(institutions={"country_code": "fr|gb"}).get()
+```
+
 #### Paging
 
 OpenAlex offers two methods for paging: [basic paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging#basic-paging) and [cursor paging](https://docs.openalex.org/how-to-use-the-api/get-lists-of-entities/paging#cursor-paging). Both methods are supported by
 PyAlex, although cursor paging seems to be easier to implement and less error-prone.
 
 ##### Basic paging
```

### Comparing `pyalex-0.8/pyalex_repocard.png` & `pyalex-0.9/pyalex_repocard.png`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/pyalex_repocard.svg` & `pyalex-0.9/pyalex_repocard.svg`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/pyproject.toml` & `pyalex-0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalex-0.8/tests/test_pyalex.py` & `pyalex-0.9/tests/test_pyalex.py`

 * *Files 18% similar despite different names*

```diff
@@ -125,14 +125,24 @@
     # )
 
     assert r["meta"]["count"] == w1["count"]
     assert r["meta"]["count"] == w2["count"]
     # assert r["meta"]["count"] == c["count"]
 
 
+def test_works_url():
+
+    url = "https://api.openalex.org/works?filter=publication_year:2020,is_oa:true"
+
+    assert url == Works().filter(publication_year=2020, is_oa=True).url
+    assert url == Works().filter(publication_year=2020).filter(is_oa=True).url
+
+    assert Works().url == "https://api.openalex.org/works"
+
+
 def test_works_multifilter_meta():
 
     _, m1 = Works().filter(publication_year=2020, is_oa=True).get(return_meta=True)
     _, m2 = (
         Works().filter(publication_year=2020).filter(is_oa=True).get(return_meta=True)
     )
 
@@ -334,7 +344,60 @@
 
     assert meta["count"] == 1068
 
 
 def test_random_publishers():
 
     assert isinstance(Publishers().random(), dict)
+
+
+def test_and_operator():
+
+    # https://github.com/J535D165/pyalex/issues/11
+    url = "https://api.openalex.org/works?filter=institutions.country_code:tw,institutions.country_code:hk,institutions.country_code:us,publication_year:2022"  # noqa
+
+    assert (
+        url
+        == Works()
+        .filter(
+            institutions={"country_code": ["tw", "hk", "us"]}, publication_year=2022
+        )
+        .url
+    )
+    assert (
+        url
+        == Works()
+        .filter(institutions={"country_code": "tw"})
+        .filter(institutions={"country_code": "hk"})
+        .filter(institutions={"country_code": "us"})
+        .filter(publication_year=2022)
+        .url
+    )
+    assert (
+        url
+        == Works()
+        .filter(institutions={"country_code": ["tw", "hk"]})
+        .filter(institutions={"country_code": "us"})
+        .filter(publication_year=2022)
+        .url
+    )
+
+
+def test_sample():
+
+    url = "https://api.openalex.org/works?filter=publication_year:2020,is_oa:true&sample=50"
+    assert url == Works().filter(publication_year=2020, is_oa=True).sample(50).url
+
+
+def test_sample_seed():
+
+    url = "https://api.openalex.org/works?filter=publication_year:2020,is_oa:true&sample=50&seed=535"  # noqa
+    assert (
+        url
+        == Works().filter(publication_year=2020, is_oa=True).sample(50, seed=535).url
+    )
+
+
+def test_subset():
+
+    url = "https://api.openalex.org/works?select=id,doi,display_name"
+    assert url == Works().select(["id", "doi", "display_name"]).url
```

