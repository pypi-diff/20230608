# Comparing `tmp/Pallets-Sphinx-Themes-2.1.0.tar.gz` & `tmp/Pallets-Sphinx-Themes-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pallets-Sphinx-Themes-2.1.0.tar", last modified: Tue Apr 25 17:30:32 2023, max compression
+gzip compressed data, was "Pallets-Sphinx-Themes-2.1.1.tar", last modified: Thu Jun  8 15:21:26 2023, max compression
```

## Comparing `Pallets-Sphinx-Themes-2.1.0.tar` & `Pallets-Sphinx-Themes-2.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/
--rw-r--r--   0 david     (1000) david     (1000)     5761 2023-04-25 17:28:30.000000 Pallets-Sphinx-Themes-2.1.0/CHANGES.rst
--rw-r--r--   0 david     (1000) david     (1000)     1475 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/LICENSE.rst
--rw-r--r--   0 david     (1000) david     (1000)      102 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)     1578 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      512 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/README.rst
--rw-r--r--   0 david     (1000) david     (1000)     1980 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      145 2023-04-25 17:21:40.000000 Pallets-Sphinx-Themes-2.1.0/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     1578 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1969 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      126 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/entry_points.txt
--rw-r--r--   0 david     (1000) david     (1000)       20 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       22 2023-04-25 17:30:32.000000 Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/top_level.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/
--rw-r--r--   0 david     (1000) david     (1000)     5359 2023-04-25 17:23:09.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     1265 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/theme_check.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/__init__.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.679424 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/static/
--rw-r--r--   0 david     (1000) david     (1000)      453 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/static/babel.css
--rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/babel/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/
--rw-r--r--   0 david     (1000) david     (1000)      174 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     7785 2023-04-25 17:19:12.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/domain.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/static/
--rw-r--r--   0 david     (1000) david     (1000)      585 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/static/click.css
--rw-r--r--   0 david     (1000) david     (1000)       70 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/static/
--rw-r--r--   0 david     (1000) david     (1000)      237 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/static/flask.css
--rw-r--r--   0 david     (1000) david     (1000)       47 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/flask/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/
--rw-r--r--   0 david     (1000) david     (1000)     1548 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     8756 2023-04-25 17:21:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/domain.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/static/
--rw-r--r--   0 david     (1000) david     (1000)      425 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/static/jinja.css
--rw-r--r--   0 david     (1000) david     (1000)       70 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/static/
--rw-r--r--   0 david     (1000) david     (1000)      449 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/static/platter.css
--rw-r--r--   0 david     (1000) david     (1000)       49 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/platter/theme.conf
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/
--rw-r--r--   0 david     (1000) david     (1000)      391 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/404.html
--rw-r--r--   0 david     (1000) david     (1000)     4052 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)       38 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/ethicalads.html
--rw-r--r--   0 david     (1000) david     (1000)      768 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/layout.html
--rw-r--r--   0 david     (1000) david     (1000)       66 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/localtoc.html
--rw-r--r--   0 david     (1000) david     (1000)      173 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/project.html
--rw-r--r--   0 david     (1000) david     (1000)      645 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/relations.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/
--rw-r--r--   0 david     (1000) david     (1000)     8153 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css
--rw-r--r--   0 david     (1000) david     (1000)     1582 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js
--rw-r--r--   0 david     (1000) david     (1000)      181 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/theme.conf
--rw-r--r--   0 david     (1000) david     (1000)      253 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/versions.html
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2023-04-25 17:30:32.682757 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/static/
--rw-r--r--   0 david     (1000) david     (1000)      237 2023-04-22 15:05:50.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/static/werkzeug.css
--rw-r--r--   0 david     (1000) david     (1000)       50 2022-12-22 18:11:42.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/werkzeug/theme.conf
--rw-r--r--   0 david     (1000) david     (1000)     4580 2022-12-23 23:44:01.000000 Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-08 15:21:26.435573 Pallets-Sphinx-Themes-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.423573 Pallets-Sphinx-Themes-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-08 15:21:26.000000 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-08 15:21:26.000000 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:21:26.000000 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 15:21:26.000000 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 15:21:26.000000 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 15:21:26.000000 Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/theme_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/babel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/babel/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/babel/static/babel.css
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/babel/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/static/click.css
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/flask/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/flask/static/flask.css
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/flask/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/static/jinja.css
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.427573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/platter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/platter/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/platter/static/platter.css
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/platter/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/ethicalads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/project.html
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/relations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/werkzeug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:21:26.431573 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/werkzeug/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/werkzeug/static/werkzeug.css
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/werkzeug/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-08 15:21:11.000000 Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/versions.py
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/CHANGES.rst` & `Pallets-Sphinx-Themes-2.1.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 2.1.1
+-------------
+
+Released 2023-06-08
+
+-   Remove leftover Python 2 compatibility code. :pr:`69`
+-   Dotted underlines on links are smaller. :issue:`70`
+
+
 Version 2.1.0
 -------------
 
 Released 2023-04-25
 
 -   Drop support for Python 3.6 and 3.7.
 -   Require Sphinx >= 3.
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/LICENSE.rst` & `Pallets-Sphinx-Themes-2.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/PKG-INFO` & `Pallets-Sphinx-Themes-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pallets-Sphinx-Themes
-Version: 2.1.0
+Version: 2.1.1
 Summary: Sphinx themes for Pallets and related projects.
 Home-page: https://github.com/pallets/pallets-sphinx-themes/
 Author: Pallets
 Author-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Source Code, https://github.com/pallets/pallets-sphinx-themes/
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/README.rst` & `Pallets-Sphinx-Themes-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/setup.cfg` & `Pallets-Sphinx-Themes-2.1.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Pallets-Sphinx-Themes
-version = 2.1.0
+version = 2.1.1
 url = https://github.com/pallets/pallets-sphinx-themes/
 project_urls = 
 	Donate = https://palletsprojects.com/donate
 	Source Code = https://github.com/pallets/pallets-sphinx-themes/
 	Issue Tracker = https://github.com/pallets/pallets-sphinx-themes/issues/
 	Chat = https://discord.gg/pallets
 license = BSD-3-Clause
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO` & `Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pallets-Sphinx-Themes
-Version: 2.1.0
+Version: 2.1.1
 Summary: Sphinx themes for Pallets and related projects.
 Home-page: https://github.com/pallets/pallets-sphinx-themes/
 Author: Pallets
 Author-email: contact@palletsprojects.com
 License: BSD-3-Clause
 Project-URL: Donate, https://palletsprojects.com/donate
 Project-URL: Source Code, https://github.com/pallets/pallets-sphinx-themes/
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt` & `Pallets-Sphinx-Themes-2.1.1/src/Pallets_Sphinx_Themes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/__init__.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/__init__.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/theme_check.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/theme_check.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/domain.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import shlex
 import subprocess
 import sys
 import tempfile
 from functools import partial
 
 import click
