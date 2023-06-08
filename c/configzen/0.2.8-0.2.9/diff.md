# Comparing `tmp/configzen-0.2.8.tar.gz` & `tmp/configzen-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.8.tar", max compression
+gzip compressed data, was "configzen-0.2.9.tar", max compression
```

## Comparing `configzen-0.2.8.tar` & `configzen-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.8/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.8/configzen/__main__.py
--rw-r--r--   0        0        0    67983 2023-06-08 01:29:52.633871 configzen-0.2.8/configzen/config.py
--rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.8/configzen/errors.py
--rw-r--r--   0        0        0    30518 2023-06-08 00:43:33.524516 configzen-0.2.8/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.8/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.8/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.8/LICENSE
--rw-r--r--   0        0        0     1154 2023-06-08 00:35:53.196628 configzen-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.8/README.md
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      765 2023-06-08 07:24:52.012706 configzen-0.2.9/configzen/__init__.py
+-rw-r--r--   0        0        0      902 2023-06-08 05:49:03.151216 configzen-0.2.9/configzen/__main__.py
+-rw-r--r--   0        0        0    71474 2023-06-08 07:28:08.379387 configzen-0.2.9/configzen/config.py
+-rw-r--r--   0        0        0     3495 2023-06-08 07:28:22.234288 configzen-0.2.9/configzen/errors.py
+-rw-r--r--   0        0        0    25376 2023-06-08 07:24:53.384157 configzen-0.2.9/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.9/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.9/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1158 2023-06-08 07:32:00.459969 configzen-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.9/README.md
+-rw-r--r--   0        0        0     8027 1970-01-01 00:00:00.000000 configzen-0.2.9/PKG-INFO
```

### Comparing `configzen-0.2.8/configzen/__main__.py` & `configzen-0.2.9/configzen/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import argparse
-
-from configzen import ConfigMeta, ConfigModel
-from configzen.config import get_context
-
-
-class Store(ConfigModel):
-    class Config(ConfigMeta):
-        extra = ConfigMeta.Extra.allow
-
-
-if __name__ == "__main__":
-    p = argparse.ArgumentParser()
-    p.add_argument("--source", help="file to load from")
-    p.add_argument("dest", help="file to save into")
-    p.add_argument("--async", dest="use_async", action="store_true", help="use async")
-
-    opt = p.parse_args()
-
-    if opt.use_async:
-        import asyncio
-
-        store = asyncio.run(Store.load_async(opt.source))
-        print(store)
-        context = get_context(store)
-        context.manager.resource = opt.dest
-        asyncio.run(store.save_async())
-    else:
-        store = Store.load(opt.source)
-        print(store)
-        context = get_context(store)
-        context.manager.resource = opt.dest
-        store.save()
+import argparse
+
+from configzen import ConfigMeta, ConfigModel
+from configzen.config import get_context
+
+
+class Store(ConfigModel):
+    class Config(ConfigMeta):
+        extra = ConfigMeta.Extra.allow
+
+
+if __name__ == "__main__":
+    p = argparse.ArgumentParser()
+    p.add_argument("--source", help="file to load from")
+    p.add_argument("dest", help="file to save into")
+    p.add_argument("--async", dest="use_async", action="store_true", help="use async")
+
+    opt = p.parse_args()
+
+    if opt.use_async:
+        import asyncio
+
+        store = asyncio.run(Store.load_async(opt.source))
+        print(store)
+        context = get_context(store)
+        context.agent.resource = opt.dest
+        asyncio.run(store.save_async())
+    else:
+        store = Store.load(opt.source)
+        print(store)
+        context = get_context(store)
+        context.agent.resource = opt.dest
+        store.save()
```

### Comparing `configzen-0.2.8/configzen/config.py` & `configzen-0.2.9/configzen/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,18 +89,19 @@
 )
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import BaseModel, ModelMetaclass
 from pydantic.utils import ROOT_KEY
 
 from configzen.errors import (
     ConfigAccessError,
-    InternalConfigError,
+    InternalSyntaxError,
     ResourceLookupError,
     UnspecifiedParserError,
-    pretty_syntax_error,
+    UnavailableParserError,
+    formatted_syntax_error,
 )
 from configzen.processor import EXPORT, DirectiveContext, Processor
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
     IncludeExcludeT,
