# Comparing `tmp/arguably-1.0.1.tar.gz` & `tmp/arguably-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arguably-1.0.1.tar", max compression
+gzip compressed data, was "arguably-1.0.2.tar", max compression
```

## Comparing `arguably-1.0.1.tar` & `arguably-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1538 2023-06-07 14:36:36.505951 arguably-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0    72211 2023-06-07 14:36:36.505951 arguably-1.0.1/arguably/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 14:36:36.505951 arguably-1.0.1/arguably/py.typed
--rw-r--r--   0        0        0     4442 2023-06-07 14:36:36.505951 arguably-1.0.1/assets/PYPI_README.md
--rw-r--r--   0        0        0      869 2023-06-07 14:36:36.505951 arguably-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5052 1970-01-01 00:00:00.000000 arguably-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-06-08 13:05:22.603853 arguably-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0    72461 2023-06-08 13:05:22.603853 arguably-1.0.2/arguably/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:05:22.603853 arguably-1.0.2/arguably/py.typed
+-rw-r--r--   0        0        0     5135 2023-06-08 13:05:22.603853 arguably-1.0.2/assets/PYPI_README.md
+-rw-r--r--   0        0        0      917 2023-06-08 13:05:22.603853 arguably-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5845 1970-01-01 00:00:00.000000 arguably-1.0.2/PKG-INFO
```

### Comparing `arguably-1.0.1/LICENSE.txt` & `arguably-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arguably-1.0.1/arguably/__init__.py` & `arguably-1.0.2/arguably/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,29 +43,36 @@
 from dataclasses import dataclass, field
 from gettext import gettext
 
 from typing import (
     Callable,
     cast,
     Any,
-    Annotated,
     TextIO,
     IO,
     Sequence,
     Collection,
-    get_args,
-    get_origin,
-    get_type_hints,
     Iterable,
     Union,
     Optional,
+    List,
+    Dict,
+    Type,
+    Tuple,
 )
 
 from docstring_parser import parse as docparse
 
+# Annotated is 3.9 and up
+if sys.version_info >= (3, 9):
+    from typing import Annotated, get_type_hints, get_args, get_origin
+else:
+    from typing_extensions import Annotated, get_type_hints, get_args, get_origin
+
+# UnionType is the new type for the `A | B` type syntax, which is 3.10 and up
 if sys.version_info >= (3, 10):
     from types import UnionType
 else:
 
     class UnionType:
         """Stub this out, we only use it for issubclass() checks"""
 
@@ -110,36 +117,36 @@
         args_string = self._format_args(action, default_metavar)
         return ", ".join(action.option_strings) + " " + args_string
 
     def _metavar_formatter(
         self,
         action: argparse.Action,
         default_metavar: str,
-    ) -> Callable[[int], tuple[str, ...]]:
+    ) -> Callable[[int], Tuple[str, ...]]:
         """Mostly copied from the original _metavar_formatter, but special-cases enum member printing"""
         if action.metavar is not None:
             result = action.metavar
         elif action.choices is not None:
             if isinstance(next(iter(action.choices)), enum.Enum):
                 choice_strs = [choice.name for choice in action.choices]
             else:
                 choice_strs = [str(choice) for choice in action.choices]
             result = "{%s}" % ",".join(choice_strs)
         else:
             result = default_metavar
 
-        def _format(tuple_size: int) -> tuple[str, ...]:
+        def _format(tuple_size: int) -> Tuple[str, ...]:
             if isinstance(result, tuple):
                 return result
             else:
                 return (result,) * tuple_size
 
         return _format
 
-    def _split_lines(self, text: str, width: int) -> list[str]:
+    def _split_lines(self, text: str, width: int) -> List[str]:
         """Copied from the original _split_lines, but we don't replace multiple spaces with only one"""
         # text = self._whitespace_matcher.sub(' ', text).strip()
         # The textwrap module is used only for formatting help.
         # Delay its import for speeding up the common usage of argparse.
         import textwrap
 
         return textwrap.wrap(text, width)
@@ -212,21 +219,21 @@
                     ]
                 ),
             }
             msg = gettext("invalid choice: %(value)r (choose from %(choices)s)")
             raise argparse.ArgumentError(action, msg % args)
 
 
-def _split_unquoted(unsplit: str, delimeter: str, limit: Union[int, float] = math.inf) -> list[str]:
+def _split_unquoted(unsplit: str, delimeter: str, limit: Union[int, float] = math.inf) -> List[str]:
     """Splits text at a delimiter, as long as that delimiter is not quoted (either single ' or double quotes ")."""
     assert len(delimeter) == 1
     assert limit > 0
     result = list()
     quote_char = None
-    accumulator: list[str] = list()
+    accumulator: List[str] = list()
     for char in unsplit:
         if char == delimeter and quote_char is None and limit > 0:
             result.append("".join(accumulator))
             accumulator.clear()
             limit -= 1
             continue
         elif char == "'":
@@ -241,15 +248,15 @@
                 quote_char = None
         accumulator.append(char)
     result.append("".join(accumulator))
     accumulator.clear()
     return result
 
 
-def _normalize_action_input(values: Union[str, Sequence[Any], None]) -> list[str]:
+def _normalize_action_input(values: Union[str, Sequence[Any], None]) -> List[str]:
     """Normalize `values` input to be a list"""
     if values is None:
         return list()
     elif isinstance(values, str):
         # "-" means empty
         return list() if values == "-" else [values]
     else:
@@ -350,15 +357,15 @@
 
 
 @dataclass
 class _BuildTypeSpec:
     """Subtype and kwargs that specify how to build a class, created by `_BuildTypeAction` and consumed later."""
 
     subtype: Optional[str]
-    kwargs: dict[str, Any]
+    kwargs: Dict[str, Any]
 
 
 class _BuildTypeAction(argparse.Action):
     """
     Special action for arguably, handles building a class with a complex signature for __init__, or when multiple
     subclasses can be chosen from.
     """
@@ -381,15 +388,15 @@
         split_values = list()
         for value in values:
             split_str_values = [_unwrap_quotes(v) for v in _split_unquoted(value, delimeter=",")]
             split_values.extend(split_str_values)
         values = split_values
 
         # Separate out subtype and kwargs
-        kwargs: dict[str, Any] = dict()
+        kwargs: Dict[str, Any] = dict()
         subtype_ = None
         if len(values) > 0 and "=" not in values[0]:
             subtype_ = values[0]
             values = values[1:]
 
         # Build kwargs dict
         for value in values:
@@ -448,15 +455,15 @@
             alias = transform(char)
             assert len(alias) == 1, f"One character became more than one: `{char}` -> `{alias}`"
             if alias not in used_aliases:
                 return alias
     return None
 
 
-def _get_ancestors(command_name: str) -> list[str]:
+def _get_ancestors(command_name: str) -> List[str]:
     """
     List all ancestors for a given command. For example, `foo bar bat` yeilds a list with:
       * `__root__`
       * `__root__ foo`
       * `__root__ foo bar`
 
     Note that `__root__` is always an implicit ancestor.
@@ -481,42 +488,42 @@
     return result
 
 
 @dataclass
 class _EnumFlagInfo:
     """Used similarly to _CommandArg, but for entries in an `enum.Flag`."""
 
-    option: Union[tuple[str], tuple[str, str]]
+    option: Union[Tuple[str], Tuple[str, str]]
     arg_name: str
     value: Any
     description: str
 
 
-def _get_enum_member_docs(enum_class: type[enum.Enum]) -> dict[str, str]:
+def _get_enum_member_docs(enum_class: Type[enum.Enum]) -> Dict[str, str]:
     """Extracts docstrings for enum members similar to PEP-224, which has become a pseudo-standard supported by a lot of
     tooling"""
     parsed = ast.parse(inspect.getsource(enum_class))
     assert len(parsed.body) == 1
 
     classdef = parsed.body[0]
     assert isinstance(classdef, ast.ClassDef)
 
     # Search for a string expression following an assignment
     prev = None
-    result: dict[str, str] = dict()
+    result: Dict[str, str] = dict()
     for item in classdef.body:
         if isinstance(item, ast.Expr) and isinstance(item.value, ast.Constant) and isinstance(item.value.value, str):
             if isinstance(prev, ast.Assign) and len(prev.targets) == 1 and isinstance(prev.targets[0], ast.Name):
                 result[cast(ast.Name, prev.targets[0]).id] = item.value.value
         prev = item
 
     return result
 
 
-def _info_for_flags(arg_name: str, flag_class: type[enum.Flag]) -> list[_EnumFlagInfo]:
+def _info_for_flags(arg_name: str, flag_class: Type[enum.Flag]) -> List[_EnumFlagInfo]:
     """Generates a list of `_EnumFlagInfo` corresponding to all flags in an `enum.Flag`."""
     result = list()
     docs = docparse(flag_class.__doc__ or "")
     enum_member_docs = _get_enum_member_docs(flag_class)
     for item in flag_class:
         options = [f"--{_normalize_name(cast(str, item.name))}"]
         arg_description = ""
@@ -541,15 +548,15 @@
 
         # Extract the alias from the docstring for the flag item
         if alias_match := re.match(r"^\[-([a-zA-Z0-9])] ", arg_description):
             arg_description = arg_description[len(alias_match.group(0)) :]
             options.insert(0, f"-{alias_match.group(1)}")
 
         result.append(
-            _EnumFlagInfo(cast(Union[tuple[str], tuple[str, str]], tuple(options)), arg_name, item, arg_description)
+            _EnumFlagInfo(cast(Union[Tuple[str], Tuple[str, str]], tuple(options)), arg_name, item, arg_description)
         )
     return result
 
 
 class _NoDefault:
     """Indicator that there is no default value for a parameter. Necessary because None can be the default value."""
 
@@ -615,16 +622,16 @@
     arg_name: str
     input_method: _InputMethod
     arg_value_type: type
     description: str
     count: int = 1
     alias: Optional[str] = None
     default: Any = _NoDefault
-    metavars: Optional[list[str]] = None
-    modifiers: list[_CommandArgModifier] = field(default_factory=list)
+    metavars: Optional[List[str]] = None
+    modifiers: List[_CommandArgModifier] = field(default_factory=list)
 
     ANY_COUNT = -1  # Used in the `count` field for an argument that can take any number of values, `*args`
 
     @staticmethod
     def _normalize_type_union(
         function_name: str,
         param: inspect.Parameter,
@@ -644,32 +651,32 @@
             value_type = filtered_types[0]
         return value_type
 
     @staticmethod
     def normalize_type(
         function_name: str,
         param: inspect.Parameter,
-        hints: dict[str, Any],
-    ) -> tuple[type, list[_CommandArgModifier]]:
+        hints: Dict[str, Any],
+    ) -> Tuple[type, List[_CommandArgModifier]]:
         """
         Normalizes the parameter type. Most of the logic here is validation. Explanation of what's returned for a given
         parameter type:
           * SomeType                    ->  value_type=SomeType, modifiers=[]
           * int | None                  ->  value_type=int, modifiers=[]
-          * tuple[float, float]         ->  value_type=type(None), modifiers=[_TupleModifier([float, float])]
-          * list[str]                   ->  value_type=str, modifiers=[_ListModifier()]
+          * Tuple[float, float]         ->  value_type=type(None), modifiers=[_TupleModifier([float, float])]
+          * List[str]                   ->  value_type=str, modifiers=[_ListModifier()]
           * Annotated[int, arg.count()] ->  value_type=int, modifiers=[_CountedModifier()]
 
         Things that will cause an exception:
-          * Parameterized type other than a Optional[] or tuple[]
-          * Flexible-length tuple[SomeType, ...]
+          * Parameterized type other than a Optional[] or Tuple[]
+          * Flexible-length Tuple[SomeType, ...]
           * Parameter lacking an annotation
         """
 
-        modifiers: list[_CommandArgModifier] = list()
+        modifiers: List[_CommandArgModifier] = list()
 
         if param.name in hints:
             value_type = hints[param.name]
         else:
             # No type hint. Guess type from default value, if any other than None. Otherwise, default to string.
             value_type = type(param.default) if param.default not in [param.empty, None] else str
 
@@ -697,15 +704,15 @@
         origin = get_origin(value_type)
         if origin == list:
             type_args = get_args(value_type)
             if len(type_args) == 0:
                 value_type = str
             elif len(type_args) > 1:
                 raise ArguablyException(
-                    f"Function parameter `{param.name}` in `{function_name}` has too many items passed to list[...]."
+                    f"Function parameter `{param.name}` in `{function_name}` has too many items passed to List[...]."
                     f"There should be exactly one item between the square brackets."
                 )
             else:
                 value_type = type_args[0]
             modifiers.append(_ListModifier())
         elif origin == tuple:
             if param.kind in [param.VAR_KEYWORD, param.VAR_POSITIONAL]:
@@ -743,16 +750,16 @@
 @dataclass
 class _Command:
     """A fully processed command"""
 
     function: Callable
     name: str
     description: str = ""
-    args: list[_CommandArg] = field(default_factory=list)
-    arg_map: dict[str, _CommandArg] = field(init=False)
+    args: List[_CommandArg] = field(default_factory=list)
+    arg_map: Dict[str, _CommandArg] = field(init=False)
     alias: Optional[str] = None
 
     has_positional_args: bool = False
     variadic_positional_arg: Optional[str] = None
 
     def __post_init__(self) -> None:
         self.arg_map = dict()
@@ -760,15 +767,15 @@
             if arg_.arg_name in self.arg_map:
                 raise ArguablyException(
                     f"Function parameter `{arg_.param_name}` in `{self.name}` conflicts with "
                     f"`{self.arg_map[arg_.arg_name].param_name}`, both names simplify to `{arg_.arg_name}`"
                 )
             self.arg_map[arg_.arg_name] = arg_
 
-    def call(self, parsed_args: dict[str, Any]) -> Any:
+    def call(self, parsed_args: Dict[str, Any]) -> Any:
         """Filters arguments from argparse to only include the ones used by this command, then calls it"""
 
         args = list()
         kwargs = dict()
 
         filtered_args = dict()
         for k, v in parsed_args.items():
@@ -808,39 +815,39 @@
     """A class that encapsulates a change to the kwargs dict to be passed to parser.add_argument()"""
 
     @classmethod
     def check_valid(cls, value_type: type, param: inspect.Parameter, function_name: str) -> None:
         """Checks whether this modifier is valid for the parameter"""
 
     @abc.abstractmethod
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
         """Modifies the kwargs passed to parser.add_argument()"""
 
 
 @dataclass(frozen=True)
 class _MissingArgDefaultModifier(_CommandArgModifier):
     """Allows an option to be a flag, passing a default value instead of a value provided via the command line"""
 
     missing_value: Any
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
-        kwargs_dict |= dict(nargs="?", const=self.missing_value)
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
+        kwargs_dict.update(nargs="?", const=self.missing_value)
 
 
 @dataclass(frozen=True)
 class _CountedModifier(_CommandArgModifier):
     """Counts the number of times a flag is provided"""
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
         if arg_.input_method != _InputMethod.OPTION:
             raise ArguablyException(
                 f"`arguably.Counted` should only be used on {_InputMethod.OPTION.name}, but was used on "
                 f"{arg_.param_name}, which is {arg_.input_method.name}."
             )
-        kwargs_dict |= dict(action="count")
+        kwargs_dict.update(action="count")
         if "type" in kwargs_dict:
             del kwargs_dict["type"]
         if "nargs" in kwargs_dict:
             del kwargs_dict["nargs"]
 
 
 @dataclass(frozen=True)
@@ -848,79 +855,79 @@
     """Marks an input as required. In the case of a variadic positional arg, uses the '+' symbol to represent this."""
 
     @classmethod
     def check_valid(cls, value_type: type, param: inspect.Parameter, function_name: str) -> None:
         if issubclass(value_type, bool):
             raise ArguablyException("Cannot mark a bool as required.")
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
         if command_.variadic_positional_arg == arg_.param_name:
-            kwargs_dict |= dict(nargs="+")
+            kwargs_dict.update(nargs="+")
         else:
-            kwargs_dict |= dict(required=True)
+            kwargs_dict.update(required=True)
 
 
 @dataclass(frozen=True)
 class _ListModifier(_CommandArgModifier):
     """Sets up arguably list handling. Sensitive to the `_RequiredModifier`."""
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
         if arg_.input_method is _InputMethod.OPTIONAL_POSITIONAL:
-            kwargs_dict |= dict(nargs="?")
+            kwargs_dict.update(nargs="?")
         if arg_.input_method is not _InputMethod.REQUIRED_POSITIONAL:
-            kwargs_dict |= dict(default=list())
+            kwargs_dict.update(default=list())
         if (arg_.default is _NoDefault and arg_.input_method is _InputMethod.OPTION) or _RequiredModifier in [
             type(mod) for mod in arg_.modifiers
         ]:
-            kwargs_dict |= dict(required=True)
-        kwargs_dict |= dict(action=_CommaSeparatedListAction)
+            kwargs_dict.update(required=True)
+        kwargs_dict.update(action=_CommaSeparatedListAction)
 
 
 @dataclass(frozen=True)
 class _TupleModifier(_CommandArgModifier):
     """Sets up arguably tuple handling"""
 
-    tuple_arg: list[type]
+    tuple_arg: List[type]
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
-        kwargs_dict |= dict(nargs=len(self.tuple_arg), action=_CommaSeparatedTupleAction, type=self.tuple_arg)
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
+        kwargs_dict.update(nargs=len(self.tuple_arg), action=_CommaSeparatedTupleAction, type=self.tuple_arg)
 
 
 @dataclass(frozen=True)
 class _BuilderModifier(_CommandArgModifier):
     """Sets up arguably builder"""
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
-        kwargs_dict |= dict(action=_BuildTypeAction)
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
+        kwargs_dict.update(action=_BuildTypeAction)
 
 
 @dataclass(frozen=True)
 class _HandlerModifier(_CommandArgModifier):
     """
     Allows full user control over how an input is handled, a function should be passed in to parse the string from the
     command line
     """
 
     handler: Callable[[str], Any]
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
-        kwargs_dict |= dict(type=self.handler)
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
+        kwargs_dict.update(type=self.handler)
 
 
 @dataclass(frozen=True)
 class _ChoicesModifier(_CommandArgModifier):
     """Restricts inputs to one of a given set of choices"""
 
     choices: Iterable[Union[str, enum.Enum]]
 
-    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: dict[str, Any]) -> None:
+    def modify_arg_dict(self, command_: _Command, arg_: _CommandArg, kwargs_dict: Dict[str, Any]) -> None:
         first = next(iter(self.choices))
         if isinstance(first, enum.Enum):
             _context.set_up_enum(type(first), list(cast(Iterable[enum.Enum], self.choices)))
-        kwargs_dict |= dict(choices=self.choices)
+        kwargs_dict.update(choices=self.choices)
 
 
 ########################################################################################################################
 ########################################################################################################################
 # Context
 
 
@@ -951,15 +958,15 @@
 
     name: Optional[str]
 
     # Behavior options
     call_ancestors: bool
     auto_alias_cmds: bool
     auto_alias_params: bool
-    version_flag: Union[bool, list[str]]
+    version_flag: Union[bool, List[str]]
 
     # Formatting options
     show_defaults: bool
     command_metavar: str
     max_description_offset: int
     max_width: int
     output: Optional[TextIO]
@@ -978,51 +985,51 @@
 
 class _Context:
     """Singleton, used for storing arguably state."""
 
     def __init__(self) -> None:
         # These are `None` right now, they're set during `run()`. No methods making use of them are called before then.
         self._options: _ContextOptions = None  # type: ignore[assignment]
-        self._extra_argparser_options: dict[str, Any] = None  # type: ignore[assignment]
+        self._extra_argparser_options: Dict[str, Any] = None  # type: ignore[assignment]
 
         # Info for all invocations of `@arguably.command`
-        self._command_decorator_info: list[_CommandDecoratorInfo] = list()
+        self._command_decorator_info: List[_CommandDecoratorInfo] = list()
 
         # Info for all invocations of `@arguably.subtype`
-        self._subtype_init_info: list[_SubtypeDecoratorInfo] = list()
+        self._subtype_init_info: List[_SubtypeDecoratorInfo] = list()
 
         # Stores mapping from normalized names for an enum type to an enum value
-        self._enum_mapping: dict[type[enum.Enum], dict[str, enum.Enum]] = dict()
+        self._enum_mapping: Dict[Type[enum.Enum], Dict[str, enum.Enum]] = dict()
 
         # Stores which flag arguments have had their default value cleared
-        self._enum_flag_default_cleared: set[tuple[argparse.ArgumentParser, str]] = set()
+        self._enum_flag_default_cleared: set[Tuple[argparse.ArgumentParser, str]] = set()
 
         # Are we currently calling the targeted command (or just an ancestor?)
         self._is_calling_target = True
 
         # Used for handling `error()`, keeps a reference to the parser for the current command
         self._current_parser: Optional[argparse.ArgumentParser] = None
 
         # These are really only set and used in the run() method
-        self._commands: dict[str, _Command] = dict()
-        self._command_aliases: dict[str, str] = dict()
-        self._parsers: dict[str, argparse.ArgumentParser] = dict()
-        self._subparsers: dict[str, Any] = dict()
+        self._commands: Dict[str, _Command] = dict()
+        self._command_aliases: Dict[str, str] = dict()
+        self._parsers: Dict[str, argparse.ArgumentParser] = dict()
+        self._subparsers: Dict[str, Any] = dict()
 
     def add_command(self, **kwargs: Any) -> None:
         """Invoked by `@arguably.command`, saves info about a command to include when the parser is set up."""
         info = _CommandDecoratorInfo(**kwargs)
         self._command_decorator_info.append(info)
 
     def add_subtype(self, **kwargs: Any) -> None:
         """Invoked by `@arguably.subtype`, saves info about a how to construct a type."""
         type_ = _SubtypeDecoratorInfo(**kwargs)
         self._subtype_init_info.append(type_)
 
-    def find_subtype(self, param_type: type) -> list[_SubtypeDecoratorInfo]:
+    def find_subtype(self, param_type: type) -> List[_SubtypeDecoratorInfo]:
         return [bi for bi in self._subtype_init_info if issubclass(bi.type_, param_type)]
 
     def is_calling_target(self) -> bool:
         """Aliased by `arguably.is_target`. Only useful when `invoke_ancestors=True`, it lets a command know whether
         it's the main targeted command or just an ancestor of the targeted command."""
         return self._is_calling_target
 
