# Comparing `tmp/pyviz_comms-2.3.0.tar.gz` & `tmp/pyviz_comms-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyviz_comms-2.3.0.tar", last modified: Wed May 24 18:22:47 2023, max compression
+gzip compressed data, was "dist/pyviz_comms-2.3.1.tar", last modified: Thu Jun  8 14:10:12 2023, max compression
```

## Comparing `pyviz_comms-2.3.0.tar` & `pyviz_comms-2.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/
--rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-24 18:22:45.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 18:22:45.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/445.482ccf5e3a3952a8b415.js
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/remoteEntry.febb837ab3b6ef743bf7.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 18:22:45.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/notebook.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/pyviz_comms/tests/test_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/pyviz_comms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:22:47.000000 pyviz_comms-2.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/icons.ts
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/manager.ts
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/plugin.ts
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/preview.tsx
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/renderer.ts
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/src/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-24 18:12:07.000000 pyviz_comms-2.3.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/
+-rw-r--r--   0 runner    (1001) docker     (123)    19946 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 14:10:10.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 14:10:10.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/445.8dcc8508e7796b2d5680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/remoteEntry.75aa6a6489839cbfc067.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 14:10:10.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/notebook.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/pyviz_comms/tests/test_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/pyviz_comms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:10:12.000000 pyviz_comms-2.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/icons.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/manager.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/plugin.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/preview.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/renderer.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/src/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 14:00:00.000000 pyviz_comms-2.3.1/tsconfig.json
```

### Comparing `pyviz_comms-2.3.0/LICENSE.txt` & `pyviz_comms-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/PKG-INFO` & `pyviz_comms-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz_comms
-Version: 2.3.0
+Version: 2.3.1
 Summary: Bidirectional communication for the HoloViz ecosystem.
 Home-page: https://holoviz.org
 Author: Philipp Rudiger
 Author-email: philipp.jfr@gmail.com
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
```

### Comparing `pyviz_comms-2.3.0/README.md` & `pyviz_comms-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/package.json` & `pyviz_comms-2.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.3.1'"}*

```diff
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.3.0"
+    "version": "2.3.1"
 }
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms/__init__.py` & `pyviz_comms-2.3.1/pyviz_comms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/pyviz_comms/labextension/package.json` & `pyviz_comms-2.3.1/pyviz_comms/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757936507936508%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.75aa6a6489839cbfc067.js'}}",*

 * * "'version'": "'2.3.1'"}*

```diff
@@ -40,15 +40,15 @@
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/holoviz/pyviz_comms",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.febb837ab3b6ef743bf7.js",
+            "load": "static/remoteEntry.75aa6a6489839cbfc067.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "pyviz_comms/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
             "@jupyter-widgets/base": {
@@ -103,9 +103,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.3.0"
+    "version": "2.3.1"
 }
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig` & `pyviz_comms-2.3.1/pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.3.1'"}*

