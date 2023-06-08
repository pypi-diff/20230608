# Comparing `tmp/json_explorer-0.1.0.tar.gz` & `tmp/json_explorer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_explorer-0.1.0.tar", max compression
+gzip compressed data, was "json_explorer-0.1.1.tar", max compression
```

## Comparing `json_explorer-0.1.0.tar` & `json_explorer-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-06-07 20:20:14.719967 json_explorer-0.1.0/LICENSE
--rw-r--r--   0        0        0     2211 2023-06-07 20:20:14.719967 json_explorer-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-07 20:20:14.719967 json_explorer-0.1.0/json_explorer/__init__.py
--rw-r--r--   0        0        0       30 2023-06-07 20:20:14.719967 json_explorer-0.1.0/json_explorer/__main__.py
--rw-r--r--   0        0        0     2055 2023-06-07 20:20:14.719967 json_explorer-0.1.0/json_explorer/cli.py
--rw-r--r--   0        0        0    13487 2023-06-07 20:20:14.723967 json_explorer-0.1.0/json_explorer/explore.py
--rw-r--r--   0        0        0     3602 2023-06-07 20:20:14.723967 json_explorer-0.1.0/json_explorer/style.css
--rw-r--r--   0        0        0     1160 2023-06-07 20:20:14.723967 json_explorer-0.1.0/json_explorer/template.html
--rw-r--r--   0        0        0     1684 2023-06-07 20:20:40.944789 json_explorer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 json_explorer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-08 02:01:38.130294 json_explorer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2211 2023-06-08 02:01:38.130294 json_explorer-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 02:01:38.130294 json_explorer-0.1.1/json_explorer/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-08 02:01:38.130294 json_explorer-0.1.1/json_explorer/__main__.py
+-rw-r--r--   0        0        0     2593 2023-06-08 02:01:38.134294 json_explorer-0.1.1/json_explorer/cli.py
+-rw-r--r--   0        0        0   220023 2023-06-08 02:01:38.134294 json_explorer-0.1.1/json_explorer/example1.jsonl
+-rw-r--r--   0        0        0    14065 2023-06-08 02:01:38.134294 json_explorer-0.1.1/json_explorer/explore.py
+-rw-r--r--   0        0        0     3602 2023-06-08 02:01:38.134294 json_explorer-0.1.1/json_explorer/style.css
+-rw-r--r--   0        0        0     1160 2023-06-08 02:01:38.134294 json_explorer-0.1.1/json_explorer/template.html
+-rw-r--r--   0        0        0     1683 2023-06-08 02:02:00.270586 json_explorer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 json_explorer-0.1.1/PKG-INFO
```

### Comparing `json_explorer-0.1.0/LICENSE` & `json_explorer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json_explorer-0.1.0/README.md` & `json_explorer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `json_explorer-0.1.0/json_explorer/cli.py` & `json_explorer-0.1.1/json_explorer/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import json
 import sys
 import threading
 import webbrowser
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
-from .explore import TripleCounter
+from .explore import THIS_DIR, TripleCounter
 
 
 def start_browser(server_ready_event, url):
     server_ready_event.wait()
     webbrowser.open(url)
 
 
@@ -17,27 +17,51 @@
     with open(filename) as infile:
         for line in infile:
             yield json.loads(line)
 
 
 def main():
     parser = argparse.ArgumentParser(
-        prog="ProgramName",
-        description="What the program does",
-        epilog="Text at the bottom of help",
+        description="visualize the structure and type of a group of JSONs",
     )
     parser.add_argument(
         "filename",
         help="filename of a file in JSON Lines format",
+        nargs="?",
+        default=None,
+    )
+    parser.add_argument(
+        "--example",
+        help="run with test data",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-p",
+        "--port",
+        default=8001,
+        type=int,
+        help="port for server (default 8001)",
+    )
+    parser.add_argument(
+        "-n",
+        "--no-serve",
+        help="write HTML to stdout instead of opening browser",
+        action="store_true",
     )
-    parser.add_argument("-p", "--port", default=8001, type=int, help="port for server (default 8001)")
-    parser.add_argument("-n", "--no-serve", help="write HTML to stdout instead of serving", action="store_true")
     args = parser.parse_args()
 
-    counter = TripleCounter.from_objects(jsonl_iterator(args.filename))
+    filename = args.filename
+    if not args.example and not args.filename:
+        parser.error("filename is required (unless --example is given)")
+    elif args.example and args.filename:
+        parser.error("can't pass both filename and --example")
+    elif args.example:
+        filename = THIS_DIR / "example1.jsonl"
+
+    counter = TripleCounter.from_objects(jsonl_iterator(filename))
     response_text = counter.html()
 
     if args.no_serve:
         print(response_text)
         return
 
     class RequestHandler(BaseHTTPRequestHandler):
```