@@ -1050,16 +1057,16 @@
         else:
             docs = docparse(info.function.__doc__)
             processed_description = "" if docs.short_description is None else docs.short_description
 
         hints = get_type_hints(info.function, include_extras=True)
 
         # Will be filled in as we loop over all parameters
-        processed_args: list[_CommandArg] = list()
-        used_arg_aliases: list[str] = list()
+        processed_args: List[_CommandArg] = list()
+        used_arg_aliases: List[str] = list()
         has_positional_args = False
         variadic_positional_arg = None
 
         # Iterate over all parameters
         for param_name, param in inspect.signature(info.function).parameters.items():
             arg_name = _normalize_name(param_name, spaces=False)
             arg_default = _NoDefault if param.default is param.empty else param.default
@@ -1166,18 +1173,18 @@
             processed_args,
             info.alias,
             has_positional_args,
             variadic_positional_arg,
         )
 
     def set_up_enum(
-        self, enum_type: type[enum.Enum], members: Optional[list[enum.Enum]] = None
-    ) -> dict[str, enum.Enum]:
+        self, enum_type: Type[enum.Enum], members: Optional[List[enum.Enum]] = None
+    ) -> Dict[str, enum.Enum]:
         if enum_type not in self._enum_mapping:
-            enum_name_dict: dict[str, enum.Enum] = dict()
+            enum_name_dict: Dict[str, enum.Enum] = dict()
             self._enum_mapping[enum_type] = enum_name_dict
 
             for enum_item in enum_type:
                 if members is not None and enum_item not in members:
                     continue
                 enum_name = _normalize_name(enum_item.name, spaces=False)
                 if enum_name in enum_name_dict:
@@ -1185,15 +1192,15 @@
                         f"Normalized name {enum_name} already taken for enum {enum_type.__name__} by "
                         f"{enum_name_dict[enum_name]}"
                     )
                 enum_name_dict[enum_name] = enum_item
 
         return self._enum_mapping[enum_type]
 
-    def get_enum_mapping(self, enum_type: type[enum.Enum]) -> dict[str, enum.Enum]:
+    def get_enum_mapping(self, enum_type: Type[enum.Enum]) -> Dict[str, enum.Enum]:
         assert enum_type in self._enum_mapping
         return self._enum_mapping[enum_type]
 
     def _set_up_args(self, cmd: _Command) -> None:
         """Adds all arguments to the parser for a given command"""
 
         parser = self._parsers[cmd.name]
@@ -1222,21 +1229,21 @@
                 for entry in _info_for_flags(arg_.arg_name, arg_.arg_value_type):
                     parser.add_argument(
                         *entry.option, action=_EnumFlagAction, const=entry, nargs=0, help=entry.description
                     )
                 continue
 
             # Optional kwargs for parser.add_argument
-            add_arg_kwargs: dict[str, Any] = dict(type=arg_.arg_value_type)
+            add_arg_kwargs: Dict[str, Any] = dict(type=arg_.arg_value_type)
 
             arg_description = arg_.description
 
             # `default` value?
             if arg_.input_method.is_optional and arg_.default is not _NoDefault:
-                add_arg_kwargs |= dict(default=arg_.default)
+                add_arg_kwargs.update(default=arg_.default)
                 if self._options.show_defaults:
                     if len(arg_description) > 0:
                         arg_description += " "
                     if isinstance(arg_.default, enum.Enum):
                         arg_description += f"(default: {_normalize_name(arg_.default.name, spaces=False)})"
                     elif isinstance(arg_.default, str):
                         str_default = arg_.default
@@ -1245,52 +1252,52 @@
                             str_default = repr(str_default)
                         arg_description += f"(default: {str_default})"
                     else:
                         arg_description += f"(default: {arg_.default})"
 
             # Number of arguments `nargs`?
             if arg_.count is _CommandArg.ANY_COUNT:
-                add_arg_kwargs |= dict(nargs="*")
+                add_arg_kwargs.update(nargs="*")
             elif arg_.input_method is _InputMethod.OPTIONAL_POSITIONAL:
-                add_arg_kwargs |= dict(nargs="?")
+                add_arg_kwargs.update(nargs="?")
             elif arg_.count != 1:
-                add_arg_kwargs |= dict(nargs=arg_.count, action=_CommaSeparatedTupleAction)
+                add_arg_kwargs.update(nargs=arg_.count, action=_CommaSeparatedTupleAction)
 
             # Any specified `metavar`s?
             if arg_.metavars is not None:
                 if len(arg_.metavars) == 1:
-                    add_arg_kwargs |= dict(metavar=arg_.metavars[0])
+                    add_arg_kwargs.update(metavar=arg_.metavars[0])
                 else:
-                    add_arg_kwargs |= dict(metavar=tuple(arg_.metavars))
+                    add_arg_kwargs.update(metavar=tuple(arg_.metavars))
 
             # Possible choices `choices`?
             if issubclass(arg_.arg_value_type, enum.Enum):
                 mapping = self.set_up_enum(arg_.arg_value_type)
-                add_arg_kwargs |= dict(choices=[n for n in mapping])
+                add_arg_kwargs.update(choices=[n for n in mapping])
 
-            arg_names: tuple[str, ...] = (arg_.arg_name,)
+            arg_names: Tuple[str, ...] = (arg_.arg_name,)
 
             # Special handling for optional arguments
             if arg_.input_method is _InputMethod.OPTION:
                 arg_names = (f"--{arg_.arg_name}",) if arg_.alias is None else (f"-{arg_.alias}", f"--{arg_.arg_name}")
 
             # `bool` should be flags
             if issubclass(arg_.arg_value_type, bool):
                 if arg_.input_method is not _InputMethod.OPTION or arg_.default is _NoDefault:
                     raise ArguablyException(
                         f"Function argument `{arg_.param_name}` in `{cmd.name}` is a `bool`. Boolean parameters must "
                         f"have a default value and be an optional, not a positional, argument."
                     )
                 # Use `store_true` or `store_false` for bools
-                add_arg_kwargs |= dict(action="store_true" if arg_.default is False else "store_false")
+                add_arg_kwargs.update(action="store_true" if arg_.default is False else "store_false")
                 if "type" in add_arg_kwargs:
                     del add_arg_kwargs["type"]
 
             # Set the help description
-            add_arg_kwargs |= dict(help=arg_description)
+            add_arg_kwargs.update(help=arg_description)
 
             # Run modifiers for this arg
             for modifier in arg_.modifiers:
                 modifier.modify_arg_dict(cmd, arg_, add_arg_kwargs)
 
             # Add the argument to the parser
             parser.add_argument(*arg_names, **add_arg_kwargs)
@@ -1341,15 +1348,15 @@
 
     def run(
         self,
         name: Optional[str] = None,
         call_ancestors: bool = False,
         auto_alias_cmds: bool = False,
         auto_alias_params: bool = False,
-        version_flag: Union[bool, tuple[str], tuple[str, str]] = False,
+        version_flag: Union[bool, Tuple[str], Tuple[str, str]] = False,
         show_defaults: bool = True,
         max_description_offset: int = 60,
         max_width: int = 120,
         command_metavar: str = "command",
         output: Optional[TextIO] = None,
     ) -> Any:
         """Set up the argument parser, parse argv, and run the appropriate command(s)"""
@@ -1371,15 +1378,15 @@
             description=description,
             formatter_class=self._formatter,
             **self._extra_argparser_options,
         )
         self._parsers["__root__"] = root_parser
 
         # Add version flags if necessary
-        argparse_version_flags: Union[tuple, tuple[str], tuple[str, str]] = tuple()
+        argparse_version_flags: Union[tuple, Tuple[str], Tuple[str, str]] = tuple()
         if self._options.version_flag:
             if not hasattr(__main__, "__version__"):
                 raise ArguablyException("__version__ must be defined if version_flag is set")
             if isinstance(self._options.version_flag, tuple):
                 argparse_version_flags = self._options.version_flag
             else:
                 argparse_version_flags = ("--version",)
@@ -1508,15 +1515,15 @@
     def _build_subtype(
         self, subtype_info: _SubtypeDecoratorInfo, type_spec: _BuildTypeSpec, parent_param_name: str
     ) -> Any:
         type_ = subtype_info.type_
         factory = subtype_info.factory or type_.__call__
         template = subtype_info.factory or type_.__init__  # type: ignore[misc]
         hints = get_type_hints(template, include_extras=True)
-        normalized_kwargs: dict[str, Any] = dict()
+        normalized_kwargs: Dict[str, Any] = dict()
 
         missing_required_keys = [
             _normalize_name(p)
             for p in inspect.signature(template).parameters
             if p not in type_spec.kwargs and p != "self"
         ]
         if len(missing_required_keys) > 0:
```

### Comparing `arguably-1.0.1/assets/PYPI_README.md` & `arguably-1.0.2/assets/PYPI_README.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,269 +10,312 @@
 00000090: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
 000000a0: 7465 7222 3e0a 2020 2020 3c65 6d3e 0a20  ter">.    <em>. 
 000000b0: 2020 2020 2020 2074 7572 6e73 2066 756e         turns fun
 000000c0: 6374 696f 6e73 2069 6e74 6f20 636f 6d6d  ctions into comm
 000000d0: 616e 6420 6c69 6e65 2069 6e74 6572 6661  and line interfa
 000000e0: 6365 730a 2020 2020 3c2f 656d 3e0a 3c2f  ces.    </em>.</
 000000f0: 703e 0a0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
