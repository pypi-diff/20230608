# Comparing `tmp/markpickle-1.5.0.tar.gz` & `tmp/markpickle-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markpickle-1.5.0.tar", max compression
+gzip compressed data, was "markpickle-1.5.1.tar", max compression
```

## Comparing `markpickle-1.5.0.tar` & `markpickle-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-06-01 02:16:20.093850 markpickle-1.5.0/LICENSE
--rw-r--r--   0        0        0     6119 2023-06-01 02:16:20.093850 markpickle-1.5.0/README.md
--rw-r--r--   0        0        0      574 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/__init__.py
--rw-r--r--   0        0        0     1397 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/__main__.py
--rw-r--r--   0        0        0     1697 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/atx_as_dictionary.py
--rw-r--r--   0        0        0     1543 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/binary_streams.py
--rw-r--r--   0        0        0       57 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/cli.py
--rw-r--r--   0        0        0     2299 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/config_class.py
--rw-r--r--   0        0        0    12988 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/deserialize.py
--rw-r--r--   0        0        0      412 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/meta.py
--rw-r--r--   0        0        0      568 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/mypy_types.py
--rw-r--r--   0        0        0       80 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/py.typed
--rw-r--r--   0        0        0     5412 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/python_to_tables.py
--rw-r--r--   0        0        0    14985 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/serialize.py
--rw-r--r--   0        0        0      737 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/simplify_types.py
--rw-r--r--   0        0        0     1032 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/split_file_code.py
--rw-r--r--   0        0        0     1252 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/third_party_tables.py
--rw-r--r--   0        0        0     1760 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/tool.py
--rw-r--r--   0        0        0      813 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/unicode_formatting.py
--rw-r--r--   0        0        0     3720 2023-06-01 02:16:20.097850 markpickle-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 markpickle-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-08 18:02:09.907821 markpickle-1.5.1/LICENSE
+-rw-r--r--   0        0        0     7182 2023-06-08 18:02:09.907821 markpickle-1.5.1/README.md
+-rw-r--r--   0        0        0      574 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/__init__.py
+-rw-r--r--   0        0        0     1437 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/__main__.py
+-rw-r--r--   0        0        0     2005 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/atx_as_dictionary.py
+-rw-r--r--   0        0        0     1614 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/binary_streams.py
+-rw-r--r--   0        0        0       57 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/cli.py
+-rw-r--r--   0        0        0     2299 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/config_class.py
+-rw-r--r--   0        0        0    13725 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/deserialize.py
+-rw-r--r--   0        0        0      412 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/meta.py
+-rw-r--r--   0        0        0     1145 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/mypy_types.py
+-rw-r--r--   0        0        0       80 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/py.typed
+-rw-r--r--   0        0        0     5581 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/python_to_tables.py
+-rw-r--r--   0        0        0    15441 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/serialize.py
+-rw-r--r--   0        0        0      737 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/simplify_types.py
+-rw-r--r--   0        0        0     1043 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/split_file_code.py
+-rw-r--r--   0        0        0     1216 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/third_party_tables.py
+-rw-r--r--   0        0        0     1760 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/tool.py
+-rw-r--r--   0        0        0      813 2023-06-08 18:02:09.911821 markpickle-1.5.1/markpickle/unicode_formatting.py
+-rw-r--r--   0        0        0     3725 2023-06-08 18:02:09.911821 markpickle-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8706 1970-01-01 00:00:00.000000 markpickle-1.5.1/PKG-INFO
```

### Comparing `markpickle-1.5.0/LICENSE` & `markpickle-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.0/README.md` & `markpickle-1.5.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 # markpickle
 
-Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
+Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. Imagine if markdown headers were used to define nested dictionaries and Markdown lists were python lists.
+
+It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
 For example this
 
 ```markdown
 - 1
 - 2
 ```
 
 becomes the python list `[1, 2]`
 
