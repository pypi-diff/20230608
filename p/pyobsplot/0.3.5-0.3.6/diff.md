# Comparing `tmp/pyobsplot-0.3.5.tar.gz` & `tmp/pyobsplot-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobsplot-0.3.5.tar", max compression
+gzip compressed data, was "pyobsplot-0.3.6.tar", max compression
```

## Comparing `pyobsplot-0.3.5.tar` & `pyobsplot-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.5/LICENSE
--rw-r--r--   0        0        0     4361 2023-06-06 12:48:48.704316 pyobsplot-0.3.5/README.md
--rw-r--r--   0        0        0     1303 2023-06-07 10:03:06.489355 pyobsplot-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-23 14:58:02.739444 pyobsplot-0.3.5/src/pyobsplot/__init__.py
--rw-r--r--   0        0        0     3428 2023-05-03 07:48:27.914955 pyobsplot-0.3.5/src/pyobsplot/data.py
--rw-r--r--   0        0        0     2116 2023-06-02 14:29:52.114261 pyobsplot-0.3.5/src/pyobsplot/jsdom.py
--rw-r--r--   0        0        0     2363 2023-04-14 11:09:43.659346 pyobsplot-0.3.5/src/pyobsplot/jsmodules.py
--rw-r--r--   0        0        0     6828 2023-06-06 12:24:31.708831 pyobsplot-0.3.5/src/pyobsplot/obsplot.py
--rw-r--r--   0        0        0     6158 2023-06-02 14:23:54.640414 pyobsplot-0.3.5/src/pyobsplot/parsing.py
--rw-r--r--   0        0        0      701 2023-06-07 10:04:52.584043 pyobsplot-0.3.5/src/pyobsplot/static/styles.css
--rw-r--r--   0        0        0  1348062 2023-06-07 10:04:52.580043 pyobsplot-0.3.5/src/pyobsplot/static/widget.js
--rw-r--r--   0        0        0     2771 2023-06-06 13:22:59.043780 pyobsplot-0.3.5/src/pyobsplot/utils.py
--rw-r--r--   0        0        0     1885 2023-06-02 14:31:27.382821 pyobsplot-0.3.5/src/pyobsplot/widget.py
--rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 pyobsplot-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.6/LICENSE
+-rw-r--r--   0        0        0     4361 2023-06-06 12:48:48.704316 pyobsplot-0.3.6/README.md
+-rw-r--r--   0        0        0     1303 2023-06-08 14:08:25.570442 pyobsplot-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-23 14:58:02.739444 pyobsplot-0.3.6/src/pyobsplot/__init__.py
+-rw-r--r--   0        0        0     3428 2023-06-08 13:58:25.559409 pyobsplot-0.3.6/src/pyobsplot/data.py
+-rw-r--r--   0        0        0     2116 2023-06-02 14:29:52.114261 pyobsplot-0.3.6/src/pyobsplot/jsdom.py
+-rw-r--r--   0        0        0     2363 2023-04-14 11:09:43.659346 pyobsplot-0.3.6/src/pyobsplot/jsmodules.py
+-rw-r--r--   0        0        0     6828 2023-06-06 12:24:31.708831 pyobsplot-0.3.6/src/pyobsplot/obsplot.py
+-rw-r--r--   0        0        0     6158 2023-06-02 14:23:54.640414 pyobsplot-0.3.6/src/pyobsplot/parsing.py
+-rw-r--r--   0        0        0      701 2023-06-08 14:00:43.500033 pyobsplot-0.3.6/src/pyobsplot/static/styles.css
+-rw-r--r--   0        0        0  1348137 2023-06-08 14:00:43.500033 pyobsplot-0.3.6/src/pyobsplot/static/widget.js
+-rw-r--r--   0        0        0     2771 2023-06-08 14:08:35.350543 pyobsplot-0.3.6/src/pyobsplot/utils.py
+-rw-r--r--   0        0        0     1635 2023-06-07 16:56:23.676710 pyobsplot-0.3.6/src/pyobsplot/widget.py
+-rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 pyobsplot-0.3.6/PKG-INFO
```

### Comparing `pyobsplot-0.3.5/LICENSE` & `pyobsplot-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/README.md` & `pyobsplot-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/pyproject.toml` & `pyobsplot-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobsplot"
-version = "0.3.5"
+version = "0.3.6"
 description = "Observable Plot in Jupyter notebooks and Quarto documents"
 authors = ["Julien Barnier <julien@nozav.org>"]
 license = "MIT"
 readme = "README.md"
 include = ["src/pyobsplot/static/*"]
 homepage = "https://github.com/juba/pyobsplot"
 documentation = "https://juba.github.io/pyobsplot"
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.urls]
 changelog = "https://github.com/juba/pyobsplot/blob/main/NEWS.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-anywidget = {extras = ["dev"], version = "^0.4.2"}
+anywidget = {extras = ["dev"], version = "^0.4.3"}
 pandas = ">=1.2.0"
 polars = ">=0.16.0"
 pyarrow = "^11.0.0"
 ipywidgets = ">=8.0.0"
 jupyterlab_widgets = ">=3.0.0"
 jupyterlab = ">=3.6.0"
 requests = "^2.28.2"