-from click._compat import text_type
 from click.testing import CliRunner
 from click.testing import EchoingStdin
 from docutils import nodes
 from docutils.parsers.rst import Directive
 from docutils.statemachine import ViewList
 from sphinx.domains import Domain
 
@@ -63,15 +62,15 @@
     finally:
         subprocess.call = old_call
 
 
 class ExampleRunner(CliRunner):
     def __init__(self):
         super().__init__(echo_stdin=True)
-        self.namespace = {"click": click, "__file__": "dummy.py", "str": text_type}
+        self.namespace = {"click": click, "__file__": "dummy.py"}
 
     @contextlib.contextmanager
     def isolation(self, *args, **kwargs):
         iso = super().isolation(*args, **kwargs)
 
         with iso as streams:
             try:
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/click/static/click.css` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/click/static/click.css`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/__init__.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/__init__.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/jinja/domain.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/jinja/domain.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/__init__.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/__init__.py`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/layout.html` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/layout.html`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/relations.html` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/relations.html`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/static/pocoo.css`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
 /* -- body styles --------------------------------------------------- */
 
 a {
   text-decoration: underline;
   text-decoration-style: dotted;
   text-decoration-color: #000;
+  text-decoration-thickness: 1px;
 }
 
 a:hover {
   text-decoration-style: solid;
 }
 
 h1, h2, h3, h4, h5, h6 {
```

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/themes/pocoo/static/version_warning_offset.js`

 * *Files identical despite different names*

### Comparing `Pallets-Sphinx-Themes-2.1.0/src/pallets_sphinx_themes/versions.py` & `Pallets-Sphinx-Themes-2.1.1/src/pallets_sphinx_themes/versions.py`

 * *Files identical despite different names*