-00000100: 6e74 6572 223e 0a20 2020 203c 212d 2d20  nter">.    <!-- 
-00000110: 544f 444f 2062 6164 6765 7320 2d2d 3e0a  TODO badges -->.
-00000120: 3c2f 703e 0a3c 6872 3e0a 0a60 6172 6775  </p>.<hr>..`argu
-00000130: 6162 6c79 6020 736f 6c76 6573 2074 6869  ably` solves thi
-00000140: 7320 7072 6f62 6c65 6d3a 0a31 2e20 596f  s problem:.1. Yo
-00000150: 7527 7665 2077 7269 7474 656e 2061 2050  u've written a P
-00000160: 7974 686f 6e20 7363 7269 7074 0a32 2e20  ython script.2. 
-00000170: 4e6f 7720 796f 7520 7761 6e74 2074 6f20  Now you want to 
-00000180: 7061 7373 2069 6e20 7061 7261 6d65 7465  pass in paramete
-00000190: 7273 2066 726f 6d20 7468 6520 636f 6d6d  rs from the comm
-000001a0: 616e 6420 6c69 6e65 0a33 2e20 596f 7520  and line.3. You 
-000001b0: 646f 6e27 7420 7761 6e74 2074 6f20 7265  don't want to re
-000001c0: 6164 2074 6865 2064 6f63 7320 666f 7220  ad the docs for 
-000001d0: 796f 7572 2066 6176 6f72 6974 6520 6172  your favorite ar
-000001e0: 6775 6d65 6e74 2070 6172 7369 6e67 206c  gument parsing l
-000001f0: 6962 7261 7279 202a 6167 6169 6e2a 0a0a  ibrary *again*..
-00000200: 4279 206c 6576 6572 6167 696e 6720 6173  By leveraging as
-00000210: 206d 616e 7920 5079 7468 6f6e 2069 6469   many Python idi
-00000220: 6f6d 7320 6173 2070 6f73 7369 626c 652c  oms as possible,
-00000230: 2060 6172 6775 6162 6c79 6020 6b65 6570   `arguably` keep
-00000240: 7320 6974 7320 4150 4920 736d 616c 6c20  s its API small 
-00000250: 616e 6420 6d65 6d6f 7261 626c 6520 7769  and memorable wi
-00000260: 7468 6f75 7420 7361 6372 6966 6963 696e  thout sacrificin
-00000270: 670a 6675 6e63 6974 6f6e 616c 6974 792e  g.funcitonality.
-00000280: 2060 6172 6775 6162 6c79 6020 7573 6573   `arguably` uses
-00000290: 2066 756e 6374 696f 6e73 2061 6e64 2074   functions and t
-000002a0: 6865 6972 2064 6f63 7374 7269 6e67 7320  heir docstrings 
-000002b0: 746f 2061 7574 6f6d 6174 6963 616c 6c79  to automatically
-000002c0: 2073 6574 2075 7020 6172 6770 6172 7365   set up argparse
-000002d0: 2e20 4e6f 7461 626c 792c 2060 6172 6775  . Notably, `argu
-000002e0: 6162 6c79 600a 6d61 7073 2079 6f75 7220  ably`.maps your 
-000002f0: 6675 6e63 7469 6f6e 2073 6967 6e61 7475  function signatu
-00000300: 7265 2074 6f20 6120 636f 6d6d 616e 642d  re to a command-
-00000310: 6c69 6e65 2069 6e74 6572 6661 6365 206c  line interface l
-00000320: 696b 6520 7468 6973 3a0a 0a60 6060 7079  ike this:..```py
-00000330: 7468 6f6e 0a40 6172 6775 6162 6c79 2e63  thon.@arguably.c
-00000340: 6f6d 6d61 6e64 0a64 6566 2073 6f6d 655f  ommand.def some_
-00000350: 6675 6e63 7469 6f6e 2872 6571 7569 7265  function(require
-00000360: 642c 206e 6f74 5f72 6571 7569 7265 643d  d, not_required=
-00000370: 2266 6f6f 222c 202a 6f74 6865 7273 2c20  "foo", *others, 
-00000380: 6f70 7469 6f6e 3d22 6261 7222 293a 0a20  option="bar"):. 
-00000390: 2020 202e 2e2e 0a60 6060 0a0a 3c70 2061     ....```..<p a
-000003a0: 6c69 676e 3d22 6365 6e74 6572 223e 3c62  lign="center"><b
-000003b0: 3e3c 656d 3e62 6563 6f6d 6573 3c2f 656d  ><em>becomes</em
-000003c0: 3e3c 2f62 3e3c 2f70 3e0a 0a60 6060 7465  ></b></p>..```te
-000003d0: 7874 0a75 7361 6765 3a20 7363 7269 7074  xt.usage: script
-000003e0: 205b 2d2d 6f70 7469 6f6e 204f 5054 494f   [--option OPTIO
-000003f0: 4e5d 2072 6571 7569 7265 6420 5b6e 6f74  N] required [not
-00000400: 2d72 6571 7569 7265 645d 205b 6f74 6865  -required] [othe
-00000410: 7273 202e 2e2e 5d0a 6060 600a 0a49 6e20  rs ...].```..In 
-00000420: 7368 6f72 742c 2060 6172 6775 6162 6c79  short, `arguably
-00000430: 6020 7475 726e 7320 796f 7572 2066 756e  ` turns your fun
-00000440: 6374 696f 6e27 7320 2a2a 706f 7369 7469  ction's **positi
-00000450: 6f6e 616c 2070 6172 616d 6574 6572 732a  onal parameters*
-00000460: 2a20 696e 746f 202a 2a70 6f73 6974 696f  * into **positio
-00000470: 6e61 6c20 636f 6d6d 616e 642d 6c69 6e65  nal command-line
-00000480: 2061 7267 756d 656e 7473 2a2a 2c20 616e   arguments**, an
-00000490: 640a 796f 7572 2066 756e 6374 696f 6e27  d.your function'
-000004a0: 7320 2a2a 6b65 7977 6f72 642d 6f6e 6c79  s **keyword-only
-000004b0: 2061 7267 756d 656e 7473 2a2a 2069 6e74   arguments** int
-000004c0: 6f20 2a2a 636f 6d6d 616e 642d 6c69 6e65  o **command-line
-000004d0: 206f 7074 696f 6e73 2a2a 2e20 4672 6f6d   options**. From
-000004e0: 2074 6865 2065 7861 6d70 6c65 2061 626f   the example abo
-000004f0: 7665 3a0a 0a7c 204e 616d 6520 2020 2020  ve:..| Name     
-00000500: 2020 2020 2020 7c20 5479 7065 2020 2020        | Type    
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 2020 2020 2020 2020 7c20 4265              | Be
-00000530: 636f 6d65 7320 2020 2020 2020 2020 2020  comes           
-00000540: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000550: 5573 6167 6520 2020 2020 2020 2020 2020  Usage           
-00000560: 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d      |.|---------
-00000570: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
-000005a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005d0: 2d2d 2d2d 2d7c 0a7c 2060 7265 7175 6972  -----|.| `requir
-000005e0: 6564 6020 2020 2020 7c20 706f 7369 7469  ed`     | positi
-000005f0: 6f6e 616c 2c20 6e6f 2064 6566 6175 6c74  onal, no default
-00000600: 2076 616c 7565 2020 2020 2020 2020 7c20   value        | 
-00000610: 7265 7175 6972 6564 2070 6f73 6974 696f  required positio
-00000620: 6e61 6c20 6172 6720 2020 2020 2020 2020  nal arg         
-00000630: 7c20 6072 6571 7569 7265 6460 2020 2020  | `required`    
-00000640: 2020 2020 2020 7c0a 7c20 606e 6f74 5f72        |.| `not_r
-00000650: 6571 7569 7265 6460 207c 2070 6f73 6974  equired` | posit
-00000660: 696f 6e61 6c2c 2077 6974 6820 6465 6661  ional, with defa
-00000670: 756c 7420 7661 6c75 6520 2020 2020 207c  ult value      |
-00000680: 206f 7074 696f 6e61 6c20 706f 7369 7469   optional positi
-00000690: 6f6e 616c 2061 7267 2020 2020 2020 2020  onal arg        
-000006a0: 207c 2060 5b6e 6f74 2d72 6571 7569 7265   | `[not-require
-000006b0: 645d 6020 2020 207c 0a7c 2060 6f74 6865  d]`    |.| `othe
-000006c0: 7273 6020 2020 2020 2020 7c20 706f 7369  rs`       | posi
-000006d0: 7469 6f6e 616c 2c20 7661 7269 6164 6963  tional, variadic
-000006e0: 2028 6c69 6b65 2060 2a61 7267 7360 2920   (like `*args`) 
-000006f0: 7c20 7468 6520 7265 7374 206f 6620 7468  | the rest of th
-00000700: 6520 706f 7369 7469 6f6e 616c 2061 7267  e positional arg
-00000710: 7320 7c20 605b 6f74 6865 7273 202e 2e2e  s | `[others ...
-00000720: 5d60 2020 2020 2020 7c0a 7c20 606f 7074  ]`      |.| `opt
-00000730: 696f 6e60 2020 2020 2020 207c 206b 6579  ion`       | key
-00000740: 776f 7264 2d6f 6e6c 7920 6172 6775 6d65  word-only argume
-00000750: 6e74 2020 2020 2020 2020 2020 2020 2020  nt              
-00000760: 207c 2061 6e20 6f70 7469 6f6e 2020 2020   | an option    
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 2020 207c 2060 5b2d 2d6f 7074 696f 6e20     | `[--option 
-00000790: 4f50 5449 4f4e 5d60 207c 0a0a 6061 7267  OPTION]` |..`arg
-000007a0: 7561 626c 7960 2061 6c73 6f20 656e 6162  uably` also enab
-000007b0: 6c65 7320 796f 7520 746f 2065 6173 696c  les you to easil
-000007c0: 7920 6164 6420 7375 6263 6f6d 6d61 6e64  y add subcommand
-000007d0: 7320 2d20 6a75 7374 2061 6e6e 6f74 6174  s - just annotat
-000007e0: 6520 6d6f 7265 2074 6861 6e20 6f6e 6520  e more than one 
-000007f0: 6675 6e63 7469 6f6e 2077 6974 6820 6040  function with `@
-00000800: 6172 6775 6162 6c79 2e63 6f6d 6d61 6e64  arguably.command
-00000810: 602e 0a59 6f75 2063 616e 2065 7665 6e20  `..You can even 
-00000820: 6861 7665 206e 6573 7465 6420 7375 6263  have nested subc
-00000830: 6f6d 6d61 6e64 7320 286d 6f72 6520 6f6e  ommands (more on
-00000840: 2074 6861 7420 6c61 7465 7229 2e0a 0a60   that later)...`
-00000850: 6172 6775 6162 6c79 6020 7265 6164 7320  arguably` reads 
-00000860: 7479 7065 2061 6e6e 6f74 6174 696f 6e73  type annotations
-00000870: 2061 6e64 2061 7574 6f6d 6174 6963 616c   and automatical
-00000880: 6c79 2063 6f6e 7665 7274 7320 6172 6775  ly converts argu
-00000890: 6d65 6e74 7320 746f 2074 6865 2064 6563  ments to the dec
-000008a0: 6c61 7265 6420 7479 7065 732e 2049 7420  lared types. It 
-000008b0: 6861 7320 736d 6172 7420 6861 6e64 6c69  has smart handli
-000008c0: 6e67 2066 6f72 0a60 7475 706c 6560 2c20  ng for.`tuple`, 
-000008d0: 606c 6973 7460 2c20 6065 6e75 6d2e 456e  `list`, `enum.En
-000008e0: 756d 602c 2061 6e64 2060 656e 756d 2e46  um`, and `enum.F
-000008f0: 6c61 6760 2e20 5468 6572 6520 6172 6520  lag`. There are 
-00000900: 616c 736f 2061 2066 6577 2073 7065 6369  also a few speci
-00000910: 616c 2062 6568 6176 696f 7273 2079 6f75  al behaviors you
-00000920: 2063 616e 2061 7474 6163 6820 746f 2061   can attach to a
-00000930: 2070 6172 616d 6574 6572 0a76 6961 2060   parameter.via `
-00000940: 416e 6e6f 7461 7465 645b 5d60 2061 6e64  Annotated[]` and
-00000950: 2074 6865 2060 6172 6775 6162 6c79 2e61   the `arguably.a
-00000960: 7267 2e2a 6020 6675 6e63 7469 6f6e 732e  rg.*` functions.
-00000970: 0a0a 6061 7267 7561 626c 7960 2070 6172  ..`arguably` par
-00000980: 7365 7320 646f 6373 7472 696e 6773 2074  ses docstrings t
-00000990: 6f20 6765 6e65 7261 7465 2064 6573 6372  o generate descr
-000009a0: 6970 7469 6f6e 7320 666f 7220 796f 7572  iptions for your
-000009b0: 2063 6f6d 6d61 6e64 7320 616e 6420 7061   commands and pa
-000009c0: 7261 6d65 7465 7273 2e20 4966 2079 6f75  rameters. If you
-000009d0: 2077 616e 7420 746f 2067 6976 6520 6120   want to give a 
-000009e0: 7061 7261 6d65 7465 720a 7468 6520 616c  parameter.the al
-000009f0: 6961 7320 602d 5860 2c20 7072 6566 6978  ias `-X`, prefix
-00000a00: 2069 7473 2064 6f63 7374 7269 6e67 2064   its docstring d
-00000a10: 6573 6372 6970 7469 6f6e 2077 6974 6820  escription with 
-00000a20: 605b 2d58 5d60 2e20 5772 6170 7069 6e67  `[-X]`. Wrapping
-00000a30: 2061 2077 6f72 6420 696e 2060 7b7d 6020   a word in `{}` 
-00000a40: 6368 616e 6765 7320 7468 6520 2a6d 6574  changes the *met
-00000a50: 6176 6172 2a20 7468 6174 2067 6574 730a  avar* that gets.
-00000a60: 7072 696e 7465 6420 2874 6869 7320 6973  printed (this is
-00000a70: 2077 6861 7427 7320 7368 6f77 6e20 696e   what's shown in
-00000a80: 2074 6865 2075 7361 6765 2073 7472 696e   the usage strin
-00000a90: 6720 6166 7465 7220 616e 206f 7074 696f  g after an optio
-00000aa0: 6e20 6e61 6d65 2c20 646f 6e27 7420 776f  n name, don't wo
-00000ab0: 7272 7920 6966 2079 6f75 2061 7265 6e27  rry if you aren'
-00000ac0: 7420 6661 6d69 6c69 6172 2077 6974 6820  t familiar with 
-00000ad0: 7468 6973 292e 0a46 6f72 2065 7861 6d70  this)..For examp
-00000ae0: 6c65 3a0a 0a60 6060 7079 7468 6f6e 0a23  le:..```python.#
-00000af0: 212f 7573 722f 6269 6e2f 656e 7620 7079  !/usr/bin/env py
-00000b00: 7468 6f6e 330a 2222 2264 6f63 7374 7269  thon3."""docstri
-00000b10: 6e67 7320 666f 7220 7468 6520 6669 6c65  ngs for the file
-00000b20: 2062 6563 6f6d 6520 7468 6520 6465 7363   become the desc
-00000b30: 7269 7074 696f 6e20 666f 7220 7468 6520  ription for the 
-00000b40: 7363 7269 7074 2e22 2222 0a5f 5f76 6572  script.""".__ver
-00000b50: 7369 6f6e 5f5f 203d 2022 312e 302e 3022  sion__ = "1.0.0"
-00000b60: 2020 2320 596f 7520 6361 6e20 616c 736f    # You can also
-00000b70: 2073 6574 2060 7665 7273 696f 6e5f 666c   set `version_fl
-00000b80: 6167 3d54 7275 6560 2074 6f20 6164 6420  ag=True` to add 
-00000b90: 6120 7665 7273 696f 6e20 666c 6167 2c20  a version flag, 
-00000ba0: 6974 2077 696c 6c20 7265 6164 2060 5f5f  it will read `__
-00000bb0: 7665 7273 696f 6e5f 5f60 0a0a 696d 706f  version__`..impo
-00000bc0: 7274 2061 7267 7561 626c 790a 0a40 6172  rt arguably..@ar
-00000bd0: 6775 6162 6c79 2e63 6f6d 6d61 6e64 2861  guably.command(a
-00000be0: 6c69 6173 3d22 6822 290a 6465 6620 6865  lias="h").def he
-00000bf0: 6c6c 6f28 6e61 6d65 3a20 7374 722c 202a  llo(name: str, *
-00000c00: 2c20 6c61 7374 6e61 6d65 3a20 7374 7220  , lastname: str 
-00000c10: 7c20 4e6f 6e65 203d 204e 6f6e 6529 3a0a  | None = None):.
-00000c20: 2020 2020 2222 220a 2020 2020 7361 7973      """.    says
-00000c30: 2068 656c 6c6f 2074 6f20 796f 750a 2020   hello to you.  
-00000c40: 2020 3a70 6172 616d 206e 616d 653a 2079    :param name: y
-00000c50: 6f75 7220 6e61 6d65 0a20 2020 203a 7061  our name.    :pa
-00000c60: 7261 6d20 6c61 7374 6e61 6d65 3a20 5b2d  ram lastname: [-
-00000c70: 6c5d 2079 6f75 7220 7b73 7572 6e61 6d65  l] your {surname
-00000c80: 7d0a 2020 2020 2222 220a 2020 2020 6675  }.    """.    fu
-00000c90: 6c6c 5f6e 616d 6520 3d20 6e61 6d65 2069  ll_name = name i
-00000ca0: 6620 6c61 7374 6e61 6d65 2069 7320 4e6f  f lastname is No
-00000cb0: 6e65 2065 6c73 6520 6622 7b6e 616d 657d  ne else f"{name}
-00000cc0: 207b 6c61 7374 6e61 6d65 7d22 0a20 2020   {lastname}".   
-00000cd0: 2070 7269 6e74 2866 2248 656c 6c6f 2c20   print(f"Hello, 
-00000ce0: 7b66 756c 6c5f 6e61 6d65 7d21 2229 0a0a  {full_name}!")..
-00000cf0: 4061 7267 7561 626c 792e 636f 6d6d 616e  @arguably.comman
-00000d00: 6428 616c 6961 733d 2267 2229 0a64 6566  d(alias="g").def
-00000d10: 2067 6f6f 6462 7965 286e 616d 653a 2073   goodbye(name: s
-00000d20: 7472 2c20 2a2c 2069 735f 7361 643a 2062  tr, *, is_sad: b
-00000d30: 6f6f 6c20 3d20 4661 6c73 6529 3a0a 2020  ool = False):.  
-00000d40: 2020 2222 220a 2020 2020 7361 7973 2067    """.    says g
-00000d50: 6f6f 6462 7965 2074 6f20 796f 750a 2020  oodbye to you.  
-00000d60: 2020 3a70 6172 616d 206e 616d 653a 2079    :param name: y
-00000d70: 6f75 7220 6e61 6d65 0a20 2020 203a 7061  our name.    :pa
-00000d80: 7261 6d20 6973 5f73 6164 3a20 5b2d 735d  ram is_sad: [-s]
-00000d90: 2077 6865 7468 6572 206f 7220 6e6f 7420   whether or not 
-00000da0: 6974 2773 2073 6164 2074 6f20 7365 6520  it's sad to see 
-00000db0: 796f 7520 676f 0a20 2020 2022 2222 0a20  you go.    """. 
-00000dc0: 2020 2070 7269 6e74 2866 2247 6f6f 6462     print(f"Goodb
-00000dd0: 7965 2c20 7b6e 616d 657d 2122 290a 2020  ye, {name}!").  
-00000de0: 2020 6966 2069 735f 7361 643a 0a20 2020    if is_sad:.   
-00000df0: 2020 2020 2070 7269 6e74 2866 2249 7427       print(f"It'
-00000e00: 7320 7361 6420 746f 2073 6565 2079 6f75  s sad to see you
-00000e10: 2067 6f21 2229 0a0a 6966 205f 5f6e 616d   go!")..if __nam
-00000e20: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-00000e30: 223a 0a20 2020 2061 7267 7561 626c 792e  ":.    arguably.
-00000e40: 7275 6e28 7665 7273 696f 6e5f 666c 6167  run(version_flag
-00000e50: 3d54 7275 6529 0a60 6060 0a0a 3c70 2061  =True).```..<p a
-00000e60: 6c69 676e 3d22 6365 6e74 6572 223e 3c62  lign="center"><b
-00000e70: 3e3c 656d 3e62 6563 6f6d 6573 3c2f 656d  ><em>becomes</em
-00000e80: 3e3c 2f62 3e3c 2f70 3e0a 0a60 6060 636f  ></b></p>..```co
-00000e90: 6e73 6f6c 650a 7573 6572 406d 6163 6869  nsole.user@machi
-00000ea0: 6e65 3a7e 2420 7079 7468 6f6e 3320 7363  ne:~$ python3 sc
-00000eb0: 7269 7074 2e70 790a 7573 6167 653a 2074  ript.py.usage: t
-00000ec0: 6573 745f 7363 7269 7074 732e 646f 6373  est_scripts.docs
-00000ed0: 3220 5b2d 685d 205b 2d2d 7665 7273 696f  2 [-h] [--versio
-00000ee0: 6e5d 2063 6f6d 6d61 6e64 202e 2e2e 0a0a  n] command .....
-00000ef0: 646f 6373 7472 696e 6773 2066 6f72 2074  docstrings for t
-00000f00: 6865 2066 696c 6520 6265 636f 6d65 2074  he file become t
-00000f10: 6865 2064 6573 6372 6970 7469 6f6e 2066  he description f
-00000f20: 6f72 2074 6865 2073 6372 6970 742e 0a0a  or the script...
-00000f30: 706f 7369 7469 6f6e 616c 2061 7267 756d  positional argum
-00000f40: 656e 7473 3a0a 2020 636f 6d6d 616e 640a  ents:.  command.
-00000f50: 2020 2020 6865 6c6c 6f20 2868 2920 2020      hello (h)   
-00000f60: 2073 6179 7320 6865 6c6c 6f20 746f 2079   says hello to y
-00000f70: 6f75 0a20 2020 2067 6f6f 6462 7965 2028  ou.    goodbye (
-00000f80: 6729 2020 7361 7973 2067 6f6f 6462 7965  g)  says goodbye
-00000f90: 2074 6f20 796f 750a 0a6f 7074 696f 6e73   to you..options
-00000fa0: 3a0a 2020 2d68 2c20 2d2d 6865 6c70 2020  :.  -h, --help  
-00000fb0: 2020 2073 686f 7720 7468 6973 2068 656c     show this hel
-00000fc0: 7020 6d65 7373 6167 6520 616e 6420 6578  p message and ex
-00000fd0: 6974 0a20 202d 2d76 6572 7369 6f6e 2020  it.  --version  
-00000fe0: 2020 2020 7368 6f77 2070 726f 6772 616d      show program
-00000ff0: 2773 2076 6572 7369 6f6e 206e 756d 6265  's version numbe
-00001000: 7220 616e 6420 6578 6974 0a0a 0a75 7365  r and exit...use
-00001010: 7240 6d61 6368 696e 653a 7e24 2070 7974  r@machine:~$ pyt
-00001020: 686f 6e33 2073 6372 6970 742e 7079 2068  hon3 script.py h
-00001030: 656c 6c6f 202d 2d68 656c 700a 7573 6167  ello --help.usag
-00001040: 653a 2074 6573 745f 7363 7269 7074 732e  e: test_scripts.
-00001050: 646f 6373 3220 6865 6c6c 6f20 5b2d 685d  docs2 hello [-h]
-00001060: 205b 2d6c 2053 5552 4e41 4d45 5d20 6e61   [-l SURNAME] na
-00001070: 6d65 0a0a 7361 7973 2068 656c 6c6f 2074  me..says hello t
-00001080: 6f20 796f 750a 0a70 6f73 6974 696f 6e61  o you..positiona
-00001090: 6c20 6172 6775 6d65 6e74 733a 0a20 206e  l arguments:.  n
-000010a0: 616d 6520 2020 2020 2020 2020 2020 2020  ame             
-000010b0: 2020 2020 2020 2079 6f75 7220 6e61 6d65         your name
-000010c0: 0a0a 6f70 7469 6f6e 733a 0a20 202d 682c  ..options:.  -h,
-000010d0: 202d 2d68 656c 7020 2020 2020 2020 2020   --help         
-000010e0: 2020 2020 2073 686f 7720 7468 6973 2068       show this h
-000010f0: 656c 7020 6d65 7373 6167 6520 616e 6420  elp message and 
-00001100: 6578 6974 0a20 202d 6c2c 202d 2d6c 6173  exit.  -l, --las
-00001110: 746e 616d 6520 5355 524e 414d 4520 2079  tname SURNAME  y
-00001120: 6f75 7220 7375 726e 616d 6520 2864 6566  our surname (def
-00001130: 6175 6c74 3a20 4e6f 6e65 290a 6060 600a  ault: None).```.
-00001140: 0a4d 6f72 6520 646f 6373 2063 6f6d 696e  .More docs comin
-00001150: 6720 736f 6f6e 2e2e 2e0a                 g soon....
+00000100: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000110: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000120: 7562 2e63 6f6d 2f74 7265 796b 656f 776e  ub.com/treykeown
+00000130: 2f61 7267 7561 626c 792f 6163 7469 6f6e  /arguably/action
+00000140: 732f 776f 726b 666c 6f77 732f 7079 7468  s/workflows/pyth
+00000150: 6f6e 2d70 6163 6b61 6765 2e79 6d6c 223e  on-package.yml">
+00000160: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f74 7265  //github.com/tre
+00000180: 796b 656f 776e 2f61 7267 7561 626c 792f  ykeown/arguably/
+00000190: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000001a0: 732f 7079 7468 6f6e 2d70 6163 6b61 6765  s/python-package
+000001b0: 2e79 6d6c 2f62 6164 6765 2e73 7667 2220  .yml/badge.svg" 
+000001c0: 616c 743d 2254 6573 7420 7374 6174 7573  alt="Test status
+000001d0: 223e 3c2f 613e 0a20 2020 203c 6120 6872  "></a>.    <a hr
+000001e0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000001f0: 7562 2e63 6f6d 2f74 7265 796b 656f 776e  ub.com/treykeown
+00000200: 2f61 7267 7561 626c 792f 7472 6565 2f6d  /arguably/tree/m
+00000210: 6169 6e2f 7465 7374 223e 3c69 6d67 2073  ain/test"><img s
+00000220: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000230: 7368 6965 6c64 732e 696f 2f65 6e64 706f  shields.io/endpo
+00000240: 696e 743f 7572 6c3d 6874 7470 733a 2f2f  int?url=https://
+00000250: 6769 7374 2e67 6974 6875 6275 7365 7263  gist.githubuserc
+00000260: 6f6e 7465 6e74 2e63 6f6d 2f74 7265 796b  ontent.com/treyk
+00000270: 656f 776e 2f66 3439 3362 3134 3238 3861  eown/f493b14288a
+00000280: 6634 6538 3335 3865 6138 3537 3863 3339  f4e8358ea8578c39
+00000290: 3332 3133 612f 7261 772f 6172 6775 6162  3213a/raw/arguab
+000002a0: 6c79 2d63 6f76 6572 6167 652d 6261 6467  ly-coverage-badg
+000002b0: 652e 6a73 6f6e 2220 616c 743d 2243 6f64  e.json" alt="Cod
+000002c0: 6520 636f 7665 7261 6765 223e 3c2f 613e  e coverage"></a>
+000002d0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000002e0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000002f0: 726f 6a65 6374 2f61 7267 7561 626c 792f  roject/arguably/
+00000300: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000310: 733a 2f2f 7368 6965 6c64 732e 696f 2f70  s://shields.io/p
+00000320: 7970 692f 7079 7665 7273 696f 6e73 2f61  ypi/pyversions/a
+00000330: 7267 7561 626c 7922 2061 6c74 3d22 5375  rguably" alt="Su
+00000340: 7070 6f72 7465 6420 5079 7468 6f6e 2076  pported Python v
+00000350: 6572 7369 6f6e 7322 3e3c 2f61 3e0a 2020  ersions"></a>.  
+00000360: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000370: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000380: 6563 742f 6172 6775 6162 6c79 2f22 3e3c  ect/arguably/"><
+00000390: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000003a0: 2f73 6869 656c 6473 2e69 6f2f 7079 7069  /shields.io/pypi
+000003b0: 2f76 2f61 7267 7561 626c 7922 2061 6c74  /v/arguably" alt
+000003c0: 3d22 5079 5049 2076 6572 7369 6f6e 223e  ="PyPI version">
+000003d0: 3c2f 613e 0a3c 2f70 3e0a 3c68 723e 0a0a  </a>.</p>.<hr>..
+000003e0: 6061 7267 7561 626c 7960 2073 6f6c 7665  `arguably` solve
+000003f0: 7320 7468 6973 2070 726f 626c 656d 3a0a  s this problem:.
+00000400: 312e 2059 6f75 2776 6520 7772 6974 7465  1. You've writte
+00000410: 6e20 6120 5079 7468 6f6e 2073 6372 6970  n a Python scrip
+00000420: 740a 322e 204e 6f77 2079 6f75 2077 616e  t.2. Now you wan
+00000430: 7420 746f 2070 6173 7320 696e 2070 6172  t to pass in par
+00000440: 616d 6574 6572 7320 6672 6f6d 2074 6865  ameters from the
+00000450: 2063 6f6d 6d61 6e64 206c 696e 650a 332e   command line.3.
+00000460: 2059 6f75 2064 6f6e 2774 2077 616e 7420   You don't want 
+00000470: 746f 2072 6561 6420 7468 6520 646f 6373  to read the docs
+00000480: 2066 6f72 2079 6f75 7220 6661 766f 7269   for your favori
+00000490: 7465 2061 7267 756d 656e 7420 7061 7273  te argument pars
+000004a0: 696e 6720 6c69 6272 6172 7920 2a61 6761  ing library *aga
+000004b0: 696e 2a0a 0a42 7920 6c65 7665 7261 6769  in*..By leveragi
+000004c0: 6e67 2061 7320 6d61 6e79 2050 7974 686f  ng as many Pytho
+000004d0: 6e20 6964 696f 6d73 2061 7320 706f 7373  n idioms as poss
+000004e0: 6962 6c65 2c20 6061 7267 7561 626c 7960  ible, `arguably`
+000004f0: 206b 6565 7073 2069 7473 2041 5049 2073   keeps its API s
+00000500: 6d61 6c6c 2061 6e64 206d 656d 6f72 6162  mall and memorab
+00000510: 6c65 2077 6974 686f 7574 2073 6163 7269  le without sacri
+00000520: 6669 6369 6e67 0a66 756e 6369 746f 6e61  ficing.funcitona
+00000530: 6c69 7479 2e20 6061 7267 7561 626c 7960  lity. `arguably`
+00000540: 2075 7365 7320 6675 6e63 7469 6f6e 7320   uses functions 
+00000550: 616e 6420 7468 6569 7220 646f 6373 7472  and their docstr
+00000560: 696e 6773 2074 6f20 6175 746f 6d61 7469  ings to automati
+00000570: 6361 6c6c 7920 7365 7420 7570 2061 7267  cally set up arg
+00000580: 7061 7273 652e 204e 6f74 6162 6c79 2c20  parse. Notably, 
+00000590: 6061 7267 7561 626c 7960 0a6d 6170 7320  `arguably`.maps 
+000005a0: 796f 7572 2066 756e 6374 696f 6e20 7369  your function si
+000005b0: 676e 6174 7572 6520 746f 2061 2063 6f6d  gnature to a com
+000005c0: 6d61 6e64 2d6c 696e 6520 696e 7465 7266  mand-line interf
+000005d0: 6163 6520 6c69 6b65 2074 6869 733a 0a0a  ace like this:..
+000005e0: 6060 6070 7974 686f 6e0a 4061 7267 7561  ```python.@argua
+000005f0: 626c 792e 636f 6d6d 616e 640a 6465 6620  bly.command.def 
+00000600: 736f 6d65 5f66 756e 6374 696f 6e28 7265  some_function(re
+00000610: 7175 6972 6564 2c20 6e6f 745f 7265 7175  quired, not_requ
+00000620: 6972 6564 3d22 666f 6f22 2c20 2a6f 7468  ired="foo", *oth
+00000630: 6572 732c 206f 7074 696f 6e3d 2262 6172  ers, option="bar
+00000640: 2229 3a0a 2020 2020 2e2e 2e0a 6060 600a  "):.    ....```.
+00000650: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000660: 7222 3e3c 623e 3c65 6d3e 6265 636f 6d65  r"><b><em>become
+00000670: 733c 2f65 6d3e 3c2f 623e 3c2f 703e 0a0a  s</em></b></p>..
+00000680: 6060 6074 6578 740a 7573 6167 653a 2073  ```text.usage: s
+00000690: 6372 6970 7420 5b2d 2d6f 7074 696f 6e20  cript [--option 
+000006a0: 4f50 5449 4f4e 5d20 7265 7175 6972 6564  OPTION] required
+000006b0: 205b 6e6f 742d 7265 7175 6972 6564 5d20   [not-required] 
+000006c0: 5b6f 7468 6572 7320 2e2e 2e5d 0a60 6060  [others ...].```
+000006d0: 0a0a 496e 2073 686f 7274 2c20 6061 7267  ..In short, `arg
+000006e0: 7561 626c 7960 2074 7572 6e73 2079 6f75  uably` turns you
+000006f0: 7220 6675 6e63 7469 6f6e 2773 202a 2a70  r function's **p
+00000700: 6f73 6974 696f 6e61 6c20 7061 7261 6d65  ositional parame
+00000710: 7465 7273 2a2a 2069 6e74 6f20 2a2a 706f  ters** into **po
+00000720: 7369 7469 6f6e 616c 2063 6f6d 6d61 6e64  sitional command
+00000730: 2d6c 696e 6520 6172 6775 6d65 6e74 732a  -line arguments*
+00000740: 2a2c 2061 6e64 0a79 6f75 7220 6675 6e63  *, and.your func
+00000750: 7469 6f6e 2773 202a 2a6b 6579 776f 7264  tion's **keyword
+00000760: 2d6f 6e6c 7920 6172 6775 6d65 6e74 732a  -only arguments*
+00000770: 2a20 696e 746f 202a 2a63 6f6d 6d61 6e64  * into **command
+00000780: 2d6c 696e 6520 6f70 7469 6f6e 732a 2a2e  -line options**.
+00000790: 2046 726f 6d20 7468 6520 6578 616d 706c   From the exampl
+000007a0: 6520 6162 6f76 653a 0a0a 7c20 4e61 6d65  e above:..| Name
+000007b0: 2020 2020 2020 2020 2020 207c 2054 7970             | Typ
+000007c0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007e0: 207c 2042 6563 6f6d 6573 2020 2020 2020   | Becomes      
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 207c 2055 7361 6765 2020 2020 2020     | Usage      
+00000810: 2020 2020 2020 2020 207c 0a7c 2d2d 2d2d           |.|----
+00000820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00000830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000850: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|-------------
+00000860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000870: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 6072  ----------|.| `r
+00000890: 6571 7569 7265 6460 2020 2020 207c 2070  equired`     | p
+000008a0: 6f73 6974 696f 6e61 6c2c 206e 6f20 6465  ositional, no de
+000008b0: 6661 756c 7420 7661 6c75 6520 2020 2020  fault value     
+000008c0: 2020 207c 2072 6571 7569 7265 6420 706f     | required po
+000008d0: 7369 7469 6f6e 616c 2061 7267 2020 2020  sitional arg    
+000008e0: 2020 2020 207c 2060 7265 7175 6972 6564       | `required
+000008f0: 6020 2020 2020 2020 2020 207c 0a7c 2060  `          |.| `
+00000900: 6e6f 745f 7265 7175 6972 6564 6020 7c20  not_required` | 
+00000910: 706f 7369 7469 6f6e 616c 2c20 7769 7468  positional, with
+00000920: 2064 6566 6175 6c74 2076 616c 7565 2020   default value  
+00000930: 2020 2020 7c20 6f70 7469 6f6e 616c 2070      | optional p
+00000940: 6f73 6974 696f 6e61 6c20 6172 6720 2020  ositional arg   
+00000950: 2020 2020 2020 7c20 605b 6e6f 742d 7265        | `[not-re
+00000960: 7175 6972 6564 5d60 2020 2020 7c0a 7c20  quired]`    |.| 
+00000970: 606f 7468 6572 7360 2020 2020 2020 207c  `others`       |
+00000980: 2070 6f73 6974 696f 6e61 6c2c 2076 6172   positional, var
+00000990: 6961 6469 6320 286c 696b 6520 602a 6172  iadic (like `*ar
+000009a0: 6773 6029 207c 2074 6865 2072 6573 7420  gs`) | the rest 
+000009b0: 6f66 2074 6865 2070 6f73 6974 696f 6e61  of the positiona
+000009c0: 6c20 6172 6773 207c 2060 5b6f 7468 6572  l args | `[other
+000009d0: 7320 2e2e 2e5d 6020 2020 2020 207c 0a7c  s ...]`      |.|
+000009e0: 2060 6f70 7469 6f6e 6020 2020 2020 2020   `option`       
+000009f0: 7c20 6b65 7977 6f72 642d 6f6e 6c79 2061  | keyword-only a
+00000a00: 7267 756d 656e 7420 2020 2020 2020 2020  rgument         
+00000a10: 2020 2020 2020 7c20 616e 206f 7074 696f        | an optio
+00000a20: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00000a30: 2020 2020 2020 2020 7c20 605b 2d2d 6f70          | `[--op
+00000a40: 7469 6f6e 204f 5054 494f 4e5d 6020 7c0a  tion OPTION]` |.
+00000a50: 0a60 6172 6775 6162 6c79 6020 616c 736f  .`arguably` also
+00000a60: 2065 6e61 626c 6573 2079 6f75 2074 6f20   enables you to 
+00000a70: 6561 7369 6c79 2061 6464 2073 7562 636f  easily add subco
+00000a80: 6d6d 616e 6473 202d 206a 7573 7420 616e  mmands - just an
+00000a90: 6e6f 7461 7465 206d 6f72 6520 7468 616e  notate more than
+00000aa0: 206f 6e65 2066 756e 6374 696f 6e20 7769   one function wi
+00000ab0: 7468 2060 4061 7267 7561 626c 792e 636f  th `@arguably.co
+00000ac0: 6d6d 616e 6460 2e0a 596f 7520 6361 6e20  mmand`..You can 
+00000ad0: 6576 656e 2068 6176 6520 6e65 7374 6564  even have nested
+00000ae0: 2073 7562 636f 6d6d 616e 6473 2028 6d6f   subcommands (mo
+00000af0: 7265 206f 6e20 7468 6174 206c 6174 6572  re on that later
+00000b00: 292e 0a0a 6061 7267 7561 626c 7960 2072  )...`arguably` r
+00000b10: 6561 6473 2074 7970 6520 616e 6e6f 7461  eads type annota
+00000b20: 7469 6f6e 7320 616e 6420 6175 746f 6d61  tions and automa
+00000b30: 7469 6361 6c6c 7920 636f 6e76 6572 7473  tically converts
+00000b40: 2061 7267 756d 656e 7473 2074 6f20 7468   arguments to th
+00000b50: 6520 6465 636c 6172 6564 2074 7970 6573  e declared types
+00000b60: 2e20 4974 2068 6173 2073 6d61 7274 2068  . It has smart h
+00000b70: 616e 646c 696e 6720 666f 720a 6074 7570  andling for.`tup
+00000b80: 6c65 602c 2060 6c69 7374 602c 2060 656e  le`, `list`, `en
+00000b90: 756d 2e45 6e75 6d60 2c20 616e 6420 6065  um.Enum`, and `e
+00000ba0: 6e75 6d2e 466c 6167 602e 2054 6865 7265  num.Flag`. There
+00000bb0: 2061 7265 2061 6c73 6f20 6120 6665 7720   are also a few 
+00000bc0: 7370 6563 6961 6c20 6265 6861 7669 6f72  special behavior
+00000bd0: 7320 796f 7520 6361 6e20 6174 7461 6368  s you can attach
+00000be0: 2074 6f20 6120 7061 7261 6d65 7465 720a   to a parameter.
+00000bf0: 7669 6120 6041 6e6e 6f74 6174 6564 5b5d  via `Annotated[]
+00000c00: 6020 616e 6420 7468 6520 6061 7267 7561  ` and the `argua
+00000c10: 626c 792e 6172 672e 2a60 2066 756e 6374  bly.arg.*` funct
+00000c20: 696f 6e73 2e0a 0a60 6172 6775 6162 6c79  ions...`arguably
+00000c30: 6020 7061 7273 6573 2064 6f63 7374 7269  ` parses docstri
+00000c40: 6e67 7320 746f 2067 656e 6572 6174 6520  ngs to generate 
+00000c50: 6465 7363 7269 7074 696f 6e73 2066 6f72  descriptions for
+00000c60: 2079 6f75 7220 636f 6d6d 616e 6473 2061   your commands a
+00000c70: 6e64 2070 6172 616d 6574 6572 732e 2049  nd parameters. I
+00000c80: 6620 796f 7520 7761 6e74 2074 6f20 6769  f you want to gi
+00000c90: 7665 2061 2070 6172 616d 6574 6572 0a74  ve a parameter.t
+00000ca0: 6865 2061 6c69 6173 2060 2d58 602c 2070  he alias `-X`, p
+00000cb0: 7265 6669 7820 6974 7320 646f 6373 7472  refix its docstr
+00000cc0: 696e 6720 6465 7363 7269 7074 696f 6e20  ing description 
+00000cd0: 7769 7468 2060 5b2d 585d 602e 2057 7261  with `[-X]`. Wra
+00000ce0: 7070 696e 6720 6120 776f 7264 2069 6e20  pping a word in 
+00000cf0: 607b 7d60 2063 6861 6e67 6573 2074 6865  `{}` changes the
+00000d00: 202a 6d65 7461 7661 722a 2074 6861 7420   *metavar* that 
+00000d10: 6765 7473 0a70 7269 6e74 6564 2028 7468  gets.printed (th
+00000d20: 6973 2069 7320 7768 6174 2773 2073 686f  is is what's sho
+00000d30: 776e 2069 6e20 7468 6520 7573 6167 6520  wn in the usage 
+00000d40: 7374 7269 6e67 2061 6674 6572 2061 6e20  string after an 
+00000d50: 6f70 7469 6f6e 206e 616d 652c 2064 6f6e  option name, don
+00000d60: 2774 2077 6f72 7279 2069 6620 796f 7520  't worry if you 
+00000d70: 6172 656e 2774 2066 616d 696c 6961 7220  aren't familiar 
+00000d80: 7769 7468 2074 6869 7329 2e0a 466f 7220  with this)..For 
+00000d90: 6578 616d 706c 653a 0a0a 6060 6070 7974  example:..```pyt
+00000da0: 686f 6e0a 2321 2f75 7372 2f62 696e 2f65  hon.#!/usr/bin/e
+00000db0: 6e76 2070 7974 686f 6e33 0a22 2222 646f  nv python3."""do
+00000dc0: 6373 7472 696e 6773 2066 6f72 2074 6865  cstrings for the
+00000dd0: 2066 696c 6520 6265 636f 6d65 2074 6865   file become the
+00000de0: 2064 6573 6372 6970 7469 6f6e 2066 6f72   description for
+00000df0: 2074 6865 2073 6372 6970 742e 2222 220a   the script.""".
+00000e00: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2231  __version__ = "1
+00000e10: 2e30 2e30 2220 2023 2059 6f75 2063 616e  .0.0"  # You can
+00000e20: 2061 6c73 6f20 7365 7420 6076 6572 7369   also set `versi
+00000e30: 6f6e 5f66 6c61 673d 5472 7565 6020 746f  on_flag=True` to
+00000e40: 2061 6464 2061 2076 6572 7369 6f6e 2066   add a version f
+00000e50: 6c61 672c 2069 7420 7769 6c6c 2072 6561  lag, it will rea
+00000e60: 6420 605f 5f76 6572 7369 6f6e 5f5f 600a  d `__version__`.
+00000e70: 0a69 6d70 6f72 7420 6172 6775 6162 6c79  .import arguably
+00000e80: 0a0a 4061 7267 7561 626c 792e 636f 6d6d  ..@arguably.comm
+00000e90: 616e 6428 616c 6961 733d 2268 2229 0a64  and(alias="h").d
+00000ea0: 6566 2068 656c 6c6f 286e 616d 653a 2073  ef hello(name: s
+00000eb0: 7472 2c20 2a2c 206c 6173 746e 616d 653a  tr, *, lastname:
+00000ec0: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
+00000ed0: 6e65 293a 0a20 2020 2022 2222 0a20 2020  ne):.    """.   
+00000ee0: 2073 6179 7320 6865 6c6c 6f20 746f 2079   says hello to y
+00000ef0: 6f75 0a20 2020 203a 7061 7261 6d20 6e61  ou.    :param na
+00000f00: 6d65 3a20 796f 7572 206e 616d 650a 2020  me: your name.  
+00000f10: 2020 3a70 6172 616d 206c 6173 746e 616d    :param lastnam
+00000f20: 653a 205b 2d6c 5d20 796f 7572 207b 7375  e: [-l] your {su
+00000f30: 726e 616d 657d 0a20 2020 2022 2222 0a20  rname}.    """. 
+00000f40: 2020 2066 756c 6c5f 6e61 6d65 203d 206e     full_name = n
+00000f50: 616d 6520 6966 206c 6173 746e 616d 6520  ame if lastname 
+00000f60: 6973 204e 6f6e 6520 656c 7365 2066 227b  is None else f"{
+00000f70: 6e61 6d65 7d20 7b6c 6173 746e 616d 657d  name} {lastname}
+00000f80: 220a 2020 2020 7072 696e 7428 6622 4865  ".    print(f"He
+00000f90: 6c6c 6f2c 207b 6675 6c6c 5f6e 616d 657d  llo, {full_name}
+00000fa0: 2122 290a 0a40 6172 6775 6162 6c79 2e63  !")..@arguably.c
+00000fb0: 6f6d 6d61 6e64 2861 6c69 6173 3d22 6722  ommand(alias="g"
+00000fc0: 290a 6465 6620 676f 6f64 6279 6528 6e61  ).def goodbye(na
+00000fd0: 6d65 3a20 7374 722c 202a 2c20 6973 5f73  me: str, *, is_s
+00000fe0: 6164 3a20 626f 6f6c 203d 2046 616c 7365  ad: bool = False
+00000ff0: 293a 0a20 2020 2022 2222 0a20 2020 2073  ):.    """.    s
+00001000: 6179 7320 676f 6f64 6279 6520 746f 2079  ays goodbye to y
+00001010: 6f75 0a20 2020 203a 7061 7261 6d20 6e61  ou.    :param na
+00001020: 6d65 3a20 796f 7572 206e 616d 650a 2020  me: your name.  
+00001030: 2020 3a70 6172 616d 2069 735f 7361 643a    :param is_sad:
+00001040: 205b 2d73 5d20 7768 6574 6865 7220 6f72   [-s] whether or
+00001050: 206e 6f74 2069 7427 7320 7361 6420 746f   not it's sad to
+00001060: 2073 6565 2079 6f75 2067 6f0a 2020 2020   see you go.    
+00001070: 2222 220a 2020 2020 7072 696e 7428 6622  """.    print(f"
+00001080: 476f 6f64 6279 652c 207b 6e61 6d65 7d21  Goodbye, {name}!
+00001090: 2229 0a20 2020 2069 6620 6973 5f73 6164  ").    if is_sad
+000010a0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+000010b0: 6622 4974 2773 2073 6164 2074 6f20 7365  f"It's sad to se
+000010c0: 6520 796f 7520 676f 2122 290a 0a69 6620  e you go!")..if 
+000010d0: 5f5f 6e61 6d65 5f5f 203d 3d20 225f 5f6d  __name__ == "__m
+000010e0: 6169 6e5f 5f22 3a0a 2020 2020 6172 6775  ain__":.    argu
+000010f0: 6162 6c79 2e72 756e 2876 6572 7369 6f6e  ably.run(version
+00001100: 5f66 6c61 673d 5472 7565 290a 6060 600a  _flag=True).```.
+00001110: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00001120: 7222 3e3c 623e 3c65 6d3e 6265 636f 6d65  r"><b><em>become
+00001130: 733c 2f65 6d3e 3c2f 623e 3c2f 703e 0a0a  s</em></b></p>..
+00001140: 6060 6063 6f6e 736f 6c65 0a75 7365 7240  ```console.user@
+00001150: 6d61 6368 696e 653a 7e24 2070 7974 686f  machine:~$ pytho
+00001160: 6e33 2073 6372 6970 742e 7079 0a75 7361  n3 script.py.usa
+00001170: 6765 3a20 7465 7374 5f73 6372 6970 7473  ge: test_scripts
+00001180: 2e64 6f63 7332 205b 2d68 5d20 5b2d 2d76  .docs2 [-h] [--v
+00001190: 6572 7369 6f6e 5d20 636f 6d6d 616e 6420  ersion] command 
+000011a0: 2e2e 2e0a 0a64 6f63 7374 7269 6e67 7320  .....docstrings 
+000011b0: 666f 7220 7468 6520 6669 6c65 2062 6563  for the file bec
+000011c0: 6f6d 6520 7468 6520 6465 7363 7269 7074  ome the descript
+000011d0: 696f 6e20 666f 7220 7468 6520 7363 7269  ion for the scri
+000011e0: 7074 2e0a 0a70 6f73 6974 696f 6e61 6c20  pt...positional 
+000011f0: 6172 6775 6d65 6e74 733a 0a20 2063 6f6d  arguments:.  com
+00001200: 6d61 6e64 0a20 2020 2068 656c 6c6f 2028  mand.    hello (
+00001210: 6829 2020 2020 7361 7973 2068 656c 6c6f  h)    says hello
+00001220: 2074 6f20 796f 750a 2020 2020 676f 6f64   to you.    good
+00001230: 6279 6520 2867 2920 2073 6179 7320 676f  bye (g)  says go
+00001240: 6f64 6279 6520 746f 2079 6f75 0a0a 6f70  odbye to you..op
+00001250: 7469 6f6e 733a 0a20 202d 682c 202d 2d68  tions:.  -h, --h
+00001260: 656c 7020 2020 2020 7368 6f77 2074 6869  elp     show thi
+00001270: 7320 6865 6c70 206d 6573 7361 6765 2061  s help message a
+00001280: 6e64 2065 7869 740a 2020 2d2d 7665 7273  nd exit.  --vers
+00001290: 696f 6e20 2020 2020 2073 686f 7720 7072  ion      show pr
+000012a0: 6f67 7261 6d27 7320 7665 7273 696f 6e20  ogram's version 
+000012b0: 6e75 6d62 6572 2061 6e64 2065 7869 740a  number and exit.
+000012c0: 0a0a 7573 6572 406d 6163 6869 6e65 3a7e  ..user@machine:~
+000012d0: 2420 7079 7468 6f6e 3320 7363 7269 7074  $ python3 script
+000012e0: 2e70 7920 6865 6c6c 6f20 2d2d 6865 6c70  .py hello --help
+000012f0: 0a75 7361 6765 3a20 7465 7374 5f73 6372  .usage: test_scr
+00001300: 6970 7473 2e64 6f63 7332 2068 656c 6c6f  ipts.docs2 hello
+00001310: 205b 2d68 5d20 5b2d 6c20 5355 524e 414d   [-h] [-l SURNAM
+00001320: 455d 206e 616d 650a 0a73 6179 7320 6865  E] name..says he
+00001330: 6c6c 6f20 746f 2079 6f75 0a0a 706f 7369  llo to you..posi
+00001340: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
+00001350: 3a0a 2020 6e61 6d65 2020 2020 2020 2020  :.  name        
+00001360: 2020 2020 2020 2020 2020 2020 796f 7572              your
+00001370: 206e 616d 650a 0a6f 7074 696f 6e73 3a0a   name..options:.
+00001380: 2020 2d68 2c20 2d2d 6865 6c70 2020 2020    -h, --help    
+00001390: 2020 2020 2020 2020 2020 7368 6f77 2074            show t
+000013a0: 6869 7320 6865 6c70 206d 6573 7361 6765  his help message
+000013b0: 2061 6e64 2065 7869 740a 2020 2d6c 2c20   and exit.  -l, 
+000013c0: 2d2d 6c61 7374 6e61 6d65 2053 5552 4e41  --lastname SURNA
+000013d0: 4d45 2020 796f 7572 2073 7572 6e61 6d65  ME  your surname
+000013e0: 2028 6465 6661 756c 743a 204e 6f6e 6529   (default: None)
+000013f0: 0a60 6060 0a0a 4d6f 7265 2064 6f63 7320  .```..More docs 
+00001400: 636f 6d69 6e67 2073 6f6f 6e2e 2e2e 0a    coming soon....
```

### Comparing `arguably-1.0.1/pyproject.toml` & `arguably-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "arguably"
-version = "1.0.1"
+version = "1.0.2"
 description = "turns functions into command line interfaces"
 authors = ["treykeown <2755914+treykeown@users.noreply.github.com>"]
 readme = "assets/PYPI_README.md"
 homepage = "https://github.com/treykeown/arguably"
 repository = "https://github.com/treykeown/arguably"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 docstring-parser = "^0.15"
