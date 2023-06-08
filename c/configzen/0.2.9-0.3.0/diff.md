# Comparing `tmp/configzen-0.2.9.tar.gz` & `tmp/configzen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.9.tar", max compression
+gzip compressed data, was "configzen-0.3.0.tar", max compression
```

## Comparing `configzen-0.2.9.tar` & `configzen-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      765 2023-06-08 07:24:52.012706 configzen-0.2.9/configzen/__init__.py
--rw-r--r--   0        0        0      902 2023-06-08 05:49:03.151216 configzen-0.2.9/configzen/__main__.py
--rw-r--r--   0        0        0    71474 2023-06-08 07:28:08.379387 configzen-0.2.9/configzen/config.py
--rw-r--r--   0        0        0     3495 2023-06-08 07:28:22.234288 configzen-0.2.9/configzen/errors.py
--rw-r--r--   0        0        0    25376 2023-06-08 07:24:53.384157 configzen-0.2.9/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.9/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.9/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.9/LICENSE
--rw-r--r--   0        0        0     1158 2023-06-08 07:32:00.459969 configzen-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.9/README.md
--rw-r--r--   0        0        0     8027 1970-01-01 00:00:00.000000 configzen-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      765 2023-06-08 07:24:52.012706 configzen-0.3.0/configzen/__init__.py
+-rw-r--r--   0        0        0      902 2023-06-08 05:49:03.151216 configzen-0.3.0/configzen/__main__.py
+-rw-r--r--   0        0        0    71657 2023-06-08 08:08:27.075017 configzen-0.3.0/configzen/config.py
+-rw-r--r--   0        0        0     3495 2023-06-08 07:28:22.234288 configzen-0.3.0/configzen/errors.py
+-rw-r--r--   0        0        0    25376 2023-06-08 07:24:53.384157 configzen-0.3.0/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.3.0/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.3.0/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1155 2023-06-08 08:09:32.832701 configzen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.3.0/README.md
+-rw-r--r--   0        0        0     8127 1970-01-01 00:00:00.000000 configzen-0.3.0/PKG-INFO
```

### Comparing `configzen-0.2.9/configzen/__init__.py` & `configzen-0.3.0/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/configzen/__main__.py` & `configzen-0.3.0/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/configzen/config.py` & `configzen-0.3.0/configzen/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,49 +304,43 @@
         return functools.partial(with_post_deserialize, func)
 
     post_deserialize.register(cls, func)
     return cls
 
 
 @functools.singledispatch
-def export(obj: Any, *, json: bool = False, **kwargs: Any) -> dict[str, Any]:
+def export(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
     obj
-    json
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return obj.export(**kwargs)
-    exporter = obj.json if json else obj.dict
-    return cast(dict[str, Any], exporter(**kwargs))
+    return cast(dict[str, Any], obj.dict(**kwargs))
 
 
 @functools.singledispatch
-async def export_async(
-    obj: Any, *, json: bool = False, **kwargs: Any
-) -> dict[str, Any]:
+async def export_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
     obj
-    json
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return await obj.export_async(**kwargs)
-    exporter = obj.json_async if json else obj.dict_async
-    return cast(dict[str, Any], await exporter(**kwargs))
+    return cast(dict[str, Any], await obj.dict_async(**kwargs))
 
 
 def with_exporter(
     func: collections.abc.Callable[[ConfigModelT], dict[str, Any]],
     cls: type[ConfigModelT] | None = None,
 ) -> type[ConfigModelT] | Any:
     """
@@ -847,15 +841,19 @@
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if ac_parser == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
-            ) | {"json": True}
+            )
+            tok = _exporting.set(True)  # noqa: FBT003
+            ctx = contextvars.copy_context()
+            _exporting.reset(tok)
+            return ctx.run(config.json, **export_kwargs)
         data = export(config, **export_kwargs)
         return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     async def dump_config_async(
         self,
         config: ConfigModelT,
         ac_parser: str | None = None,
@@ -879,15 +877,19 @@
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
         export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if ac_parser == "json" and self.use_pydantic_json:
             export_kwargs |= filter_options(
                 self.JSON_KWARGS, self.dump_options | kwargs
-            ) | {"json": True}
+            )
+            tok = _exporting.set(True)  # noqa: FBT003
+            task = asyncio.create_task(config.json_async(**export_kwargs))
+            _exporting.reset(tok)
+            return await task
         data = await export_async(config, **export_kwargs)
         return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
```

### Comparing `configzen-0.2.9/configzen/errors.py` & `configzen-0.3.0/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/configzen/processor.py` & `configzen-0.3.0/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/configzen/typedefs.py` & `configzen-0.3.0/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/LICENSE` & `configzen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/pyproject.toml` & `configzen-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.9"
+version = "0.3.0"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.7"
 anyconfig = "^0.13.0"
 typing-extensions = { version = "^4.5.0", python = ">=3.9,<3.11"}
-aiofiles = {version = "^23.1.0", extras = ["async"]}
-pyyaml = {version = "^6.0", extras = ["yaml"]}
-toml = {version = "^0.10.2", extras = ["toml"]}
+aiofiles = {version = "^23.1.0"}
+pyyaml = {version = "^6.0"}
+toml = {version = "^0.10.2"}
+
+[tool.poetry.extras]
+async = ["aiofiles"]
+yaml = ["pyyaml"]
+toml = ["toml"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.267"
 mypy = "^1.3.0"
 black = "^23.3.0"
-pre-commit = "^3.3.1"
 pytest = "^7.3.1"
 
 [tool.ruff]
 target-version = "py39"
 select = ["F","E","W","I","UP","N","S","C","B","A","T","Q","RUF","YTT","BLE","ANN","FBT","PL","TRY","RSE","SLF","DTZ","EXE","ISC","ICN","G","INP","PIE","RET","SIM","TID","TCH","ARG","PTH"]
 ignore = ["DTZ005","INP001","TCH003","ANN101","ANN102","ANN401","I001","TID252","T201","B905","S101","TRY003","PLR2004"]
 fix = true
```

### Comparing `configzen-0.2.9/README.md` & `configzen-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.9/PKG-INFO` & `configzen-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.9
+Version: 0.3.0
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles[async] (>=23.1.0,<24.0.0)
+Provides-Extra: async
+Provides-Extra: toml
+Provides-Extra: yaml
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0) ; extra == "async"
 Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pyyaml[yaml] (>=6.0,<7.0)
-Requires-Dist: toml[toml] (>=0.10.2,<0.11.0)
+Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "toml"
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # configzen
 _configzen_ – managing configuration files easily.
 Currently under development, not ready for production use.
```

