# Comparing `tmp/ream2-2.6.0.tar.gz` & `tmp/ream2-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.6.0.tar", max compression
+gzip compressed data, was "ream2-2.6.1.tar", max compression
```

## Comparing `ream2-2.6.0.tar` & `ream2-2.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-05-19 00:38:31.312440 ream2-2.6.0/LICENSE
--rw-r--r--   0        0        0     5267 2023-05-19 00:38:31.312440 ream2-2.6.0/README.md
--rw-r--r--   0        0        0      752 2023-05-19 00:38:31.316441 ream2-2.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/__init__.py
--rw-r--r--   0        0        0    13032 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actor_graph.py
--rw-r--r--   0        0        0     2197 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/__init__.py
--rw-r--r--   0        0        0     3815 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/base.py
--rw-r--r--   0        0        0     1155 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/dsid.py
--rw-r--r--   0        0        0      976 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/actors/interface.py
--rw-r--r--   0        0        0    37569 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/cli_helper.py
--rw-r--r--   0        0        0    34210 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/data_model_helper.py
--rw-r--r--   0        0        0    14434 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/dataset_helper.py
--rw-r--r--   0        0        0     9669 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/helper.py
--rw-r--r--   0        0        0     5684 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/prelude.py
--rw-r--r--   0        0        0     2248 2023-05-19 00:38:31.316441 ream2-2.6.0/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-07 23:26:17.540756 ream2-2.6.1/LICENSE
+-rw-r--r--   0        0        0     5267 2023-06-07 23:26:17.540756 ream2-2.6.1/README.md
+-rw-r--r--   0        0        0      752 2023-06-07 23:26:17.540756 ream2-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/__init__.py
+-rw-r--r--   0        0        0    13032 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/__init__.py
+-rw-r--r--   0        0        0     3815 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/dsid.py
+-rw-r--r--   0        0        0      976 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/actors/interface.py
+-rw-r--r--   0        0        0    37569 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9838 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/helper.py
+-rw-r--r--   0        0        0     5684 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/params_helper.py
+-rw-r--r--   0        0        0     1090 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-06-07 23:26:17.540756 ream2-2.6.1/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.6.1/PKG-INFO
```

### Comparing `ream2-2.6.0/LICENSE` & `ream2-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/README.md` & `ream2-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/pyproject.toml` & `ream2-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.6.0"
+version = "2.6.1"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.6.0/ream/actor_graph.py` & `ream2-2.6.1/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/actor_state.py` & `ream2-2.6.1/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/actor_version.py` & `ream2-2.6.1/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/actors/base.py` & `ream2-2.6.1/ream/actors/base.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/actors/dsid.py` & `ream2-2.6.1/ream/actors/dsid.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/actors/enum.py` & `ream2-2.6.1/ream/actors/enum.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/cache_helper.py` & `ream2-2.6.1/ream/cache_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/cli_helper.py` & `ream2-2.6.1/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/data_model_helper.py` & `ream2-2.6.1/ream/data_model_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/dataset_helper.py` & `ream2-2.6.1/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/fs.py` & `ream2-2.6.1/ream/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,19 +202,22 @@
                 if last_id is None:
                     last_id = 0
 
                 pdiskpath = Path(self.diskpath)
                 ext = "".join(pdiskpath.suffixes)
                 if self.subdir and ext == "":
                     if self.subdir_incr:
-                        dirs = [
-                            int(d.name)
-                            for d in pdiskpath.iterdir()
-                            if d.is_dir() and d.name.isdigit()
-                        ]
+                        if (self.fs.root / pdiskpath).exists():
+                            dirs = [
+                                int(d.name)
+                                for d in (self.fs.root / pdiskpath).iterdir()
+                                if d.is_dir() and d.name.isdigit()
+                            ]
+                        else:
+                            dirs = []
                         if len(dirs) == 0:
                             subdirname = f"{0:03d}"
                         else:
                             subdirname = f"{max(dirs) + 1:03d}"
                         self._realdiskpath = str(pdiskpath / subdirname)
                     else:
                         self._realdiskpath = str(pdiskpath / f"{last_id + 1:03d}")
```

### Comparing `ream2-2.6.0/ream/helper.py` & `ream2-2.6.1/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/params_helper.py` & `ream2-2.6.1/ream/params_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/prelude.py` & `ream2-2.6.1/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/ream/workspace.py` & `ream2-2.6.1/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.6.0/PKG-INFO` & `ream2-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.6.0
+Version: 2.6.1
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

