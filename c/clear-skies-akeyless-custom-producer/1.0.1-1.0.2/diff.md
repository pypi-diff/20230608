# Comparing `tmp/clear_skies_akeyless_custom_producer-1.0.1.tar.gz` & `tmp/clear_skies_akeyless_custom_producer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_akeyless_custom_producer-1.0.1.tar", max compression
+gzip compressed data, was "clear_skies_akeyless_custom_producer-1.0.2.tar", max compression
```

## Comparing `clear_skies_akeyless_custom_producer-1.0.1.tar` & `clear_skies_akeyless_custom_producer-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1053 2023-05-10 15:19:24.285335 clear_skies_akeyless_custom_producer-1.0.1/LICENSE
--rw-r--r--   0        0        0     6259 2023-05-12 15:20:11.769906 clear_skies_akeyless_custom_producer-1.0.1/README.md
--rw-r--r--   0        0        0      710 2023-06-07 12:57:28.170389 clear_skies_akeyless_custom_producer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-10 10:54:42.233306 clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/__init__.py
--rw-r--r--   0        0        0       30 2023-05-11 19:55:49.528090 clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/__init__.py
--rw-r--r--   0        0        0     9756 2023-06-01 11:15:55.029296 clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/no_input.py
--rw-r--r--   0        0        0     7392 2023-06-01 11:17:20.022617 clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/no_input_test.py
--rw-r--r--   0        0        0     5948 2023-05-12 14:49:21.358575 clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/with_input.py
--rw-r--r--   0        0        0     7063 1970-01-01 00:00:00.000000 clear_skies_akeyless_custom_producer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-05-10 15:19:24.285335 clear_skies_akeyless_custom_producer-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6259 2023-05-12 15:20:11.769906 clear_skies_akeyless_custom_producer-1.0.2/README.md
+-rw-r--r--   0        0        0      710 2023-06-08 21:57:41.037527 clear_skies_akeyless_custom_producer-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-10 10:54:42.233306 clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-11 19:55:49.528090 clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/__init__.py
+-rw-r--r--   0        0        0     9843 2023-06-08 21:57:33.197478 clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/no_input.py
+-rw-r--r--   0        0        0     7392 2023-06-01 11:17:20.022617 clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/no_input_test.py
+-rw-r--r--   0        0        0     5948 2023-05-12 14:49:21.358575 clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/with_input.py
+-rw-r--r--   0        0        0     7063 1970-01-01 00:00:00.000000 clear_skies_akeyless_custom_producer-1.0.2/PKG-INFO
```

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/LICENSE` & `clear_skies_akeyless_custom_producer-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/README.md` & `clear_skies_akeyless_custom_producer-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/pyproject.toml` & `clear_skies_akeyless_custom_producer-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-akeyless-custom-producer"
-version = "1.0.1"
+version = "1.0.2"
 description = "clearskies handlers for hosting Akeyless custom producer endpoints"
 authors = [
     "Conor Mancone <cmancone@gmail.com>"
 ]
 repository = "https://github.com/cmancone/clearskies-akeyless-custom-producer"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/no_input.py` & `clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/no_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,16 @@
         # we need to return a meaningful id if we are going to revoke at the end
         if self.configuration('can_revoke'):
             id_column_name = self.configuration('id_column_name')
             if id_column_name not in credentials:
                 raise ValueError(
                     f"Response from create callable did not include the required id column: '{id_column_name}'"
                 )
-            credential_id = credentials[id_column_name]
+            # akeyless will only accept strings as the id value - no integers/etc
+            credential_id = str(credentials[id_column_name])
         else:
             credential_id = 'i_dont_need_an_id'
 
         return input_output.respond({
             'id': credential_id,
             'response': credentials,
         }, 200)
```

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/no_input_test.py` & `clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/no_input_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/src/clearskies_akeyless_custom_producer/handlers/with_input.py` & `clear_skies_akeyless_custom_producer-1.0.2/src/clearskies_akeyless_custom_producer/handlers/with_input.py`

 * *Files identical despite different names*

### Comparing `clear_skies_akeyless_custom_producer-1.0.1/PKG-INFO` & `clear_skies_akeyless_custom_producer-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-akeyless-custom-producer
-Version: 1.0.1
+Version: 1.0.2
 Summary: clearskies handlers for hosting Akeyless custom producer endpoints
 Home-page: https://github.com/cmancone/clearskies-akeyless-custom-producer
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