```

### Comparing `pyobsplot-0.3.5/src/pyobsplot/__init__.py` & `pyobsplot-0.3.6/src/pyobsplot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/data.py` & `pyobsplot-0.3.6/src/pyobsplot/data.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/jsdom.py` & `pyobsplot-0.3.6/src/pyobsplot/jsdom.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/jsmodules.py` & `pyobsplot-0.3.6/src/pyobsplot/jsmodules.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/obsplot.py` & `pyobsplot-0.3.6/src/pyobsplot/obsplot.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/parsing.py` & `pyobsplot-0.3.6/src/pyobsplot/parsing.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/static/styles.css` & `pyobsplot-0.3.6/src/pyobsplot/static/styles.css`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.5/src/pyobsplot/static/widget.js` & `pyobsplot-0.3.6/src/pyobsplot/static/widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -48419,15 +48419,24 @@
     let result = Array();
     for (let d of data) {
         if (d["pyobsplot-type"] == "DataFrame") {
             let value = d["value"];
             if (renderer == "jsdom") {
                 value = Buffer.from(value, "base64");
             }
-            result.push(tableFromIPC(value));
+            let table = tableFromIPC(value);
+            const date_columns = table.schema.fields.filter((d2) => d2.type.toString().startsWith("Timestamp")).map((d2) => d2.name);
+            table = Array.from(table);
+            table = table.map((d2) => {
+                for (let col of date_columns) {
+                    d2[col] = new Date(d2[col]);
+                }
+                return d2;
+            });
+            result.push(table);
         } else {
             result.push(d);
         }
     }
     return result;
 }
 
@@ -48533,34 +48542,26 @@
 
 // js/widget/widget.js
 window.d3 = src_exports;
 window.Plot = src_exports2;
 
 function render(view) {
     let spec = () => view.model.get("spec");
-    let theme = () => view.model.get("theme");
     let plot_div = document.createElement("div");
     plot_div.classList.add("pyobsplot-plot");
-    plot_div.classList.add(theme());
+    plot_div.classList.add(spec()["theme"]);
     let plot2 = generate_plot(spec(), "widget");
     plot_div.appendChild(plot2);
     view.el.appendChild(plot_div);
     view.model.on("change:spec", () => _onSpecValueChanged(view, view.el));
     view.model.on("change:theme", () => _onThemeValueChanged(view, view.el));
 }
 
 function _onSpecValueChanged(view, el) {
     let plot2 = el.querySelector(".pyobsplot-plot");
     plot2.replaceChildren();
     let spec = () => view.model.get("spec");
     plot2.appendChild(generate_plot(spec(), "widget"));
 }
-
-function _onThemeValueChanged(view, el) {
-    let plot2 = el.querySelector(".pyobsplot-plot");
-    let theme = () => view.model.get("theme");
-    plot2.classList.remove("light", "dark", "current");
-    plot2.classList.add(theme());
-}
 export {
     render
 };
```

### Comparing `pyobsplot-0.3.5/src/pyobsplot/utils.py` & `pyobsplot-0.3.6/src/pyobsplot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 
 # Output directory of esbuild
 bundler_output_dir = pathlib.Path(__file__).parent / "static"
 
 # Minimum npm package version
-min_npm_version = "0.3.5"
+min_npm_version = "0.3.6"
 
 # Allowed default values
 allowed_defaults = [
     "marginTop",
     "marginRight",
     "marginBottom",
     "marginLeft",
```

### Comparing `pyobsplot-0.3.5/src/pyobsplot/widget.py` & `pyobsplot-0.3.6/src/pyobsplot/widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Obsplot widget handling.
 """
 
 
 import anywidget
 import traitlets
 
-from .utils import bundler_output_dir, available_themes, default_theme
+from .utils import bundler_output_dir, default_theme
 from .parsing import SpecParser
 
 
 class ObsplotWidget(anywidget.AnyWidget):
     """Obsplot widget class.
 
     It inherits from anywidget.Anywidget.
@@ -27,34 +27,31 @@
         bundler_output_dir / "widget.js", start_thread=False
     )
     _css = anywidget._file_contents.FileContents(  # type: ignore
         bundler_output_dir / "styles.css", start_thread=False
     )
     # spec traitlet : plot specification
     spec = traitlets.Dict().tag(sync=True)
-    # theme traitlet : plot theme (dark, light or current)
-    theme = traitlets.Unicode().tag(sync=True)
 
     def __init__(
         self, spec, theme: str = default_theme, default: dict = {}, debug: bool = False
     ):
         """Obsplot widget constructor."""
         self._debug = debug
         self._default = default
+        self._theme = theme
         # Init widget
-        super().__init__(spec=spec, theme=theme)
+        super().__init__(spec=spec)
 
     @traitlets.validate("spec")
     def _validate_spec(self, proposal):
         spec = proposal["value"]
         parser = SpecParser(renderer="widget", default=self._default)
         parser.spec = spec
         code = parser.parse_spec()
-        spec = {"data": parser.serialize_data(), "code": code, "debug": self._debug}
+        spec = {
+            "data": parser.serialize_data(),
+            "code": code,
+            "debug": self._debug,
+            "theme": self._theme,
+        }
         return spec
-
-    @traitlets.validate("theme")
-    def _validate_theme(self, proposal):
-        new_theme = proposal["value"]
-        if new_theme not in available_themes:
-            new_theme = default_theme
-        return new_theme
```

### Comparing `pyobsplot-0.3.5/PKG-INFO` & `pyobsplot-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobsplot
-Version: 0.3.5
+Version: 0.3.6
 Summary: Observable Plot in Jupyter notebooks and Quarto documents
 Home-page: https://github.com/juba/pyobsplot
 License: MIT
 Author: Julien Barnier
 Author-email: julien@nozav.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Dist: anywidget[dev] (>=0.4.2,<0.5.0)
+Requires-Dist: anywidget[dev] (>=0.4.3,<0.5.0)
 Requires-Dist: ipywidgets (>=8.0.0)
 Requires-Dist: jupyterlab (>=3.6.0)
 Requires-Dist: jupyterlab_widgets (>=3.0.0)
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: polars (>=0.16.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

