# Comparing `tmp/satori_playbook_validator-1.0.6.tar.gz` & `tmp/satori_playbook_validator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.6.tar", last modified: Thu May 25 02:15:22 2023, max compression
+gzip compressed data, was "satori_playbook_validator-1.0.8.tar", last modified: Wed Jun  7 18:04:57 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.6.tar` & `satori_playbook_validator-1.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       30 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/README.md
--rw-r--r--   0        0        0      433 2023-05-25 02:15:22.191980 satori_playbook_validator-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     3268 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1818 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-07 18:04:39.994040 satori_playbook_validator-1.0.8/README.md
+-rw-r--r--   0        0        0      433 2023-06-07 18:04:57.877850 satori_playbook_validator-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     3270 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1818 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.8/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.6/src/satorici/validator/_validator.py` & `satori_playbook_validator-1.0.8/src/satorici/validator/_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             else:
                 raise PlaybookVariableError(
                     f"No valid inputs for variable: {variable}", parameter=variable
                 )
 
         if not found_prefix:
             raise PlaybookVariableError(
-                f"Can't resolve variable: {variable}", parameter=variable
+                f"Can't resolve variable: {variable}. ", parameter=variable
             )
 
 
 def validate_playbook(config: dict):
     """
     Validate yaml loaded playbook config and return corresponding dict
```

### Comparing `satori_playbook_validator-1.0.6/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-1.0.8/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.6/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-1.0.8/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.6/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-1.0.8/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

