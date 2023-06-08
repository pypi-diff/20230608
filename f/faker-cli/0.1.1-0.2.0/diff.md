# Comparing `tmp/faker_cli-0.1.1.tar.gz` & `tmp/faker_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_cli-0.1.1.tar", max compression
+gzip compressed data, was "faker_cli-0.2.0.tar", max compression
```

## Comparing `faker_cli-0.1.1.tar` & `faker_cli-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-01 06:00:07.671393 faker_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     2916 2023-06-01 06:00:07.671393 faker_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/__init__.py
--rw-r--r--   0        0        0     2799 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/cli.py
--rw-r--r--   0        0        0    27694 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/templates.py
--rw-r--r--   0        0        0      809 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/writer.py
--rw-r--r--   0        0        0      461 2023-06-01 06:00:12.147436 faker_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 faker_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-08 20:43:16.777604 faker_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3217 2023-06-08 20:43:16.777604 faker_cli-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/__init__.py
+-rw-r--r--   0        0        0     3157 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/cli.py
+-rw-r--r--   0        0        0    27694 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/templates.py
+-rw-r--r--   0        0        0     1517 2023-06-08 20:43:16.777604 faker_cli-0.2.0/faker_cli/writer.py
+-rw-r--r--   0        0        0      569 2023-06-08 20:43:42.865893 faker_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 faker_cli-0.2.0/PKG-INFO
```

### Comparing `faker_cli-0.1.1/LICENSE` & `faker_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_cli-0.1.1/README.md` & `faker_cli-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Faker CLI
 
 Faker is an awesome Python library, but I often just want a simple command I can run to generate data in a variety of formats.
 
-With Faker CLI, you can easily generate CSV or JSON data with fields of your choosing.
+With Faker CLI, you can easily generate CSV, JSON, or Parquet data with fields of your choosing.
 
 You can also utilize pre-built templates for common data formats!
 
 ## Usage
 
 By default, `fake` will generate a CSV output for you. You just specify the number of rows you want and the column types.
 
@@ -66,14 +66,28 @@
 {"id": 6071, "awesome_name": "wilcoxrick", "last_attention_at": "2023-01-17"}
 {"id": 9646, "awesome_name": "michael92", "last_attention_at": "2023-04-22"}
 {"id": 6986, "awesome_name": "ballen", "last_attention_at": "2023-01-08"}
 {"id": 6892, "awesome_name": "jennifer61", "last_attention_at": "2023-01-03"}
 {"id": 1967, "awesome_name": "jmendoza", "last_attention_at": "2023-01-23"}
 ```
 
+### Parquet
+
+OK, it had to happen, you can even write Parquet. 
+
+```bash
+fake -n 10 pyint,user_name,date_this_year -f parquet -o sample.parquet
+```
+
+_youcanevenwritestraighttos3_ 🤭
+
+```bash
+fake -n 10 pyint,user_name,date_this_year -f parquet -o s3://YOUR_BUCKET/data/sample.parquet
+```
+
 ## Templates
 
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
 fake -t s3access -n 10
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `faker_cli-0.1.1/faker_cli/templates.py` & `faker_cli-0.2.0/faker_cli/templates.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.1.1/PKG-INFO` & `faker_cli-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: faker-cli
-Version: 0.1.1
-Summary: 
+Version: 0.2.0
+Summary: Command-line fake data generator
 Author: Damon P. Cortesi
 Author-email: d.lifehacker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: faker (>=18.9.0,<19.0.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Description-Content-Type: text/markdown
 
 # Faker CLI
 
 Faker is an awesome Python library, but I often just want a simple command I can run to generate data in a variety of formats.
 
-With Faker CLI, you can easily generate CSV or JSON data with fields of your choosing.
+With Faker CLI, you can easily generate CSV, JSON, or Parquet data with fields of your choosing.
 
 You can also utilize pre-built templates for common data formats!
 
 ## Usage
 
 By default, `fake` will generate a CSV output for you. You just specify the number of rows you want and the column types.
 
@@ -81,14 +82,28 @@
 {"id": 6071, "awesome_name": "wilcoxrick", "last_attention_at": "2023-01-17"}
 {"id": 9646, "awesome_name": "michael92", "last_attention_at": "2023-04-22"}
 {"id": 6986, "awesome_name": "ballen", "last_attention_at": "2023-01-08"}
 {"id": 6892, "awesome_name": "jennifer61", "last_attention_at": "2023-01-03"}
 {"id": 1967, "awesome_name": "jmendoza", "last_attention_at": "2023-01-23"}
 ```
 
+### Parquet
+
+OK, it had to happen, you can even write Parquet. 
+
+```bash
+fake -n 10 pyint,user_name,date_this_year -f parquet -o sample.parquet
+```
+
+_youcanevenwritestraighttos3_ 🤭
+
+```bash
+fake -n 10 pyint,user_name,date_this_year -f parquet -o s3://YOUR_BUCKET/data/sample.parquet
+```
+
 ## Templates
 
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
 fake -t s3access -n 10
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