+typing-extensions = "^4.6.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 mypy = "^1.3.0"
 ruff = "^0.0.263"
 pre-commit = "^3.3.2"
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.12.0"
+nox = "^2023.4.22"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
```

### Comparing `arguably-1.0.1/PKG-INFO` & `arguably-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,316 +1,366 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6172 6775  : 2.1.Name: argu
 00000020: 6162 6c79 0a56 6572 7369 6f6e 3a20 312e  ably.Version: 1.
-00000030: 302e 310a 5375 6d6d 6172 793a 2074 7572  0.1.Summary: tur
+00000030: 302e 320a 5375 6d6d 6172 793a 2074 7572  0.2.Summary: tur
 00000040: 6e73 2066 756e 6374 696f 6e73 2069 6e74  ns functions int
 00000050: 6f20 636f 6d6d 616e 6420 6c69 6e65 2069  o command line i
 00000060: 6e74 6572 6661 6365 730a 486f 6d65 2d70  nterfaces.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7472 6579 6b65 6f77  hub.com/treykeow
 00000090: 6e2f 6172 6775 6162 6c79 0a41 7574 686f  n/arguably.Autho
 000000a0: 723a 2074 7265 796b 656f 776e 0a41 7574  r: treykeown.Aut
 000000b0: 686f 722d 656d 6169 6c3a 2032 3735 3539  hor-email: 27559
 000000c0: 3134 2b74 7265 796b 656f 776e 4075 7365  14+treykeown@use
 000000d0: 7273 2e6e 6f72 6570 6c79 2e67 6974 6875  rs.noreply.githu
 000000e0: 622e 636f 6d0a 5265 7175 6972 6573 2d50  b.com.Requires-P