### Comparing `json_explorer-0.1.0/json_explorer/explore.py` & `json_explorer-0.1.1/json_explorer/explore.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,19 @@
 
     def escape(self, string, truncate_length=140):
         raw = repr(string)
         if len(raw) > truncate_length:
             first = raw[: truncate_length // 2]
             second = raw[-(truncate_length // 2) :]
             length = len(raw) - len(first) - len(second)
-            return html.escape(first) + f'<span class="truncated" data-length="{length}"></span>' + html.escape(second)
+            return (
+                html.escape(first)
+                + f'<span class="truncated" data-length="{length}"></span>'
+                + html.escape(second)
+            )
         else:
             return html.escape(raw)
 
     def _counter_summary_html(self, type_, counter):
         value_or_length = "value"
         if type_ == "list":
             value_or_length = "length"
@@ -168,15 +172,20 @@
 
         if len(counter) == 1:
             value, count = list(counter.items())[0]
             return f"<p>Always {value_or_length} {self.escape(value)}</p>"
         elif len(counter) <= 5:
             return (
                 f"<p>{value_or_length} is "
-                + oxford_join([f"{self.escape(v)} {self.format_count(c)}" for v, c in counter.most_common()])
+                + oxford_join(
+                    [
+                        f"{self.escape(v)} {self.format_count(c)}"
+                        for v, c in counter.most_common()
+                    ]
+                )
                 + "</p>"
             )
         else:
             n_unique = len(counter)
             min_ = min(counter)
             min_count = counter[min_]
             max_ = max(counter)
@@ -201,15 +210,19 @@
             inside = f"{count:,}"
         else:
             n_unique = len(counter)
             values = list(counter.most_common(3))
             if value_type == "NoneType":
                 inside = f"{count:,}"
             elif value_type == "bool":
-                inside = f"{count:,}, always {values[0][0]!r}" if n_unique == 1 else f"{count:,}"
+                inside = (
+                    f"{count:,}, always {values[0][0]!r}"
+                    if n_unique == 1
+                    else f"{count:,}"
+                )
             elif value_type == "int" or value_type == "number":
                 if n_unique == 1:
                     inside = f"{count:,}, always {values[0][0]!r}"
                 elif n_unique <= 3:
                     values_string = oxford_join([f"{k!r}" for k, v in values])
                     inside = f"{count:,}, either {values_string}"
                 else:
@@ -217,57 +230,70 @@
             elif value_type == "str":
                 MAX_LENGTH_TO_SHOW = 30
                 if n_unique == 1:
                     n_chars = len(values[0][0])
                     if n_chars <= MAX_LENGTH_TO_SHOW:
                         inside = f"{count:,}, always {values[0][0]!r}"
                     else:
-                        inside = f"{count:,}, {n_unique:,} unique {n_chars:,} characters"
+                        inside = (
+                            f"{count:,}, {n_unique:,} unique"
+                            f" {n_chars:,} characters"
+                        )
                 elif n_unique <= 3:
                     combined = "".join(k for k, v in values)
                     if len(combined) <= MAX_LENGTH_TO_SHOW:
-                        values_string = oxford_join([f"{k!r}" for k, v in values])
+                        values_string = oxford_join(
+                            [f"{k!r}" for k, v in values]
+                        )
                         inside = f"{count:,}, either {values_string}"
                     else:
                         inside = f"{count:,}, {n_unique:,} unique"
 
                 else:
                     inside = f"{count:,}, {n_unique:,} unique"
                 pass
             elif value_type == "list":
                 if n_unique == 1:
                     inside = f"{count:,}, always length {values[0][0]:,}"
                 elif n_unique == 2:
                     values_string = oxford_join([f"{k:,}" for k, v in values])
                     inside = f"{count:,}, length either {values_string}"
                 else:
-                    inside = f"{count:,}, length between {min(counter):,} and {max(counter):,}"
+                    inside = (
+                        f"{count:,}, length between {min(counter):,} and"
+                        f" {max(counter):,}"
+                    )
             elif value_type == "dict":
                 if n_unique == 1:
                     inside = f"{count:,}, always {values[0][0]:,} properties"
                 elif n_unique == 2:
                     values_string = oxford_join([f"{k:,}" for k, v in values])
                     inside = f"{count:,}, either {values_string} properties"
                 else:
-                    inside = f"{count:,}, between {min(counter):,} and {max(counter):,} properties"
+                    inside = (
+                        f"{count:,}, between {min(counter):,} and"
+                        f" {max(counter):,} properties"
+                    )
             else:
                 raise ValueError(f"unknown type {value_type!r}")
         return outside.format(inside)
 
     def summary_html(self):
         if "float" in self["value_or_length_counter"]:
             float_counter = self["value_or_length_counter"].pop("float")
             int_counter = self["value_or_length_counter"].pop("int", {})
             for k, v in int_counter.items():
                 float_counter[k] += v
             self["value_or_length_counter"]["number"] = float_counter
 
         html = "<div>"
         for type_, counter in self["value_or_length_counter"].items():
-            html += f"<h3>{TYPE_TRANSLATE[type_]} {self.format_count(counter.total())}</h3>"
+            html += (
+                f"<h3>{TYPE_TRANSLATE[type_]} {self.format_count(counter.total())}</h3>"
+            )
             html += self._counter_summary_html(type_, counter)
         html += "</div>"
         return html
 
     def details_html(self):
         html = f"""
 <dialog id="{self.jmespath()}"><form method="dialog"><h2 class="jmespath">{self.jmespath()}</h2><div>{self.summary_html()}</div><button>Close</button></form></dialog>"""
```

### Comparing `json_explorer-0.1.0/json_explorer/style.css` & `json_explorer-0.1.1/json_explorer/style.css`

 * *Files identical despite different names*

### Comparing `json_explorer-0.1.0/json_explorer/template.html` & `json_explorer-0.1.1/json_explorer/template.html`

 * *Files identical despite different names*

### Comparing `json_explorer-0.1.0/pyproject.toml` & `json_explorer-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json_explorer"
-version = "0.1.0"
+version = "0.1.1"
 description = "Explore the structure of a bunch of jsons"
 authors = ["Mike Stringer <fmike.stringer.internet@gmail.com>"]
 repository = "https://github.com/stringertheory/json-explorer"
 documentation = "https://stringertheory.github.io/json-explorer/"
 readme = "README.md"
 packages = [
   {include = "json_explorer"}
@@ -29,15 +29,15 @@
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 120
+line-length = 80
 target-version = ['py37']
 preview = true
 
 [tool.ruff]
 target-version = "py37"
 line-length = 120
 fix = true
```

### Comparing `json_explorer-0.1.0/PKG-INFO` & `json_explorer-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-explorer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Explore the structure of a bunch of jsons
 Home-page: https://github.com/stringertheory/json-explorer
 Author: Mike Stringer
 Author-email: fmike.stringer.internet@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