```diff
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.3.0"
+    "version": "2.3.1"
 }
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms/labextension/static/445.482ccf5e3a3952a8b415.js` & `pyviz_comms-2.3.1/pyviz_comms/labextension/static/445.8dcc8508e7796b2d5680.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,29 @@
 "use strict";
 (self.webpackChunk_pyviz_jupyterlab_pyviz = self.webpackChunk_pyviz_jupyterlab_pyviz || []).push([
     [445], {
         445: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => N
+                default: () => M
             });
-            var o = n(123),
-                i = n(687),
-                s = n(33),
-                r = n(142),
-                a = n(986),
-                d = n(38),
-                l = n(344),
+            var o = n(779),
+                i = n(175),
+                s = n(764),
+                r = n(58),
+                a = n(263),
+                d = n(85),
+                l = n(308),
                 c = n(923),
-                m = n(502);
-            const h = new m.LabIcon({
-                name: "@pyviz/jupyterlab_pyviz:panel",
-                svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   xmlns:dc="http://purl.org/dc/elements/1.1/"\n   xmlns:cc="http://creativecommons.org/ns#"\n   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"\n   xmlns:svg="http://www.w3.org/2000/svg"\n   xmlns="http://www.w3.org/2000/svg"\n   width="63.84808mm"\n   height="63.912464mm"\n   viewBox="0 0 63.84808 63.912464"\n   version="1.1"\n   id="svg867">\n  <defs\n     id="defs861" />\n  <metadata\n     id="metadata864">\n    <rdf:RDF>\n      <cc:Work\n         rdf:about="">\n        <dc:format>image/svg+xml</dc:format>\n        <dc:type\n           rdf:resource="http://purl.org/dc/dcmitype/StillImage" />\n        <dc:title></dc:title>\n      </cc:Work>\n    </rdf:RDF>\n  </metadata>\n  <g\n     id="layer1"\n     transform="translate(-41.403339,-133.59734)">\n    <g\n       id="g5614"\n       transform="matrix(0.56444446,0,0,0.56444446,819.73897,-509.17309)">\n      <rect\n         y="1138.7665"\n         x="-1378.941"\n         height="113.23074"\n         width="113.11668"\n         id="rect4136-8-8-1"\n         style="opacity:1;fill:#0072b5;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n         ry="9.4330282" />\n      <g\n         id="g5603">\n        <g\n           id="g5591">\n          <rect\n             y="1165.5731"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-3-71"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1169.5731"\n             cx="-1341.4192"\n             id="path4355-79-2"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n        <g\n           id="g5595">\n          <rect\n             y="1191.3817"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-5-1-0"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1195.3817"\n             cx="-1305.4111"\n             id="path4355-7-3-7"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n        <g\n           id="g5599">\n          <rect\n             y="1217.1904"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-54-6-2"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:1;stroke-miterlimit:4;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1221.1904"\n             cx="-1341.4274"\n             id="path4355-3-9-8"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n      </g>\n    </g>\n  </g>\n</svg>\n'
-            });
-            class p {
+                m = n(667);
+            const h = '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   xmlns:dc="http://purl.org/dc/elements/1.1/"\n   xmlns:cc="http://creativecommons.org/ns#"\n   xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"\n   xmlns:svg="http://www.w3.org/2000/svg"\n   xmlns="http://www.w3.org/2000/svg"\n   width="63.84808mm"\n   height="63.912464mm"\n   viewBox="0 0 63.84808 63.912464"\n   version="1.1"\n   id="svg867">\n  <defs\n     id="defs861" />\n  <metadata\n     id="metadata864">\n    <rdf:RDF>\n      <cc:Work\n         rdf:about="">\n        <dc:format>image/svg+xml</dc:format>\n        <dc:type\n           rdf:resource="http://purl.org/dc/dcmitype/StillImage" />\n        <dc:title></dc:title>\n      </cc:Work>\n    </rdf:RDF>\n  </metadata>\n  <g\n     id="layer1"\n     transform="translate(-41.403339,-133.59734)">\n    <g\n       id="g5614"\n       transform="matrix(0.56444446,0,0,0.56444446,819.73897,-509.17309)">\n      <rect\n         y="1138.7665"\n         x="-1378.941"\n         height="113.23074"\n         width="113.11668"\n         id="rect4136-8-8-1"\n         style="opacity:1;fill:#0072b5;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none"\n         ry="9.4330282" />\n      <g\n         id="g5603">\n        <g\n           id="g5591">\n          <rect\n             y="1165.5731"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-3-71"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1169.5731"\n             cx="-1341.4192"\n             id="path4355-79-2"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n        <g\n           id="g5595">\n          <rect\n             y="1191.3817"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-5-1-0"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1195.3817"\n             cx="-1305.4111"\n             id="path4355-7-3-7"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n        <g\n           id="g5599">\n          <rect\n             y="1217.1904"\n             x="-1361.4104"\n             height="8"\n             width="78.055412"\n             id="rect4327-54-6-2"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:1;stroke-miterlimit:4;stroke-dasharray:none" />\n          <circle\n             r="9"\n             cy="1221.1904"\n             cx="-1341.4274"\n             id="path4355-3-9-8"\n             style="opacity:1;fill:#eeeeee;fill-opacity:1;stroke:none;stroke-width:4;stroke-miterlimit:1;stroke-dasharray:none" />\n        </g>\n      </g>\n    </g>\n  </g>\n</svg>\n',
+                p = new m.LabIcon({
+                    name: "@pyviz/jupyterlab_pyviz:panel",
+                    svgstr: h
+                });
+            class u {
                 constructor(e, t) {
                     this._context = e, this._wManager = t, this._comm = null, e.sessionContext.statusChanged.connect(((e, t) => {
                         "restarting" !== t && "dead" !== t || (this._comm = null)
                     }), this)
                 }
                 get context() {
                     return this._context
@@ -37,23 +38,38 @@
                 get isDisposed() {
                     return null === this._context
                 }
                 dispose() {
                     this.isDisposed || (this._context = null, this._comm = null)
                 }
             }
-            var u = n(819),
+            var g = n(676),
                 _ = n(526),
-                g = n(840),
-                w = n(271);
-            const v = new _.Token("@pyviz/jupyterlab_pyviz:IPanelPreviewTracker");
-            class y extends u.DocumentWidget {
+                w = n(840),
+                v = n(271);
+            const y = new _.Token("@pyviz/jupyterlab_pyviz:IPanelPreviewTracker");
+            class f extends s.IFrame {
+                constructor(e = {}) {
+                    super(e), this.srcdoc = e.srcdoc || null
+                }
+                get srcdoc() {
+                    return this._srcdoc
+                }
+                set srcdoc(e) {
+                    this._srcdoc = e;
+                    const t = this.node.querySelector("iframe");
+                    null != e && (t.setAttribute("srcdoc", e), t.addEventListener("load", (() => t.removeAttribute("srcdoc"))))
+                }
+            }
+            const x = `\n<!DOCTYPE html>\n<html>\n<head>\n  <title>Jupyter Kernel Starting</title>\n  <style>\n    body {\n      display: flex;\n      align-items: center;\n      justify-content: center;\n      flex-direction: column;\n      height: 100vh;\n      background-color: #f7f7f7;\n      font-family: Futura;\n    }\n\n    .loading-container {\n      display: flex;\n      align-items: center;\n      justify-content: center;\n      margin: 20px 0;\n    }\n\n    .loading-indicator {\n      width: 100px;\n      height: 100px;\n      border: 8px solid rgb(48, 112, 146);\n      border-top-color: #f7f7f7;\n      border-radius: 50%;\n      animation: spin 1s infinite linear;\n    }\n\n    @keyframes spin {\n      from {\n        transform: rotate(0deg);\n      }\n      to {\n        transform: rotate(360deg);\n      }\n    }\n  </style>\n</head>\n<body>\n  ${h}\n  <h1>Panel Preview Launching...</h1>\n  <div class="loading-container">\n    <div class="loading-indicator"></div>\n  </div>\n</body>\n</html>\n`;
+            class k extends g.DocumentWidget {
                 constructor(e) {
                     super(Object.assign(Object.assign({}, e), {
-                        content: new s.IFrame({
+                        content: new f({
+                            srcdoc: x,
                             sandbox: ["allow-same-origin", "allow-scripts", "allow-downloads"]
                         })
                     })), window.onmessage = e => {
                         var t, n, o, i, s;
                         switch (null === (t = e.data) || void 0 === t ? void 0 : t.level) {
                             case "debug":
                                 console.debug(...null === (n = e.data) || void 0 === n ? void 0 : n.msg);
@@ -72,84 +88,83 @@
                         }
                     };
                     const {
                         getPanelUrl: t,
                         context: n,
                         renderOnSave: o
                     } = e;
-                    this.content.url = t(n.path), this.content.title.icon = h, this._renderOnSave = null != o && o, n.pathChanged.connect((() => {
+                    this.content.url = t(n.path), this.content.title.icon = p, this._renderOnSave = null != o && o, n.pathChanged.connect((() => {
                         this.content.url = t(n.path)
                     }));
                     const i = new s.ToolbarButton({
                             icon: m.refreshIcon,
                             tooltip: "Reload Preview",
                             onClick: () => {
                                 this.reload()
                             }
                         }),
-                        r = s.ReactWidget.create(w.createElement("label", {
+                        r = s.ReactWidget.create(v.createElement("label", {
                             className: "jp-PanelPreview-renderOnSave"
-                        }, w.createElement("input", {
-                            style: {
-                                verticalAlign: "middle"
-                            },
+                        }, v.createElement("input", {
                             name: "renderOnSave",
                             type: "checkbox",
                             defaultChecked: o,
                             onChange: e => {
                                 this._renderOnSave = e.target.checked
                             }
-                        }), "Render on Save"));
+                        }), v.createElement("span", null, "Render on Save")));
                     this.toolbar.addItem("reload", i), n && (this.toolbar.addItem("renderOnSave", r), n.ready.then((() => {
                         n.fileChanged.connect((() => {
                             this.renderOnSave && this.reload()
                         }))
                     })))
                 }
                 dispose() {
-                    this.isDisposed || (super.dispose(), g.Signal.clearData(this))
+                    this.isDisposed || (super.dispose(), w.Signal.clearData(this))
                 }
                 reload() {
                     const e = this.content.node.querySelector("iframe");
-                    null != e.contentWindow && e.contentWindow.location.reload()
+                    null != e.contentWindow && (e.parentElement.classList.add("jp-PanelPreview-loading"), e.contentWindow.location.reload(), e.addEventListener("load", (() => {
+                        e.parentElement.classList.remove("jp-PanelPreview-loading")
+                    })))
                 }
                 get renderOnSave() {
                     return this._renderOnSave
                 }
                 set renderOnSave(e) {
                     this._renderOnSave = e
                 }
             }
-            class x extends u.ABCWidgetFactory {
+            class b extends g.ABCWidgetFactory {
                 constructor(e, t) {
                     super(t), this.getPanelUrl = e, this.defaultRenderOnSave = !1
                 }
                 createNewWidget(e) {
-                    return new y({
+                    return new k({
                         context: e,
                         getPanelUrl: this.getPanelUrl,
                         renderOnSave: this.defaultRenderOnSave
                     })
                 }
             }
-            var f = n(832);
-            const k = "application/vnd.holoviews_load.v0+json",
-                b = "application/vnd.holoviews_exec.v0+json";
-            class C extends f.Widget {
+            var P = n(832);
+            const C = "application/vnd.holoviews_load.v0+json",
+                R = "application/vnd.holoviews_exec.v0+json";
+            class O extends P.Widget {
                 constructor(e, t) {
-                    super(), this._load_mimetype = k, this._script_element = document.createElement("script"), this._manager = t
+                    super(), this._load_mimetype = C, this._script_element = document.createElement("script"), this._manager = t
                 }
                 renderModel(e) {
                     const t = e.data[this._load_mimetype];
                     return this._script_element.textContent = t, this.node.appendChild(this._script_element), this._manager.comm, Promise.resolve()
                 }
             }
-            class P extends f.Widget {
+            class z extends P.Widget {
                 constructor(e, t) {
-                    super(), this._html_mimetype = "text/html", this._js_mimetype = "application/javascript", this._exec_mimetype = b, this._createNodes(), this._manager = t, this._displayed = !1, this._dispose = !0
+                    super(), this._html_mimetype = "text/html", this._js_mimetype = "application/javascript", this._exec_mimetype = R, this._createNodes(), this._manager = t, this._displayed = !1, this._dispose = !0
                 }
                 _createNodes() {
                     this._div_element = document.createElement("div"), this._script_element = document.createElement("script"), this._script_element.setAttribute("type", "text/javascript")
                 }
                 _registerKernel(e) {
                     var t;
                     const n = {
@@ -249,86 +264,86 @@
                         this._document_id = null
                     }
                 }
                 dispose() {
                     this.isDisposed || (super.dispose(), this._disposePlot(), this._manager = null)
                 }
             }
-            let R = null;
+            let S = null;
             try {
                 const e = n(294);
-                R = e.registerWidgetManager
+                S = e.registerWidgetManager
             } catch (e) {
                 console.log("Could not load ipywidgets support for @pyviz/jupyterlab_pyviz")
             }
-            var O;
+            var T;
             ! function(e) {
                 e.panelRender = "notebook:render-with-panel", e.panelOpen = "notebook:open-with-panel", e.lumenRender = "notebook:render-with-lumen", e.lumenOpen = "notebook:open-with-lumen"
-            }(O || (O = {}));
-            class z {
+            }(T || (T = {}));
+            class E {
                 constructor(e) {
                     this._commands = e
                 }
                 createNew(e) {
                     const t = new s.ToolbarButton({
                         className: "panelRender",
                         tooltip: "Render with Panel",
-                        icon: h,
+                        icon: p,
                         onClick: () => {
-                            this._commands.execute(O.panelRender)
+                            this._commands.execute(T.panelRender)
                         }
                     });
                     return e.toolbar.insertAfter("cellType", "panelRender", t), t
                 }
             }
-            class T {
+            class W {
                 constructor(e) {
                     this._commands = e
                 }
                 createNew(e) {
                     const t = new s.ToolbarButton({
                         className: "lumenRender",
                         tooltip: "Render with Lumen",
-                        icon: h,
+                        icon: p,
                         onClick: () => {
-                            this._commands.execute(O.lumenRender)
+                            this._commands.execute(T.lumenRender)
                         }
                     });
                     return e.toolbar.addItem("lumenRender", t), t
                 }
             }
-            class W {
+            class N {
                 createNew(e, t) {
                     const n = this._docmanager._findContext(t.path, "notebook"),
                         o = {
                             manager: null
                         };
-                    null != R && R(n, e.content.rendermime, [o]);
-                    const i = new p(t, o.manager);
+                    null != S && S(n, e.content.rendermime, [o]);
+                    const i = new u(t, o.manager);
                     return e.content.rendermime.addFactory({
                         safe: !1,
-                        mimeTypes: [k],
-                        createRenderer: e => new C(e, i)
+                        mimeTypes: [C],
+                        createRenderer: e => new O(e, i)
                     }, -1), e.content.rendermime.addFactory({
                         safe: !1,
-                        mimeTypes: [b],
-                        createRenderer: e => new P(e, i)
+                        mimeTypes: [R],
+                        createRenderer: e => new z(e, i)
                     }, -1), new c.DisposableDelegate((() => {
-                        e.content.rendermime && e.content.rendermime.removeMimeType(b), i.dispose()
+                        e.content.rendermime && e.content.rendermime.removeMimeType(R), i.dispose()
                     }))
                 }
             }
-            const S = {
+            const j = {
                     id: "@pyviz/jupyterlab_pyviz:plugin",
                     autoStart: !0,
                     requires: [a.IDocumentManager, o.INotebookTracker],
                     optional: [s.ICommandPalette, i.ILayoutRestorer, l.IMainMenu, d.ISettingRegistry],
-                    provides: v,
+                    provides: y,
                     activate: (e, t, n, o, i, a, d) => {
-                        const l = new W;
+                        const l = new N;
                         l._docmanager = t, e.docRegistry.addWidgetExtension("Notebook", l);
                         const c = new s.WidgetTracker({
                             namespace: "panel-preview"
                         });
 
                         function m(t) {
                             const o = n.currentWidget;
@@ -348,98 +363,98 @@
                             args: e => ({
                                 path: e.context.path,
                                 factory: u.name
                             }),
                             name: e => e.context.path,
                             when: e.serviceManager.ready
                         });
-                        const u = new x(p, {
+                        const u = new b(p, {
                                 name: "Panel-preview",
                                 fileTypes: ["notebook"],
                                 modelName: "notebook"
                             }),
-                            _ = new x(p, {
+                            g = new b(p, {
                                 name: "Lumen-preview",
                                 fileTypes: ["yaml", "yml", "text", "py"],
                                 modelName: "text"
                             });
                         u.widgetCreated.connect(((e, t) => {
                             t.context.pathChanged.connect((() => {
                                 c.save(t)
                             })), c.add(t)
-                        })), _.widgetCreated.connect(((e, t) => {
+                        })), g.widgetCreated.connect(((e, t) => {
                             c.add(t)
                         }));
-                        const g = e => {
+                        const _ = e => {
                             u.defaultRenderOnSave = e.get("renderOnSave").composite
                         };
-                        d && Promise.all([d.load(S.id), e.restored]).then((([e]) => {
-                            g(e), e.changed.connect(g)
+                        d && Promise.all([d.load(j.id), e.restored]).then((([e]) => {
+                            _(e), e.changed.connect(_)
                         })).catch((e => {
                             console.error(e.message)
-                        })), e.docRegistry.addWidgetFactory(u), e.docRegistry.addWidgetFactory(_);
+                        })), e.docRegistry.addWidgetFactory(u), e.docRegistry.addWidgetFactory(g);
                         const {
                             commands: w,
                             docRegistry: v
                         } = e;
-                        if (w.addCommand(O.panelRender, {
+                        if (w.addCommand(T.panelRender, {
                                 label: "Render Notebook with Panel",
                                 execute: async e => {
                                     const t = m(e);
                                     let n;
                                     t && (n = t.context, await n.save(), w.execute("docmanager:open", {
                                         path: n.path,
                                         factory: "Panel-preview",
                                         options: {
                                             mode: "split-right"
                                         }
                                     }))
                                 },
                                 isEnabled: h
-                            }), w.addCommand(O.lumenRender, {
+                            }), w.addCommand(T.lumenRender, {
                                 label: "Render Yaml with Lumen",
                                 execute: async t => {
                                     const n = e.shell.currentWidget;
                                     let o;
                                     n && (o = n.context, await o.save(), w.execute("docmanager:open", {
                                         path: o.path,
                                         factory: "Lumen-preview",
                                         options: {
                                             mode: "split-right"
                                         }
                                     }))
                                 },
                                 isEnabled: h
-                            }), w.addCommand(O.panelOpen, {
+                            }), w.addCommand(T.panelOpen, {
                                 label: "Open with Panel in New Browser Tab",
                                 execute: async e => {
                                     const t = m(e);
                                     if (!t) return;
                                     await t.context.save();
                                     const n = p(t.context.path);
                                     window.open(n)
                                 },
                                 isEnabled: h
                             }), o) {
                             const e = "Notebook Operations";
-                            [O.panelRender, O.panelOpen].forEach((t => {
+                            [T.panelRender, T.panelOpen].forEach((t => {
                                 o.addItem({
                                     command: t,
                                     category: e
                                 })
                             }))
                         }
                         a && a.viewMenu.addGroup([{
-                            command: O.panelRender
+                            command: T.panelRender
                         }, {
-                            command: O.panelOpen
+                            command: T.panelOpen
                         }], 1e3);
-                        const y = new z(w);
+                        const y = new E(w);
                         v.addWidgetExtension("Notebook", y);
-                        const f = new T(w);
+                        const f = new W(w);
                         return v.addWidgetExtension("Editor", f), c
                     }
                 },
-                N = S
+                M = j
         }
     }
 ]);
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js` & `pyviz_comms-2.3.1/pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(n, {
                 Z: () => o
             });
             var r = t(645),
                 i = t.n(r)()((function(e) {
                     return e[1]
                 }));
-            i.push([e.id, "", ""]);
+            i.push([e.id, ".jp-PanelPreview-renderOnSave {\n  display: flex;\n  align-items: center;\n}\n\n.jp-PanelPreview-loading {\n  background: rgba(0, 0, 0, 0.05);\n  pointer-events: none;\n  position: relative;\n}\n\n.jp-PanelPreview-loading::before {\n  content: '';\n  display: block;\n  position: absolute;\n  top: 50%;\n  left: 50%;\n  transform: translate(-50%, -50%);\n  width: 80px;\n  height: 80px;\n  border: 8px solid rgb(48, 112, 146);\n  border-left-color: #f3f3f3;\n  border-radius: 50%;\n  animation: spin 1s infinite linear;\n  z-index: 9999;\n}\n\n@keyframes spin {\n  from {\n    transform: rotate(0deg);\n  }\n  to {\n    transform: rotate(360deg);\n  }\n}\n", ""]);
             const o = i
         },
         645: e => {
             e.exports = function(e) {
                 var n = [];
                 return n.toString = function() {
                     return this.map((function(n) {
@@ -26,17 +26,17 @@
                     ]);
                     var i = {};
                     if (r)
                         for (var o = 0; o < this.length; o++) {
                             var a = this[o][0];
                             null != a && (i[a] = !0)
                         }
-                    for (var c = 0; c < e.length; c++) {
-                        var s = [].concat(e[c]);
-                        r && i[s[0]] || (t && (s[2] ? s[2] = "".concat(t, " and ").concat(s[2]) : s[2] = t), n.push(s))
+                    for (var s = 0; s < e.length; s++) {
+                        var c = [].concat(e[s]);
+                        r && i[c[0]] || (t && (c[2] ? c[2] = "".concat(t, " and ").concat(c[2]) : c[2] = t), n.push(c))
                     }
                 }, n
             }
         },
         379: (e, n, t) => {
             var r, i = function() {
                     var e = {};
@@ -59,36 +59,36 @@
                 for (var n = -1, t = 0; t < o.length; t++)
                     if (o[t].identifier === e) {
                         n = t;
                         break
                     } return n
             }
 
-            function c(e, n) {
+            function s(e, n) {
                 for (var t = {}, r = [], i = 0; i < e.length; i++) {
-                    var c = e[i],
-                        s = n.base ? c[0] + n.base : c[0],
-                        u = t[s] || 0,
-                        l = "".concat(s, " ").concat(u);
-                    t[s] = u + 1;
-                    var f = a(l),
+                    var s = e[i],
+                        c = n.base ? s[0] + n.base : s[0],
+                        l = t[c] || 0,
+                        u = "".concat(c, " ").concat(l);
+                    t[c] = l + 1;
+                    var f = a(u),
                         d = {
-                            css: c[1],
-                            media: c[2],
-                            sourceMap: c[3]
+                            css: s[1],
+                            media: s[2],
+                            sourceMap: s[3]
                         }; - 1 !== f ? (o[f].references++, o[f].updater(d)) : o.push({
-                        identifier: l,
+                        identifier: u,
                         updater: h(d, n),
                         references: 1
-                    }), r.push(l)
+                    }), r.push(u)
                 }
                 return r
             }
 
-            function s(e) {
+            function c(e) {
                 var n = document.createElement("style"),
                     r = e.attributes || {};
                 if (void 0 === r.nonce) {
                     var o = t.nc;
                     o && (r.nonce = o)
                 }
                 if (Object.keys(r).forEach((function(e) {
@@ -97,21 +97,21 @@
                 else {
                     var a = i(e.insert || "head");
                     if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                     a.appendChild(n)
                 }
                 return n
             }
-            var u, l = (u = [], function(e, n) {
-                return u[e] = n, u.filter(Boolean).join("\n")
+            var l, u = (l = [], function(e, n) {
+                return l[e] = n, l.filter(Boolean).join("\n")
             });
 
             function f(e, n, t, r) {
                 var i = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
-                if (e.styleSheet) e.styleSheet.cssText = l(n, i);
+                if (e.styleSheet) e.styleSheet.cssText = u(n, i);
                 else {
                     var o = document.createTextNode(i),
                         a = e.childNodes;
                     a[n] && e.removeChild(a[n]), a.length ? e.insertBefore(o, a[n]) : e.appendChild(o)
                 }
             }
 
@@ -128,16 +128,16 @@
             var p = null,
                 v = 0;
 
             function h(e, n) {
                 var t, r, i;
                 if (n.singleton) {
                     var o = v++;
-                    t = p || (p = s(n)), r = f.bind(null, t, o, !1), i = f.bind(null, t, o, !0)
-                } else t = s(n), r = d.bind(null, t, n), i = function() {
+                    t = p || (p = c(n)), r = f.bind(null, t, o, !1), i = f.bind(null, t, o, !0)
+                } else t = c(n), r = d.bind(null, t, n), i = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
                     }(t)
                 };
                 return r(e),
                     function(n) {
@@ -145,26 +145,26 @@
                             if (n.css === e.css && n.media === e.media && n.sourceMap === e.sourceMap) return;
                             r(e = n)
                         } else i()
                     }
             }
             e.exports = function(e, n) {
                 (n = n || {}).singleton || "boolean" == typeof n.singleton || (n.singleton = (void 0 === r && (r = Boolean(window && document && document.all && !window.atob)), r));
-                var t = c(e = e || [], n);
+                var t = s(e = e || [], n);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var r = 0; r < t.length; r++) {
                             var i = a(t[r]);
                             o[i].references--
                         }
-                        for (var s = c(e, n), u = 0; u < t.length; u++) {
-                            var l = a(t[u]);
-                            0 === o[l].references && (o[l].updater(), o.splice(l, 1))
+                        for (var c = s(e, n), l = 0; l < t.length; l++) {
+                            var u = a(t[l]);
+                            0 === o[u].references && (o[u].updater(), o.splice(u, 1))
                         }
-                        t = s
+                        t = c
                     }
                 }
             }
         },
         747: (e, n, t) => {
             t.r(n);
             var r = t(379),
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms/labextension/static/remoteEntry.febb837ab3b6ef743bf7.js` & `pyviz_comms-2.3.1/pyviz_comms/labextension/static/remoteEntry.75aa6a6489839cbfc067.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, v, h, y, b, g, m, j, w, S = {
+    var e, r, t, n, a, o, i, u, l, s, d, p, f, c, v, h, y, b, g, m, j, w, S = {
             281: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(445).then((() => () => t(445))),
                         "./extension": () => t.e(445).then((() => () => t(445))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        445: "482ccf5e3a3952a8b415",
-        747: "872484f6c86b06b5c3f4"
+        445: "8dcc8508e7796b2d5680",
+        747: "0551e937e8f929740f5d"
     } [e] + ".js?v=" + {
-        445: "482ccf5e3a3952a8b415",
-        747: "872484f6c86b06b5c3f4"
+        445: "8dcc8508e7796b2d5680",
+        747: "0551e937e8f929740f5d"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@pyviz/jupyterlab_pyviz:", k.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+                    var d = l[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
+                        i = d;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var p = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(f);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                f = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var a = o[e] = o[e] || {},
                         u = a[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (a[r] = {
                         get: () => k.e(445).then((() => () => k(445))),
                         from: i,
                         eager: !1
                     })
-                })("@pyviz/jupyterlab_pyviz", "2.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@pyviz/jupyterlab_pyviz", "2.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,86 +164,86 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var s, d, p = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == p ? u > n && !a : "" == p != a);
+                if ("u" == d) {
+                    if (!l || "u" != p) return !1
                 } else if (l)
-                    if (d == f)
+                    if (p == d)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (a ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != p && "n" != p) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != a) return !1;
+                    if (u <= n || d < p != a) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var f = [],
+            c = f.pop.bind(f);
         for (i = 1; i < e.length; i++) {
             var v = e[i];
-            p.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? o(v, r) : !c())
+            f.push(1 == v ? c() | c() : 2 == v ? c() & c() : v ? o(v, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = l(e, t);
         return o(n, a) || c(s(e, t, a, n)), h(e[t][a])
-    }, d = (e, r, t) => {
+    }, p = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, p = (e, r, t, n) => {
+    }, f = (e, r, t, n) => {
         var o = e[t];
         return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, v = (e, r, t, n) => {
-        c(p(e, r, t, n))
+        c(f(e, r, t, n))
     }, h = e => (e.loaded = 1, e.get()), b = (y = e => function(r, t, n, a) {
         var o = k.I(r);
         return o && o.then ? o.then(e.bind(e, r, k.S[r], t, n, a)) : e(r, k.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || v(r, e, t, n) || u(r, t))))), g = y(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = {}, j = {
-        33: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
-        38: () => g("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
-        123: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
-        142: () => g("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+    })(((e, r, t, n) => (i(e, t), h(p(r, t, n) || v(r, e, t, n) || u(r, t))))), g = y(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), m = {}, j = {
+        58: () => g("default", "@jupyterlab/coreutils", [1, 5, 6, 4]),
+        85: () => g("default", "@jupyterlab/settingregistry", [1, 3, 6, 4]),
+        175: () => g("default", "@jupyterlab/application", [1, 3, 6, 4]),
+        263: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 4]),
         271: () => g("default", "react", [1, 17, 0, 1]),
         294: () => g("default", "@jupyter-widgets/jupyterlab-manager", [1, 5, 0, 4]),
-        344: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
-        502: () => g("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        308: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 4]),
         526: () => g("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        687: () => g("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        819: () => b("default", "@jupyterlab/docregistry", [1, 3, 6, 3]),
+        667: () => g("default", "@jupyterlab/ui-components", [1, 3, 6, 4]),
+        676: () => b("default", "@jupyterlab/docregistry", [1, 3, 6, 4]),
+        764: () => g("default", "@jupyterlab/apputils", [1, 3, 6, 4]),
+        779: () => g("default", "@jupyterlab/notebook", [1, 3, 6, 4]),
         832: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
         840: () => g("default", "@lumino/signaling", [1, 1, 10, 0]),
-        923: () => g("default", "@lumino/disposable", [1, 1, 10, 0]),
-        986: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 3])
+        923: () => g("default", "@lumino/disposable", [1, 1, 10, 0])
     }, w = {
-        445: [33, 38, 123, 142, 271, 294, 344, 502, 526, 687, 819, 832, 840, 923, 986]
+        445: [58, 85, 175, 263, 271, 294, 308, 526, 667, 676, 764, 779, 832, 840, 923]
     }, k.f.consumes = (e, r) => {
         k.o(w, e) && w[e].forEach((e => {
             if (k.o(m, e)) return r.push(m[e]);
             var t = r => {
                     m[e] = 0, k.m[e] = t => {
                         delete k.c[e], t.exports = r()
                     }
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms/labextension/static/third-party-licenses.json` & `pyviz_comms-2.3.1/pyviz_comms/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/pyviz_comms/notebook.js` & `pyviz_comms-2.3.1/pyviz_comms/notebook.js`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/pyviz_comms/tests/test_extension.py` & `pyviz_comms-2.3.1/pyviz_comms/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/pyviz_comms.egg-info/PKG-INFO` & `pyviz_comms-2.3.1/pyviz_comms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz-comms
-Version: 2.3.0
+Version: 2.3.1
 Summary: Bidirectional communication for the HoloViz ecosystem.
 Home-page: https://holoviz.org
 Author: Philipp Rudiger
 Author-email: philipp.jfr@gmail.com
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
```

### Comparing `pyviz_comms-2.3.0/pyviz_comms.egg-info/SOURCES.txt` & `pyviz_comms-2.3.1/pyviz_comms.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 pyviz_comms.egg-info/SOURCES.txt
 pyviz_comms.egg-info/dependency_links.txt
 pyviz_comms.egg-info/requires.txt
 pyviz_comms.egg-info/top_level.txt
 pyviz_comms/labextension/package.json
 pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/package.json.orig
 pyviz_comms/labextension/schemas/@pyviz/jupyterlab_pyviz/plugin.json
-pyviz_comms/labextension/static/445.482ccf5e3a3952a8b415.js
-pyviz_comms/labextension/static/747.872484f6c86b06b5c3f4.js
-pyviz_comms/labextension/static/remoteEntry.febb837ab3b6ef743bf7.js
+pyviz_comms/labextension/static/445.8dcc8508e7796b2d5680.js
+pyviz_comms/labextension/static/747.0551e937e8f929740f5d.js
+pyviz_comms/labextension/static/remoteEntry.75aa6a6489839cbfc067.js
 pyviz_comms/labextension/static/style.js
 pyviz_comms/labextension/static/third-party-licenses.json
 pyviz_comms/tests/__init__.py
 pyviz_comms/tests/test_extension.py
 src/icons.ts
 src/index.ts
 src/manager.ts
```

### Comparing `pyviz_comms-2.3.0/setup.py` & `pyviz_comms-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/src/manager.ts` & `pyviz_comms-2.3.1/src/manager.ts`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/src/plugin.ts` & `pyviz_comms-2.3.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/src/preview.tsx` & `pyviz_comms-2.3.1/src/preview.tsx`

 * *Files 22% similar despite different names*

```diff
@@ -17,41 +17,122 @@
 
 import { Signal } from '@lumino/signaling';
 
 import * as React from 'react';
 
 import { panelIcon } from './icons';
 
+import panelSvgStr from '../style/panel.svg';
+
 /**
  * A class that tracks Panel Preview widgets.
  */
 export type IPanelPreviewTracker = IWidgetTracker<PanelPreview>;
 
 /**
  * The Panel Preview tracker token.
  */
 export const IPanelPreviewTracker = new Token<IPanelPreviewTracker>(
   '@pyviz/jupyterlab_pyviz:IPanelPreviewTracker'
 );
 
+export interface IOptions extends IFrame.IOptions {
+  srcdoc?: string;
+}
+
+export class CustomIFrame extends IFrame {
+  constructor(options: IOptions = {}) {
+    super(options);
+    this.srcdoc = options.srcdoc || null;
+  }
+
+  get srcdoc() {
+    return this._srcdoc;
+  }
+
+  set srcdoc(value: string) {
+    this._srcdoc = value;
+    const iframe = this.node.querySelector('iframe')!;
+    if (value != null) {
+      iframe.setAttribute('srcdoc', value);
+      iframe.addEventListener('load', () => iframe.removeAttribute('srcdoc'));
+    }
+  }
+
+  private _srcdoc: string;
+}
+
+const CUSTOM_LOADER = `
+<!DOCTYPE html>
+<html>
+<head>
+  <title>Jupyter Kernel Starting</title>
+  <style>
+    body {
+      display: flex;
+      align-items: center;
+      justify-content: center;
+      flex-direction: column;
+      height: 100vh;
+      background-color: #f7f7f7;
+      font-family: Futura;
+    }
+
+    .loading-container {
+      display: flex;
+      align-items: center;
+      justify-content: center;
+      margin: 20px 0;
+    }
+
+    .loading-indicator {
+      width: 100px;
+      height: 100px;
+      border: 8px solid rgb(48, 112, 146);
+      border-top-color: #f7f7f7;
+      border-radius: 50%;
+      animation: spin 1s infinite linear;
+    }
+
+    @keyframes spin {
+      from {
+        transform: rotate(0deg);
+      }
+      to {
+        transform: rotate(360deg);
+      }
+    }
+  </style>
+</head>
+<body>
+  ${panelSvgStr}
+  <h1>Panel Preview Launching...</h1>
+  <div class="loading-container">
+    <div class="loading-indicator"></div>
+  </div>
+</body>
+</html>
+`;
+
 /**
  * A DocumentWidget that shows a Panel preview in an IFrame.
  */
 export class PanelPreview extends DocumentWidget<
-  IFrame,
+  CustomIFrame,
   DocumentRegistry.ICodeModel
 > {
   /**
    * Instantiate a new PanelPreview.
    * @param options The PanelPreview instantiation options.
    */
   constructor(options: PanelPreview.IOptions) {
     super({
       ...options,
-      content: new IFrame({
+      content: new CustomIFrame({
+        srcdoc: CUSTOM_LOADER,
         sandbox: ['allow-same-origin', 'allow-scripts', 'allow-downloads']
       })
     });
 
     window.onmessage = (event: any): void => {
       switch (event.data?.level) {
         case 'debug':
@@ -94,23 +175,22 @@
         this.reload();
       }
     });
 
     const renderOnSaveCheckbox = ReactWidget.create(
       <label className="jp-PanelPreview-renderOnSave">
         <input
-          style={{ verticalAlign: 'middle' }}
           name="renderOnSave"
           type="checkbox"
           defaultChecked={renderOnSave}
           onChange={(event: React.ChangeEvent<HTMLInputElement>): void => {
             this._renderOnSave = event.target.checked;
           }}
         />
-        Render on Save
+        <span>Render on Save</span>
       </label>
     );
 
     this.toolbar.addItem('reload', reloadButton);
 
     if (context) {
       this.toolbar.addItem('renderOnSave', renderOnSaveCheckbox);
@@ -137,15 +217,19 @@
 
   /**
    * Reload the preview.
    */
   reload(): void {
     const iframe = this.content.node.querySelector('iframe')!;
     if (iframe.contentWindow != null) {
+      iframe.parentElement.classList.add('jp-PanelPreview-loading');
       iframe.contentWindow.location.reload();
+      iframe.addEventListener('load', () => {
+        iframe.parentElement.classList.remove('jp-PanelPreview-loading');
+      });
     }
   }
 
   /**
    * Get whether the preview reloads when the context is saved.
    */
   get renderOnSave(): boolean {
```

### Comparing `pyviz_comms-2.3.0/src/renderer.ts` & `pyviz_comms-2.3.1/src/renderer.ts`

 * *Files identical despite different names*

### Comparing `pyviz_comms-2.3.0/tsconfig.json` & `pyviz_comms-2.3.1/tsconfig.json`

 * *Files identical despite different names*

