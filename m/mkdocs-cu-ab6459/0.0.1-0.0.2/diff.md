# Comparing `tmp/mkdocs_cu_ab6459-0.0.1.tar.gz` & `tmp/mkdocs_cu_ab6459-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_cu_ab6459-0.0.1.tar", last modified: Thu Jun  8 10:13:20 2023, max compression
+gzip compressed data, was "mkdocs_cu_ab6459-0.0.2.tar", last modified: Thu Jun  8 10:29:15 2023, max compression
```

## Comparing `mkdocs_cu_ab6459-0.0.1.tar` & `mkdocs_cu_ab6459-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:13:20.991230 mkdocs_cu_ab6459-0.0.1/
--rw-rw-r--   0 ian       (1000) ian       (1000)      174 2023-06-08 10:13:17.000000 mkdocs_cu_ab6459-0.0.1/MANIFEST.in
--rw-rw-r--   0 ian       (1000) ian       (1000)      445 2023-06-08 10:13:20.991230 mkdocs_cu_ab6459-0.0.1/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)       76 2023-06-08 09:59:30.000000 mkdocs_cu_ab6459-0.0.1/README.md
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:13:20.987230 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/
--rw-rw-r--   0 ian       (1000) ian       (1000)     6140 2023-06-08 08:55:10.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/base.html
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:13:20.987230 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/
--rw-rw-r--   0 ian       (1000) ian       (1000)    70353 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    51819 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    70427 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    51894 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    11933 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    10010 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    11926 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    10082 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)   107678 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    85188 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)   107546 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    85117 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)   280812 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.css
--rw-rw-r--   0 ian       (1000) ian       (1000)   232914 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)   280391 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.rtl.css
--rw-rw-r--   0 ian       (1000) ian       (1000)   233021 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css
--rw-rw-r--   0 ian       (1000) ian       (1000)     6469 2023-06-08 08:38:54.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/custom.css
--rw-rw-r--   0 ian       (1000) ian       (1000)     2080 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/diagram.css
--rw-rw-r--   0 ian       (1000) ian       (1000)    11470 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/prism.css
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:13:20.987230 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/images/
--rw-rw-r--   0 ian       (1000) ian       (1000)     7231 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/images/logo_dark.png
--rw-rw-r--   0 ian       (1000) ian       (1000)     7592 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/images/logo_light.png
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:13:20.991230 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/
--rw-rw-r--   0 ian       (1000) ian       (1000)   207425 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.bundle.js
--rw-rw-r--   0 ian       (1000) ian       (1000)    80421 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js
--rw-rw-r--   0 ian       (1000) ian       (1000)   135457 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.esm.js
--rw-rw-r--   0 ian       (1000) ian       (1000)    73914 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.esm.min.js
--rw-rw-r--   0 ian       (1000) ian       (1000)   145007 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.js
--rw-rw-r--   0 ian       (1000) ian       (1000)    60348 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.min.js
--rw-rw-r--   0 ian       (1000) ian       (1000)     1197 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/darkmode.js
--rw-rw-r--   0 ian       (1000) ian       (1000)    42176 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/prism.js
--rw-rw-r--   0 ian       (1000) ian       (1000)    23168 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/simple-diagram.js
--rw-rw-r--   0 ian       (1000) ian       (1000)       25 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/main.html
--rw-rw-r--   0 ian       (1000) ian       (1000)       25 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/mkdocs_theme.yml
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:13:20.987230 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/
--rw-rw-r--   0 ian       (1000) ian       (1000)      445 2023-06-08 10:13:20.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)     1615 2023-06-08 10:13:20.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/SOURCES.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 10:13:20.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       45 2023-06-08 10:13:20.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/entry_points.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 10:10:42.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/not-zip-safe
--rw-rw-r--   0 ian       (1000) ian       (1000)        7 2023-06-08 10:13:20.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/requires.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 10:13:20.000000 mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-06-08 10:13:20.991230 mkdocs_cu_ab6459-0.0.1/setup.cfg
--rw-rw-r--   0 ian       (1000) ian       (1000)      800 2023-06-08 10:10:38.000000 mkdocs_cu_ab6459-0.0.1/setup.py
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/
+-rw-rw-r--   0 ian       (1000) ian       (1000)      174 2023-06-08 10:13:17.000000 mkdocs_cu_ab6459-0.0.2/MANIFEST.in
+-rw-rw-r--   0 ian       (1000) ian       (1000)      445 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)       76 2023-06-08 09:59:30.000000 mkdocs_cu_ab6459-0.0.2/README.md
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/
+-rw-rw-r--   0 ian       (1000) ian       (1000)        0 2023-06-08 10:28:01.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/__init__.py
+-rw-rw-r--   0 ian       (1000) ian       (1000)     6140 2023-06-08 08:55:10.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/base.html
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/
+-rw-rw-r--   0 ian       (1000) ian       (1000)    70353 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    51819 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    70427 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    51894 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    11933 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    10010 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    11926 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    10082 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)   107678 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    85188 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)   107546 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    85117 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)   280812 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)   232914 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)   280391 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.rtl.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)   233021 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)     6469 2023-06-08 08:38:54.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/custom.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)     2080 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/diagram.css
+-rw-rw-r--   0 ian       (1000) ian       (1000)    11470 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/prism.css
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/images/
+-rw-rw-r--   0 ian       (1000) ian       (1000)     7231 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/images/logo_dark.png
+-rw-rw-r--   0 ian       (1000) ian       (1000)     7592 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/images/logo_light.png
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/
+-rw-rw-r--   0 ian       (1000) ian       (1000)   207425 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.bundle.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)    80421 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)   135457 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.esm.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)    73914 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.esm.min.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)   145007 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)    60348 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.min.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1197 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/darkmode.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)    42176 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/prism.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)    23168 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/simple-diagram.js
+-rw-rw-r--   0 ian       (1000) ian       (1000)       25 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/main.html
+-rw-rw-r--   0 ian       (1000) ian       (1000)       25 2023-06-08 07:28:33.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/mkdocs_theme.yml
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 10:29:15.467527 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/
+-rw-rw-r--   0 ian       (1000) ian       (1000)      445 2023-06-08 10:29:15.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)     1644 2023-06-08 10:29:15.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/SOURCES.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 10:29:15.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       45 2023-06-08 10:29:15.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/entry_points.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 10:10:42.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/not-zip-safe
+-rw-rw-r--   0 ian       (1000) ian       (1000)        7 2023-06-08 10:29:15.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/requires.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       17 2023-06-08 10:29:15.000000 mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/top_level.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-06-08 10:29:15.471527 mkdocs_cu_ab6459-0.0.2/setup.cfg
+-rw-rw-r--   0 ian       (1000) ian       (1000)      800 2023-06-08 10:29:08.000000 mkdocs_cu_ab6459-0.0.2/setup.py
```

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/base.html` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.rtl.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/custom.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/custom.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/diagram.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/diagram.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/css/prism.css` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/css/prism.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/images/logo_dark.png` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/images/logo_dark.png`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/images/logo_light.png` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/images/logo_light.png`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.bundle.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.esm.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.esm.min.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/bootstrap.min.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/darkmode.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/darkmode.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/prism.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/prism.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459/js/simple-diagram.js` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459/js/simple-diagram.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.1/mkdocs_cu_ab6459.egg-info/SOURCES.txt` & `mkdocs_cu_ab6459-0.0.2/mkdocs_cu_ab6459.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
+mkdocs_cu_ab6459/__init__.py
 mkdocs_cu_ab6459/base.html
 mkdocs_cu_ab6459/main.html
 mkdocs_cu_ab6459/mkdocs_theme.yml
 mkdocs_cu_ab6459.egg-info/PKG-INFO
 mkdocs_cu_ab6459.egg-info/SOURCES.txt
 mkdocs_cu_ab6459.egg-info/dependency_links.txt
 mkdocs_cu_ab6459.egg-info/entry_points.txt
```

### Comparing `mkdocs_cu_ab6459-0.0.1/setup.py` & `mkdocs_cu_ab6459-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_desc = fh.read()
 
 setup(
     name="mkdocs_cu_ab6459",
-    version="0.0.1",
+    version="0.0.2",
     url='',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Topic :: Documentation',
         'Topic :: Text Processing',
     ],
     install_requires=[
```