-000000f0: 7974 686f 6e3a 203e 3d33 2e39 2c3c 342e  ython: >=3.9,<4.
+000000f0: 7974 686f 6e3a 203e 3d33 2e38 2c3c 342e  ython: >=3.8,<4.
 00000100: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
 00000110: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000120: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000130: 330a 436c 6173 7369 6669 6572 3a20 5072  3.Classifier: Pr
 00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+00000160: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
 00000170: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000180: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000190: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-000001a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001c0: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
-000001d0: 6573 2d44 6973 743a 2064 6f63 7374 7269  es-Dist: docstri
-000001e0: 6e67 2d70 6172 7365 7220 283e 3d30 2e31  ng-parser (>=0.1
-000001f0: 352c 3c30 2e31 3629 0a50 726f 6a65 6374  5,<0.16).Project
-00000200: 2d55 524c 3a20 5265 706f 7369 746f 7279  -URL: Repository
-00000210: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000220: 2e63 6f6d 2f74 7265 796b 656f 776e 2f61  .com/treykeown/a
-00000230: 7267 7561 626c 790a 4465 7363 7269 7074  rguably.Descript
-00000240: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000250: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000260: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00000270: 7222 3e0a 2020 2020 2020 3c69 6d67 2061  r">.      <img a
-00000280: 6c74 3d22 6172 6775 6162 6c79 206c 6f67  lt="arguably log
-00000290: 6f22 2073 7263 3d22 6874 7470 733a 2f2f  o" src="https://
-000002a0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-000002b0: 6e74 656e 742e 636f 6d2f 7472 6579 6b65  ntent.com/treyke
-000002c0: 6f77 6e2f 6172 6775 6162 6c79 2f6d 6169  own/arguably/mai
-000002d0: 6e2f 6173 7365 7473 2f61 7267 7561 626c  n/assets/arguabl
-000002e0: 795f 626c 6163 6b2e 706e 6722 3e0a 3c2f  y_black.png">.</
-000002f0: 703e 0a0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
-00000300: 6e74 6572 223e 0a20 2020 203c 656d 3e0a  nter">.    <em>.
-00000310: 2020 2020 2020 2020 7475 726e 7320 6675          turns fu
-00000320: 6e63 7469 6f6e 7320 696e 746f 2063 6f6d  nctions into com
-00000330: 6d61 6e64 206c 696e 6520 696e 7465 7266  mand line interf
-00000340: 6163 6573 0a20 2020 203c 2f65 6d3e 0a3c  aces.    </em>.<
-00000350: 2f70 3e0a 0a3c 7020 616c 6967 6e3d 2263  /p>..<p align="c
-00000360: 656e 7465 7222 3e0a 2020 2020 3c21 2d2d  enter">.    <!--
-00000370: 2054 4f44 4f20 6261 6467 6573 202d 2d3e   TODO badges -->
-00000380: 0a3c 2f70 3e0a 3c68 723e 0a0a 6061 7267  .</p>.<hr>..`arg
-00000390: 7561 626c 7960 2073 6f6c 7665 7320 7468  uably` solves th
-000003a0: 6973 2070 726f 626c 656d 3a0a 312e 2059  is problem:.1. Y
-000003b0: 6f75 2776 6520 7772 6974 7465 6e20 6120  ou've written a 
-000003c0: 5079 7468 6f6e 2073 6372 6970 740a 322e  Python script.2.
-000003d0: 204e 6f77 2079 6f75 2077 616e 7420 746f   Now you want to
-000003e0: 2070 6173 7320 696e 2070 6172 616d 6574   pass in paramet
-000003f0: 6572 7320 6672 6f6d 2074 6865 2063 6f6d  ers from the com
-00000400: 6d61 6e64 206c 696e 650a 332e 2059 6f75  mand line.3. You
-00000410: 2064 6f6e 2774 2077 616e 7420 746f 2072   don't want to r
-00000420: 6561 6420 7468 6520 646f 6373 2066 6f72  ead the docs for
-00000430: 2079 6f75 7220 6661 766f 7269 7465 2061   your favorite a
-00000440: 7267 756d 656e 7420 7061 7273 696e 6720  rgument parsing 
-00000450: 6c69 6272 6172 7920 2a61 6761 696e 2a0a  library *again*.
-00000460: 0a42 7920 6c65 7665 7261 6769 6e67 2061  .By leveraging a
-00000470: 7320 6d61 6e79 2050 7974 686f 6e20 6964  s many Python id
-00000480: 696f 6d73 2061 7320 706f 7373 6962 6c65  ioms as possible
-00000490: 2c20 6061 7267 7561 626c 7960 206b 6565  , `arguably` kee
-000004a0: 7073 2069 7473 2041 5049 2073 6d61 6c6c  ps its API small
-000004b0: 2061 6e64 206d 656d 6f72 6162 6c65 2077   and memorable w
-000004c0: 6974 686f 7574 2073 6163 7269 6669 6369  ithout sacrifici
-000004d0: 6e67 0a66 756e 6369 746f 6e61 6c69 7479  ng.funcitonality
-000004e0: 2e20 6061 7267 7561 626c 7960 2075 7365  . `arguably` use
-000004f0: 7320 6675 6e63 7469 6f6e 7320 616e 6420  s functions and 
-00000500: 7468 6569 7220 646f 6373 7472 696e 6773  their docstrings
-00000510: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
-00000520: 7920 7365 7420 7570 2061 7267 7061 7273  y set up argpars
-00000530: 652e 204e 6f74 6162 6c79 2c20 6061 7267  e. Notably, `arg
-00000540: 7561 626c 7960 0a6d 6170 7320 796f 7572  uably`.maps your
-00000550: 2066 756e 6374 696f 6e20 7369 676e 6174   function signat
-00000560: 7572 6520 746f 2061 2063 6f6d 6d61 6e64  ure to a command
-00000570: 2d6c 696e 6520 696e 7465 7266 6163 6520  -line interface 
-00000580: 6c69 6b65 2074 6869 733a 0a0a 6060 6070  like this:..```p
-00000590: 7974 686f 6e0a 4061 7267 7561 626c 792e  ython.@arguably.
-000005a0: 636f 6d6d 616e 640a 6465 6620 736f 6d65  command.def some
-000005b0: 5f66 756e 6374 696f 6e28 7265 7175 6972  _function(requir
-000005c0: 6564 2c20 6e6f 745f 7265 7175 6972 6564  ed, not_required
-000005d0: 3d22 666f 6f22 2c20 2a6f 7468 6572 732c  ="foo", *others,
-000005e0: 206f 7074 696f 6e3d 2262 6172 2229 3a0a   option="bar"):.
-000005f0: 2020 2020 2e2e 2e0a 6060 600a 0a3c 7020      ....```..<p 
-00000600: 616c 6967 6e3d 2263 656e 7465 7222 3e3c  align="center"><
-00000610: 623e 3c65 6d3e 6265 636f 6d65 733c 2f65  b><em>becomes</e
-00000620: 6d3e 3c2f 623e 3c2f 703e 0a0a 6060 6074  m></b></p>..```t
-00000630: 6578 740a 7573 6167 653a 2073 6372 6970  ext.usage: scrip
-00000640: 7420 5b2d 2d6f 7074 696f 6e20 4f50 5449  t [--option OPTI
-00000650: 4f4e 5d20 7265 7175 6972 6564 205b 6e6f  ON] required [no
-00000660: 742d 7265 7175 6972 6564 5d20 5b6f 7468  t-required] [oth
-00000670: 6572 7320 2e2e 2e5d 0a60 6060 0a0a 496e  ers ...].```..In
-00000680: 2073 686f 7274 2c20 6061 7267 7561 626c   short, `arguabl
-00000690: 7960 2074 7572 6e73 2079 6f75 7220 6675  y` turns your fu
-000006a0: 6e63 7469 6f6e 2773 202a 2a70 6f73 6974  nction's **posit
-000006b0: 696f 6e61 6c20 7061 7261 6d65 7465 7273  ional parameters
-000006c0: 2a2a 2069 6e74 6f20 2a2a 706f 7369 7469  ** into **positi
-000006d0: 6f6e 616c 2063 6f6d 6d61 6e64 2d6c 696e  onal command-lin
-000006e0: 6520 6172 6775 6d65 6e74 732a 2a2c 2061  e arguments**, a
-000006f0: 6e64 0a79 6f75 7220 6675 6e63 7469 6f6e  nd.your function
-00000700: 2773 202a 2a6b 6579 776f 7264 2d6f 6e6c  's **keyword-onl
-00000710: 7920 6172 6775 6d65 6e74 732a 2a20 696e  y arguments** in
-00000720: 746f 202a 2a63 6f6d 6d61 6e64 2d6c 696e  to **command-lin
-00000730: 6520 6f70 7469 6f6e 732a 2a2e 2046 726f  e options**. Fro
-00000740: 6d20 7468 6520 6578 616d 706c 6520 6162  m the example ab
-00000750: 6f76 653a 0a0a 7c20 4e61 6d65 2020 2020  ove:..| Name    
-00000760: 2020 2020 2020 207c 2054 7970 6520 2020         | Type   
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 2020 2020 2020 2020 2020 2020 207c 2042               | B
-00000790: 6563 6f6d 6573 2020 2020 2020 2020 2020  ecomes          
-000007a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000007b0: 2055 7361 6765 2020 2020 2020 2020 2020   Usage          
-000007c0: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
-000007d0: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-000007e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000007f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-00000800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000820: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
-00000830: 2d2d 2d2d 2d2d 7c0a 7c20 6072 6571 7569  ------|.| `requi
-00000840: 7265 6460 2020 2020 207c 2070 6f73 6974  red`     | posit
-00000850: 696f 6e61 6c2c 206e 6f20 6465 6661 756c  ional, no defaul
-00000860: 7420 7661 6c75 6520 2020 2020 2020 207c  t value        |
-00000870: 2072 6571 7569 7265 6420 706f 7369 7469   required positi
-00000880: 6f6e 616c 2061 7267 2020 2020 2020 2020  onal arg        
-00000890: 207c 2060 7265 7175 6972 6564 6020 2020   | `required`   
-000008a0: 2020 2020 2020 207c 0a7c 2060 6e6f 745f         |.| `not_
-000008b0: 7265 7175 6972 6564 6020 7c20 706f 7369  required` | posi
-000008c0: 7469 6f6e 616c 2c20 7769 7468 2064 6566  tional, with def
-000008d0: 6175 6c74 2076 616c 7565 2020 2020 2020  ault value      
-000008e0: 7c20 6f70 7469 6f6e 616c 2070 6f73 6974  | optional posit
-000008f0: 696f 6e61 6c20 6172 6720 2020 2020 2020  ional arg       
-00000900: 2020 7c20 605b 6e6f 742d 7265 7175 6972    | `[not-requir
-00000910: 6564 5d60 2020 2020 7c0a 7c20 606f 7468  ed]`    |.| `oth
-00000920: 6572 7360 2020 2020 2020 207c 2070 6f73  ers`       | pos
-00000930: 6974 696f 6e61 6c2c 2076 6172 6961 6469  itional, variadi
-00000940: 6320 286c 696b 6520 602a 6172 6773 6029  c (like `*args`)
-00000950: 207c 2074 6865 2072 6573 7420 6f66 2074   | the rest of t
-00000960: 6865 2070 6f73 6974 696f 6e61 6c20 6172  he positional ar
-00000970: 6773 207c 2060 5b6f 7468 6572 7320 2e2e  gs | `[others ..
-00000980: 2e5d 6020 2020 2020 207c 0a7c 2060 6f70  .]`      |.| `op
-00000990: 7469 6f6e 6020 2020 2020 2020 7c20 6b65  tion`       | ke
-000009a0: 7977 6f72 642d 6f6e 6c79 2061 7267 756d  yword-only argum
-000009b0: 656e 7420 2020 2020 2020 2020 2020 2020  ent             
-000009c0: 2020 7c20 616e 206f 7074 696f 6e20 2020    | an option   
-000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009e0: 2020 2020 7c20 605b 2d2d 6f70 7469 6f6e      | `[--option
-000009f0: 204f 5054 494f 4e5d 6020 7c0a 0a60 6172   OPTION]` |..`ar
-00000a00: 6775 6162 6c79 6020 616c 736f 2065 6e61  guably` also ena
-00000a10: 626c 6573 2079 6f75 2074 6f20 6561 7369  bles you to easi
-00000a20: 6c79 2061 6464 2073 7562 636f 6d6d 616e  ly add subcomman
-00000a30: 6473 202d 206a 7573 7420 616e 6e6f 7461  ds - just annota
-00000a40: 7465 206d 6f72 6520 7468 616e 206f 6e65  te more than one
-00000a50: 2066 756e 6374 696f 6e20 7769 7468 2060   function with `
-00000a60: 4061 7267 7561 626c 792e 636f 6d6d 616e  @arguably.comman
-00000a70: 6460 2e0a 596f 7520 6361 6e20 6576 656e  d`..You can even
-00000a80: 2068 6176 6520 6e65 7374 6564 2073 7562   have nested sub
-00000a90: 636f 6d6d 616e 6473 2028 6d6f 7265 206f  commands (more o
-00000aa0: 6e20 7468 6174 206c 6174 6572 292e 0a0a  n that later)...
-00000ab0: 6061 7267 7561 626c 7960 2072 6561 6473  `arguably` reads
-00000ac0: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
-00000ad0: 7320 616e 6420 6175 746f 6d61 7469 6361  s and automatica
-00000ae0: 6c6c 7920 636f 6e76 6572 7473 2061 7267  lly converts arg
-00000af0: 756d 656e 7473 2074 6f20 7468 6520 6465  uments to the de
-00000b00: 636c 6172 6564 2074 7970 6573 2e20 4974  clared types. It
-00000b10: 2068 6173 2073 6d61 7274 2068 616e 646c   has smart handl
-00000b20: 696e 6720 666f 720a 6074 7570 6c65 602c  ing for.`tuple`,
-00000b30: 2060 6c69 7374 602c 2060 656e 756d 2e45   `list`, `enum.E
-00000b40: 6e75 6d60 2c20 616e 6420 6065 6e75 6d2e  num`, and `enum.
-00000b50: 466c 6167 602e 2054 6865 7265 2061 7265  Flag`. There are
-00000b60: 2061 6c73 6f20 6120 6665 7720 7370 6563   also a few spec
-00000b70: 6961 6c20 6265 6861 7669 6f72 7320 796f  ial behaviors yo
-00000b80: 7520 6361 6e20 6174 7461 6368 2074 6f20  u can attach to 
-00000b90: 6120 7061 7261 6d65 7465 720a 7669 6120  a parameter.via 
-00000ba0: 6041 6e6e 6f74 6174 6564 5b5d 6020 616e  `Annotated[]` an
-00000bb0: 6420 7468 6520 6061 7267 7561 626c 792e  d the `arguably.
-00000bc0: 6172 672e 2a60 2066 756e 6374 696f 6e73  arg.*` functions
-00000bd0: 2e0a 0a60 6172 6775 6162 6c79 6020 7061  ...`arguably` pa
-00000be0: 7273 6573 2064 6f63 7374 7269 6e67 7320  rses docstrings 
-00000bf0: 746f 2067 656e 6572 6174 6520 6465 7363  to generate desc
-00000c00: 7269 7074 696f 6e73 2066 6f72 2079 6f75  riptions for you
-00000c10: 7220 636f 6d6d 616e 6473 2061 6e64 2070  r commands and p
-00000c20: 6172 616d 6574 6572 732e 2049 6620 796f  arameters. If yo
-00000c30: 7520 7761 6e74 2074 6f20 6769 7665 2061  u want to give a
-00000c40: 2070 6172 616d 6574 6572 0a74 6865 2061   parameter.the a
-00000c50: 6c69 6173 2060 2d58 602c 2070 7265 6669  lias `-X`, prefi
-00000c60: 7820 6974 7320 646f 6373 7472 696e 6720  x its docstring 
-00000c70: 6465 7363 7269 7074 696f 6e20 7769 7468  description with
-00000c80: 2060 5b2d 585d 602e 2057 7261 7070 696e   `[-X]`. Wrappin
-00000c90: 6720 6120 776f 7264 2069 6e20 607b 7d60  g a word in `{}`
-00000ca0: 2063 6861 6e67 6573 2074 6865 202a 6d65   changes the *me
-00000cb0: 7461 7661 722a 2074 6861 7420 6765 7473  tavar* that gets
-00000cc0: 0a70 7269 6e74 6564 2028 7468 6973 2069  .printed (this i
-00000cd0: 7320 7768 6174 2773 2073 686f 776e 2069  s what's shown i
-00000ce0: 6e20 7468 6520 7573 6167 6520 7374 7269  n the usage stri
-00000cf0: 6e67 2061 6674 6572 2061 6e20 6f70 7469  ng after an opti
-00000d00: 6f6e 206e 616d 652c 2064 6f6e 2774 2077  on name, don't w
-00000d10: 6f72 7279 2069 6620 796f 7520 6172 656e  orry if you aren
-00000d20: 2774 2066 616d 696c 6961 7220 7769 7468  't familiar with
-00000d30: 2074 6869 7329 2e0a 466f 7220 6578 616d   this)..For exam
-00000d40: 706c 653a 0a0a 6060 6070 7974 686f 6e0a  ple:..```python.
-00000d50: 2321 2f75 7372 2f62 696e 2f65 6e76 2070  #!/usr/bin/env p
-00000d60: 7974 686f 6e33 0a22 2222 646f 6373 7472  ython3."""docstr
-00000d70: 696e 6773 2066 6f72 2074 6865 2066 696c  ings for the fil
-00000d80: 6520 6265 636f 6d65 2074 6865 2064 6573  e become the des
-00000d90: 6372 6970 7469 6f6e 2066 6f72 2074 6865  cription for the
-00000da0: 2073 6372 6970 742e 2222 220a 5f5f 7665   script.""".__ve
-00000db0: 7273 696f 6e5f 5f20 3d20 2231 2e30 2e30  rsion__ = "1.0.0
-00000dc0: 2220 2023 2059 6f75 2063 616e 2061 6c73  "  # You can als
-00000dd0: 6f20 7365 7420 6076 6572 7369 6f6e 5f66  o set `version_f
-00000de0: 6c61 673d 5472 7565 6020 746f 2061 6464  lag=True` to add
-00000df0: 2061 2076 6572 7369 6f6e 2066 6c61 672c   a version flag,
-00000e00: 2069 7420 7769 6c6c 2072 6561 6420 605f   it will read `_
-00000e10: 5f76 6572 7369 6f6e 5f5f 600a 0a69 6d70  _version__`..imp
-00000e20: 6f72 7420 6172 6775 6162 6c79 0a0a 4061  ort arguably..@a
-00000e30: 7267 7561 626c 792e 636f 6d6d 616e 6428  rguably.command(
-00000e40: 616c 6961 733d 2268 2229 0a64 6566 2068  alias="h").def h
-00000e50: 656c 6c6f 286e 616d 653a 2073 7472 2c20  ello(name: str, 
-00000e60: 2a2c 206c 6173 746e 616d 653a 2073 7472  *, lastname: str
-00000e70: 207c 204e 6f6e 6520 3d20 4e6f 6e65 293a   | None = None):
-00000e80: 0a20 2020 2022 2222 0a20 2020 2073 6179  .    """.    say
-00000e90: 7320 6865 6c6c 6f20 746f 2079 6f75 0a20  s hello to you. 
-00000ea0: 2020 203a 7061 7261 6d20 6e61 6d65 3a20     :param name: 
-00000eb0: 796f 7572 206e 616d 650a 2020 2020 3a70  your name.    :p
-00000ec0: 6172 616d 206c 6173 746e 616d 653a 205b  aram lastname: [
-00000ed0: 2d6c 5d20 796f 7572 207b 7375 726e 616d  -l] your {surnam
-00000ee0: 657d 0a20 2020 2022 2222 0a20 2020 2066  e}.    """.    f
-00000ef0: 756c 6c5f 6e61 6d65 203d 206e 616d 6520  ull_name = name 
-00000f00: 6966 206c 6173 746e 616d 6520 6973 204e  if lastname is N
-00000f10: 6f6e 6520 656c 7365 2066 227b 6e61 6d65  one else f"{name
-00000f20: 7d20 7b6c 6173 746e 616d 657d 220a 2020  } {lastname}".  
-00000f30: 2020 7072 696e 7428 6622 4865 6c6c 6f2c    print(f"Hello,
-00000f40: 207b 6675 6c6c 5f6e 616d 657d 2122 290a   {full_name}!").
-00000f50: 0a40 6172 6775 6162 6c79 2e63 6f6d 6d61  .@arguably.comma
-00000f60: 6e64 2861 6c69 6173 3d22 6722 290a 6465  nd(alias="g").de
-00000f70: 6620 676f 6f64 6279 6528 6e61 6d65 3a20  f goodbye(name: 
-00000f80: 7374 722c 202a 2c20 6973 5f73 6164 3a20  str, *, is_sad: 
-00000f90: 626f 6f6c 203d 2046 616c 7365 293a 0a20  bool = False):. 
-00000fa0: 2020 2022 2222 0a20 2020 2073 6179 7320     """.    says 
-00000fb0: 676f 6f64 6279 6520 746f 2079 6f75 0a20  goodbye to you. 
-00000fc0: 2020 203a 7061 7261 6d20 6e61 6d65 3a20     :param name: 
-00000fd0: 796f 7572 206e 616d 650a 2020 2020 3a70  your name.    :p
-00000fe0: 6172 616d 2069 735f 7361 643a 205b 2d73  aram is_sad: [-s
-00000ff0: 5d20 7768 6574 6865 7220 6f72 206e 6f74  ] whether or not
-00001000: 2069 7427 7320 7361 6420 746f 2073 6565   it's sad to see
-00001010: 2079 6f75 2067 6f0a 2020 2020 2222 220a   you go.    """.
-00001020: 2020 2020 7072 696e 7428 6622 476f 6f64      print(f"Good
-00001030: 6279 652c 207b 6e61 6d65 7d21 2229 0a20  bye, {name}!"). 
-00001040: 2020 2069 6620 6973 5f73 6164 3a0a 2020     if is_sad:.  
-00001050: 2020 2020 2020 7072 696e 7428 6622 4974        print(f"It
-00001060: 2773 2073 6164 2074 6f20 7365 6520 796f  's sad to see yo
-00001070: 7520 676f 2122 290a 0a69 6620 5f5f 6e61  u go!")..if __na
-00001080: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
-00001090: 5f22 3a0a 2020 2020 6172 6775 6162 6c79  _":.    arguably
-000010a0: 2e72 756e 2876 6572 7369 6f6e 5f66 6c61  .run(version_fla
-000010b0: 673d 5472 7565 290a 6060 600a 0a3c 7020  g=True).```..<p 
-000010c0: 616c 6967 6e3d 2263 656e 7465 7222 3e3c  align="center"><
-000010d0: 623e 3c65 6d3e 6265 636f 6d65 733c 2f65  b><em>becomes</e
-000010e0: 6d3e 3c2f 623e 3c2f 703e 0a0a 6060 6063  m></b></p>..```c
-000010f0: 6f6e 736f 6c65 0a75 7365 7240 6d61 6368  onsole.user@mach
-00001100: 696e 653a 7e24 2070 7974 686f 6e33 2073  ine:~$ python3 s
-00001110: 6372 6970 742e 7079 0a75 7361 6765 3a20  cript.py.usage: 
-00001120: 7465 7374 5f73 6372 6970 7473 2e64 6f63  test_scripts.doc
-00001130: 7332 205b 2d68 5d20 5b2d 2d76 6572 7369  s2 [-h] [--versi
-00001140: 6f6e 5d20 636f 6d6d 616e 6420 2e2e 2e0a  on] command ....
-00001150: 0a64 6f63 7374 7269 6e67 7320 666f 7220  .docstrings for 
-00001160: 7468 6520 6669 6c65 2062 6563 6f6d 6520  the file become 
-00001170: 7468 6520 6465 7363 7269 7074 696f 6e20  the description 
-00001180: 666f 7220 7468 6520 7363 7269 7074 2e0a  for the script..
-00001190: 0a70 6f73 6974 696f 6e61 6c20 6172 6775  .positional argu
-000011a0: 6d65 6e74 733a 0a20 2063 6f6d 6d61 6e64  ments:.  command
-000011b0: 0a20 2020 2068 656c 6c6f 2028 6829 2020  .    hello (h)  
-000011c0: 2020 7361 7973 2068 656c 6c6f 2074 6f20    says hello to 
-000011d0: 796f 750a 2020 2020 676f 6f64 6279 6520  you.    goodbye 
-000011e0: 2867 2920 2073 6179 7320 676f 6f64 6279  (g)  says goodby
-000011f0: 6520 746f 2079 6f75 0a0a 6f70 7469 6f6e  e to you..option
-00001200: 733a 0a20 202d 682c 202d 2d68 656c 7020  s:.  -h, --help 
-00001210: 2020 2020 7368 6f77 2074 6869 7320 6865      show this he
-00001220: 6c70 206d 6573 7361 6765 2061 6e64 2065  lp message and e
-00001230: 7869 740a 2020 2d2d 7665 7273 696f 6e20  xit.  --version 
-00001240: 2020 2020 2073 686f 7720 7072 6f67 7261       show progra
-00001250: 6d27 7320 7665 7273 696f 6e20 6e75 6d62  m's version numb
-00001260: 6572 2061 6e64 2065 7869 740a 0a0a 7573  er and exit...us
-00001270: 6572 406d 6163 6869 6e65 3a7e 2420 7079  er@machine:~$ py
-00001280: 7468 6f6e 3320 7363 7269 7074 2e70 7920  thon3 script.py 
-00001290: 6865 6c6c 6f20 2d2d 6865 6c70 0a75 7361  hello --help.usa
-000012a0: 6765 3a20 7465 7374 5f73 6372 6970 7473  ge: test_scripts
-000012b0: 2e64 6f63 7332 2068 656c 6c6f 205b 2d68  .docs2 hello [-h
-000012c0: 5d20 5b2d 6c20 5355 524e 414d 455d 206e  ] [-l SURNAME] n
-000012d0: 616d 650a 0a73 6179 7320 6865 6c6c 6f20  ame..says hello 
-000012e0: 746f 2079 6f75 0a0a 706f 7369 7469 6f6e  to you..position
-000012f0: 616c 2061 7267 756d 656e 7473 3a0a 2020  al arguments:.  
-00001300: 6e61 6d65 2020 2020 2020 2020 2020 2020  name            
-00001310: 2020 2020 2020 2020 796f 7572 206e 616d          your nam
-00001320: 650a 0a6f 7074 696f 6e73 3a0a 2020 2d68  e..options:.  -h
-00001330: 2c20 2d2d 6865 6c70 2020 2020 2020 2020  , --help        
-00001340: 2020 2020 2020 7368 6f77 2074 6869 7320        show this 
-00001350: 6865 6c70 206d 6573 7361 6765 2061 6e64  help message and
-00001360: 2065 7869 740a 2020 2d6c 2c20 2d2d 6c61   exit.  -l, --la
-00001370: 7374 6e61 6d65 2053 5552 4e41 4d45 2020  stname SURNAME  
-00001380: 796f 7572 2073 7572 6e61 6d65 2028 6465  your surname (de
-00001390: 6661 756c 743a 204e 6f6e 6529 0a60 6060  fault: None).```
-000013a0: 0a0a 4d6f 7265 2064 6f63 7320 636f 6d69  ..More docs comi
-000013b0: 6e67 2073 6f6f 6e2e 2e2e 0a0a            ng soon.....
+00000190: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
+000001a0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000001b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001c0: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
+000001d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e20 3a3a 2033 2e31 310a 5265 7175  hon :: 3.11.Requ
+00000200: 6972 6573 2d44 6973 743a 2064 6f63 7374  ires-Dist: docst
+00000210: 7269 6e67 2d70 6172 7365 7220 283e 3d30  ring-parser (>=0
+00000220: 2e31 352c 3c30 2e31 3629 0a52 6571 7569  .15,<0.16).Requi
+00000230: 7265 732d 4469 7374 3a20 7479 7069 6e67  res-Dist: typing
+00000240: 2d65 7874 656e 7369 6f6e 7320 283e 3d34  -extensions (>=4
+00000250: 2e36 2e33 2c3c 352e 302e 3029 0a50 726f  .6.3,<5.0.0).Pro
+00000260: 6a65 6374 2d55 524c 3a20 5265 706f 7369  ject-URL: Reposi
+00000270: 746f 7279 2c20 6874 7470 733a 2f2f 6769  tory, https://gi
+00000280: 7468 7562 2e63 6f6d 2f74 7265 796b 656f  thub.com/treykeo
+00000290: 776e 2f61 7267 7561 626c 790a 4465 7363  wn/arguably.Desc
+000002a0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+000002b0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+000002c0: 6f77 6e0a 0a3c 7020 616c 6967 6e3d 2263  own..<p align="c
+000002d0: 656e 7465 7222 3e0a 2020 2020 2020 3c69  enter">.      <i
+000002e0: 6d67 2061 6c74 3d22 6172 6775 6162 6c79  mg alt="arguably
+000002f0: 206c 6f67 6f22 2073 7263 3d22 6874 7470   logo" src="http
+00000300: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000310: 6572 636f 6e74 656e 742e 636f 6d2f 7472  ercontent.com/tr
+00000320: 6579 6b65 6f77 6e2f 6172 6775 6162 6c79  eykeown/arguably
+00000330: 2f6d 6169 6e2f 6173 7365 7473 2f61 7267  /main/assets/arg
+00000340: 7561 626c 795f 626c 6163 6b2e 706e 6722  uably_black.png"
+00000350: 3e0a 3c2f 703e 0a0a 3c70 2061 6c69 676e  >.</p>..<p align
+00000360: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+00000370: 656d 3e0a 2020 2020 2020 2020 7475 726e  em>.        turn
+00000380: 7320 6675 6e63 7469 6f6e 7320 696e 746f  s functions into
+00000390: 2063 6f6d 6d61 6e64 206c 696e 6520 696e   command line in
+000003a0: 7465 7266 6163 6573 0a20 2020 203c 2f65  terfaces.    </e
+000003b0: 6d3e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  m>.</p>..<p alig
+000003c0: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+000003d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000003e0: 2f67 6974 6875 622e 636f 6d2f 7472 6579  /github.com/trey
+000003f0: 6b65 6f77 6e2f 6172 6775 6162 6c79 2f61  keown/arguably/a
+00000400: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000410: 2f70 7974 686f 6e2d 7061 636b 6167 652e  /python-package.
+00000420: 796d 6c22 3e3c 696d 6720 7372 633d 2268  yml"><img src="h
+00000430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000440: 6d2f 7472 6579 6b65 6f77 6e2f 6172 6775  m/treykeown/argu
+00000450: 6162 6c79 2f61 6374 696f 6e73 2f77 6f72  ably/actions/wor
+00000460: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7061  kflows/python-pa
+00000470: 636b 6167 652e 796d 6c2f 6261 6467 652e  ckage.yml/badge.
+00000480: 7376 6722 2061 6c74 3d22 5465 7374 2073  svg" alt="Test s
+00000490: 7461 7475 7322 3e3c 2f61 3e0a 2020 2020  tatus"></a>.    
+000004a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000004b0: 2f67 6974 6875 622e 636f 6d2f 7472 6579  /github.com/trey
+000004c0: 6b65 6f77 6e2f 6172 6775 6162 6c79 2f74  keown/arguably/t
+000004d0: 7265 652f 6d61 696e 2f74 6573 7422 3e3c  ree/main/test"><
+000004e0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000004f0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000500: 656e 6470 6f69 6e74 3f75 726c 3d68 7474  endpoint?url=htt
+00000510: 7073 3a2f 2f67 6973 742e 6769 7468 7562  ps://gist.github
+00000520: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000530: 7472 6579 6b65 6f77 6e2f 6634 3933 6231  treykeown/f493b1
+00000540: 3432 3838 6166 3465 3833 3538 6561 3835  4288af4e8358ea85
+00000550: 3738 6333 3933 3231 3361 2f72 6177 2f61  78c393213a/raw/a
+00000560: 7267 7561 626c 792d 636f 7665 7261 6765  rguably-coverage
+00000570: 2d62 6164 6765 2e6a 736f 6e22 2061 6c74  -badge.json" alt
+00000580: 3d22 436f 6465 2063 6f76 6572 6167 6522  ="Code coverage"
+00000590: 3e3c 2f61 3e0a 2020 2020 3c61 2068 7265  ></a>.    <a hre
+000005a0: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+000005b0: 6f72 672f 7072 6f6a 6563 742f 6172 6775  org/project/argu
+000005c0: 6162 6c79 2f22 3e3c 696d 6720 7372 633d  ably/"><img src=
+000005d0: 2268 7474 7073 3a2f 2f73 6869 656c 6473  "https://shields
+000005e0: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
+000005f0: 6f6e 732f 6172 6775 6162 6c79 2220 616c  ons/arguably" al
+00000600: 743d 2253 7570 706f 7274 6564 2050 7974  t="Supported Pyt
+00000610: 686f 6e20 7665 7273 696f 6e73 223e 3c2f  hon versions"></
+00000620: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000630: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000640: 2f70 726f 6a65 6374 2f61 7267 7561 626c  /project/arguabl
+00000650: 792f 223e 3c69 6d67 2073 7263 3d22 6874  y/"><img src="ht
+00000660: 7470 733a 2f2f 7368 6965 6c64 732e 696f  tps://shields.io
+00000670: 2f70 7970 692f 762f 6172 6775 6162 6c79  /pypi/v/arguably
+00000680: 2220 616c 743d 2250 7950 4920 7665 7273  " alt="PyPI vers
+00000690: 696f 6e22 3e3c 2f61 3e0a 3c2f 703e 0a3c  ion"></a>.</p>.<
+000006a0: 6872 3e0a 0a60 6172 6775 6162 6c79 6020  hr>..`arguably` 
+000006b0: 736f 6c76 6573 2074 6869 7320 7072 6f62  solves this prob
+000006c0: 6c65 6d3a 0a31 2e20 596f 7527 7665 2077  lem:.1. You've w
+000006d0: 7269 7474 656e 2061 2050 7974 686f 6e20  ritten a Python 
+000006e0: 7363 7269 7074 0a32 2e20 4e6f 7720 796f  script.2. Now yo
+000006f0: 7520 7761 6e74 2074 6f20 7061 7373 2069  u want to pass i
+00000700: 6e20 7061 7261 6d65 7465 7273 2066 726f  n parameters fro
+00000710: 6d20 7468 6520 636f 6d6d 616e 6420 6c69  m the command li
+00000720: 6e65 0a33 2e20 596f 7520 646f 6e27 7420  ne.3. You don't 
+00000730: 7761 6e74 2074 6f20 7265 6164 2074 6865  want to read the
+00000740: 2064 6f63 7320 666f 7220 796f 7572 2066   docs for your f
+00000750: 6176 6f72 6974 6520 6172 6775 6d65 6e74  avorite argument
+00000760: 2070 6172 7369 6e67 206c 6962 7261 7279   parsing library
+00000770: 202a 6167 6169 6e2a 0a0a 4279 206c 6576   *again*..By lev
+00000780: 6572 6167 696e 6720 6173 206d 616e 7920  eraging as many 
+00000790: 5079 7468 6f6e 2069 6469 6f6d 7320 6173  Python idioms as
+000007a0: 2070 6f73 7369 626c 652c 2060 6172 6775   possible, `argu
+000007b0: 6162 6c79 6020 6b65 6570 7320 6974 7320  ably` keeps its 
+000007c0: 4150 4920 736d 616c 6c20 616e 6420 6d65  API small and me
+000007d0: 6d6f 7261 626c 6520 7769 7468 6f75 7420  morable without 
+000007e0: 7361 6372 6966 6963 696e 670a 6675 6e63  sacrificing.func
+000007f0: 6974 6f6e 616c 6974 792e 2060 6172 6775  itonality. `argu
+00000800: 6162 6c79 6020 7573 6573 2066 756e 6374  ably` uses funct
+00000810: 696f 6e73 2061 6e64 2074 6865 6972 2064  ions and their d
+00000820: 6f63 7374 7269 6e67 7320 746f 2061 7574  ocstrings to aut
+00000830: 6f6d 6174 6963 616c 6c79 2073 6574 2075  omatically set u
+00000840: 7020 6172 6770 6172 7365 2e20 4e6f 7461  p argparse. Nota
+00000850: 626c 792c 2060 6172 6775 6162 6c79 600a  bly, `arguably`.
+00000860: 6d61 7073 2079 6f75 7220 6675 6e63 7469  maps your functi
+00000870: 6f6e 2073 6967 6e61 7475 7265 2074 6f20  on signature to 
+00000880: 6120 636f 6d6d 616e 642d 6c69 6e65 2069  a command-line i
+00000890: 6e74 6572 6661 6365 206c 696b 6520 7468  nterface like th
+000008a0: 6973 3a0a 0a60 6060 7079 7468 6f6e 0a40  is:..```python.@
+000008b0: 6172 6775 6162 6c79 2e63 6f6d 6d61 6e64  arguably.command
+000008c0: 0a64 6566 2073 6f6d 655f 6675 6e63 7469  .def some_functi
+000008d0: 6f6e 2872 6571 7569 7265 642c 206e 6f74  on(required, not
+000008e0: 5f72 6571 7569 7265 643d 2266 6f6f 222c  _required="foo",
+000008f0: 202a 6f74 6865 7273 2c20 6f70 7469 6f6e   *others, option
+00000900: 3d22 6261 7222 293a 0a20 2020 202e 2e2e  ="bar"):.    ...
+00000910: 0a60 6060 0a0a 3c70 2061 6c69 676e 3d22  .```..<p align="
+00000920: 6365 6e74 6572 223e 3c62 3e3c 656d 3e62  center"><b><em>b
+00000930: 6563 6f6d 6573 3c2f 656d 3e3c 2f62 3e3c  ecomes</em></b><
+00000940: 2f70 3e0a 0a60 6060 7465 7874 0a75 7361  /p>..```text.usa
+00000950: 6765 3a20 7363 7269 7074 205b 2d2d 6f70  ge: script [--op
+00000960: 7469 6f6e 204f 5054 494f 4e5d 2072 6571  tion OPTION] req
+00000970: 7569 7265 6420 5b6e 6f74 2d72 6571 7569  uired [not-requi
+00000980: 7265 645d 205b 6f74 6865 7273 202e 2e2e  red] [others ...
+00000990: 5d0a 6060 600a 0a49 6e20 7368 6f72 742c  ].```..In short,
+000009a0: 2060 6172 6775 6162 6c79 6020 7475 726e   `arguably` turn
+000009b0: 7320 796f 7572 2066 756e 6374 696f 6e27  s your function'
+000009c0: 7320 2a2a 706f 7369 7469 6f6e 616c 2070  s **positional p
+000009d0: 6172 616d 6574 6572 732a 2a20 696e 746f  arameters** into
+000009e0: 202a 2a70 6f73 6974 696f 6e61 6c20 636f   **positional co
+000009f0: 6d6d 616e 642d 6c69 6e65 2061 7267 756d  mmand-line argum
+00000a00: 656e 7473 2a2a 2c20 616e 640a 796f 7572  ents**, and.your
+00000a10: 2066 756e 6374 696f 6e27 7320 2a2a 6b65   function's **ke
+00000a20: 7977 6f72 642d 6f6e 6c79 2061 7267 756d  yword-only argum
+00000a30: 656e 7473 2a2a 2069 6e74 6f20 2a2a 636f  ents** into **co
+00000a40: 6d6d 616e 642d 6c69 6e65 206f 7074 696f  mmand-line optio
+00000a50: 6e73 2a2a 2e20 4672 6f6d 2074 6865 2065  ns**. From the e
+00000a60: 7861 6d70 6c65 2061 626f 7665 3a0a 0a7c  xample above:..|
+00000a70: 204e 616d 6520 2020 2020 2020 2020 2020   Name           
+00000a80: 7c20 5479 7065 2020 2020 2020 2020 2020  | Type          
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 7c20 4265 636f 6d65 7320        | Becomes 
+00000ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ac0: 2020 2020 2020 2020 7c20 5573 6167 6520          | Usage 
+00000ad0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00000ae0: 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |---------------
+00000af0: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00000b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b10: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
+00000b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000b30: 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d  ---------|------
+00000b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00000b50: 0a7c 2060 7265 7175 6972 6564 6020 2020  .| `required`   
+00000b60: 2020 7c20 706f 7369 7469 6f6e 616c 2c20    | positional, 
+00000b70: 6e6f 2064 6566 6175 6c74 2076 616c 7565  no default value
+00000b80: 2020 2020 2020 2020 7c20 7265 7175 6972          | requir
+00000b90: 6564 2070 6f73 6974 696f 6e61 6c20 6172  ed positional ar
+00000ba0: 6720 2020 2020 2020 2020 7c20 6072 6571  g         | `req
+00000bb0: 7569 7265 6460 2020 2020 2020 2020 2020  uired`          
+00000bc0: 7c0a 7c20 606e 6f74 5f72 6571 7569 7265  |.| `not_require
+00000bd0: 6460 207c 2070 6f73 6974 696f 6e61 6c2c  d` | positional,
+00000be0: 2077 6974 6820 6465 6661 756c 7420 7661   with default va
+00000bf0: 6c75 6520 2020 2020 207c 206f 7074 696f  lue      | optio
+00000c00: 6e61 6c20 706f 7369 7469 6f6e 616c 2061  nal positional a
+00000c10: 7267 2020 2020 2020 2020 207c 2060 5b6e  rg         | `[n
+00000c20: 6f74 2d72 6571 7569 7265 645d 6020 2020  ot-required]`   
+00000c30: 207c 0a7c 2060 6f74 6865 7273 6020 2020   |.| `others`   
+00000c40: 2020 2020 7c20 706f 7369 7469 6f6e 616c      | positional
+00000c50: 2c20 7661 7269 6164 6963 2028 6c69 6b65  , variadic (like
+00000c60: 2060 2a61 7267 7360 2920 7c20 7468 6520   `*args`) | the 
+00000c70: 7265 7374 206f 6620 7468 6520 706f 7369  rest of the posi
+00000c80: 7469 6f6e 616c 2061 7267 7320 7c20 605b  tional args | `[
+00000c90: 6f74 6865 7273 202e 2e2e 5d60 2020 2020  others ...]`    
+00000ca0: 2020 7c0a 7c20 606f 7074 696f 6e60 2020    |.| `option`  
+00000cb0: 2020 2020 207c 206b 6579 776f 7264 2d6f       | keyword-o
+00000cc0: 6e6c 7920 6172 6775 6d65 6e74 2020 2020  nly argument    
+00000cd0: 2020 2020 2020 2020 2020 207c 2061 6e20             | an 
+00000ce0: 6f70 7469 6f6e 2020 2020 2020 2020 2020  option          
+00000cf0: 2020 2020 2020 2020 2020 2020 207c 2060               | `
+00000d00: 5b2d 2d6f 7074 696f 6e20 4f50 5449 4f4e  [--option OPTION
+00000d10: 5d60 207c 0a0a 6061 7267 7561 626c 7960  ]` |..`arguably`
+00000d20: 2061 6c73 6f20 656e 6162 6c65 7320 796f   also enables yo
+00000d30: 7520 746f 2065 6173 696c 7920 6164 6420  u to easily add 
+00000d40: 7375 6263 6f6d 6d61 6e64 7320 2d20 6a75  subcommands - ju
+00000d50: 7374 2061 6e6e 6f74 6174 6520 6d6f 7265  st annotate more
+00000d60: 2074 6861 6e20 6f6e 6520 6675 6e63 7469   than one functi
+00000d70: 6f6e 2077 6974 6820 6040 6172 6775 6162  on with `@arguab
+00000d80: 6c79 2e63 6f6d 6d61 6e64 602e 0a59 6f75  ly.command`..You
+00000d90: 2063 616e 2065 7665 6e20 6861 7665 206e   can even have n
+00000da0: 6573 7465 6420 7375 6263 6f6d 6d61 6e64  ested subcommand
+00000db0: 7320 286d 6f72 6520 6f6e 2074 6861 7420  s (more on that 
+00000dc0: 6c61 7465 7229 2e0a 0a60 6172 6775 6162  later)...`arguab
+00000dd0: 6c79 6020 7265 6164 7320 7479 7065 2061  ly` reads type a
+00000de0: 6e6e 6f74 6174 696f 6e73 2061 6e64 2061  nnotations and a
+00000df0: 7574 6f6d 6174 6963 616c 6c79 2063 6f6e  utomatically con
+00000e00: 7665 7274 7320 6172 6775 6d65 6e74 7320  verts arguments 
+00000e10: 746f 2074 6865 2064 6563 6c61 7265 6420  to the declared 
+00000e20: 7479 7065 732e 2049 7420 6861 7320 736d  types. It has sm
+00000e30: 6172 7420 6861 6e64 6c69 6e67 2066 6f72  art handling for
+00000e40: 0a60 7475 706c 6560 2c20 606c 6973 7460  .`tuple`, `list`
+00000e50: 2c20 6065 6e75 6d2e 456e 756d 602c 2061  , `enum.Enum`, a
+00000e60: 6e64 2060 656e 756d 2e46 6c61 6760 2e20  nd `enum.Flag`. 
+00000e70: 5468 6572 6520 6172 6520 616c 736f 2061  There are also a
+00000e80: 2066 6577 2073 7065 6369 616c 2062 6568   few special beh
+00000e90: 6176 696f 7273 2079 6f75 2063 616e 2061  aviors you can a
+00000ea0: 7474 6163 6820 746f 2061 2070 6172 616d  ttach to a param
+00000eb0: 6574 6572 0a76 6961 2060 416e 6e6f 7461  eter.via `Annota
+00000ec0: 7465 645b 5d60 2061 6e64 2074 6865 2060  ted[]` and the `
+00000ed0: 6172 6775 6162 6c79 2e61 7267 2e2a 6020  arguably.arg.*` 
+00000ee0: 6675 6e63 7469 6f6e 732e 0a0a 6061 7267  functions...`arg
+00000ef0: 7561 626c 7960 2070 6172 7365 7320 646f  uably` parses do
+00000f00: 6373 7472 696e 6773 2074 6f20 6765 6e65  cstrings to gene
+00000f10: 7261 7465 2064 6573 6372 6970 7469 6f6e  rate description
+00000f20: 7320 666f 7220 796f 7572 2063 6f6d 6d61  s for your comma
+00000f30: 6e64 7320 616e 6420 7061 7261 6d65 7465  nds and paramete
+00000f40: 7273 2e20 4966 2079 6f75 2077 616e 7420  rs. If you want 
+00000f50: 746f 2067 6976 6520 6120 7061 7261 6d65  to give a parame
+00000f60: 7465 720a 7468 6520 616c 6961 7320 602d  ter.the alias `-
+00000f70: 5860 2c20 7072 6566 6978 2069 7473 2064  X`, prefix its d
+00000f80: 6f63 7374 7269 6e67 2064 6573 6372 6970  ocstring descrip
+00000f90: 7469 6f6e 2077 6974 6820 605b 2d58 5d60  tion with `[-X]`
+00000fa0: 2e20 5772 6170 7069 6e67 2061 2077 6f72  . Wrapping a wor
+00000fb0: 6420 696e 2060 7b7d 6020 6368 616e 6765  d in `{}` change
+00000fc0: 7320 7468 6520 2a6d 6574 6176 6172 2a20  s the *metavar* 
+00000fd0: 7468 6174 2067 6574 730a 7072 696e 7465  that gets.printe
+00000fe0: 6420 2874 6869 7320 6973 2077 6861 7427  d (this is what'
+00000ff0: 7320 7368 6f77 6e20 696e 2074 6865 2075  s shown in the u
+00001000: 7361 6765 2073 7472 696e 6720 6166 7465  sage string afte
+00001010: 7220 616e 206f 7074 696f 6e20 6e61 6d65  r an option name
+00001020: 2c20 646f 6e27 7420 776f 7272 7920 6966  , don't worry if
+00001030: 2079 6f75 2061 7265 6e27 7420 6661 6d69   you aren't fami
+00001040: 6c69 6172 2077 6974 6820 7468 6973 292e  liar with this).
+00001050: 0a46 6f72 2065 7861 6d70 6c65 3a0a 0a60  .For example:..`
+00001060: 6060 7079 7468 6f6e 0a23 212f 7573 722f  ``python.#!/usr/
+00001070: 6269 6e2f 656e 7620 7079 7468 6f6e 330a  bin/env python3.
+00001080: 2222 2264 6f63 7374 7269 6e67 7320 666f  """docstrings fo
+00001090: 7220 7468 6520 6669 6c65 2062 6563 6f6d  r the file becom
+000010a0: 6520 7468 6520 6465 7363 7269 7074 696f  e the descriptio
+000010b0: 6e20 666f 7220 7468 6520 7363 7269 7074  n for the script
+000010c0: 2e22 2222 0a5f 5f76 6572 7369 6f6e 5f5f  .""".__version__
+000010d0: 203d 2022 312e 302e 3022 2020 2320 596f   = "1.0.0"  # Yo
+000010e0: 7520 6361 6e20 616c 736f 2073 6574 2060  u can also set `
+000010f0: 7665 7273 696f 6e5f 666c 6167 3d54 7275  version_flag=Tru
+00001100: 6560 2074 6f20 6164 6420 6120 7665 7273  e` to add a vers
+00001110: 696f 6e20 666c 6167 2c20 6974 2077 696c  ion flag, it wil
+00001120: 6c20 7265 6164 2060 5f5f 7665 7273 696f  l read `__versio
+00001130: 6e5f 5f60 0a0a 696d 706f 7274 2061 7267  n__`..import arg
+00001140: 7561 626c 790a 0a40 6172 6775 6162 6c79  uably..@arguably
+00001150: 2e63 6f6d 6d61 6e64 2861 6c69 6173 3d22  .command(alias="
+00001160: 6822 290a 6465 6620 6865 6c6c 6f28 6e61  h").def hello(na
+00001170: 6d65 3a20 7374 722c 202a 2c20 6c61 7374  me: str, *, last
+00001180: 6e61 6d65 3a20 7374 7220 7c20 4e6f 6e65  name: str | None
+00001190: 203d 204e 6f6e 6529 3a0a 2020 2020 2222   = None):.    ""
+000011a0: 220a 2020 2020 7361 7973 2068 656c 6c6f  ".    says hello
+000011b0: 2074 6f20 796f 750a 2020 2020 3a70 6172   to you.    :par
+000011c0: 616d 206e 616d 653a 2079 6f75 7220 6e61  am name: your na
+000011d0: 6d65 0a20 2020 203a 7061 7261 6d20 6c61  me.    :param la
+000011e0: 7374 6e61 6d65 3a20 5b2d 6c5d 2079 6f75  stname: [-l] you
+000011f0: 7220 7b73 7572 6e61 6d65 7d0a 2020 2020  r {surname}.    
+00001200: 2222 220a 2020 2020 6675 6c6c 5f6e 616d  """.    full_nam
+00001210: 6520 3d20 6e61 6d65 2069 6620 6c61 7374  e = name if last
+00001220: 6e61 6d65 2069 7320 4e6f 6e65 2065 6c73  name is None els
+00001230: 6520 6622 7b6e 616d 657d 207b 6c61 7374  e f"{name} {last
+00001240: 6e61 6d65 7d22 0a20 2020 2070 7269 6e74  name}".    print
+00001250: 2866 2248 656c 6c6f 2c20 7b66 756c 6c5f  (f"Hello, {full_
+00001260: 6e61 6d65 7d21 2229 0a0a 4061 7267 7561  name}!")..@argua
+00001270: 626c 792e 636f 6d6d 616e 6428 616c 6961  bly.command(alia
+00001280: 733d 2267 2229 0a64 6566 2067 6f6f 6462  s="g").def goodb
+00001290: 7965 286e 616d 653a 2073 7472 2c20 2a2c  ye(name: str, *,
+000012a0: 2069 735f 7361 643a 2062 6f6f 6c20 3d20   is_sad: bool = 
+000012b0: 4661 6c73 6529 3a0a 2020 2020 2222 220a  False):.    """.
+000012c0: 2020 2020 7361 7973 2067 6f6f 6462 7965      says goodbye
+000012d0: 2074 6f20 796f 750a 2020 2020 3a70 6172   to you.    :par
+000012e0: 616d 206e 616d 653a 2079 6f75 7220 6e61  am name: your na
+000012f0: 6d65 0a20 2020 203a 7061 7261 6d20 6973  me.    :param is
+00001300: 5f73 6164 3a20 5b2d 735d 2077 6865 7468  _sad: [-s] wheth
+00001310: 6572 206f 7220 6e6f 7420 6974 2773 2073  er or not it's s
+00001320: 6164 2074 6f20 7365 6520 796f 7520 676f  ad to see you go
+00001330: 0a20 2020 2022 2222 0a20 2020 2070 7269  .    """.    pri
+00001340: 6e74 2866 2247 6f6f 6462 7965 2c20 7b6e  nt(f"Goodbye, {n
+00001350: 616d 657d 2122 290a 2020 2020 6966 2069  ame}!").    if i
+00001360: 735f 7361 643a 0a20 2020 2020 2020 2070  s_sad:.        p
+00001370: 7269 6e74 2866 2249 7427 7320 7361 6420  rint(f"It's sad 
+00001380: 746f 2073 6565 2079 6f75 2067 6f21 2229  to see you go!")
+00001390: 0a0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+000013a0: 2022 5f5f 6d61 696e 5f5f 223a 0a20 2020   "__main__":.   
+000013b0: 2061 7267 7561 626c 792e 7275 6e28 7665   arguably.run(ve
+000013c0: 7273 696f 6e5f 666c 6167 3d54 7275 6529  rsion_flag=True)
+000013d0: 0a60 6060 0a0a 3c70 2061 6c69 676e 3d22  .```..<p align="
+000013e0: 6365 6e74 6572 223e 3c62 3e3c 656d 3e62  center"><b><em>b
+000013f0: 6563 6f6d 6573 3c2f 656d 3e3c 2f62 3e3c  ecomes</em></b><
+00001400: 2f70 3e0a 0a60 6060 636f 6e73 6f6c 650a  /p>..```console.
+00001410: 7573 6572 406d 6163 6869 6e65 3a7e 2420  user@machine:~$ 
+00001420: 7079 7468 6f6e 3320 7363 7269 7074 2e70  python3 script.p
+00001430: 790a 7573 6167 653a 2074 6573 745f 7363  y.usage: test_sc
+00001440: 7269 7074 732e 646f 6373 3220 5b2d 685d  ripts.docs2 [-h]
+00001450: 205b 2d2d 7665 7273 696f 6e5d 2063 6f6d   [--version] com
+00001460: 6d61 6e64 202e 2e2e 0a0a 646f 6373 7472  mand .....docstr
+00001470: 696e 6773 2066 6f72 2074 6865 2066 696c  ings for the fil
+00001480: 6520 6265 636f 6d65 2074 6865 2064 6573  e become the des
+00001490: 6372 6970 7469 6f6e 2066 6f72 2074 6865  cription for the
+000014a0: 2073 6372 6970 742e 0a0a 706f 7369 7469   script...positi
+000014b0: 6f6e 616c 2061 7267 756d 656e 7473 3a0a  onal arguments:.
+000014c0: 2020 636f 6d6d 616e 640a 2020 2020 6865    command.    he
+000014d0: 6c6c 6f20 2868 2920 2020 2073 6179 7320  llo (h)    says 
+000014e0: 6865 6c6c 6f20 746f 2079 6f75 0a20 2020  hello to you.   
+000014f0: 2067 6f6f 6462 7965 2028 6729 2020 7361   goodbye (g)  sa
+00001500: 7973 2067 6f6f 6462 7965 2074 6f20 796f  ys goodbye to yo
+00001510: 750a 0a6f 7074 696f 6e73 3a0a 2020 2d68  u..options:.  -h
+00001520: 2c20 2d2d 6865 6c70 2020 2020 2073 686f  , --help     sho
+00001530: 7720 7468 6973 2068 656c 7020 6d65 7373  w this help mess
+00001540: 6167 6520 616e 6420 6578 6974 0a20 202d  age and exit.  -
+00001550: 2d76 6572 7369 6f6e 2020 2020 2020 7368  -version      sh
+00001560: 6f77 2070 726f 6772 616d 2773 2076 6572  ow program's ver
+00001570: 7369 6f6e 206e 756d 6265 7220 616e 6420  sion number and 
+00001580: 6578 6974 0a0a 0a75 7365 7240 6d61 6368  exit...user@mach
+00001590: 696e 653a 7e24 2070 7974 686f 6e33 2073  ine:~$ python3 s
+000015a0: 6372 6970 742e 7079 2068 656c 6c6f 202d  cript.py hello -
+000015b0: 2d68 656c 700a 7573 6167 653a 2074 6573  -help.usage: tes
+000015c0: 745f 7363 7269 7074 732e 646f 6373 3220  t_scripts.docs2 
+000015d0: 6865 6c6c 6f20 5b2d 685d 205b 2d6c 2053  hello [-h] [-l S
+000015e0: 5552 4e41 4d45 5d20 6e61 6d65 0a0a 7361  URNAME] name..sa
+000015f0: 7973 2068 656c 6c6f 2074 6f20 796f 750a  ys hello to you.
+00001600: 0a70 6f73 6974 696f 6e61 6c20 6172 6775  .positional argu
+00001610: 6d65 6e74 733a 0a20 206e 616d 6520 2020  ments:.  name   
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2079 6f75 7220 6e61 6d65 0a0a 6f70 7469   your name..opti
+00001640: 6f6e 733a 0a20 202d 682c 202d 2d68 656c  ons:.  -h, --hel
+00001650: 7020 2020 2020 2020 2020 2020 2020 2073  p              s
+00001660: 686f 7720 7468 6973 2068 656c 7020 6d65  how this help me
+00001670: 7373 6167 6520 616e 6420 6578 6974 0a20  ssage and exit. 
+00001680: 202d 6c2c 202d 2d6c 6173 746e 616d 6520   -l, --lastname 
+00001690: 5355 524e 414d 4520 2079 6f75 7220 7375  SURNAME  your su
+000016a0: 726e 616d 6520 2864 6566 6175 6c74 3a20  rname (default: 
+000016b0: 4e6f 6e65 290a 6060 600a 0a4d 6f72 6520  None).```..More 
+000016c0: 646f 6373 2063 6f6d 696e 6720 736f 6f6e  docs coming soon
+000016d0: 2e2e 2e0a 0a                             .....
```

