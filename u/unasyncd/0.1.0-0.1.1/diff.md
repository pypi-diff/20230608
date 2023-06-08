# Comparing `tmp/unasyncd-0.1.0.tar.gz` & `tmp/unasyncd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unasyncd-0.1.0.tar", max compression
+gzip compressed data, was "unasyncd-0.1.1.tar", max compression
```

## Comparing `unasyncd-0.1.0.tar` & `unasyncd-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-08 12:12:23.613180 unasyncd-0.1.0/LICENSE
--rw-r--r--   0        0        0    14752 2023-06-08 12:12:23.617179 unasyncd-0.1.0/README.md
--rw-r--r--   0        0        0      814 2023-06-08 12:12:23.617179 unasyncd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 12:12:23.617179 unasyncd-0.1.0/unasyncd/__init__.py
--rw-r--r--   0        0        0     3693 2023-06-08 12:12:23.617179 unasyncd-0.1.0/unasyncd/cli.py
--rw-r--r--   0        0        0     2475 2023-06-08 12:12:23.617179 unasyncd-0.1.0/unasyncd/config.py
--rw-r--r--   0        0        0    10470 2023-06-08 12:12:23.617179 unasyncd-0.1.0/unasyncd/main.py
--rw-r--r--   0        0        0    34690 2023-06-08 12:12:23.617179 unasyncd-0.1.0/unasyncd/transformers.py
--rw-r--r--   0        0        0    15347 1970-01-01 00:00:00.000000 unasyncd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-08 18:10:22.032836 unasyncd-0.1.1/LICENSE
+-rw-r--r--   0        0        0    14752 2023-06-08 18:10:22.032836 unasyncd-0.1.1/README.md
+-rw-r--r--   0        0        0      814 2023-06-08 18:10:22.032836 unasyncd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/__init__.py
+-rw-r--r--   0        0        0     3693 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/cli.py
+-rw-r--r--   0        0        0     2475 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/config.py
+-rw-r--r--   0        0        0    10308 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/main.py
+-rw-r--r--   0        0        0    34690 2023-06-08 18:10:22.032836 unasyncd-0.1.1/unasyncd/transformers.py
+-rw-r--r--   0        0        0    15347 1970-01-01 00:00:00.000000 unasyncd-0.1.1/PKG-INFO
```

### Comparing `unasyncd-0.1.0/LICENSE` & `unasyncd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unasyncd-0.1.0/README.md` & `unasyncd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unasyncd-0.1.0/pyproject.toml` & `unasyncd-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unasyncd"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Janek Nouvertné <j.a.nouvertne@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `unasyncd-0.1.0/unasyncd/cli.py` & `unasyncd-0.1.1/unasyncd/cli.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.1.0/unasyncd/config.py` & `unasyncd-0.1.1/unasyncd/config.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.1.0/unasyncd/main.py` & `unasyncd-0.1.1/unasyncd/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,30 +197,26 @@
         their expected state.
 
         The files are considered equal if since the last run:
 
         - ``source_file`` stats have not changed
         - ``source_file`` is AST-equivalent to its previous version
         - ``target_file`` does exist
-        - ``target_file`` is AST-equivalent to its previous version
 
         If the ``force_regen`` option is used, always return ``True``.
         """
         if self.config.force_regen:
             return True
 
         if not await source.meta_equal(await self.get_meta(source)):
             return True
 
         if not await target.exists():
             return True
 
-        if not await target.meta_equal(await self.get_meta(target)):
-            return True
-
         return False
 
     async def _restore_from_cache(self, source: File, target: File) -> bool:
         """If a cached transformation for ``source`` exists, copy it to ``target``.
         If ``force_regen`` is ``True``, do nothing.
         """
         if self.config.force_regen:
```

### Comparing `unasyncd-0.1.0/unasyncd/transformers.py` & `unasyncd-0.1.1/unasyncd/transformers.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.1.0/PKG-INFO` & `unasyncd-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unasyncd
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Janek Nouvertné
 Author-email: j.a.nouvertne@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

