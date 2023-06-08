# Comparing `tmp/custom_flet-0.1.0.tar.gz` & `tmp/custom_flet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_flet-0.1.0.tar", last modified: Thu Jun  8 14:30:51 2023, max compression
+gzip compressed data, was "custom_flet-0.1.1.tar", last modified: Thu Jun  8 16:16:36 2023, max compression
```

## Comparing `custom_flet-0.1.0.tar` & `custom_flet-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:30:51.227864 custom_flet-0.1.0/
--rw-rw-rw-   0        0        0      117 2023-06-08 14:30:51.226920 custom_flet-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 14:30:51.212860 custom_flet-0.1.0/components/
--rw-rw-rw-   0        0        0      154 2023-06-08 14:29:04.000000 custom_flet-0.1.0/components/__init__.py
--rw-rw-rw-   0        0        0      607 2023-06-07 13:30:58.000000 custom_flet-0.1.0/components/custom_icon.py
--rw-rw-rw-   0        0        0      962 2023-06-07 13:36:18.000000 custom_flet-0.1.0/components/custom_icon_button.py
--rw-rw-rw-   0        0        0     2090 2023-06-08 14:16:08.000000 custom_flet-0.1.0/components/elevated_custom_logo_button.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:30:51.225942 custom_flet-0.1.0/custom_flet.egg-info/
--rw-rw-rw-   0        0        0      117 2023-06-08 14:30:51.000000 custom_flet-0.1.0/custom_flet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-08 14:30:51.000000 custom_flet-0.1.0/custom_flet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:30:51.000000 custom_flet-0.1.0/custom_flet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 14:30:51.000000 custom_flet-0.1.0/custom_flet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 14:30:51.227864 custom_flet-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      207 2023-06-08 14:30:44.000000 custom_flet-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:16:36.342941 custom_flet-0.1.1/
+-rw-rw-rw-   0        0        0      184 2023-06-08 16:16:36.341630 custom_flet-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 16:16:36.321105 custom_flet-0.1.1/custom_flet/
+-rw-rw-rw-   0        0        0      187 2023-06-08 16:12:15.000000 custom_flet-0.1.1/custom_flet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:16:36.340628 custom_flet-0.1.1/custom_flet.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-06-08 16:16:36.000000 custom_flet-0.1.1/custom_flet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-06-08 16:16:36.000000 custom_flet-0.1.1/custom_flet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:16:36.000000 custom_flet-0.1.1/custom_flet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 16:16:36.000000 custom_flet-0.1.1/custom_flet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:16:36.342941 custom_flet-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      307 2023-06-08 16:16:32.000000 custom_flet-0.1.1/setup.py
```