@@ -115,15 +116,15 @@
 
     AIOFILES_AVAILABLE = True
 except ImportError:
     aiofiles = None  # type: ignore[assignment]
     AIOFILES_AVAILABLE = False
 
 __all__ = (
-    "ConfigManager",
+    "ConfigAgent",
     "ConfigModel",
     "ConfigMeta",
     "save",
     "save_async",
     "reload",
     "reload_async",
     "pre_serialize",
@@ -161,15 +162,15 @@
         if not field.field_info.exclude and not field.required:
             if isinstance(default, pydantic.BaseModel):
                 default = default.dict()
             defaults[field.alias] = default
     return defaults
 
 
-def _vars(obj: Any) -> dict[str, Any]:
+def _vars_or_dict(obj: Any) -> dict[str, Any]:
     obj_dict = obj
     if not isinstance(obj, dict):
         obj_dict = obj.__dict__
     return cast(dict[str, Any], obj_dict)
 
 
 def _is_namedtuple(
@@ -303,43 +304,49 @@
         return functools.partial(with_post_deserialize, func)
 
     post_deserialize.register(cls, func)
     return cls
 
 
 @functools.singledispatch
-def export(obj: Any, **kwargs: Any) -> dict[str, Any]:
+def export(obj: Any, *, json: bool = False, **kwargs: Any) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
     obj
+    json
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return obj.export(**kwargs)
-    return cast(dict[str, Any], obj.dict(**kwargs))
+    exporter = obj.json if json else obj.dict
+    return cast(dict[str, Any], exporter(**kwargs))
 
 
 @functools.singledispatch
-async def export_async(obj: Any, **kwargs: Any) -> dict[str, Any]:
+async def export_async(
+    obj: Any, *, json: bool = False, **kwargs: Any
+) -> dict[str, Any]:
     """
     Export a ConfigModel to a safely-serializable format.
     Register a custom exporter for a type using the `with_exporter` decorator,
     which can help to exclude particular values from the export if needed.
 
     Parameters
     ----------
     obj
+    json
     """
     if isinstance(obj, ConfigModel) and not _exporting.get():
         return await obj.export_async(**kwargs)
-    return cast(dict[str, Any], await obj.dict_async(**kwargs))
+    exporter = obj.json_async if json else obj.dict_async
+    return cast(dict[str, Any], await exporter(**kwargs))
 
 
 def with_exporter(
     func: collections.abc.Callable[[ConfigModelT], dict[str, Any]],
     cls: type[ConfigModelT] | None = None,
 ) -> type[ConfigModelT] | Any:
     """
@@ -453,26 +460,26 @@
             targets = [load_options]
         else:
             actual_key = key
             targets = [load_options, dump_options]
         for target in targets:
             if actual_key in target:
                 msg = (
-                    f"option {key}={value!r} overlaps with "
+                    f"Option {key}={value!r} overlaps with "
                     f"defined {actual_key}={target[actual_key]!r}"
                 )
                 raise ValueError(msg)
             target[actual_key] = value
 
 
-class ConfigManager(Generic[ConfigModelT]):
+class ConfigAgent(Generic[ConfigModelT]):
     """
-    A configuration resource loader and saver.
+    Configuration resource agent: loader and saver.
 
-    This class is used to represent a configuration resource, which
+    This class is used to broke between the model and the home resource, which
     can be a file, a URL, or a file-like object. It is used internally
     by `ConfigModel` and `AsyncConfigModel` to load and save
     configuration files.
 
     Parameters
     ----------
     resource
@@ -552,14 +559,22 @@
         "allow_nan",
         "cls",
         "indent",
         "separators",
         "default",
         "sort_keys",
     }
+    EXPORT_KWARGS: ClassVar[set[str]] = {
+        "by_alias",
+        "include",
+        "exclude",
+        "exclude_unset",
+        "exclude_defaults",
+        "exclude_none",
+    }
 
     def __init__(
         self,
         resource: RawResourceT,
         ac_parser: str | None = None,
         processor_class: type[Processor[ConfigModelT]] | None = None,
         *,
@@ -639,22 +654,27 @@
             from the file extension.
 
         Returns
         -------
         The resource of the configuration.
         """
         self._resource = value
-        self.ac_parser = self.ac_parser or self._guess_ac_parser()
+        if self.ac_parser is None:
+            self.ac_parser = self._guess_ac_parser()
 
     def _guess_ac_parser(self) -> str | None:
         ac_parser = None
         if isinstance(self.resource, pathlib.Path):
             ac_parser = self.resource.suffix[1:].casefold()
             if not ac_parser:
-                msg = f"Could not guess the engine to use for {self.resource!r}."
+                msg = (
+                    "Could not guess the anyconfig parser to use for "
+                    f"{self.resource!r}.\n"
+                    f"Available parsers: {', '.join(anyconfig.list_types())}"
+                )
                 raise UnspecifiedParserError(msg)
         return ac_parser
 
     def load_into(
         self,
         config_class: type[ConfigModelT],
         blob: str,
@@ -706,34 +726,37 @@
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration.
         """
         dict_config = await self.load_into_dict_async(
-            blob,
-            ac_parser=ac_parser,
-            **kwargs
+            blob, ac_parser=ac_parser, **kwargs
         )
         if dict_config is None:
             dict_config = {}
         return config_class.parse_obj(dict_config)
 
     def _load_into_dict_impl(
         self,
         blob: str,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> dict[str, Any]:
+        ac_parser = ac_parser or self.ac_parser or self._guess_ac_parser()
         if ac_parser is None:
-            ac_parser = self.ac_parser
+            msg = "Cannot read configuration because `ac_parser` was not specified"
+            raise UnspecifiedParserError(msg)
         kwargs = self.load_options | kwargs
-        loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
-            blob, ac_parser=ac_parser, **kwargs
-        )
+        try:
+            loaded = anyconfig.loads(  # type: ignore[no-untyped-call]
+                blob, ac_parser=ac_parser, **kwargs
+            )
+        except anyconfig.UnknownParserTypeError as exc:
+            raise UnavailableParserError(str(exc).split()[-1], self) from exc
         if not isinstance(loaded, collections.abc.Mapping):
             msg = (
                 f"Expected a mapping as a result of loading {self.resource}, "
                 f"got {type(loaded).__name__}."
             )
             raise TypeError(msg)
         return dict(loaded)
@@ -761,15 +784,15 @@
         **kwargs
             Additional keyword arguments to pass to `anyconfig.loads()`.
 
         Returns
         -------
         The loaded configuration dictionary.
         """
-        loaded = self._load_into_dict_impl(blob, ac_parser, **kwargs)
+        loaded = self._load_into_dict_impl(blob, ac_parser=ac_parser, **kwargs)
         if preprocess:
             loaded = self.processor_class(self, loaded).preprocess()
         return loaded
 
     async def load_into_dict_async(
         self,
         blob: str,
@@ -820,18 +843,21 @@
 
         Returns
         -------
         The dumped configuration.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
+        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if ac_parser == "json" and self.use_pydantic_json:
-            kwargs = filter_options(self.JSON_KWARGS, self.dump_options | kwargs)
-            return config.json(**kwargs)
-        return self.dump_data(export(config), ac_parser=ac_parser, **kwargs)
+            export_kwargs |= filter_options(
+                self.JSON_KWARGS, self.dump_options | kwargs
+            ) | {"json": True}
+        data = export(config, **export_kwargs)
+        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     async def dump_config_async(
         self,
         config: ConfigModelT,
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
@@ -849,18 +875,21 @@
 
         Returns
         -------
         The dumped configuration.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
+        export_kwargs = filter_options(self.EXPORT_KWARGS, kwargs)
         if ac_parser == "json" and self.use_pydantic_json:
-            kwargs = filter_options(self.JSON_KWARGS, self.dump_options | kwargs)
-            return await config.json_async(**kwargs)
-        return self.dump_data(await export_async(config), ac_parser=ac_parser, **kwargs)
+            export_kwargs |= filter_options(
+                self.JSON_KWARGS, self.dump_options | kwargs
+            ) | {"json": True}
+        data = await export_async(config, **export_kwargs)
+        return self.dump_data(data, ac_parser=ac_parser, **kwargs)
 
     def dump_data(
         self,
         data: dict[str, Any],
         ac_parser: str | None = None,
         **kwargs: Any,
     ) -> str:
@@ -878,16 +907,24 @@
 
         Returns
         -------
         The dumped configuration.
         """
         if ac_parser is None:
             ac_parser = self.ac_parser
+        if ac_parser is None:
+            msg = (
+                "Cannot write configuration because `ac_parser` was not specified"
+                f"for agent {self}"
+            )
+            raise UnspecifiedParserError(msg)
         kwargs = self.dump_options | kwargs
-        return anyconfig.dumps(pre_serialize(data), ac_parser=ac_parser, **kwargs)
+        return anyconfig.dumps(
+            pre_serialize(data), ac_parser=ac_parser.casefold(), **kwargs
+        )
 
     @property
     def is_url(self) -> bool:
         """Whether the resource is a URL."""
         return isinstance(self.resource, str)
 
     def open_resource(self, **kwds: Any) -> ConfigIO:
@@ -942,19 +979,19 @@
             Keyword arguments to pass to the opening routine.
 
         Returns
         -------
         The opened resource.
         """
         if self.is_url:
-            msg = "asynchronous URL opening is not supported"
+            msg = "Asynchronous URL opening is not supported"
             raise NotImplementedError(msg)
         if not AIOFILES_AVAILABLE:
             msg = (
-                "aiofiles is not available, cannot open file "
+                "Aiofiles is not available, cannot open file "
                 "asynchronously (install with `pip install aiofiles`)"
             )
             raise RuntimeError(msg)
         if isinstance(self.resource, (int, pathlib.Path)):
             kwds = filter_options(self.OPEN_KWARGS, kwds)
             return aiofiles.open(self.resource, **kwds)
         raise RuntimeError("cannot open resource asynchronously")
@@ -1007,15 +1044,15 @@
         new_kwargs = cast(dict[str, Any], kwargs).copy()
         if not self.is_url:
             if method == "read":
                 new_kwargs.setdefault("mode", "r")
             elif method == "write":
                 new_kwargs.setdefault("mode", "w")
             else:
-                msg = f"invalid resource access method: {method!r}"
+                msg = f"Invalid resource access method: {method!r}"
                 raise ValueError(msg)
         return new_kwargs
 
     def read(
         self,
         *,
         config_class: type[ConfigModelT],
@@ -1133,28 +1170,28 @@
     @classmethod
     def from_directive_context(
         cls,
         ctx: DirectiveContext,
         /,
         route_separator: str = ":",
         route_class: type[Route] | None = None,
-    ) -> tuple[ConfigManager[ConfigModelT], SupportsRoute | None]:
+    ) -> tuple[ConfigAgent[ConfigModelT], SupportsRoute | None]:
         """
-        Create a configuration manager from a preprocessor directive context.
+        Create a configuration agent from a preprocessor directive context.
         Return an optional scope that the context points to.
 
         Parameters
         ----------
         route_class
         route_separator
         ctx
 
         Returns
         -------
-        The configuration manager.
+        The configuration agent.
         """
         if route_class is None:
             route_class = Route
         route: SupportsRoute | None = None
         args: list[Any] = []
         kwargs: dict[str, Any] = {}
         if isinstance(ctx.snippet, str):
@@ -1165,95 +1202,125 @@
             args.append(ctx.snippet)
         elif is_dict_like(ctx.snippet):
             kwargs |= ctx.snippet
         elif is_list_like(ctx.snippet):
             args += list(ctx.snippet)
         else:
             msg = (
-                f"invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
+                f"Invalid snippet for the {ctx.directive!r} directive: {ctx.snippet!r}"
             )
             raise ValueError(msg)
         return cls(*args, **kwargs), str(route)
 
     def __repr__(self) -> str:
         resource = self.resource
         return f"{type(self).__name__}({resource=!r})"
 
 
 class Route:
     TOK_DOT: ClassVar[str] = "."
-    TOK_DOTLIST_ESCAPE_ENTER: ClassVar[str] = "["
-    TOK_DOTLIST_ESCAPE_EXIT: ClassVar[str] = "]"
+    TOK_ESCAPE: ClassVar[str] = "\\"
+    TOK_DOTLISTESC_ENTER: ClassVar[str] = "["
+    TOK_DOTLISTESC_EXIT: ClassVar[str] = "]"
 
     def __init__(self, route: SupportsRoute) -> None:
         self.list_route = self.parse(route)
 
     @classmethod
     def parse(cls, route: SupportsRoute) -> list[str]:
         if isinstance(route, Route):
             return route.list_route
         if isinstance(route, list):
             return route
         if isinstance(route, str):
-            with pretty_syntax_error(route):
+            with formatted_syntax_error(route):
                 return cls._decompose(route)
         raise TypeError(f"invalid route type {type(route)!r}")
 
     @classmethod
-    def _decompose(cls, route: str) -> list[str]:
-        route = route.removesuffix(cls.TOK_DOT) + cls.TOK_DOT
-        argument = ""
-        escape_ctx = False
-        prev_char: str | None = None
-        list_route = []
-        for char_no, char in enumerate(route, start=1):
-            if char in cls.TOK_DOT:
-                if escape_ctx:
-                    argument += char
+    def _decompose(cls, route: str) -> list[str]:  # noqa: C901, PLR0912
+        tok_dot = cls.TOK_DOT
+        tok_escape = cls.TOK_ESCAPE
+        tok_dle_enter = cls.TOK_DOTLISTESC_ENTER
+        tok_dle_exit = cls.TOK_DOTLISTESC_EXIT
+
+        route = route.removesuffix(tok_dot) + tok_dot
+
+        part = ""
+        dle_ctx = None
+        list_route: list[str] = []
+        enter = list_route.append
+        error = functools.partial(InternalSyntaxError, prefix="Route(", suffix=")")
+        escape = False
+
+        for index, char in enumerate(route):
+            if escape:
+                part += char
+                escape = False
+                continue
+            is_last = index == len(route) - 1
+            if char == tok_dot:
+                if dle_ctx is not None:
+                    part += char
                 else:
-                    list_route.append(argument)
-                    argument = ""
-            elif char in cls.TOK_DOTLIST_ESCAPE_ENTER:
-                if prev_char and prev_char in cls.TOK_DOTLIST_ESCAPE_EXIT:
-                    raise InternalConfigError(
-                        "invalid escape sequence "
-                        f"(expected {cls.TOK_DOT} between escape sequences)",
-                        extra=char_no,
-                    )
-                if escape_ctx:
-                    msg = "invalid escape sequence"
-                    raise InternalConfigError(msg, extra=char_no)
-                escape_ctx = True
-            elif char in cls.TOK_DOTLIST_ESCAPE_EXIT:
-                if not escape_ctx:
-                    msg = "invalid escape sequence"
-                    raise InternalConfigError(msg, extra=char_no)
-                escape_ctx = False
-                list_route.append(argument)
-                argument = ""
+                    enter(part)
+                    part = ""
+            elif char == tok_escape:
+                if is_last:
+                    part += char
+                else:
+                    escape = True
+            elif char == tok_dle_enter:
+                if dle_ctx is not None:
+                    # a special character at its place
+                    part += char
+                else:
+                    dle_ctx = index
+            elif char == tok_dle_exit:
+                if is_last or route[index + 1] == tok_dot:
+                    if dle_ctx is None:
+                        msg = (
+                            "Dotlist escape sequence "
+                            f"was not opened with {tok_dle_enter!r}"
+                        )
+                        raise error(msg, index=index)
+                    dle_ctx = None
+                else:
+                    # a special character at its place
+                    part += char
             else:
-                argument += char
-            prev_char = char
+                part += char
+            if is_last and dle_ctx is not None:
+                msg = (
+                    "Unclosed dotlist escape sequence "
+                    f"(expected {tok_dle_exit!r} token)"
+                )
+                raise error(msg, index=dle_ctx)
         return list_route
 
     @classmethod
     def decompose(cls, route: str) -> list[str]:
-        with pretty_syntax_error(route):
+        with formatted_syntax_error(route):
             return cls._decompose(route)
 
     def compose(self) -> str:
-        escape = (self.TOK_DOTLIST_ESCAPE_ENTER, self.TOK_DOTLIST_ESCAPE_EXIT)
+        escape = (self.TOK_DOTLISTESC_ENTER, self.TOK_DOTLISTESC_EXIT)
         raw = ("", "")
         return self.TOK_DOT.join(
-            fragment.join(escape) if self.TOK_DOT in fragment else fragment.join(raw)
+            fragment.join(escape).replace(
+                self.TOK_DOTLISTESC_EXIT + self.TOK_DOT,
+                self.TOK_DOTLISTESC_EXIT + self.TOK_ESCAPE + self.TOK_DOT,
+            )
+            if self.TOK_DOT in fragment
+            else fragment.join(raw)
             for fragment in self.list_route
         )
 
-    def enter(self, *args: str) -> Route:
-        return type(self)(self.list_route + list(args))
+    def enter(self, subroute: SupportsRoute) -> Route:
+        return type(self)(self.list_route + self.parse(subroute))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Route):
             return self.list_route == other.list_route
         if isinstance(other, str):
             return self.list_route == self.decompose(other)
         if isinstance(other, list):
@@ -1262,46 +1329,49 @@
 
     def __str__(self) -> str:
         return self.compose()
 
     def __iter__(self) -> collections.abc.Iterator[str]:
         yield from self.list_route
 
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.list_route})"
+
 
 def at(
     mapping: Any,
     route: SupportsRoute,
-    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _vars,
-    manager: ConfigManager[ConfigModelT] | None = None,
+    converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _vars_or_dict,
+    agent: ConfigAgent[ConfigModelT] | None = None,
 ) -> Any:
     """
     Get an item at a route.
 
     Parameters
     ----------
     mapping
         The mapping to use.
     route
         The route to the item.
     converter_func
-    manager
+    agent
 
     Returns
     -------
     The item at the route.
     """
     route = Route(route)
     route_here = []
-    scope = _vars(mapping)
+    scope = _vars_or_dict(mapping)
     try:
         for part in route:
             route_here.append(part)
             scope = converter_func(scope)[part]
     except KeyError:
-        raise ResourceLookupError(manager, route_here) from None
+        raise ResourceLookupError(agent, route_here) from None
     return scope
 
 
 @dataclasses.dataclass(frozen=True)
 class ConfigAt(Generic[ConfigModelT]):
     """
     A configuration item at a specific location.
@@ -1347,21 +1417,21 @@
         Returns
         -------
         The updated mapping.
         """
         route = list(Route(self.route))
         mapping = self.mapping or self.owner
         key = route.pop()
-        submapping = _vars(mapping)
+        scope = _vars_or_dict(mapping)
         route_here = []
         try:
             for part in route:
                 route_here.append(part)
-                submapping = _vars(submapping[part])
-            submapping[key] = value
+                scope = _vars_or_dict(scope[part])
+            scope[key] = value
         except KeyError:
             raise ConfigAccessError(self.owner, route_here) from None
         return mapping
 
     async def save_async(self, **kwargs: Any) -> int:
         """
         Save the configuration asynchronously.
@@ -1452,15 +1522,15 @@
         write_kwargs = {}
 
     config = section.owner
     data = config.initial_state
     scope = ConfigAt(config, data, section.route)
     data = scope.update(section.get())
     context = get_context(config)
-    blob = context.manager.dump_config(config.copy(update=data), **kwargs)
+    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
     result = config.write(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
 async def save_async(
     section: ConfigModelT | ConfigAt[ConfigModelT],
@@ -1491,15 +1561,15 @@
         write_kwargs = {}
 
     config = section.owner
     data = config.initial_state
     scope = ConfigAt(config, data, section.route)
     data = scope.update(section.get())
     context = get_context(config)
-    blob = context.manager.dump_config(config.copy(update=data), **kwargs)
+    blob = context.agent.dump_config(config.copy(update=data), **kwargs)
     result = await config.write_async(blob, **write_kwargs)
     context.initial_state = data
     return result
 
 
 def reload(section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any) -> Any:
     """
@@ -1519,15 +1589,15 @@
     if isinstance(section, ConfigModel):
         config = section
         return config.reload()
 
     config = section.owner
     context = get_context(config)
     state = config.__dict__
-    newest = context.manager.read(config_class=type(config), **kwargs)
+    newest = context.agent.read(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     ConfigAt(config, state, section.route).update(section_data)
     return section_data
 
 
 async def reload_async(
     section: ConfigModelT | ConfigAt[ConfigModelT], **kwargs: Any
@@ -1549,15 +1619,15 @@
     if isinstance(section, ConfigModel):
         config = section
         return await config.reload_async()
 
     config = section.owner
     context = get_context(config)
     state = config.__dict__
-    newest = await context.manager.read_async(config_class=type(config), **kwargs)
+    newest = await context.agent.read_async(config_class=type(config), **kwargs)
     section_data = ConfigAt(newest, newest.__dict__, section.route).get()
     ConfigAt(config, state, section.route).update(section_data)
     return section_data
 
 
 class BaseContext(abc.ABC, Generic[ConfigModelT]):
     """
@@ -1611,16 +1681,16 @@
         """
         if part is None:
             return self
         return Subcontext(self, part)
 
     @property
     @abc.abstractmethod
-    def manager(self) -> ConfigManager[ConfigModelT]:
-        """The configuration resource manager."""
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        """The configuration agent responsible for loading and saving."""
 
     @property
     @abc.abstractmethod
     def owner(self) -> ConfigModelT | None:
         """
         The top-level configuration model instance,
         holding all adjacent contexts.
@@ -1637,40 +1707,40 @@
 
 class Context(BaseContext[ConfigModelT], Generic[ConfigModelT]):
     """
     The context of a configuration model.
 
     Parameters
     ----------
-    manager
-        The configuration resource.
+    agent
+        The configuration resource agent.
     owner
         The top-level configuration model instance,
         holding all belonging subcontexts.
     """
 
     _initial_state: dict[str, Any]
 
     def __init__(
         self,
-        manager: ConfigManager[ConfigModelT],
+        agent: ConfigAgent[ConfigModelT],
         owner: ConfigModelT | None = None,
     ) -> None:
-        self._manager = manager
+        self._agent = agent
         self._owner = None
         self._initial_state = {}
 
         self.owner = owner
 
     def trace_route(self) -> collections.abc.Iterator[str]:
         yield from ()
 
     @property
-    def manager(self) -> ConfigManager[ConfigModelT]:
-        return self._manager
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        return self._agent
 
     @property
     def at(self) -> ConfigModelT | None:
         return self.owner
 
     @property
     def owner(self) -> ConfigModelT | None:
@@ -1687,19 +1757,19 @@
         return copy.deepcopy(self._initial_state)
 
     @initial_state.setter
     def initial_state(self, initial_state: dict[str, Any]) -> None:
         self._initial_state = copy.deepcopy(initial_state)
 
     def __repr__(self) -> str:
-        manager = self.manager
+        agent = self.agent
         return (
             f"<{type(self).__name__} "
             f"of {type(self.owner).__name__!r} configuration "
-            f"({manager=})>"
+            f"({agent=})>"
         )
 
 
 class Subcontext(BaseContext[ConfigModelT], Generic[ConfigModelT]):
     """
     The subcontext of a configuration model.
 
@@ -1712,16 +1782,16 @@
     """
 
     def __init__(self, parent: BaseContext[ConfigModelT], part: str) -> None:
         self._parent = parent
         self._part = part
 
     @property
-    def manager(self) -> ConfigManager[ConfigModelT]:
-        return self._parent.manager
+    def agent(self) -> ConfigAgent[ConfigModelT]:
+        return self._parent.agent
 
     def trace_route(self) -> collections.abc.Iterator[str]:
         yield from self._parent.trace_route()
         yield self._part
 
     @property
     def at(self) -> ConfigAt[ConfigModelT]:
@@ -1741,20 +1811,20 @@
     @initial_state.setter
     def initial_state(self, value: dict[str, Any]) -> None:
         data = self._parent.initial_state
         data[self._part] = copy.deepcopy(value)
         self._parent.initial_state = data
 
     def __repr__(self) -> str:
-        manager = self.manager
+        agent = self.agent
         route = self.route
         return (
             f"<{type(self).__name__} "
             f"of {type(self.owner).__name__ + '.' + str(route)!r} configuration "
-            f"({manager=})>"
+            f"({agent=})>"
         )
 
 
 def get_context(config: ConfigModelT) -> BaseContext[ConfigModelT]:
     """
     Get the context of the configuration model.
 
@@ -1937,30 +2007,30 @@
         if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
                 state[key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
-                context.manager.processor_class.export(state, metadata=metadata)
+                context.agent.processor_class.export(state, metadata=metadata)
             yield from state.items()
         else:
             yield from super()._iter(**kwargs)
 
     async def _iter_async(
         self, **kwargs: Any
     ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
                 state[key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
-                await context.manager.processor_class.export_async(
+                await context.agent.processor_class.export_async(
                     state, metadata=metadata
                 )
             return ((key, value) for key, value in state.items())
         return super()._iter(**kwargs)
 
     @classmethod
     @no_type_check
@@ -1973,32 +2043,40 @@
                 value_dict = export(value, **kwds)
                 if ROOT_KEY in value_dict:
                     return value_dict[ROOT_KEY]
                 return value_dict
         return super()._get_value(value, to_dict=to_dict, **kwds)
 
     @classmethod
-    def _resolve_manager(
+    def _resolve_agent(
         cls,
-        resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
-    ) -> ConfigManager[ConfigModelT]:
+        ac_parser: str | None = None,
+    ) -> ConfigAgent[ConfigModelT]:
         if resource is None:
             resource = getattr(cls.__config__, "resource", None)
         if resource is None:
             raise ValueError("No resource specified")
-        manager: ConfigManager[ConfigModelT]
-        if isinstance(resource, ConfigManager):
-            manager = resource
+        if ac_parser is None:
+            ac_parser = getattr(cls.__config__, "ac_parser", None)
+        agent: ConfigAgent[ConfigModelT]
+        if isinstance(resource, ConfigAgent):
+            agent = resource
         else:
-            manager = ConfigManager(resource)
+            agent = ConfigAgent(
+                resource,
+                ac_parser=ac_parser,
+            )
         if create_if_missing is not None:
-            manager.create_if_missing = create_if_missing
-        return manager
+            agent.create_if_missing = create_if_missing
+        if ac_parser is not None:
+            agent.ac_parser = cast(str, ac_parser)
+        return agent
 
     @property
     def initial_state(self) -> dict[str, Any]:
         """
         The initial configuration state.
 
         It is a copy of the configuration state
@@ -2061,42 +2139,54 @@
         state.pop(LOCAL, None)
         state.pop(TOKEN, None)
         return type(self)(**copy.deepcopy(state))
 
     @classmethod
     def load(
         cls: type[ConfigModelT],
-        resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
         create_if_missing: bool | None = None,
+        ac_parser: str | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file.
         To reload the configuration, use the `reload()` method.
 
         Parameters
         ----------
         resource
             The configuration resource to read from/write to.
+        ac_parser
+            The anyconfig parser to use.
         create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
-        cls.update_forward_refs()
-        manager = cls._resolve_manager(resource, create_if_missing=create_if_missing)
-        context = Context(manager)  # type: Context[ConfigModelT]
+        agent = cls._resolve_agent(
+            resource,
+            ac_parser=ac_parser,
+            create_if_missing=create_if_missing,
+        )
+        context = Context(agent)  # type: Context[ConfigModelT]
         current_context.set(context)
         local = contextvars.copy_context()
-        config = manager.read(config_class=cls, **kwargs)
+        if getattr(
+            cls.__config__,
+            "autoupdate_forward_refs",
+            ConfigMeta.autoupdate_forward_refs,
+        ):
+            cls.update_forward_refs()
+        config = agent.read(config_class=cls, **kwargs)
         setattr(config, LOCAL, local)
         context.owner = config
         context.initial_state = config.__dict__
         return config
 
     def reload(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
@@ -2110,15 +2200,15 @@
         Returns
         -------
         self
         """
         context = get_context(self)
         tok = current_context.set(get_context(context.owner))
         if context.owner is self:
-            changed = context.manager.read(config_class=type(self), **kwargs)
+            changed = context.agent.read(config_class=type(self), **kwargs)
         else:
             changed = reload(cast(ConfigAt[ConfigModelT], context.at), **kwargs)
         current_context.reset(tok)
         state = changed.__dict__
         context.initial_state = state
         self.update(**state)
         return self
@@ -2140,15 +2230,15 @@
         -------
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
-            blob = context.manager.dump_config(self, **kwargs)
+            blob = context.agent.dump_config(self, **kwargs)
             result = self.write(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return save(
             cast(ConfigAt[ConfigModelT], context.at),
             write_kwargs=write_kwargs,
             **kwargs,
@@ -2166,49 +2256,60 @@
             Keyword arguments to pass to the open method.
 
         Returns
         -------
         The number of bytes written.
         """
         context = get_context(self)
-        if context.manager.is_url:
+        if context.agent.is_url:
             msg = "Writing to URLs is not yet supported"
             raise NotImplementedError(msg)
-        return context.manager.write(blob, **kwargs)
+        return context.agent.write(blob, **kwargs)
 
     @classmethod
     async def load_async(
         cls: type[ConfigModelT],
-        resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
+        resource: ConfigAgent[ConfigModelT] | RawResourceT | None = None,
         *,
+        ac_parser: str | None = None,
         create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file asynchronously.
         To reload the configuration, use the `reload_async()` method.
 
         Parameters
         ----------
         resource
             The configuration resource.
+        ac_parser
+            The anyconfig parser to use.
         create_if_missing
             Whether to create the configuration file if it does not exist.
         **kwargs
             Keyword arguments to pass to the read method.
 
         Returns
         -------
         self
         """
-        manager = cls._resolve_manager(resource, create_if_missing=create_if_missing)
-        context = Context(manager)  # type: Context[ConfigModelT]
+        agent = cls._resolve_agent(
+            resource, create_if_missing=create_if_missing, ac_parser=ac_parser
+        )
+        context = Context(agent)  # type: Context[ConfigModelT]
         current_context.set(context)
         local = contextvars.copy_context()
-        config = await manager.read_async(config_class=cls, **kwargs)
+        if getattr(
+            cls.__config__,
+            "autoupdate_forward_refs",
+            ConfigMeta.autoupdate_forward_refs,
+        ):
+            cls.update_forward_refs()
+        config = await agent.read_async(config_class=cls, **kwargs)
         setattr(config, LOCAL, local)
         context.owner = config
         return config
 
     async def reload_async(self: ConfigModelT, **kwargs: Any) -> ConfigModelT:
         """
         Reload the configuration file asynchronously.
@@ -2221,17 +2322,15 @@
         Returns
         -------
         self
         """
         context = get_context(self)
         tok = current_context.set(get_context(context.owner))
         if context.owner is self:
-            changed = await context.manager.read_async(
-                config_class=type(self), **kwargs
-            )
+            changed = await context.agent.read_async(config_class=type(self), **kwargs)
         else:
             changed = await reload_async(
                 cast(ConfigAt[ConfigModelT], context.at), **kwargs
             )
         current_context.reset(tok)
         state = changed.__dict__
         context.initial_state = state
@@ -2256,17 +2355,15 @@
         The number of bytes written.
         """
         context = get_context(self)
         if context.owner is self:
             if write_kwargs is None:
                 write_kwargs = {}
             tok = _exporting.set(True)  # noqa: FBT003
-            task = asyncio.create_task(
-                context.manager.dump_config_async(self, **kwargs)
-            )
+            task = asyncio.create_task(context.agent.dump_config_async(self, **kwargs))
             _exporting.reset(tok)
             blob = await task
             result = await self.write_async(blob, **write_kwargs)
             context.initial_state = self.__dict__
             return result
         return await save_async(
             cast(ConfigAt[ConfigModelT], context.at),
@@ -2286,26 +2383,26 @@
             Keyword arguments to pass to the open method.
 
         Returns
         -------
         The number of bytes written.
         """
         context = get_context(self)
-        if context.manager.is_url:
+        if context.agent.is_url:
             msg = "Saving to URLs is not yet supported"
             raise NotImplementedError(msg)
-        return await context.manager.write_async(blob, **kwargs)
+        return await context.agent.write_async(blob, **kwargs)
 
     @classmethod
     def __field_setup__(cls, value: Any, field: ModelField) -> Any:
         context = current_context.get()
         if context is not None:
             subcontext = context.enter(field.name)
             tok = current_context.set(subcontext)
-            vs = _vars(value)
+            vs = _vars_or_dict(value)
             vs[TOKEN] = tok
             vs[LOCAL] = contextvars.copy_context()
         return value
 
 
 class ConfigMeta(pydantic.BaseSettings.Config):
     """
@@ -2314,14 +2411,24 @@
     Attributes
     ----------
     resource
         The configuration resource to read from/write to.
 
         If a string, it will be interpreted as a path to a file.
 
+    ac_parser
+        The anyconfig parser to use.
+
+    autoupdate_forward_refs
+        Whether to automatically update forward references
+        when `ConfigModel.load()` or `ConfigModel.load_async()`
+        methods are called. For convenience, defaults to `True`.
+
     And all other attributes from `pydantic.BaseSettings.Config`.
     """
 
-    resource: ConfigManager[ConfigModel] | RawResourceT | None = None
+    resource: ConfigAgent[ConfigModel] | RawResourceT | None = None
+    ac_parser: str | None = None
     validate_assignment: bool = True
+    autoupdate_forward_refs: bool = True
 
     Extra = pydantic.Extra
```

### Comparing `configzen-0.2.8/configzen/processor.py` & `configzen-0.2.9/configzen/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
 from configzen.errors import (
     ConfigPreprocessingError,
-    InternalConfigError,
-    pretty_syntax_error,
 )
 from configzen.typedefs import ConfigModelT, SupportsRoute
 
 if TYPE_CHECKING:
-    from configzen.config import BaseContext, ConfigManager
+    from configzen.config import BaseContext, ConfigAgent
 
 __all__ = (
     "DirectiveContext",
     "directive",
     "Processor",
 )
 
@@ -90,158 +88,30 @@
         The dictionary that contains the :attr:`dict`.
 
     """
 
     directive: str
     key: str
     prefix: str
-    arguments: list[str]
     snippet: dict[str, Any]
     container: dict[str, Any]
 
-    def has_duplicates(self, *, require_same_arguments: bool = True) -> bool:
-        """
-        Return whether the directive has duplicates.
-
-        Returns
-        -------
-        Whether the directive has duplicates.
-        """
-        for key in self.container:
-            directive_name, arguments = parse_directive_call(self.prefix, key)
-            if directive_name == self.directive:
-                if require_same_arguments and arguments != self.arguments:
-                    continue
-                return True
-        return False
-
-
-class Tokens(str, enum.Enum):
-    LPAREN: str = "("
-    RPAREN: str = ")"
-    COMMAS: str = ",;"
-    STRING: str = "\"'"
-    ESCAPE: str = "\\"
-
-
-class ArgumentSyntaxError(ValueError):
-    """
-    Raised when there is a syntax error in an argument.
-    """
-
-
-def _parse_argument_string_impl(  # noqa: C901, PLR0912, PLR0915
-    raw_argument_string: str,
-    tokens: type[Tokens] = Tokens,
-) -> list[str]:
-    prev_char = None
-    string_ctx = None
-    escape_ctx = False
-    arguments: list[str] = []
-    argument = ""
-    emit = arguments.append
-    explicit_strings_ctx = True
-
-    tok_escape = tokens.ESCAPE
-    tok_string = tokens.STRING
-    tok_commas = tokens.COMMAS
-
-    for char_no, char in enumerate(raw_argument_string, start=1):
-        if escape_ctx:
-            escape_ctx = False
-            argument += char
-        elif char in tok_escape:
-            escape_ctx = True
-        elif char in tok_string:
-            if string_ctx and not explicit_strings_ctx:
-                msg = f"Implicit string closed with explicit string character {char}"
-                raise InternalConfigError(msg, extra=char_no)
-            explicit_strings_ctx = True
-            if string_ctx is None:
-                # we enter a string
-                string_ctx = char
-            elif string_ctx == char:
-                # we exit a string
-                string_ctx = None
-            else:
-                # we are in a string
-                argument += char
-        elif char in tok_commas:
-            if string_ctx:
-                if not explicit_strings_ctx:
-                    string_ctx = None
-                    explicit_strings_ctx = True
-                    emit(argument)
-                    argument = ""
-            else:
-                if prev_char in {*tok_commas, None}:
-                    msg = "Empty argument"
-                    raise InternalConfigError(msg, extra=char_no)
-                emit(argument)
-                argument = ""
-                explicit_strings_ctx = False
-        elif not string_ctx and not char.isspace():
-            if prev_char in {*tok_commas, None}:
-                string_ctx = char
-                argument += char
-                explicit_strings_ctx = False
-            if explicit_strings_ctx:
-                msg = "Unexpected character after explicit string"
-                raise InternalConfigError(msg, extra=char_no)
-        else:
-            argument += char
-        prev_char = char
-    return arguments
-
-
-def _parse_argument_string(
-    raw_argument_string: str,
-    tokens: type[Tokens] = Tokens,
-) -> list[str]:
-    """Half for jokes, half for serious use"""
-
-    tok_commas = tokens.COMMAS
-
-    if any(raw_argument_string.endswith(tok) for tok in tok_commas):
-        raw_argument_string = raw_argument_string[:-1]
-    raw_argument_string += tok_commas[0]
-
-    if raw_argument_string in tok_commas:
-        return []
-
-    with pretty_syntax_error(raw_argument_string):
-        return _parse_argument_string_impl(raw_argument_string, tokens)
-
 
 def parse_directive_call(
     prefix: str,
     directive_name: str,
-    tokens: type[Tokens] = Tokens,
-) -> tuple[str, list[str]]:
-    arguments = []
+) -> str:
     if directive_name.startswith(prefix):
         directive_name = directive_name[len(prefix) :].casefold()
 
-        if directive_name.endswith(tokens.RPAREN):
-            try:
-                lpar = directive_name.index(tokens.LPAREN)
-            except ValueError:
-                msg = f"invalid directive call: {directive_name}"
-                raise ConfigPreprocessingError(msg) from None
-            (directive_name, raw_argument_string) = (
-                directive_name[:lpar],
-                directive_name[lpar + 1 : -1],
-            )
-            arguments = _parse_argument_string(raw_argument_string, tokens)
-
         if not directive_name.isidentifier():
-            msg = f"invalid directive name: {directive_name}"
+            msg = f"Invalid directive name: {directive_name}"
             raise ConfigPreprocessingError(msg)
 
-    return directive_name, arguments
+    return directive_name
 
 
 if TYPE_CHECKING:
 
     class ExportMetadata(TypedDict, Generic[ConfigModelT]):
         route: str | None
         context: BaseContext[ConfigModelT]
@@ -283,18 +153,18 @@
     _directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
     _async_directive_handlers: dict[str, Any] = None  # type: ignore[assignment]
     directive_prefix: ClassVar[str]
     extension_prefix: ClassVar[str]
 
     def __init__(
         self,
-        manager: ConfigManager[ConfigModelT],
+        agent: ConfigAgent[ConfigModelT],
         dict_config: dict[str, Any],
     ) -> None:
-        self.manager = manager
+        self.agent = agent
         self.dict_config = dict_config
 
     @classmethod
     def export(
         cls,
         state: Any,
         *,
@@ -413,24 +283,21 @@
                         f"{self.extension_prefix} can be used only for overriding "
                         f"dictionary sections but item at {actual_key!r} "
                         f"is not a dictionary"
                     )
                 replacement = overridden | value
                 result[actual_key] = self._preprocess(replacement)
             elif key.startswith(self.directive_prefix):
-                directive_name, arguments = parse_directive_call(
-                    self.directive_prefix, key
-                )
+                directive_name = parse_directive_call(self.directive_prefix, key)
                 context_container = container.copy()
                 del context_container[key]
                 context = DirectiveContext(
                     directive=directive_name,
                     key=key,
                     prefix=self.directive_prefix,
-                    arguments=arguments,
                     snippet=value,
                     container=context_container,
                 )
                 self._call_directive(context)
                 new_container = self._preprocess(context.container)
                 result |= new_container
             else:
@@ -457,24 +324,21 @@
                         f"{self.extension_prefix} can be used only for overriding "
                         f"dictionary sections but item at {actual_key!r} "
                         f"is not a dictionary"
                     )
                 replacement = overridden | value
                 result[actual_key] = await self._preprocess_async(replacement)
             elif key.startswith(self.directive_prefix):
-                directive_name, arguments = parse_directive_call(
-                    self.directive_prefix, key
-                )
+                directive_name = parse_directive_call(self.directive_prefix, key)
                 context_container = container.copy()
                 del context_container[key]
                 context = DirectiveContext(
                     directive=directive_name,
                     key=key,
                     prefix=self.directive_prefix,
-                    arguments=arguments,
                     snippet=value,
                     container=context_container,
                 )
                 await self._call_directive_async(context)
                 new_container = await self._preprocess_async(context.container)
                 result |= new_container
             else:
@@ -518,45 +382,31 @@
     @classmethod
     def register_directive(cls, name: str, func: Any) -> None:
         if cls._directive_handlers is None:
             cls._directive_handlers = {}
         cls._directive_handlers[name] = func
 
     @classmethod
-    def directive(cls, directive_name: str, arguments: list[str] | None = None) -> str:
+    def directive(cls, directive_name: str) -> str:
         """
         Create a directive call.
 
         Parameters
         ----------
         directive_name
             The name of the directive.
-        arguments
-            The arguments to pass to the directive.
 
         Returns
         -------
         The directive call.
         """
-        if arguments is None:
-            arguments = []
-
-        def _fmt_argument(argument: str) -> str:
-            if '"' in argument:
-                argument = argument.replace("\\", "\\\\")
-                return f'"{argument}"'
-            return argument
-
         if isinstance(directive_name, enum.Enum):
             directive_name = directive_name.value
 
-        fmt_arguments = (
-            ",".join(map(_fmt_argument, arguments)).join("()") if arguments else ""
-        )
-        return cls.directive_prefix + directive_name + fmt_arguments
+        return cls.directive_prefix + directive_name
 
 
 class Directives(str, enum.Enum):
     EXTEND = "extend"
     INCLUDE = "include"
     COPY = "copy"
 
@@ -701,106 +551,105 @@
     async def copy_async(self, ctx: DirectiveContext) -> None:
         """
         Copy a configuration and paste into another configuration asynchronously.
         For more information see `copy`.
         """
         await self._substitute_async(ctx, preprocess=False, preserve=False)
 
-    def _get_substitution_info(
-        self, ctx: DirectiveContext, *, preserve: bool
+    def _get_substitution_means(
+        self, ctx: DirectiveContext  # , *, preserve: bool
     ) -> tuple[
-        ConfigManager[ConfigModelT], ConfigManager[ConfigModelT], SupportsRoute | None
+        ConfigAgent[ConfigModelT], ConfigAgent[ConfigModelT], SupportsRoute | None
     ]:
-        manager_class = type(self.manager)
-
-        if len(ctx.arguments):
-            msg = f"{ctx.directive!r} directive takes no () arguments"
-            raise ConfigPreprocessingError(msg)
+        agent_class = type(self.agent)
 
-        if preserve and ctx.has_duplicates(require_same_arguments=False):
-            msg = (
-                f"using more than one {ctx.directive!r} directive "
-                "in the same section is not allowed"
-            )
-            raise ConfigPreprocessingError(msg)
+        # todo(bswck): raise on include and extend combined
+        # if preserve and ???:
+        #     msg = (
+        #         "Using more than one ??? directive "
+        #         "in the same scope is not allowed"
+        #     )
+        #     raise ConfigPreprocessingError(msg)
 
-        manager, route = manager_class.from_directive_context(
+        agent, route = agent_class.from_directive_context(
             ctx, route_separator=self.route_separator
         )
 
-        if manager.resource == self.manager.resource:
+        if agent.resource == self.agent.resource:
             raise ConfigPreprocessingError(
-                f"{manager.resource} tried to {ctx.directive!r} on itself"
+                f"{agent.resource} tried to {ctx.directive!r} on itself"
             )
 
-        actual_manager = manager
-        if manager.relative:
-            parent = cast(pathlib.Path, self.manager.resource).parent
-            child = cast(pathlib.Path, manager.resource)
+        actual_agent = agent
+        if agent.relative:
+            parent = cast(pathlib.Path, self.agent.resource).parent
+            child = cast(pathlib.Path, agent.resource)
 
-            actual_manager = copy.copy(manager)
-            actual_manager.resource = parent / child
+            actual_agent = copy.copy(agent)
+            actual_agent.resource = parent / child
 
-        return actual_manager, manager, route
+        return actual_agent, agent, route
 
     def _substitute(
         self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
     ) -> None:
-        actual_mgr, mgr, route = self._get_substitution_info(ctx, preserve=preserve)
+        agent, orig_agent, route = self._get_substitution_means(ctx)
 
-        with actual_mgr.processor_open_resource() as reader:
-            source = mgr.load_into_dict(reader.read(), preprocess=preprocess)
+        with agent.processor_open_resource() as reader:
+            source = orig_agent.load_into_dict(reader.read(), preprocess=preprocess)
 
         self._substitute_impl(
             ctx,
             route,
             source=source,
-            manager=mgr,
+            agent=orig_agent,
             preprocess=preprocess,
             preserve=preserve,
         )
 
     async def _substitute_async(
         self, ctx: DirectiveContext, *, preprocess: bool, preserve: bool
     ) -> None:
-        actual_mgr, mgr, route = self._get_substitution_info(ctx, preserve=preserve)
+        agent, orig_agent, route = self._get_substitution_means(ctx)
 
-        async with actual_mgr.processor_open_resource_async() as reader:
-            source = mgr.load_into_dict(await reader.read(), preprocess=preprocess)
+        async with agent.processor_open_resource_async() as reader:
+            source = orig_agent.load_into_dict(
+                await reader.read(), preprocess=preprocess
+            )
 
         self._substitute_impl(
             ctx,
             route,
             source=source,
-            manager=mgr,
+            agent=orig_agent,
             preprocess=preprocess,
             preserve=preserve,
         )
 
     @staticmethod
     def _substitute_impl(  # noqa: PLR0913
         ctx: DirectiveContext,
         route: SupportsRoute | None,
         *,
         source: dict[str, Any],
-        manager: ConfigManager[ConfigModelT],
+        agent: ConfigAgent[ConfigModelT],
         preprocess: bool,
         preserve: bool,
     ) -> None:
         from configzen.config import CONTEXT, Context, at
 
         if route:
-            source = at(source, route, manager=manager)
+            source = at(source, route, agent=agent)
             if not is_dict_like(source):
                 raise ConfigPreprocessingError(
                     f"imported item {route!r} "
-                    f"from {manager.resource} is not a dictionary"
+                    f"from {agent.resource} is not a dictionary"
                 )
 
-        context: Context[ConfigModelT] = Context(manager)
+        context: Context[ConfigModelT] = Context(agent)
         ctx.container = source | ctx.container
 
         if preserve:
             ctx.container |= {
                 CONTEXT: context,
                 EXPORT: ExportMetadata(
                     route=str(route),
@@ -827,22 +676,22 @@
         from configzen.config import CONTEXT, at, pre_serialize
 
         overrides = {}
 
         route = metadata["route"]
         context = metadata["context"]
         key_order = metadata["key_order"]
-        manager = context.manager
+        agent = context.agent
 
-        with manager.processor_open_resource() as reader:
+        with agent.processor_open_resource() as reader:
             # Here we intentionally always preprocess the loaded configuration.
-            loaded = manager.load_into_dict(reader.read())
+            loaded = agent.load_into_dict(reader.read())
 
             if route:
-                loaded = at(loaded, route, manager=manager)
+                loaded = at(loaded, route, agent=agent)
 
         substituted_values = loaded.copy()
 
         missing = object()
 
         for key, value in loaded.items():
             counterpart_value = state.pop(key, missing)
@@ -858,15 +707,15 @@
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
                         (orig := value.get(sub_key, missing)) is missing or orig != comp
                     )
                 }
                 if overrides_for_key:
-                    export_key = manager.processor_class.extension_prefix + key
+                    export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
                 cls.export(value, metadata=None)
 
             elif counterpart_value != value:
                 overrides[key] = counterpart_value
@@ -901,22 +750,22 @@
         from configzen.config import CONTEXT, at, pre_serialize
 
         overrides = {}
 
         route = metadata["route"]
         context = metadata["context"]
         key_order = metadata["key_order"]
-        manager = context.manager
+        agent = context.agent
 
-        async with manager.processor_open_resource_async() as reader:
+        async with agent.processor_open_resource_async() as reader:
             # Here we intentionally always preprocess the loaded configuration.
-            loaded = await manager.load_into_dict_async(await reader.read())
+            loaded = await agent.load_into_dict_async(await reader.read())
 
             if route:
-                loaded = at(loaded, route, manager=manager)
+                loaded = at(loaded, route, agent=agent)
 
         substituted_values = loaded.copy()
 
         missing = object()
 
         for key, value in loaded.items():
             counterpart_value = state.pop(key, missing)
@@ -932,15 +781,15 @@
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
                         (orig := value.get(sub_key, missing)) is missing or orig != comp
                     )
                 }
                 if overrides_for_key:
-                    export_key = manager.processor_class.extension_prefix + key
+                    export_key = agent.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
                 await cls.export_async(value, metadata=None)
 
             elif counterpart_value != value:
                 overrides[key] = counterpart_value
@@ -965,24 +814,24 @@
         *,
         state: dict[str, Any],
         overrides: dict[str, Any],
         values: dict[str, Any],
         route: str | None,
         key_order: list[str],
     ) -> None:
-        # TODO: Optimize. We iterate over the same too many times.
+        # TODO: Optimize. We iterate over the same way too many times.
 
         state |= overrides
         extras: dict[str, Any] = {
             key: state.pop(key) for key in set(state) if key not in key_order
         }
 
         if values:
             substitution_directive = cls.directive(Directives.EXTEND)
-            resource = str(context.manager.resource)
+            resource = str(context.agent.resource)
             if route:
                 resource = cls.route_separator.join((resource, route))
             # Put the substitution directive at the beginning of the state in-place.
             state |= {substitution_directive: resource} | {
                 key: state.pop(key) for key in set(state)
             }
```

### Comparing `configzen-0.2.8/configzen/typedefs.py` & `configzen-0.2.9/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.8/LICENSE` & `configzen-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.8/pyproject.toml` & `configzen-0.2.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.8"
+version = "0.2.9"
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
+aiofiles = {version = "^23.1.0", extras = ["async"]}
+pyyaml = {version = "^6.0", extras = ["yaml"]}
+toml = {version = "^0.10.2", extras = ["toml"]}
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.267"
 mypy = "^1.3.0"
 black = "^23.3.0"
 pre-commit = "^3.3.1"
-
-[tool.poetry.group.async.dependencies]
-aiofiles = "^23.1.0"
-
-[tool.poetry.group.yaml.dependencies]
-pyyaml = "^6.0"
-
-[tool.poetry.group.toml.dependencies]
-toml = "^0.10.2"
+pytest = "^7.3.1"
 
 [tool.ruff]
 target-version = "py39"
 select = ["F","E","W","I","UP","N","S","C","B","A","T","Q","RUF","YTT","BLE","ANN","FBT","PL","TRY","RSE","SLF","DTZ","EXE","ISC","ICN","G","INP","PIE","RET","SIM","TID","TCH","ARG","PTH"]
 ignore = ["DTZ005","INP001","TCH003","ANN101","ANN102","ANN401","I001","TID252","T201","B905","S101","TRY003","PLR2004"]
 fix = true
-exclude = ["examples/"]
+exclude = ["examples/", "tests/"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `configzen-0.2.8/README.md` & `configzen-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.8/PKG-INFO` & `configzen-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.8
+Version: 0.2.9
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
+Requires-Dist: aiofiles[async] (>=23.1.0,<24.0.0)
 Requires-Dist: anyconfig (>=0.13.0,<0.14.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyyaml[yaml] (>=6.0,<7.0)
+Requires-Dist: toml[toml] (>=0.10.2,<0.11.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version >= "3.9" and python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # configzen
 _configzen_ – managing configuration files easily.
 Currently under development, not ready for production use.
```

