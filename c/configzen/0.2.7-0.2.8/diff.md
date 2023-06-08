# Comparing `tmp/configzen-0.2.7.tar.gz` & `tmp/configzen-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.7.tar", max compression
+gzip compressed data, was "configzen-0.2.8.tar", max compression
```

## Comparing `configzen-0.2.7.tar` & `configzen-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.7/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.7/configzen/__main__.py
--rw-r--r--   0        0        0    67943 2023-06-08 00:25:44.808854 configzen-0.2.7/configzen/config.py
--rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.7/configzen/errors.py
--rw-r--r--   0        0        0    30568 2023-06-06 18:05:58.215336 configzen-0.2.7/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.7/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.7/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.7/LICENSE
--rw-r--r--   0        0        0     1154 2023-06-08 00:27:45.715601 configzen-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.7/README.md
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.8/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.8/configzen/__main__.py
+-rw-r--r--   0        0        0    67983 2023-06-08 01:29:52.633871 configzen-0.2.8/configzen/config.py
+-rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.8/configzen/errors.py
+-rw-r--r--   0        0        0    30518 2023-06-08 00:43:33.524516 configzen-0.2.8/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.8/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.8/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1154 2023-06-08 00:35:53.196628 configzen-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.8/README.md
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.8/PKG-INFO
```

### Comparing `configzen-0.2.7/configzen/__main__.py` & `configzen-0.2.8/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.7/configzen/config.py` & `configzen-0.2.8/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     # otherhost  # <- not anotherhost, because we reloaded only port
     # 5432
 """
 
 from __future__ import annotations
 
 import abc
+import asyncio
 import collections.abc
 import contextvars
 import copy
 import dataclasses
 import functools
 import io
 import os
@@ -1881,17 +1882,17 @@
         Export the configuration model.
 
         Returns
         -------
         The exported configuration model.
         """
         tok = _exporting.set(True)  # noqa: FBT003
-        ctx = contextvars.copy_context()
+        task = asyncio.create_task(self.dict_async(**kwargs))
         _exporting.reset(tok)
-        return await ctx.run(self.dict_async, **kwargs)
+        return await task
 
     async def dict_async(self, **kwargs: Any) -> dict[str, Any]:
         """
         Get the dictionary representation of the configuration model.
 
         Returns
         -------
@@ -2173,22 +2174,22 @@
             msg = "Writing to URLs is not yet supported"
             raise NotImplementedError(msg)
         return context.manager.write(blob, **kwargs)
 
     @classmethod
     async def load_async(
         cls: type[ConfigModelT],
-        resource: ConfigManager[ConfigModelT] | RawResourceT | None,
+        resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file asynchronously.
-        To reload the configuration, use the `reload()` method.
+        To reload the configuration, use the `reload_async()` method.
 
         Parameters
         ----------
         resource
             The configuration resource.
         create_if_missing
             Whether to create the configuration file if it does not exist.
@@ -2255,17 +2256,19 @@
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
             tok = _exporting.set(True)  # noqa: FBT003
-            ctx = contextvars.copy_context()
+            task = asyncio.create_task(
+                context.manager.dump_config_async(self, **kwargs)
+            )
             _exporting.reset(tok)
-            blob = await ctx.run(context.manager.dump_config_async, self, **kwargs)
+            blob = await task
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return await save_async(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
```

### Comparing `configzen-0.2.7/configzen/errors.py` & `configzen-0.2.8/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.7/configzen/processor.py` & `configzen-0.2.8/configzen/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -555,16 +555,14 @@
         return cls.directive_prefix + directive_name + fmt_arguments
 
 
 class Directives(str, enum.Enum):
     EXTEND = "extend"
     INCLUDE = "include"
     COPY = "copy"
-    PROCESSOR = "processor"
-    DEFINE = "define"
 
 
 class Processor(BaseProcessor[ConfigModelT]):
     directive_prefix = "^"
     extension_prefix = "+"
     route_separator: ClassVar[str] = ":"
```

### Comparing `configzen-0.2.7/configzen/typedefs.py` & `configzen-0.2.8/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.7/LICENSE` & `configzen-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.7/pyproject.toml` & `configzen-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.7"
+version = "0.2.8"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.7/README.md` & `configzen-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.7/PKG-INFO` & `configzen-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.7
+Version: 0.2.8
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

