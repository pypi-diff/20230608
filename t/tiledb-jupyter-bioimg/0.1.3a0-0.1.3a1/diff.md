# Comparing `tmp/tiledb_jupyter_bioimg-0.1.3a0.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.3a0.tar", last modified: Wed Jun  7 13:57:13 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.3a1.tar", last modified: Wed Jun  7 15:05:35 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.3a0.tar` & `tiledb_jupyter_bioimg-0.1.3a1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-07 13:55:06.000000 tiledb_jupyter_bioimg-0.1.3a0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.395265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)   755430 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   516678 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/744.32875cac115e9f54b48d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.9bb49b46696448b14690.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 13:56:47.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    85180 2023-06-07 13:57:12.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:57:13.391265 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:56:05.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 13:57:13.000000 tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 13:53:09.000000 tiledb_jupyter_bioimg-0.1.3a0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.596772 tiledb_jupyter_bioimg-0.1.3a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 15:05:35.596772 tiledb_jupyter_bioimg-0.1.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-07 15:03:24.000000 tiledb_jupyter_bioimg-0.1.3a1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:05:35.596772 tiledb_jupyter_bioimg-0.1.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.588771 tiledb_jupyter_bioimg-0.1.3a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.588771 tiledb_jupyter_bioimg-0.1.3a1/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.588771 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.592771 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.596772 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)   755430 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   516678 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/744.2af523a36da1211c0055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.843901c4475b4ee0154e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 15:05:08.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85180 2023-06-07 15:05:34.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:05:35.592771 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 15:05:35.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-07 15:05:35.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:05:35.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:04:26.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 15:05:35.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 15:05:35.000000 tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 15:01:26.000000 tiledb_jupyter_bioimg-0.1.3a1/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/LICENSE` & `tiledb_jupyter_bioimg-0.1.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.3a0
+Version: 0.1.3a1
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/README.md` & `tiledb_jupyter_bioimg-0.1.3a1/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/package.json` & `tiledb_jupyter_bioimg-0.1.3a1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.3-alpha.1'"}*

