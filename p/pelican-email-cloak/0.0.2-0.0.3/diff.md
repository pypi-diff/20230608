# Comparing `tmp/pelican_email_cloak-0.0.2.tar.gz` & `tmp/pelican_email_cloak-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_email_cloak-0.0.2.tar", max compression
+gzip compressed data, was "pelican_email_cloak-0.0.3.tar", max compression
```

## Comparing `pelican_email_cloak-0.0.2.tar` & `pelican_email_cloak-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-08 13:02:48.379033 pelican_email_cloak-0.0.2/LICENSE
--rw-r--r--   0        0        0      693 2023-06-08 13:04:16.936932 pelican_email_cloak-0.0.2/README.md
--rw-r--r--   0        0        0       35 2023-06-08 11:14:20.652110 pelican_email_cloak-0.0.2/pelican/plugins/email_cloak/__init__.py
--rw-r--r--   0        0        0     1754 2023-06-08 12:30:17.060680 pelican_email_cloak-0.0.2/pelican/plugins/email_cloak/email_cloak.py
--rw-r--r--   0        0        0     2460 2023-06-08 13:12:42.178795 pelican_email_cloak-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pelican_email_cloak-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-08 13:02:48.379033 pelican_email_cloak-0.0.3/LICENSE
+-rw-r--r--   0        0        0      826 2023-06-08 13:14:16.143047 pelican_email_cloak-0.0.3/README.md
+-rw-r--r--   0        0        0       35 2023-06-08 11:14:20.652110 pelican_email_cloak-0.0.3/pelican/plugins/email_cloak/__init__.py
+-rw-r--r--   0        0        0     1754 2023-06-08 12:30:17.060680 pelican_email_cloak-0.0.3/pelican/plugins/email_cloak/email_cloak.py
+-rw-r--r--   0        0        0     2460 2023-06-08 13:13:45.474052 pelican_email_cloak-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 pelican_email_cloak-0.0.3/PKG-INFO
```

### Comparing `pelican_email_cloak-0.0.2/LICENSE` & `pelican_email_cloak-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.0.2/pelican/plugins/email_cloak/email_cloak.py` & `pelican_email_cloak-0.0.3/pelican/plugins/email_cloak/email_cloak.py`

 * *Files identical despite different names*

### Comparing `pelican_email_cloak-0.0.2/pyproject.toml` & `pelican_email_cloak-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-email-cloak"
-version = "0.0.2"
+version = "0.0.3"
 description = "E-mail cloaking plugin for Pelican"
 authors = ["Demetrio Battaglia <deme3.iot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pelican", "plugin"]
 repository = "https://github.com/deme3/pelican-email-cloak"
 documentation = "https://docs.getpelican.com"
```

### Comparing `pelican_email_cloak-0.0.2/PKG-INFO` & `pelican_email_cloak-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-email-cloak
-Version: 0.0.2
+Version: 0.0.3
 Summary: E-mail cloaking plugin for Pelican
 Home-page: https://github.com/deme3/pelican-email-cloak
 License: MIT
 Keywords: pelican,plugin
 Author: Demetrio Battaglia
 Author-email: deme3.iot@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -52,15 +52,20 @@
 PLUGINS = [
     # ...
     'email_cloak',
     # ...
 ]
 ```
 
-and place the plugin at `pelican/plugins/email_cloak` in your plugins folder.
+Pelican should automatically discover the plugin after installation under the namespace `pelican.plugins`.
 
 E-mails in articles and pages will be cloaked.
 
+## Changelog
+
+-   0.0.1 up to 0.0.3: Initial release
+    -   Version bumped to update PyPI description
+
 ## License
 
 This project is licensed under the MIT license.
```

