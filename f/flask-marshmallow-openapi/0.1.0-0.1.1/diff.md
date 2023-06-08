# Comparing `tmp/flask-marshmallow-openapi-0.1.0.tar.gz` & `tmp/flask-marshmallow-openapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.0.tar", last modified: Thu Jun  8 12:52:41 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.1.1.tar", last modified: Thu Jun  8 13:23:59 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.0.tar` & `flask-marshmallow-openapi-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.888424 flask-marshmallow-openapi-0.1.0/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-08 12:33:06.000000 flask-marshmallow-openapi-0.1.0/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.0/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.0/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.0/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.0/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3531 2023-06-08 12:52:41.888424 flask-marshmallow-openapi-0.1.0/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2689 2023-06-08 12:42:08.000000 flask-marshmallow-openapi-0.1.0/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-08 12:43:14.000000 flask-marshmallow-openapi-0.1.0/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-08 12:52:41.888424 flask-marshmallow-openapi-0.1.0/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.876424 flask-marshmallow-openapi-0.1.0/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.880424 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      107 2023-06-08 12:33:06.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12468 2023-06-08 07:51:47.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/helpers.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-08 11:36:11.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/open_api.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.876424 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.888424 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3694 2023-06-08 11:52:49.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.888424 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 12:52:41.880424 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3531 2023-06-08 12:52:41.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2056 2023-06-08 12:52:41.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 12:52:41.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-08 12:52:41.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-08 12:52:41.000000 flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.202645 flask-marshmallow-openapi-0.1.1/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-08 13:23:23.000000 flask-marshmallow-openapi-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.1/.gitignore
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.1/.python-version
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.1/LICENSE
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      819 2023-06-08 12:23:57.000000 flask-marshmallow-openapi-0.1.1/MANIFEST.in
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3531 2023-06-08 13:23:59.202645 flask-marshmallow-openapi-0.1.1/PKG-INFO
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2689 2023-06-08 13:12:32.000000 flask-marshmallow-openapi-0.1.1/README.md
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-08 13:23:23.000000 flask-marshmallow-openapi-0.1.1/pyproject.toml
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-08 13:23:59.202645 flask-marshmallow-openapi-0.1.1/setup.cfg
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.190645 flask-marshmallow-openapi-0.1.1/src/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.194645 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      107 2023-06-08 13:23:23.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/__init__.py
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    12468 2023-06-08 07:51:47.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/helpers.py
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-08 11:36:11.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/open_api.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.194645 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.202645 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1538481 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1286259 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1534168 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   517830 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   251096 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)   305131 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3731 2023-06-08 13:22:44.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static_collector.py
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.202645 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)      852 2023-06-08 08:13:47.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-08 13:23:59.194645 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3531 2023-06-08 13:23:59.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2056 2023-06-08 13:23:59.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 13:23:59.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-08 13:23:59.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-08 13:23:59.000000 flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.0/.gitignore` & `flask-marshmallow-openapi-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/LICENSE` & `flask-marshmallow-openapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/MANIFEST.in` & `flask-marshmallow-openapi-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/PKG-INFO` & `flask-marshmallow-openapi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.0/README.md` & `flask-marshmallow-openapi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/pyproject.toml` & `flask-marshmallow-openapi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/open_api.py` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/open_api.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/static_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
             if ext == "json":
                 dest = swagger_json_filename = f"swagger_{digest}.{ext}"
             else:
                 dest = f"swagger_{digest}.{ext}"
 
             os.rename(self.docs_static / "open_api_spec.tmp", self.docs_static / dest)
 
-        new_swagger_json_path = flask.url_for("static", filename=swagger_json_filename)
+        new_swagger_json_path = flask.url_for(
+            "open_api.swagger_json", filename=swagger_json_filename
+        )
 
         return new_swagger_json_path
 
     def _write_redoc_html(self, swagger_json_url):
         page = flask.render_template(
             "re_doc.jinja2", swagger_json_path=swagger_json_url
         )
```

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.1.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

