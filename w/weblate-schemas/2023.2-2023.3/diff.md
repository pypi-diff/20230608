# Comparing `tmp/weblate_schemas-2023.2.tar.gz` & `tmp/weblate_schemas-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblate_schemas-2023.2.tar", last modified: Thu Mar  2 09:34:26 2023, max compression
+gzip compressed data, was "weblate_schemas-2023.3.tar", last modified: Thu Jun  8 18:02:14 2023, max compression
```

## Comparing `weblate_schemas-2023.2.tar` & `weblate_schemas-2023.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:34:26.791060 weblate_schemas-2023.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-03-02 09:34:26.791060 weblate_schemas-2023.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-03-02 09:34:26.791060 weblate_schemas-2023.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      275 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:34:26.787060 weblate_schemas-2023.2/weblate_schemas/
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:34:26.791060 weblate_schemas-2023.2/weblate_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/schemas/weblate-backup.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)    21715 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/schemas/weblate-component.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/schemas/weblate-memory.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)     8346 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/schemas/weblate-userdata.schema.json
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-03-02 09:34:15.000000 weblate_schemas-2023.2/weblate_schemas/test_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 09:34:26.787060 weblate_schemas-2023.2/weblate_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-03-02 09:34:26.000000 weblate_schemas-2023.2/weblate_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-02 09:34:26.000000 weblate_schemas-2023.2/weblate_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 09:34:26.000000 weblate_schemas-2023.2/weblate_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 09:34:26.000000 weblate_schemas-2023.2/weblate_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-02 09:34:26.000000 weblate_schemas-2023.2/weblate_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-02 09:34:26.000000 weblate_schemas-2023.2/weblate_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-06-08 18:02:14.158708 weblate_schemas-2023.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      302 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.150708 weblate_schemas-2023.3/weblate_schemas/
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/weblate_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-backup.schema.json
+-rw-r--r--   0 runner    (1001) docker     (122)    21715 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-component.schema.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-memory.schema.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8600 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/schemas/weblate-userdata.schema.json
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-06-08 18:01:55.000000 weblate_schemas-2023.3/weblate_schemas/test_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 18:02:14.154708 weblate_schemas-2023.3/weblate_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-08 18:02:14.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-08 18:02:13.000000 weblate_schemas-2023.3/weblate_schemas.egg-info/top_level.txt
```

### Comparing `weblate_schemas-2023.2/CHANGES.rst` & `weblate_schemas-2023.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2023.3
+------
+
+* Released on 8th June 2023.
+* Added theme to user data.
+
 2023.2
 ------
 
 * Released on 2nd March 2023.
 * Fixed project backup with unicode website URLs.
 
 2023.1
```

### Comparing `weblate_schemas-2023.2/LICENSE` & `weblate_schemas-2023.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.2/PKG-INFO` & `weblate_schemas-2023.3/weblate_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: weblate_schemas
-Version: 2023.2
+Name: weblate-schemas
+Version: 2023.3
 Summary: A collection of JSON schemas used by Weblate
 Home-page: https://weblate.org/
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: MIT
 Download-URL: https://github.com/WeblateOrg/weblate_schemas
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/weblate_schemas/issues
@@ -13,15 +13,15 @@
 Project-URL: Twitter, https://twitter.com/WeblateOrg
 Project-URL: Funding, https://weblate.org/donate/
 Description: .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
            :alt: Weblate
            :target: https://weblate.org/
            :height: 80px
         
-        **Weblate is a copylefted libre software web-based continuous localization system,
+        **Weblate is libre software web-based continuous localization system,
         used by over 2500 libre projects and companies in more than 165 countries.**
         
         This module contains schemas used in Weblate exports.
         
         .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
             :alt: Website
             :target: https://weblate.org/
```

### Comparing `weblate_schemas-2023.2/README.rst` & `weblate_schemas-2023.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 This module contains schemas used in Weblate exports.
 
 .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
     :alt: Website
     :target: https://weblate.org/
```

### Comparing `weblate_schemas-2023.2/setup.cfg` & `weblate_schemas-2023.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weblate_schemas
-version = 2023.2
+version = 2023.3
 description = A collection of JSON schemas used by Weblate
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@cihar.com
 license = MIT
@@ -51,20 +51,11 @@
 per-file-ignores = 
 
 [pycodestyle]
 extend-select = E,W1,W2,W3,W504,W505,W6
 exclude = 
 max-line-length = 88
 
-[isort]
-multi_line_output = 3
-include_trailing_comma = True
-force_grid_wrap = 0
-use_parentheses = True
-line_length = 88
-known_first_party = weblate_schema
-known_third_party = jsonschema
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `weblate_schemas-2023.2/weblate_schemas/__init__.py` & `weblate_schemas-2023.3/weblate_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.2/weblate_schemas/schemas/weblate-backup.schema.json` & `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-backup.schema.json`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.2/weblate_schemas/schemas/weblate-component.schema.json` & `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-component.schema.json`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.2/weblate_schemas/schemas/weblate-memory.schema.json` & `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-memory.schema.json`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.2/weblate_schemas/schemas/weblate-userdata.schema.json` & `weblate_schemas-2023.3/weblate_schemas/schemas/weblate-userdata.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999416433239963%*

 * *Differences: {"'properties'": "{'profile': {'properties': {'theme': OrderedDict([('$id', "*

 * *                 "'#root/profile/theme'), ('title', 'Theme'), ('type', 'string'), ('default', "*

 * *                 "'auto'), ('examples', ['auto']), ('pattern', '^(auto|dark|light)$')])}}}"}*

```diff
@@ -235,14 +235,24 @@
                     "default": 0,
                     "examples": [
                         1
                     ],
                     "title": "Number of suggested strings",
                     "type": "integer"
                 },
+                "theme": {
+                    "$id": "#root/profile/theme",
+                    "default": "auto",
+                    "examples": [
+                        "auto"
+                    ],
+                    "pattern": "^(auto|dark|light)$",
+                    "title": "Theme",
+                    "type": "string"
+                },
                 "translate_mode": {
                     "$id": "#root/profile/translate_mode",
                     "default": 0,
                     "examples": [
                         0
                     ],
                     "title": "Translation editor mode",
```

### Comparing `weblate_schemas-2023.2/weblate_schemas/test_valid.py` & `weblate_schemas-2023.3/weblate_schemas/test_valid.py`

 * *Files identical despite different names*

### Comparing `weblate_schemas-2023.2/weblate_schemas.egg-info/PKG-INFO` & `weblate_schemas-2023.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: weblate-schemas
-Version: 2023.2
+Name: weblate_schemas
+Version: 2023.3
 Summary: A collection of JSON schemas used by Weblate
 Home-page: https://weblate.org/
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: MIT
 Download-URL: https://github.com/WeblateOrg/weblate_schemas
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/weblate_schemas/issues
@@ -13,15 +13,15 @@
 Project-URL: Twitter, https://twitter.com/WeblateOrg
 Project-URL: Funding, https://weblate.org/donate/
 Description: .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
            :alt: Weblate
            :target: https://weblate.org/
            :height: 80px
         
-        **Weblate is a copylefted libre software web-based continuous localization system,
+        **Weblate is libre software web-based continuous localization system,
         used by over 2500 libre projects and companies in more than 165 countries.**
         
         This module contains schemas used in Weblate exports.
         
         .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
             :alt: Website
             :target: https://weblate.org/
```

### Comparing `weblate_schemas-2023.2/weblate_schemas.egg-info/SOURCES.txt` & `weblate_schemas-2023.3/weblate_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

