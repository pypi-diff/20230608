# Comparing `tmp/polario-0.2.4.tar.gz` & `tmp/polario-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polario-0.2.4.tar", max compression
+gzip compressed data, was "polario-0.2.5.tar", max compression
```

## Comparing `polario-0.2.4.tar` & `polario-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-08 12:50:19.990759 polario-0.2.4/LICENSE
--rw-r--r--   0        0        0      694 2023-06-08 12:50:19.990759 polario-0.2.4/README.md
--rw-r--r--   0        0        0      106 2023-06-08 12:50:19.990759 polario-0.2.4/polario/__init__.py
--rw-r--r--   0        0        0    11585 2023-06-08 12:50:19.990759 polario-0.2.4/polario/dataset.py
--rw-r--r--   0        0        0     1644 2023-06-08 12:50:19.990759 polario-0.2.4/polario/main.py
--rw-r--r--   0        0        0        0 2023-06-08 12:50:19.990759 polario-0.2.4/polario/py.typed
--rw-r--r--   0        0        0      999 2023-06-08 12:50:45.798943 polario-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 polario-0.2.4/setup.py
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 polario-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 13:37:04.504427 polario-0.2.5/LICENSE
+-rw-r--r--   0        0        0      694 2023-06-08 13:37:04.504427 polario-0.2.5/README.md
+-rw-r--r--   0        0        0      106 2023-06-08 13:37:04.508427 polario-0.2.5/polario/__init__.py
+-rw-r--r--   0        0        0    11649 2023-06-08 13:37:04.508427 polario-0.2.5/polario/dataset.py
+-rw-r--r--   0        0        0     1644 2023-06-08 13:37:04.508427 polario-0.2.5/polario/main.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:37:04.508427 polario-0.2.5/polario/py.typed
+-rw-r--r--   0        0        0      999 2023-06-08 13:37:23.492444 polario-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 polario-0.2.5/setup.py
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 polario-0.2.5/PKG-INFO
```

### Comparing `polario-0.2.4/LICENSE` & `polario-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polario-0.2.4/README.md` & `polario-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `polario-0.2.4/polario/dataset.py` & `polario-0.2.5/polario/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,18 @@
         partition_location = self.partition_location(partition_values=partition_values)
         fs = fsspec.filesystem(self.location.scheme)
         parquet_files = [
             fragment_location
             for fragment_location in fs.ls(partition_location, detail=False)
             if fragment_location.endswith(".parquet")
         ]
+        scheme_prefix = f"{self.location.scheme}://" if self.location.scheme else ""
         return pl.concat(
             [
-                pl.read_parquet(urlunsplit(self.location._replace(path=parquet_file)))
+                pl.read_parquet(f"{scheme_prefix}{parquet_file}")
                 for parquet_file in parquet_files
             ]
         ).with_columns(
             [
                 pl.lit(parcol_value).alias(parcol_name)
                 for parcol_name, parcol_value in partition_values.items()
             ]
```

### Comparing `polario-0.2.4/polario/main.py` & `polario-0.2.5/polario/main.py`

 * *Files identical despite different names*

### Comparing `polario-0.2.4/pyproject.toml` & `polario-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polario"
-version = "0.2.4"
+version = "0.2.5"
 description = "Polars IO"
 authors = ["Bram Neijt <bram@neijt.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bneijt.github.io/polario/"
 repository = "https://github.com/bneijt/polario"
 classifiers = [
```

### Comparing `polario-0.2.4/setup.py` & `polario-0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['fsspec>=2023.1.0,<2024.0.0', 'polars>=0.16.8', 'pyarrow>=11.0.0']
 
 entry_points = \
 {'console_scripts': ['polario = polario.main:main']}
 
 setup_kwargs = {
     'name': 'polario',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'Polars IO',
     'long_description': 'Polars IO utility library\n=================\n\nHelpers to make it easier to read and write Hive partitioned parquet dataset with Polars.\n\nIt is meant to be a library to deal with datasets easily, but also contains a commandline interface\nwhich allows you to inspect parquet files and datasets more easily.\n\nDataset\n=======\nExample of use of `polario.dataset.HiveDataset`\n```python\n\nfrom polario.dataset import HiveDataset\nimport polars as pl\ndf = pl.from_dicts(\n        [\n            {"p1": 1, "v": 1},\n            {"p1": 2, "v": 1},\n        ]\n    )\n\nds = HiveDataset("file:///tmp/", partition_columns=["p1"])\n\nds.write(df)\n\nfor partition_df in ds.read_partitions():\n    print(partition_df)\n\n```\n',
     'author': 'Bram Neijt',
     'author_email': 'bram@neijt.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bneijt.github.io/polario/',
```

### Comparing `polario-0.2.4/PKG-INFO` & `polario-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polario
-Version: 0.2.4
+Version: 0.2.5
 Summary: Polars IO
 Home-page: https://bneijt.github.io/polario/
 License: Apache-2.0
 Author: Bram Neijt
 Author-email: bram@neijt.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