```diff
@@ -93,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3-alpha.0"
+    "version": "0.1.3-alpha.1"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/setup.py` & `tiledb_jupyter_bioimg-0.1.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/src/index.ts` & `tiledb_jupyter_bioimg-0.1.3a1/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/src/version.ts` & `tiledb_jupyter_bioimg-0.1.3a1/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.3a1/src/widget.ts`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 }
 
 export class BioImageViewerView extends DOMWidgetView {
   values: IValues = this.model.get('value');
 
   render(): void {
     const wrapper = document.createElement('div');
+    wrapper.style.height = '700px';
     this.el.appendChild(wrapper);
 
     createViewer({
       rootElement: wrapper,
       apiKey: this.values.token,
       groupID: this.values.groupID,
       basePath: this.values.basePath,
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.843901c4475b4ee0154e.js'}}",*

 * * "'version'": "'0.1.3-alpha.1'"}*

```diff
@@ -27,15 +27,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9bb49b46696448b14690.js",
+            "load": "static/remoteEntry.843901c4475b4ee0154e.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3-alpha.0"
+    "version": "0.1.3-alpha.1"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/744.32875cac115e9f54b48d.js` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/744.2af523a36da1211c0055.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -33,15 +33,15 @@
             d.model_module = r, d.model_module_version = a, d.view_module = r, d.view_module_version = a, d.serializers = Object.assign({}, s.DOMWidgetModel.serializers), d.model_name = "BioImageViewerModel", d.view_name = "BioImageViewerView";
             class p extends s.DOMWidgetView {
                 constructor() {
                     super(...arguments), this.values = this.model.get("value")
                 }
                 render() {
                     const e = document.createElement("div");
-                    this.el.appendChild(e), u()({
+                    e.style.height = "700px", this.el.appendChild(e), u()({
                         rootElement: e,
                         apiKey: this.values.token,
                         groupID: this.values.groupID,
                         basePath: this.values.basePath,
                         baseGroup: this.values.baseGroup,
                         namespace: this.values.namespace
                     })
@@ -57,11 +57,11 @@
                         version: a,
                         exports: t
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.3-alpha.0","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.1-beta.2"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.3-alpha.1","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.1-beta.2"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/experimental":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@deck.gl/aggregation-layers":"8.8.12","@deck.gl/core":"8.8.12","@deck.gl/carto":"8.8.12","@deck.gl/extensions":"8.8.12","@deck.gl/geo-layers":"8.8.12","@deck.gl/google-maps":"8.8.12","@deck.gl/mapbox":"8.8.12","@deck.gl/json":"8.8.12","@deck.gl/layers":"8.8.12","@deck.gl/mesh-layers":"8.8.12","@deck.gl/react":"8.8.12"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.9bb49b46696448b14690.js` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.843901c4475b4ee0154e.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, d, l, f, u, s, c, p, h, v, b, m, g, y = {
+    var e, r, t, n, i, o, a, d, l, u, f, s, c, p, h, v, b, m, g, y = {
             5290: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -48,22 +48,22 @@
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         241: "3606da7606ad147cbcb2",
         446: "3bf34f45c93ace9c0f28",
         556: "f09c354898cd66a026b3",
         635: "a03dea4f48d4a0dc1e4c",
-        744: "32875cac115e9f54b48d",
+        744: "2af523a36da1211c0055",
         747: "433530952542f03ebc71"
     } [e] + ".js?v=" + {
         241: "3606da7606ad147cbcb2",
         446: "3bf34f45c93ace9c0f28",
         556: "f09c354898cd66a026b3",
         635: "a03dea4f48d4a0dc1e4c",
-        744: "32875cac115e9f54b48d",
+        744: "2af523a36da1211c0055",
         747: "433530952542f03ebc71"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -74,18 +74,18 @@
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
     }), e), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", S.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
             var a, d;
             if (void 0 !== i)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var u = l[f];
-                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + i) {
-                        a = u;
+                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
+                    var f = l[u];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + i) {
+                        a = f;
                         break
                     }
                 }
             a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
             var s = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(c);
                     var i = e[t];
@@ -121,15 +121,15 @@
                         (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (i[r] = {
                             get: t,
                             from: a,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (d("@tiledb-inc/bioimage-viewer", "0.1.1-beta.2", (() => Promise.all([S.e(635), S.e(556), S.e(446)]).then((() => () => S(1556))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.3-alpha.0", (() => S.e(744).then((() => () => S(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@tiledb-inc/bioimage-viewer", "0.1.1-beta.2", (() => Promise.all([S.e(635), S.e(556), S.e(446)]).then((() => () => S(1556))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.3-alpha.1", (() => S.e(744).then((() => () => S(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -179,31 +179,31 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
             for (var a = 0, d = 1, l = !0;; d++, a++) {
-                var f, u, s = d < e.length ? (typeof e[d])[0] : "";
-                if (a >= r.length || "o" == (u = (typeof(f = r[a]))[0])) return !l || ("u" == s ? d > n && !i : "" == s != i);
-                if ("u" == u) {
+                var u, f, s = d < e.length ? (typeof e[d])[0] : "";
+                if (a >= r.length || "o" == (f = (typeof(u = r[a]))[0])) return !l || ("u" == s ? d > n && !i : "" == s != i);
+                if ("u" == f) {
                     if (!l || "u" != s) return !1
                 } else if (l)
-                    if (s == u)
+                    if (s == f)
                         if (d <= n) {
-                            if (f != e[d]) return !1
+                            if (u != e[d]) return !1
                         } else {
-                            if (i ? f > e[d] : f < e[d]) return !1;
-                            f != e[d] && (l = !1)
+                            if (i ? u > e[d] : u < e[d]) return !1;
+                            u != e[d] && (l = !1)
                         }
                 else if ("s" != s && "n" != s) {
                     if (i || d <= n) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= n || u < s != i) return !1;
+                    if (d <= n || f < s != i) return !1;
                     l = !1
                 } else "s" != s && "n" != s && (l = !1, d--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (a = 1; a < e.length; a++) {
@@ -214,27 +214,27 @@
     }, a = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", f = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
         var i = d(e, t);
         return o(n, i) || s(l(e, t, i, n)), c(e[t][i])
-    }, u = (e, r, t) => {
+    }, f = (e, r, t) => {
         var i = e[r];
         return (r = Object.keys(i).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && i[r]
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, i) {
         var o = S.I(r);
         return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, i)) : e(r, S.S[r], t, n, i)
-    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
-        var o = r && S.o(r, t) && u(r, t, n);
+    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, i) => {
+        var o = r && S.o(r, t) && f(r, t, n);
         return o ? c(o) : i()
     })), b = {}, m = {
         1395: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.3a0
+Version: 0.1.3a1
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.3a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
 tiledb_jupyter_bioimg/labextension/static/241.3606da7606ad147cbcb2.js
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
 tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js
 tiledb_jupyter_bioimg/labextension/static/556.f09c354898cd66a026b3.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js
 tiledb_jupyter_bioimg/labextension/static/635.a03dea4f48d4a0dc1e4c.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.32875cac115e9f54b48d.js
+tiledb_jupyter_bioimg/labextension/static/744.2af523a36da1211c0055.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.9bb49b46696448b14690.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.843901c4475b4ee0154e.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.3a0/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.3a1/tsconfig.json`

 * *Files identical despite different names*

