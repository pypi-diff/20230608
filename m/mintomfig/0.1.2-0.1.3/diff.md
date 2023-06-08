# Comparing `tmp/mintomfig-0.1.2.tar.gz` & `tmp/mintomfig-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintomfig-0.1.2.tar", max compression
+gzip compressed data, was "mintomfig-0.1.3.tar", max compression
```

## Comparing `mintomfig-0.1.2.tar` & `mintomfig-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       30 2023-06-07 19:02:13.667768 mintomfig-0.1.2/README.md
--rw-r--r--   0        0        0     1770 2023-06-07 19:17:57.853322 mintomfig-0.1.2/mintomfig/__init__.py
--rw-r--r--   0        0        0      295 2023-06-07 19:22:00.837022 mintomfig-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 mintomfig-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-06-07 19:02:13.667768 mintomfig-0.1.3/README.md
+-rw-r--r--   0        0        0     1772 2023-06-08 05:41:44.062190 mintomfig-0.1.3/mintomfig/__init__.py
+-rw-r--r--   0        0        0      295 2023-06-08 05:41:16.215492 mintomfig-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 mintomfig-0.1.3/PKG-INFO
```

### Comparing `mintomfig-0.1.2/mintomfig/__init__.py` & `mintomfig-0.1.3/mintomfig/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 
 class ConfigError(Exception):
     def __init__(self, message=""):
         super().__init__(message)
 
 
 class TomlConfigFile:
-    def get_config_section(self, section, required=True):
+    def get_config_section(self, section, required=False):
         if section not in self.config:
             if required:
                 raise ConfigError(f"config file missing [{section}] section")
             else:
                 return {}
         return self.config[section]
 
-    def get_config_value(self, table, key, required=True, default=None):
+    def get_config_value(self, table, key, default=None, required=False):
         if key not in table:
             if required:
                 raise ConfigError(f"config table {table} missing {key} key")
             else:
                 return default
         return table[key]
```

### Comparing `mintomfig-0.1.2/PKG-INFO` & `mintomfig-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintomfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

