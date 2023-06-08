# Comparing `tmp/rosa_python_client-1.0.7.tar.gz` & `tmp/rosa_python_client-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.7.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.8.tar", max compression
```

## Comparing `rosa_python_client-1.0.7.tar` & `rosa_python_client-1.0.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      511 2023-05-21 12:42:53.461794 rosa_python_client-1.0.7/README.md
--rw-r--r--   0        0        0      353 2023-05-21 12:42:53.462794 rosa_python_client-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 12:42:53.462794 rosa_python_client-1.0.7/rosa/__init__.py
--rw-r--r--   0        0        0     5360 2023-05-21 12:42:53.462794 rosa_python_client-1.0.7/rosa/cli.py
--rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      511 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/README.md
+-rw-r--r--   0        0        0      353 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/rosa/__init__.py
+-rw-r--r--   0        0        0     6338 2023-06-08 08:13:24.162913 rosa_python_client-1.0.8/rosa/cli.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.8/PKG-INFO
```

### Comparing `rosa_python_client-1.0.7/rosa/cli.py` & `rosa_python_client-1.0.8/rosa/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -104,21 +104,46 @@
                     flag_str=auto_mode_str,
                 )
 
     return commands_dict
 
 
 def parse_json_response(response):
-    try:
-        return json.loads(response)
-    except json.decoder.JSONDecodeError:
-        return response.splitlines()
+    def _try_json_load(arg):
+        try:
+            return json.loads(arg)
+        except json.decoder.JSONDecodeError:
+            return arg
+
+    return {
+        "out": _try_json_load(response.stdout),
+        "err": _try_json_load(response.stderr),
+    }
 
 
 def execute(command, allowed_commands=None):
+    """
+    Support commands and execute with ROSA cli
+
+    Args:
+        command (str): ROSA cli command to execute
+        allowed_commands (dict): Commands dict of dicts with following
+            options for each entry
+            Example:
+                {'create':
+                    {'account-roles': {'json_output': False, 'auto_answer_yes': True,
+                        'auto_mode': True, 'billing_model': False},
+                    'admin': {'json_output': True, 'auto_answer_yes': True, 'auto_mode': False, 'billing_model': False},
+                    'cluster': {'json_output': True, 'auto_answer_yes': True, 'auto_mode': True, 'billing_model': False}
+                    }}
+
+    Returns:
+        dict: {'out': res.stdout, 'err': res.stderr}
+                res.stdout/stderr will be parsed as json if possible, else str
+    """
     allowed_commands = allowed_commands or parse_help()
     _user_command = shlex.split(command)
     command = ["rosa"]
     command.extend(_user_command)
     json_output = {}
     auto_answer_yes = {}
     auto_update = {}
@@ -137,13 +162,13 @@
             command.append("--yes")
 
         auto_update = allowed_commands.get(cmd, auto_update.get(cmd, {}))
         add_auto_update = auto_update.get("auto_mode") is True
         if add_auto_update:
             command.append("--mode=auto")
 
-        if add_json_output or add_auto_answer_yes or add_auto_update:
+        if any([add_json_output, add_auto_answer_yes, add_auto_update]):
             break
 
     LOGGER.info(f"Executing command: {' '.join(command)}")
     res = subprocess.run(command, capture_output=True, check=True, text=True)
-    return parse_json_response(response=res.stdout)
+    return parse_json_response(response=res)
```

### Comparing `rosa_python_client-1.0.7/PKG-INFO` & `rosa_python_client-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosa-python-client
-Version: 1.0.7
+Version: 1.0.8
 Summary: Wrapper for rosa cli
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

