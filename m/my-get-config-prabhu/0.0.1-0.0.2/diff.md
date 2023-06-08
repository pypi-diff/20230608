# Comparing `tmp/my_get_config_prabhu-0.0.1.tar.gz` & `tmp/my_get_config_prabhu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_get_config_prabhu-0.0.1.tar", last modified: Thu Jun  8 17:52:12 2023, max compression
+gzip compressed data, was "my_get_config_prabhu-0.0.2.tar", last modified: Thu Jun  8 17:55:24 2023, max compression
```

## Comparing `my_get_config_prabhu-0.0.1.tar` & `my_get_config_prabhu-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 17:52:12.721840 my_get_config_prabhu-0.0.1/
--rw-rw-rw-   0        0        0      161 2023-06-08 17:52:12.720821 my_get_config_prabhu-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 17:52:12.688339 my_get_config_prabhu-0.0.1/my_first_package/
--rw-rw-rw-   0        0        0        0 2023-06-08 17:25:56.000000 my_get_config_prabhu-0.0.1/my_first_package/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-06-08 17:29:16.000000 my_get_config_prabhu-0.0.1/my_first_package/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 17:52:12.719666 my_get_config_prabhu-0.0.1/my_get_config_prabhu.egg-info/
--rw-rw-rw-   0        0        0      161 2023-06-08 17:52:12.000000 my_get_config_prabhu-0.0.1/my_get_config_prabhu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-08 17:52:12.000000 my_get_config_prabhu-0.0.1/my_get_config_prabhu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 17:52:12.000000 my_get_config_prabhu-0.0.1/my_get_config_prabhu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 17:52:12.000000 my_get_config_prabhu-0.0.1/my_get_config_prabhu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 17:52:12.000000 my_get_config_prabhu-0.0.1/my_get_config_prabhu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 17:52:12.722819 my_get_config_prabhu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      249 2023-06-08 17:51:54.000000 my_get_config_prabhu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 17:55:24.609522 my_get_config_prabhu-0.0.2/
+-rw-rw-rw-   0        0        0      161 2023-06-08 17:55:24.608393 my_get_config_prabhu-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 17:55:24.579146 my_get_config_prabhu-0.0.2/my_first_package/
+-rw-rw-rw-   0        0        0        0 2023-06-08 17:25:56.000000 my_get_config_prabhu-0.0.2/my_first_package/__init__.py
+-rw-rw-rw-   0        0        0     1791 2023-06-08 17:54:31.000000 my_get_config_prabhu-0.0.2/my_first_package/main.py
+drwxrwxrwx   0        0        0        0 2023-06-08 17:55:24.605903 my_get_config_prabhu-0.0.2/my_get_config_prabhu.egg-info/
+-rw-rw-rw-   0        0        0      161 2023-06-08 17:55:24.000000 my_get_config_prabhu-0.0.2/my_get_config_prabhu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-08 17:55:24.000000 my_get_config_prabhu-0.0.2/my_get_config_prabhu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 17:55:24.000000 my_get_config_prabhu-0.0.2/my_get_config_prabhu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-08 17:55:24.000000 my_get_config_prabhu-0.0.2/my_get_config_prabhu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-08 17:55:24.000000 my_get_config_prabhu-0.0.2/my_get_config_prabhu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 17:55:24.610024 my_get_config_prabhu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      249 2023-06-08 17:55:10.000000 my_get_config_prabhu-0.0.2/setup.py
```

### Comparing `my_get_config_prabhu-0.0.1/my_first_package/main.py` & `my_get_config_prabhu-0.0.2/my_first_package/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json, requests
 
-def getConfig():
+def getConfigPrabhu():
     ConfigData = {
         "configdata":
             {                    
                 "app_url": {
                     "field_label": "Enter Application URL",
                     "datatype": "url",
                     "required": "yes",
```

