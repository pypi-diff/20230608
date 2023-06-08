# Comparing `tmp/satori_playbook_validator-1.0.8.tar.gz` & `tmp/satori_playbook_validator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.8.tar", last modified: Wed Jun  7 18:04:57 2023, max compression
+gzip compressed data, was "satori_playbook_validator-2.0.0.tar", last modified: Thu Jun  8 16:16:43 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.8.tar` & `satori_playbook_validator-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       30 2023-06-07 18:04:39.994040 satori_playbook_validator-1.0.8/README.md
--rw-r--r--   0        0        0      433 2023-06-07 18:04:57.877850 satori_playbook_validator-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     3270 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1818 2023-06-07 18:04:39.998040 satori_playbook_validator-1.0.8/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/README.md
+-rw-r--r--   0        0        0      474 2023-06-08 16:16:43.138033 satori_playbook_validator-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5093 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1837 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0     2276 2023-06-08 16:16:28.173823 satori_playbook_validator-2.0.0/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.0.0/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.8/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-2.0.0/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.8/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-2.0.0/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.8/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-2.0.0/src/satorici/validator/schemas/test.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428571%*

 * *Differences: {"'additionalProperties'": "{'anyOf': {0: {'$ref': 'file://./import.json'}, 1: {'$ref': "*

 * *                           "'file://./input.json'}, 2: {'$ref': 'file://./command.json'}, 3: "*

 * *                           "{'$ref': '#'}}}"}*

```diff
@@ -1,22 +1,22 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": {
         "anyOf": [
             {
-                "$ref": "import.json"
+                "$ref": "file://./import.json"
             },
             {
-                "$ref": "input.json"
+                "$ref": "file://./input.json"
             },
             {
-                "$ref": "command.json"
+                "$ref": "file://./command.json"
             },
             {
-                "$ref": "test.json"
+                "$ref": "#"
             }
         ]
     },
     "description": "Test",
     "patternProperties": {
         "^assert(File|Command)Exists$": {
             "items": {
```

