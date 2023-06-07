# Comparing `tmp/wicked_expressions-0.7.0.tar.gz` & `tmp/wicked_expressions-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wicked_expressions-0.7.0.tar", max compression
+gzip compressed data, was "wicked_expressions-0.7.1.tar", max compression
```

## Comparing `wicked_expressions-0.7.0.tar` & `wicked_expressions-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-06-06 22:52:39.484761 wicked_expressions-0.7.0/LICENSE
--rw-r--r--   0        0        0     2119 2023-06-06 22:52:39.484761 wicked_expressions-0.7.0/README.md
--rw-r--r--   0        0        0     1219 2023-06-06 22:54:04.418242 wicked_expressions-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-06-06 22:54:04.398242 wicked_expressions-0.7.0/wicked_expressions/__init__.py
--rw-r--r--   0        0        0      714 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/api.bolt
--rw-r--r--   0        0        0     9403 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/comparison.bolt
--rw-r--r--   0        0        0      305 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/config.bolt
--rw-r--r--   0        0        0     1850 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/internal_api.bolt
--rw-r--r--   0        0        0      360 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/nbtlib.bolt
--rw-r--r--   0        0        0     8436 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/raw_operations.bolt
--rw-r--r--   0        0        0      375 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/rebindable.bolt
--rw-r--r--   0        0        0      596 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/safe_load.bolt
--rw-r--r--   0        0        0     3118 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/sources.bolt
--rw-r--r--   0        0        0     1181 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/utils.bolt
--rw-r--r--   0        0        0     1333 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/var.bolt
--rw-r--r--   0        0        0     6303 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/modules/var_sources.bolt
--rw-r--r--   0        0        0        0 2023-06-06 22:52:39.492761 wicked_expressions-0.7.0/wicked_expressions/py.typed
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-07 23:15:25.309006 wicked_expressions-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2119 2023-06-07 23:15:25.309006 wicked_expressions-0.7.1/README.md
+-rw-r--r--   0        0        0     1219 2023-06-07 23:16:58.194575 wicked_expressions-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-06-07 23:16:58.174575 wicked_expressions-0.7.1/wicked_expressions/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/api.bolt
+-rw-r--r--   0        0        0     9084 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/comparison.bolt
+-rw-r--r--   0        0        0      305 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/config.bolt
+-rw-r--r--   0        0        0     1850 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/internal_api.bolt
+-rw-r--r--   0        0        0      360 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/nbtlib.bolt
+-rw-r--r--   0        0        0     8436 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/raw_operations.bolt
+-rw-r--r--   0        0        0      375 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/rebindable.bolt
+-rw-r--r--   0        0        0      596 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/safe_load.bolt
+-rw-r--r--   0        0        0     3118 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/sources.bolt
+-rw-r--r--   0        0        0     1181 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/utils.bolt
+-rw-r--r--   0        0        0     1333 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/var.bolt
+-rw-r--r--   0        0        0     6303 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/modules/var_sources.bolt
+-rw-r--r--   0        0        0        0 2023-06-07 23:15:25.321006 wicked_expressions-0.7.1/wicked_expressions/py.typed
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 wicked_expressions-0.7.1/PKG-INFO
```

### Comparing `wicked_expressions-0.7.0/LICENSE` & `wicked_expressions-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/README.md` & `wicked_expressions-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/pyproject.toml` & `wicked_expressions-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wicked_expressions"
-version = "0.7.0"
+version = "0.7.1"
 description = "Extension of bolt-expressions written in Bolt."
 authors = ["Yeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/wicked-expressions"
 readme = "README.md"
```

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/api.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/comparison.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/comparison.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from ./config import Config
 
 
 runtime = ctx.inject(Runtime)
 
 
 class ExpressionComparison(Rebindable):
-    last_bool_check = None
     incr_index = 0
     _INVERTED_OPERATOR = {
         '==': '!=',
         '!=': '==',
         '<': '>=',
         '>': '<=',
         '<=': '>',
@@ -122,31 +121,23 @@
     def __not__(self):
         return self.__class__(self.arg_0, self._INVERTED_OPERATOR[self.operator], self.arg_1, initialized=self.initialized, check_exists=self.check_exists)
 
     @contextmanager
     def check_boolean(self, arg_0):
         temp = self.temp_scoreboard['$temp']
 
-        if self.last_bool_check != str(arg_0):       # hacky fix since initializing doesnt work here
-            temp = arg_0
+        temp = arg_0
 
         if self.operator == '==':
             if score temp.holder temp.obj matches 1:
                 yield True
         elif self.operator == '!=':
             if score temp.holder temp.obj matches 0:
                 yield True
 
-        # self.last_bool_check = str(arg_0)
-        self._set_last_bool_check(str(arg_0))
-
-    @classmethod
-    def _set_last_bool_check(cls, value):
-        cls.last_bool_check = value
-
     @contextmanager
     def compare_score_to_constant(self, arg_0, arg_1):
         arg_0_holder = parse_holder(arg_0.holder)
 
         if self.operator == '==':
             if score arg_0_holder arg_0.obj matches arg_1:
                 yield True
```

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/internal_api.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/internal_api.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/raw_operations.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/raw_operations.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/safe_load.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/safe_load.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/sources.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/utils.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/utils.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/var.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/var.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/wicked_expressions/modules/var_sources.bolt` & `wicked_expressions-0.7.1/wicked_expressions/modules/var_sources.bolt`

 * *Files identical despite different names*

### Comparing `wicked_expressions-0.7.0/PKG-INFO` & `wicked_expressions-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wicked-expressions
-Version: 0.7.0
+Version: 0.7.1
 Summary: Extension of bolt-expressions written in Bolt.
 Home-page: https://github.com/reapermc/wicked-expressions
 License: MIT
 Keywords: beet,bolt,minecraft,minecraft-commands,mcfunction
 Author: Yeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
```