-Almost all markdown libraries use it as intended, as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data.
+```markdown
+# Cat
+## Name
+Ringo
+## Species
+Felix
+```
+
+becomes the python list `{"cat":{"Name":"Ringo","Species":"Felix"}`
+
+See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for representable types.
+
+Almost all markdown libraries use it as intended, as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data. See [guidance](docs/choosing_a_library.md) for which library make sense for you.
 
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/markpickle) [![Downloads](https://pepy.tech/badge/markpickle/month)](https://pepy.tech/project/markpickle/month)
 
 ______________________________________________________________________
 
 ## Installation
 
@@ -100,28 +114,44 @@
 
 [markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle, but is somewhat broken, unmaintained and depends on the unmaintained commonmark library.
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
 [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
+## Representable Types
+
+There is one optional root dictionary representable with ATX headers, e.g. `#`, `##`, etc. Lists are nestable lists or dicts. For the most part, this looks like the types that JSON can represent.
+
+```python
+from typing import Union, TypeAlias
+import datetime
+import PIL
+MarkSerializable: TypeAlias = Union[
+    dict[str, "MarkSerializable"],
+    list["MarkSerializable"], str, int, float, bool, datetime, PIL.image, bytes, None]
+```
+
+The deserialized types is the same except all Scalars are strings.
+
 ## Schema Validation for Markdown
 
 In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
 
 I haven't really found anything that says, for example, "This markdown document shall have one # Header and a 3 column table and nothing else."
 
 - [schema-markdown-js](https://craigahobbs.github.io/schema-markdown-js/language/) A json schema that happens to be using markdown as its syntax.
 
 ## Credits
 
 I copied the ATX-dictionary-like header parsing from [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
 ## Documentation
 
+- [Choosing a Library](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/choosing_a_library.md)
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
 ## Change Log
 
 - 1.1.0 - Basic functionality. See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for what is supported.
```

### Comparing `markpickle-1.5.0/markpickle/__init__.py` & `markpickle-1.5.1/markpickle/__init__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.0/markpickle/__main__.py` & `markpickle-1.5.1/markpickle/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 CLI support
 """
 import argparse
 import json
 import sys
 from pathlib import Path
+from typing import Any
 
 import markpickle
 
 if __name__ == "__main__":
 
     def run() -> None:
         """CLI entry point"""
@@ -21,15 +22,15 @@
             type=argparse.FileType(encoding="utf-8"),
             help="a Markdown file to be pretty-printed",
             default=sys.stdin,
         )
         parser.add_argument("outfile", nargs="?", type=Path, help="write the output of infile to outfile", default=None)
         options = parser.parse_args()
 
-        dump_args = {}
+        dump_args: dict[str, Any] = {}
 
         with options.infile as infile:
             try:
                 objs = (markpickle.load(infile),)
 
                 if options.outfile is None:
                     out = sys.stdout
```

### Comparing `markpickle-1.5.0/markpickle/atx_as_dictionary.py` & `markpickle-1.5.1/markpickle/atx_as_dictionary.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 """
 Code follows structure of
 
 https://github.com/njvack/markdown-to-json/blob/master/markdown_to_json/markdown_to_json.py#L58
 
 Reused with MIT license and credit to https://github.com/njvack
 """
-from typing import Any, Optional
+from typing import Any, Optional, cast
+
+from markpickle.mypy_types import MistuneTokenList, PossibleDictTypes
 
 
 def parse_outermost_dict(
-    token_list: list[dict[Optional[str], Any]], level: int
-) -> dict[Optional[str], list[dict[Optional[str], Any]]]:
+    token_list: list[PossibleDictTypes], level: int
+) -> PossibleDictTypes:  # was dict[Optional[str], list[dict[Optional[str], Any]]]
     """
     ATX headers, e.g. # Header, ## Subheader, can be used for a single set of nested dictionaries.
     """
-    candidate = recursive_part(level, token_list)
+    candidate = recursive_part(level, cast(MistuneTokenList, token_list))
 
     # recursive
     if isinstance(candidate, dict):
         for token_key, token_list in candidate.items():
-            candidate[token_key] = recursive_part(level + 1, token_list)
+            candidate[token_key] = recursive_part(level + 1, cast(MistuneTokenList, token_list))
 
     if candidate:
         return candidate
     # no ATX dict-like structures here.
-    return {None: token_list}
+    # mypy doesn't like this, but this is really just a hack to hold a list.
+    return cast(PossibleDictTypes, {None: token_list})
 
 
-def recursive_part(level: int, token_list: list[dict[str, Any]]):
+def recursive_part(level: int, token_list: MistuneTokenList):
     """Recursive part of processing headers"""
     candidate = {}
     key = None
-    between_values = []
+    between_values: list[dict[Optional[str], Any]] = []
     # First pass, yields candidate full of keys and lists of tokens
     for item in token_list:
         if item["type"] == "newline":
             # ignore whitespace
             continue
         if item["type"] == "heading" and item["level"] == level:
             if key:
                 candidate[key] = between_values
             key = "".join(_["text"] for _ in item["children"])
             between_values = []
             continue
 
-        between_values.append(item)
+        between_values.append(cast(dict[Optional[str], Any], item))
 
     # left overs
     if key and between_values:
         candidate[key] = between_values
     if not candidate:
         return between_values
     return candidate
```

### Comparing `markpickle-1.5.0/markpickle/binary_streams.py` & `markpickle-1.5.1/markpickle/binary_streams.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Add support for binary streams via images and data URLs
 """
 import base64
 import io
-from typing import Optional, Union
+from typing import Any, Optional
 
 from PIL import Image
 
 from markpickle.config_class import Config
 
 
 def bytes_to_markdown(key: Optional[str], value: bytes) -> str:
@@ -15,15 +15,16 @@
     Convert bytes to markdown image
     """
     base64_data = base64.b64encode(value).decode("utf-8")
     key = key or "bytes"
     return f"![{key}](data:application/octet-stream;base64,{base64_data})"
 
 
-def extract_bytes(src: str, config: Config) -> Optional[Union[bytes, Image]]:
+# Can't correctly type the return value because Pillow's Image module acts like module and class.
+def extract_bytes(src: str, config: Config) -> Any:
     """
     Extract bytes from a markdown image or pillow Image
     """
     if "," not in src:
         return None
 
     # Extract the mime type and data portion from the src
```

### Comparing `markpickle-1.5.0/markpickle/config_class.py` & `markpickle-1.5.1/markpickle/config_class.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.0/markpickle/deserialize.py` & `markpickle-1.5.1/markpickle/deserialize.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,31 @@
 
 Arbitrary strings might not pass or may pass but create values that still have unparsed markdown in them.
 """
 import datetime
 import io
 import logging
 import textwrap
-import urllib
+import urllib.parse
 from typing import Any, Generator, Optional, cast
 
 import mistune
 
 import markpickle.python_to_tables as python_to_tables
 from markpickle.atx_as_dictionary import parse_outermost_dict
 from markpickle.binary_streams import extract_bytes
 from markpickle.config_class import Config
-from markpickle.mypy_types import ListTypes, ScalarTypes, SerializableTypes
+from markpickle.mypy_types import (
+    DictTypes,
+    ListTypes,
+    MistuneTokenList,
+    PossibleDictTypes,
+    ScalarTypes,
+    SerializableTypes,
+)
 
 
 def loads(value: str, config: Optional[Config] = None, object_hook=None) -> SerializableTypes:
     """
     Convert certain markdown strings into simple Python types
 
     >>> loads("- a\\n- b\\n - c\\n")
@@ -84,31 +91,32 @@
             # that wasn't a date!
             pass
 
     # Return the value as a string if no other type matched
     return value
 
 
-def process_list(list_ast: Any, config: Config) -> Optional[ListTypes]:
+def process_list(list_ast: Any, config: Config) -> ListTypes:
     """Deserialize a markdown list in AST form"""
-    current_list = []
+    current_list: ListTypes = []
     for token in list_ast["children"]:
         if token["type"] == "list_item":
             for child in token["children"]:
                 if child["type"] == "block_text":
                     block_text = child
                     if block_text["children"][0]["type"] == "text":
                         # This fails if not all text!
                         current_value = ",".join(str(text.get("text")) for text in block_text["children"])
                         scalar = extract_scalar(current_value, config)
                         current_list.append(scalar)
                     elif block_text["children"][0]["type"] == "link":
                         # Doesn't handle title or text
                         url = urllib.parse.urlparse(block_text["children"][0]["link"])
-                        current_list.append(url)
+                        # HACK: Turn off type checking
+                        current_list.append(cast(Any, url))
                     else:
                         raise NotImplementedError(block_text["children"])
                 elif child["type"] == "list":
                     current_list.append(process_list(child, config))
                 else:
                     raise NotImplementedError(child["type"])
         else:
@@ -158,18 +166,18 @@
             break
         part.write(line)
         has_data = True
     if has_data:
         yield loads(part.read(), config, object_hook)
 
 
-def process_list_of_tokens(list_of_tokens: list[dict[str, Any]], config: Config):
+def process_list_of_tokens(list_of_tokens: MistuneTokenList, config: Config) -> Optional[SerializableTypes]:
     """Process a list of tokens to lists and scalars and so on."""
     # Tokens that are not ATX-dict-like headers
-    return_value = None
+    return_value: Optional[SerializableTypes] = None
     for token in list_of_tokens:
         if token["type"] == "newline":
             # Whitespace, no impact on datatype
             continue
 
         # if token["type"] == "heading" and current_key is None:
         #     # Dict key, value not found yet
@@ -182,15 +190,17 @@
         #     if not all("text" in _ for _ in token["children"]):
         #         print("uh oh")
         #     current_key = ",".join([_["text"] for _ in token["children"]])
         #     possible_dict[current_key] = None
         if token["type"] == "list":
             # Dict value of type list
             if token["children"][0]["type"] == "text":
-                return_value = [",".join(_["text"] for _ in item["children"]) for item in token["children"]]
+                return_value = cast(
+                    Optional[ListTypes], [",".join(_["text"] for _ in item["children"]) for item in token["children"]]
+                )
             elif token["children"][0]["type"] == "list_item":
                 return_value = process_list(token, config)
             else:
                 raise NotImplementedError()
 
         elif (
             token["type"] == "paragraph"
@@ -237,15 +247,16 @@
         #     current_key = None
         elif token["type"] == "block_code":
             # Treat block code as just more text, no "styling"
             continuation_value: str = token["text"]
             scalar = extract_scalar(continuation_value, config)
             # continuation of text
             if return_value:
-                return_value += "\n\n" + scalar
+                # mypy isn't sure if scalar is always a string.
+                return_value = str(return_value) + "\n\n" + str(scalar)
             else:
                 return_value = scalar
         elif token["type"] == "heading":
             # handled elsewhere?
             pass
         # else:
         #     raise NotImplementedError(token["type"])
@@ -291,15 +302,15 @@
 
     dict_wrapper = False
     # handle ATX-dict-like headers
     has_headers = any(True if item["type"] == "heading" else False for item in result)
     if has_headers:
         minimum = min(item["level"] if item["type"] == "heading" else 100000000 for item in result)
         outermost_dict = parse_outermost_dict(result, minimum)
-        outermost_dict = walk_dict(outermost_dict, config)
+        outermost_dict = walk_dict(cast(PossibleDictTypes, outermost_dict), config)
     else:
         dict_wrapper = True
         outermost_dict = {None: process_list_of_tokens(result, config)}
 
     # if possible_dict and possible_dict.get("python_type"):
     #     python_type = possible_dict.get("python_type")
     #     if constructor := globals().get(python_type):
@@ -310,40 +321,45 @@
 
     # really? do I misunderstand this?
     if object_hook:
         return object_hook(outermost_dict)
 
     if dict_wrapper:
         # Not ATX
-        return outermost_dict.get(None)
-    return outermost_dict
+        # mypy can't tell what is going on with dict_wrapper
+        return cast(SerializableTypes, outermost_dict.get(None))
+    # mypy can't tell what is going on with dict_wrapper
+    return cast(SerializableTypes, outermost_dict)
 
 
-def walk_dict(outermost_dict: dict[str, Any], config: Config):
+def walk_dict(outermost_dict: PossibleDictTypes, config: Config):
     """Process all lists of tokens found anywhere in this dictionary"""
     if isinstance(outermost_dict, dict):
         for current_key, list_or_dict_of_tokens in outermost_dict.items():
             if isinstance(list_or_dict_of_tokens, list):
-                outermost_dict[current_key] = process_list_of_tokens(list_or_dict_of_tokens, config)
+                outermost_dict[current_key] = process_list_of_tokens(
+                    cast(MistuneTokenList, list_or_dict_of_tokens), config
+                )
             elif isinstance(list_or_dict_of_tokens, dict):
-                outermost_dict[current_key] = walk_dict(list_or_dict_of_tokens, config)
+                outermost_dict[current_key] = walk_dict(cast(PossibleDictTypes, list_or_dict_of_tokens), config)
             else:
                 raise NotImplementedError("Expected list or dict")
     return outermost_dict
 
 
-def handle_series_of_children(config: Config, most_recent_key: str, possible_dict: dict[str, Any], series_of_children):
+def handle_series_of_children(config: Config, most_recent_key: str, possible_dict: DictTypes, series_of_children):
     """Handle a series of children, which may be text, images, or links."""
     for inner_token in series_of_children:
         if inner_token["type"] == "image":
             possible_dict[most_recent_key] += extract_bytes(inner_token["src"], config)
         elif inner_token["type"] in ("image", "link"):
             logging.warning("not handling image or link")
             continue
         if "text" not in inner_token:
             raise NotImplementedError("Not text like?")
         continuation_value: str = inner_token["text"]
         scalar = extract_scalar(continuation_value, config)
         # continuation of text
-        possible_dict[most_recent_key] += "\n\n" + scalar
+        # HACK: str() to make mypy happy.
+        possible_dict[most_recent_key] = str(possible_dict[most_recent_key]) + "\n\n" + str(scalar)
 
     return most_recent_key
```

### Comparing `markpickle-1.5.0/markpickle/python_to_tables.py` & `markpickle-1.5.1/markpickle/python_to_tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Function created with help of ChatGPT
 """
 import io
 import re
-from typing import Optional
+from typing import Optional, TextIO, Union, cast
 
-from markpickle.mypy_types import DictTypes, ScalarTypes
+from markpickle.mypy_types import ColumnsValuesTableType, DictTypes, ListTypes
 
 
-def list_of_dict_to_markdown(builder: io.IOBase, data: list[dict[str, ScalarTypes]], indent: int = 0):
+def list_of_dict_to_markdown(builder: Union[io.IOBase, TextIO], data: list[DictTypes], indent: int = 0) -> None:
     """
     Create a markdown table. Assumes dict are compatible (have similar keys) and shallow (no dicts of dict values)
     """
     row_id = 0
 
     column_widths: dict[str, int] = {}
     for schema in data:
@@ -71,40 +71,41 @@
         table = header + separator + row
     else:
         table = row
 
     return f"{indentation}{table}"
 
 
-def parse_table_to_list_of_dict(md_table: str) -> list[dict[str, str]]:
+def parse_table_to_list_of_dict(md_table: str) -> ListTypes:
     """Treat tables as list of dictionaries"""
     tuple_stuff = parse_table_with_regex(md_table)
     headers = tuple_stuff[0]
     rows = tuple_stuff[1:]
     dict_stuff = []
     for row in rows:
         dict_row = {}
         for column_id, column in enumerate(row):
             dict_row[headers[column_id]] = column
         dict_stuff.append(dict_row)
-    return dict_stuff
+    # mypy complains, but list[dict[str,str]] is a subtype of ListTypes!
+    return cast(ListTypes, dict_stuff)
 
 
-def parse_table_with_regex(md_table: str) -> list[tuple[str, ...]]:
+def parse_table_with_regex(md_table: str) -> ColumnsValuesTableType:
     """
     Created by ChatGPT 3.5 Turbo model.
 
     First element is headers, subsequent elements are rows.
     """
     rows = md_table.strip().split("\n")
     # Get the column names from the first row
     col_names = re.findall(r"\| *([^\|\n ]+) *", rows[0])
     num_cols = len(col_names)
     # Initialize the table data as a list of empty lists
-    table_data = [[] for i in range(num_cols)]
+    table_data: list[list[str]] = [[] for i in range(num_cols)]
     # Parse the remaining rows
     for row in rows[2:]:
         # Split the row into cells
         # cells = re.findall(r"\| *([^\|\n]+?) *", row)
         cells = [_.strip() for _ in row.strip().split("|")[1:-1]]
         # Check that the row has the correct number of cells
         if len(cells) != num_cols:
@@ -112,24 +113,24 @@
         # Add each cell to the appropriate column in the table data
         for i, cell in enumerate(cells):
             table_data[i].append(cell)
     # Combine the column names with the table data and return the result
     return [col_names] + list(zip(*table_data))
 
 
-def parse_table(md_table: str) -> list[tuple[str, ...]]:
+def parse_table(md_table: str) -> ColumnsValuesTableType:
     """
     Created by ChatGPT 3.5 Turbo model
     """
     rows = md_table.strip().split("\n")
     # Get the column names from the first row
     col_names = [cell.strip() for cell in rows[0].split("|")[1:-1]]
     num_cols = len(col_names)
     # Initialize the table data as a list of empty lists
-    table_data = [[] for i in range(num_cols)]
+    table_data: list[list[str]] = [[] for _ in range(num_cols)]
     # Parse the remaining rows
     for row in rows[2:]:
         # Split the row into cells
         cells = [cell.strip() for cell in row.split("|")[1:-1]]
         # Check that the row has the correct number of cells
         if len(cells) != num_cols:
             raise ValueError(f"Row has {len(cells)} cells, but expected {num_cols}")
```

### Comparing `markpickle-1.5.0/markpickle/serialize.py` & `markpickle-1.5.1/markpickle/serialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 This module provides functions to serialize many Python types to Markdown.
 """
 
 import datetime
 import io
 import logging
 import textwrap
-from typing import Callable, Optional, TextIO, Union
+from typing import Any, Callable, Optional, TextIO, Union, cast
 
 import markpickle.python_to_tables as python_to_tables
 import markpickle.simplify_types as simplify_types
 import markpickle.third_party_tables as third_party_tables
 from markpickle.binary_streams import bytes_to_markdown
 from markpickle.config_class import Config
-from markpickle.mypy_types import ScalarTypes, SerializableTypes
+from markpickle.mypy_types import DictTypes, SerializableTypes
 
 
 def dumps_all(
-    value: SerializableTypes,
+    value: list[SerializableTypes],
     config: Optional[Config] = None,
     default: Optional[Callable[[object], str]] = None,
 ) -> str:
     """Iterate value and serialize documents with horizontal lines between documents"""
     if default and config:
         config.default = default
     if default and not config:
@@ -85,15 +85,15 @@
     # results in a copy! ugh!
     if result.endswith("\n"):
         result = result[0:-1]
     return result
 
 
 def dump_all(
-    value: SerializableTypes,
+    value: list[SerializableTypes],
     stream: Union[io.IOBase, TextIO],
     config: Optional[Config] = None,
     default: Optional[Callable[[object], str]] = None,
 ) -> None:
     """Iterate value and serialize documents with horizontal lines between documents"""
     if default and config:
         config.default = default
@@ -104,15 +104,15 @@
     for document in value:
         if docs > 0:
             stream.write("---\n")
         dump(document, stream, config, default)
 
 
 def render_scalar(
-    builder: io.IOBase,
+    builder: Union[io.IOBase, TextIO],
     value: SerializableTypes,
     config: Config,
     indent: int = 0,
     header_level: int = 1,
 ) -> None:
     """Render a scalar value to Markdown"""
     if isinstance(value, (str, int, float, bool)):
@@ -163,21 +163,22 @@
         config = Config()
     # TODO: support formatting when stream can't go backwards- seek(0)
     builder = stream
     header_level = 1
 
     outtermost_type = type(value).__qualname__
 
-    if hasattr(value, "__getstate__") and value.__getstate__():
-        value = value.__getstate__()
+    # mypy doesn't use info from the hadattr check.
+    if hasattr(value, "__getstate__") and cast(Any, value).__getstate__():
+        value = cast(Any, value).__getstate__()
         if isinstance(value, dict) and config.serialize_include_python_type:
             value["python_type"] = outtermost_type
 
     if isinstance(value, list):
-        render_list(builder, value, config, indent=0, header_level=header_level)
+        render_list(builder, cast(list[SerializableTypes], value), config, indent=0, header_level=header_level)
     # elif isinstance(value, dict) and all(isinstance(_, dict) for _ in value.values()):
     #     for key, item in value.items():
     #         builder.write(f"{ '#' * header_level} {key}")
     #         render_dict(builder, item, config, indent=1, header_level=header_level)
     elif isinstance(value, dict):
         render_dict(builder, value, config, indent=0, header_level=header_level)
     elif isinstance(value, (str, int, float, bool)):
@@ -198,28 +199,29 @@
         image_text = bytes_to_markdown("bytes", value)
         builder.write(image_text)
     else:
         raise NotImplementedError()
 
 
 def render_dict(
-    builder: io.IOBase, value: SerializableTypes, config: Config, indent: int = 0, header_level: int = 1
+    builder: Union[io.IOBase, TextIO], value: DictTypes, config: Config, indent: int = 0, header_level: int = 1
 ) -> int:
     """Convert a Python dictionary to Markdown.
 
     Args:
         builder: The file-like object to write the Markdown to.
         value: The dictionary to be converted.
         config: Configuration object.
         indent: The current indentation level.
         header_level: The current header level.
 
     Returns:
         The current indentation level.
     """
+
     for key, item in value.items():
         if not isinstance(item, (list, dict, set)):
             # `- key : value` is not markdown
             if config.serialize_headers_are_dict_keys and indent == 0:
                 # headers dict keys. Can't nest.
                 minibuilder = io.StringIO()
                 render_scalar(minibuilder, item, config)
@@ -237,19 +239,20 @@
                     # headers dict keys. Can't nest.
                     header = f"{header_level * '#'} {key}\n"
                     builder.write(header)
                 else:
                     # Some markdown parsers treat 1 space indents as 0!
                     header = f"{indent * '  '}{config.list_bullet_style} {key}\n"
                     builder.write(header)
-                python_to_tables.list_of_dict_to_markdown(builder, item, indent)
+                # assume if first is dict, they all are
+                python_to_tables.list_of_dict_to_markdown(builder, cast(list[DictTypes], item), indent)
             else:
                 # Some markdown parsers treat 1 space indents as 0!
                 builder.write(f"{indent * '  '}{config.list_bullet_style} {key}\n")
-                render_list(builder, item, config, indent + 1)
+                render_list(builder, cast(list[SerializableTypes], item), config, indent + 1)
         elif isinstance(item, dict):
             builder.write(f"{'#' * header_level} {key}\n\n")
             if config.serialize_child_dict_as_table:
                 success = False
                 if config.serialize_tables_tabulate_style:
                     # pylint: disable=broad-exception-caught
                     try:
@@ -274,15 +277,19 @@
             except Exception as ex:
                 logging.warning(f"Tabulate can't handle it either: {ex}")
                 raise NotImplementedError() from ex
     return indent
 
 
 def render_list(
-    builder: io.IOBase, value: list[SerializableTypes], config: Config, indent: int = 0, header_level: int = 1
+    builder: Union[io.IOBase, TextIO],
+    value: list[SerializableTypes],
+    config: Config,
+    indent: int = 0,
+    header_level: int = 1,
 ) -> int:
     """
     Convert a Python list to Markdown.
 
     Args:
         builder: The file-like object to write the Markdown to.
         value: The list to be converted.
@@ -293,38 +300,39 @@
     Returns:
         The current indentation level.
     """
     if not value:
         return indent
     # This list is a list of dictionaries and we want a big table.
     if value and all(isinstance(_, dict) for _ in value):
-        python_to_tables.list_of_dict_to_markdown(builder, value, indent)
+        python_to_tables.list_of_dict_to_markdown(builder, cast(list[DictTypes], value), indent)
         return indent
 
     # The list is not of dictionaries or we don't want tables.
     for item in value:
         if not isinstance(item, (list, dict, set)):
             minibuilder = io.StringIO()
             render_scalar(minibuilder, item, config)
             seralialized_scalar = minibuilder.getvalue()
             builder.write(f"{indent * ' '}{config.list_bullet_style} {seralialized_scalar}\n")
         elif isinstance(item, list):
             if item and isinstance(item[0], dict):
-                python_to_tables.list_of_dict_to_markdown(builder, item, indent)
+                # assuming if the first is dict, they all are dict.
+                python_to_tables.list_of_dict_to_markdown(builder, cast(list[DictTypes], item), indent)
             else:
-                render_list(builder, item, config, indent + 1, header_level)
+                render_list(builder, cast(list[SerializableTypes], item), config, indent + 1, header_level)
         elif isinstance(item, dict):
             # We don't want tables or we'd have handled it above.
             render_dict(builder, item, config, indent + 1, header_level)
         else:
             raise NotImplementedError()
     return indent
 
 
-def unsafe_falsy_type(value: ScalarTypes) -> bool:
+def unsafe_falsy_type(value: SerializableTypes) -> bool:
     """
     Warn the user that blank structures don't have an equivalent in Markdown.
 
     Args:
         value: The value to be checked.
 
     Returns:
@@ -346,15 +354,15 @@
                 if any(key in ([], {}, (), "", "0", None) for key in inner.keys()):
                     return True
                 if any(dict_value in ([], {}, (), "", "0", None) for dict_value in inner.values()):
                     return True
     return False
 
 
-def unsafe_scalar_type(value: ScalarTypes) -> bool:
+def unsafe_scalar_type(value: SerializableTypes) -> bool:
     """
       Warn the user that non-string types won't round trip.
 
     Args:
         value: The value to be checked.
 
     Returns:
```

### Comparing `markpickle-1.5.0/markpickle/simplify_types.py` & `markpickle-1.5.1/markpickle/simplify_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.0/markpickle/split_file_code.py` & `markpickle-1.5.1/markpickle/split_file_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Generator
 
 
 def split_file(file: io.FileIO) -> Generator[str, None, None]:
     """
     Split a file into a list of lines.
     """
-    current_section = []
+    current_section: list[str] = []
     last_row_is_blank = False
 
     def is_separator(row: bytes) -> bool:
         """Is this a markdown horizontal rule"""
         return (
             (row.startswith(b"___") and all(_ == b"_" for _ in row))
             or (row.startswith(b"***") and all(_ == b"*" for _ in row))
```

### Comparing `markpickle-1.5.0/markpickle/third_party_tables.py` & `markpickle-1.5.1/markpickle/third_party_tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Use 3rd party library to create tables
 """
-import tabulate
+from typing import Any
 
-from markpickle.mypy_types import ScalarTypes
+import tabulate
 
 
 # from pytablewriter import MarkdownTableWriter
 #
 # def main():
 #     writer = MarkdownTableWriter(
 #         table_name="example_table",
@@ -16,15 +16,15 @@
 #             [0,   0.1,      "hoge", True,   0,      "2017-01-01 03:04:05+0900"],
 #             [2,   "-2.23",  "foo",  False,  None,   "2017-12-23 45:01:23+0900"],
 #             [3,   0,        "bar",  "true",  "inf", "2017-03-03 33:44:55+0900"],
 #             [-10, -9.9,     "",     "FALSE", "nan", "2017-01-01 00:00:00+0900"],
 #         ],
 #     )
 #     writer.write_table()
-def to_table_tablulate_style(value: list[list[ScalarTypes]]):
+def to_table_tablulate_style(value: Any) -> str:
     """
     The following tabular data types are supported:
 
     list of lists or another iterable of iterables
     list or another iterable of dicts (keys as columns)
     dict of iterables (keys as columns)
     list of dataclasses (Python 3.7+ only, field names as columns)
```

### Comparing `markpickle-1.5.0/markpickle/tool.py` & `markpickle-1.5.1/markpickle/tool.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.0/markpickle/unicode_formatting.py` & `markpickle-1.5.1/markpickle/unicode_formatting.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.5.0/pyproject.toml` & `markpickle-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markpickle"
-version = "1.5.0"
+version = "1.5.1"
 description = "Lossy python to markdown serializer"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -32,15 +32,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/matthewdeanmartin/markpickle/issues"
 "Change Log" = "https://github.com/matthewdeanmartin/markpickle/blob/main/CHANGES.md"
 
 [tool.poetry.dependencies]
 # DOM parser
-mistune = "*"
+mistune = "<3.0.0"
 # alternate formatter
 mdformat = "*"
 # support more types to table
 tabulate = "*"
 # image/binary support
 pillow = "*"
```

### Comparing `markpickle-1.5.0/PKG-INFO` & `markpickle-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markpickle
-Version: 1.5.0
+Version: 1.5.1
 Summary: Lossy python to markdown serializer
 Home-page: https://github.com/matthewdeanmartin/markpickle
 License: MIT
 Keywords: serializer,deserializer,markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
@@ -20,37 +20,51 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mdformat
-Requires-Dist: mistune
+Requires-Dist: mistune (<3.0.0)
 Requires-Dist: pillow
 Requires-Dist: tabulate
 Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/markpickle/issues
 Project-URL: Change Log, https://github.com/matthewdeanmartin/markpickle/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/matthewdeanmartin/markpickle
 Project-URL: Repository, https://github.com/matthewdeanmartin/markpickle
 Description-Content-Type: text/markdown
 
 # markpickle
 
-Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
+Markpickle is a Python library for lossy serialization of markdown to simple python data types and back. Imagine if markdown headers were used to define nested dictionaries and Markdown lists were python lists.
+
+It will create predictable markdown from a python object, but can't turn all markdown files into sensible python objects (for that use a markdown library that creates an AST). I created this because I wanted a way to turn json into Markdown. It is an accidental successor to [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
 For example this
 
 ```markdown
 - 1
 - 2
 ```
 
 becomes the python list `[1, 2]`
 
-Almost all markdown libraries use it as intended, as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data.
+```markdown
+# Cat
+## Name
+Ringo
+## Species
+Felix
+```
+
+becomes the python list `{"cat":{"Name":"Ringo","Species":"Felix"}`
+
+See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for representable types.
+
+Almost all markdown libraries use it as intended, as a way to generate HTML fragments from untrusted sources for insertion into some other HTML template. We are using it to represent data. See [guidance](docs/choosing_a_library.md) for which library make sense for you.
 
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/markpickle) [![Downloads](https://pepy.tech/badge/markpickle/month)](https://pepy.tech/project/markpickle/month)
 
 ______________________________________________________________________
 
 ## Installation
 
@@ -135,28 +149,44 @@
 
 [markdown-to-json](https://github.com/njvack/markdown-to-json) is the library most similar to markpickle, but is somewhat broken, unmaintained and depends on the unmaintained commonmark library.
 
 [mistune](https://pypi.org/project/mistune/) will turn markdown into an Abstract Syntax Tree. The AST is faithful representation of the Markdown, including concepts that have no semantic equivalent to python datatypes.
 
 [beautifulsoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) will let you navigate the HTML DOM. So you can turn the markdown into HTML, then parse with Beautiful Soup.
 
+## Representable Types
+
+There is one optional root dictionary representable with ATX headers, e.g. `#`, `##`, etc. Lists are nestable lists or dicts. For the most part, this looks like the types that JSON can represent.
+
+```python
+from typing import Union, TypeAlias
+import datetime
+import PIL
+MarkSerializable: TypeAlias = Union[
+    dict[str, "MarkSerializable"],
+    list["MarkSerializable"], str, int, float, bool, datetime, PIL.image, bytes, None]
+```
+
+The deserialized types is the same except all Scalars are strings.
+
 ## Schema Validation for Markdown
 
 In the case of a serialization library, you'd want something that would indicate if your markdown file will successfully deserialize back into python.
 
 I haven't really found anything that says, for example, "This markdown document shall have one # Header and a 3 column table and nothing else."
 
 - [schema-markdown-js](https://craigahobbs.github.io/schema-markdown-js/language/) A json schema that happens to be using markdown as its syntax.
 
 ## Credits
 
 I copied the ATX-dictionary-like header parsing from [markdown-to-json](https://github.com/njvack/markdown-to-json).
 
 ## Documentation
 
+- [Choosing a Library](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/choosing_a_library.md)
 - [Examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md)
 - [TODO](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/TODO.md)
 - [People solving similar problems on StackOverflow](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/stackoverflow.md)
 
 ## Change Log
 
 - 1.1.0 - Basic functionality. See [examples](https://github.com/matthewdeanmartin/markpickle/blob/main/docs/examples.md) for what is supported.
```

