# Comparing `tmp/satori_playbook_validator-2.0.1.tar.gz` & `tmp/satori_playbook_validator-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-2.0.1.tar", last modified: Thu Jun  8 16:27:49 2023, max compression
+gzip compressed data, was "satori_playbook_validator-2.0.2.tar", last modified: Thu Jun  8 21:43:02 2023, max compression
```

## Comparing `satori_playbook_validator-2.0.1.tar` & `satori_playbook_validator-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       30 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/README.md
--rw-r--r--   0        0        0      474 2023-06-08 16:27:49.153746 satori_playbook_validator-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      176 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     5091 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1049 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1837 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      351 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/tests/test_playbook_validator.py
--rw-r--r--   0        0        0     2276 2023-06-08 16:27:34.929562 satori_playbook_validator-2.0.1/tests/test_reference_finder.py
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/README.md
+-rw-r--r--   0        0        0      474 2023-06-08 21:43:02.034712 satori_playbook_validator-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     5094 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-06-08 21:42:40.218434 satori_playbook_validator-2.0.2/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1049 2023-06-08 21:42:40.222434 satori_playbook_validator-2.0.2/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1837 2023-06-08 21:42:40.222434 satori_playbook_validator-2.0.2/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      351 2023-06-08 21:42:40.222434 satori_playbook_validator-2.0.2/tests/test_playbook_validator.py
+-rw-r--r--   0        0        0     2469 2023-06-08 21:42:40.222434 satori_playbook_validator-2.0.2/tests/test_reference_finder.py
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 satori_playbook_validator-2.0.2/PKG-INFO
```

### Comparing `satori_playbook_validator-2.0.1/src/satorici/validator/_validator.py` & `satori_playbook_validator-2.0.2/src/satorici/validator/_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             if key == limit_key:
                 limit_key = current.get("^key")
                 current = current.get("^dict")
                 break
 
             if key in variables:
                 if validate_inputs(value) or (
-                    validate_test(value) and has_input(value)
+                    isinstance(value, dict) and has_input(value)
                 ):
                     valid.add(key)
                 else:
                     failed = True
                     break
 
     if valid != variables:
```

### Comparing `satori_playbook_validator-2.0.1/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-2.0.2/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.0.1/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-2.0.2/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.0.1/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-2.0.2/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-2.0.1/tests/test_reference_finder.py` & `satori_playbook_validator-2.0.2/tests/test_reference_finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,13 +98,22 @@
                 "cmd": [["$(root)"]],
             },
             "child2": {
                 "input": ["1"],
             },
         }
     },
+    {
+        # Ref an adjacent test that has one input
+        "root": {
+            "sub": {
+                "input": ["1"],
+            },
+            "cmd": [["$(sub)"]],
+        },
+    },
 ]
 
 
 @pytest.mark.parametrize("playbook", passed_refs)
 def test_passed_references(playbook):
     validate_playbook(playbook)
```

