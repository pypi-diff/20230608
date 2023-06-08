# Comparing `tmp/jupyter_echarts-0.1.tar.gz` & `tmp/jupyter_echarts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_echarts-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jupyter_echarts-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jupyter_echarts-0.1.tar` & `jupyter_echarts-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1067 2023-06-07 19:17:58.935620 jupyter_echarts-0.1/LICENSE
--rw-r--r--   0        0        0     2331 2023-06-07 19:22:44.191555 jupyter_echarts-0.1/jupyter_echarts.py
--rw-r--r--   0        0        0      258 2023-06-07 19:22:22.163560 jupyter_echarts-0.1/pyproject.toml
--rw-r--r--   0        0        0      141 1970-01-01 00:00:00.000000 jupyter_echarts-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-07 19:17:58.935620 jupyter_echarts-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2310 2023-06-08 04:18:12.960207 jupyter_echarts-0.1.7/jupyter_echarts.py
+-rw-r--r--   0        0        0      278 2023-06-08 06:09:23.613530 jupyter_echarts-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      143 1970-01-01 00:00:00.000000 jupyter_echarts-0.1.7/PKG-INFO
```

### Comparing `jupyter_echarts-0.1/LICENSE` & `jupyter_echarts-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_echarts-0.1/jupyter_echarts.py` & `jupyter_echarts-0.1.7/jupyter_echarts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Use echarts in jupyter!"""
 
-__version__ = "0.1"
-
 ECHARTS_CDN = "https://cdn.jsdelivr.net/npm/echarts@5.3.2/dist/echarts.min"
 ECHARTS_REQUIREJS_CONF = f"requirejs.config({{paths: {{echarts: '{ECHARTS_CDN}',}}}});"
 ECHARTS_TEMPLATE = f"""
     <div id="{{ID}}" style="width: {{WIDTH}};height:{{HEIGHT}};"></div>
     <script type="module">
     {ECHARTS_REQUIREJS_CONF}    
     requirejs(["echarts"], (echarts) => {{
```

