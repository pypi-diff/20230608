# Comparing `tmp/yjs_widgets-0.3.3.tar.gz` & `tmp/yjs_widgets-0.3.4.tar.gz`

## Comparing `yjs_widgets-0.3.3.tar` & `yjs_widgets-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,42 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.eslintrc.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.prettierignore
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.prettierrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.yarnrc.yml
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/install.json
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/tsconfig.json
--rw-r--r--   0        0        0   201745 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/yarn.lock
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/index.ts
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/model.ts
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/types.ts
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/index.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/model.ts
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/types.ts
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/view.ts
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/widgetManager.ts
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/yCommProvider.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/style/index.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/yjs_widgets/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/yjs_widgets/_version.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/LICENSE
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/README.md
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/.eslintrc.js
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/.prettierignore
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/.yarnrc.yml
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/install.json
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/tsconfig.json
+-rw-r--r--   0        0        0   201745 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/yarn.lock
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/.yarnrc.yml
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/LICENSE
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/README.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/install.json
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/package.json
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/pyproject.toml
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/tsconfig.json
+-rw-r--r--   0        0        0   202600 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/yarn.lock
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/notebooks/simple.ipynb
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/simple_yjs_widget/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/src/index.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/examples/simple-yjs-widget/style/index.js
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/index.ts
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/model.ts
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/types.ts
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/notebookrenderer/types.ts
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/style/index.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/yjs_widgets/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/yjs_widgets/_version.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/README.md
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 yjs_widgets-0.3.4/PKG-INFO
```

### Comparing `yjs_widgets-0.3.3/.eslintrc.js` & `yjs_widgets-0.3.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/CONTRIBUTING.md` & `yjs_widgets-0.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/package.json` & `yjs_widgets-0.3.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.3.4'"}*

```diff
@@ -95,9 +95,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.3"
+    "version": "0.3.4"
 }
```

### Comparing `yjs_widgets-0.3.3/tsconfig.json` & `yjs_widgets-0.3.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/yarn.lock` & `yjs_widgets-0.3.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/model.ts` & `yjs_widgets-0.3.4/src/model.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/types.ts` & `yjs_widgets-0.3.4/src/types.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/notebookrenderer/index.ts` & `yjs_widgets-0.3.4/src/notebookrenderer/index.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/notebookrenderer/model.ts` & `yjs_widgets-0.3.4/src/notebookrenderer/model.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/notebookrenderer/types.ts` & `yjs_widgets-0.3.4/src/notebookrenderer/types.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/notebookrenderer/view.ts` & `yjs_widgets-0.3.4/src/notebookrenderer/view.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/notebookrenderer/widgetManager.ts` & `yjs_widgets-0.3.4/src/notebookrenderer/widgetManager.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/src/notebookrenderer/yCommProvider.ts` & `yjs_widgets-0.3.4/src/notebookrenderer/yCommProvider.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/.gitignore` & `yjs_widgets-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/LICENSE` & `yjs_widgets-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/README.md` & `yjs_widgets-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.3/pyproject.toml` & `yjs_widgets-0.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,19 @@
     "hatchling",
     "hatch-nodejs-version",
     "jupyterlab>=4.0.0,<5",
 ]
 
 
 [project]
-name = "yjs_widgets"
+name = "yjs-widgets"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
-dependencies = [
-    "jupyterlab>=4.0.0",
-    "ypywidgets>=0.4.0,<1",
-    "comm>=0.1.3,<0.2.0"
-]
+dependencies = []
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `yjs_widgets-0.3.3/PKG-INFO` & `yjs_widgets-0.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yjs_widgets
-Version: 0.3.3
+Name: yjs-widgets
+Version: 0.3.4
 Summary: A JupyterLab extension for widgets based on Yjs.
 Project-URL: Homepage, https://github.com/QuantStack/yjs-widgets
 Project-URL: Bug Tracker, https://github.com/QuantStack/yjs-widgets/issues
 Project-URL: Repository, https://github.com/QuantStack/yjs-widgets.git
 Author-email: Trung Le <leductrungxf@gmail.com>
 License: BSD 3-Clause License
         
@@ -46,17 +46,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
-Requires-Dist: comm<0.2.0,>=0.1.3
-Requires-Dist: jupyterlab>=4.0.0
-Requires-Dist: ypywidgets<1,>=0.4.0
 Description-Content-Type: text/markdown
 
 # JupyterLab extension for widgets based on Yjs
 
 ## Requirements
 
 - JupyterLab == 4.0.0b0
```

