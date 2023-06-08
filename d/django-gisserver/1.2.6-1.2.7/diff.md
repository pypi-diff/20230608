# Comparing `tmp/django-gisserver-1.2.6.tar.gz` & `tmp/django-gisserver-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gisserver-1.2.6.tar", last modified: Wed Jun  7 10:52:10 2023, max compression
+gzip compressed data, was "django-gisserver-1.2.7.tar", last modified: Thu Jun  8 09:12:21 2023, max compression
```

## Comparing `django-gisserver-1.2.6.tar` & `django-gisserver-1.2.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/
--rw-rw-r--   0 jan       (1000) jan       (1000)    12992 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/CHANGES.md
--rw-rw-r--   0 jan       (1000) jan       (1000)    16725 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/LICENSE
--rw-rw-r--   0 jan       (1000) jan       (1000)      227 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/MANIFEST.in
--rw-rw-r--   0 jan       (1000) jan       (1000)     5369 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     4027 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/README.md
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.696781 django-gisserver-1.2.6/django_gisserver.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)     5369 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     1915 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2022-09-07 10:15:14.000000 django-gisserver-1.2.6/django_gisserver.egg-info/not-zip-safe
--rw-rw-r--   0 jan       (1000) jan       (1000)      180 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       10 2023-06-07 10:52:10.000000 django-gisserver-1.2.6/django_gisserver.egg-info/top_level.txt
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/
--rw-rw-r--   0 jan       (1000) jan       (1000)       40 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2108 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/conf.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5329 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/db.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4596 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/exceptions.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    32232 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/features.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12619 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/geometries.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/operations/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/operations/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    16780 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/operations/base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    18240 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/operations/wfs20.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/output/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1950 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7954 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1542 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/buffer.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6198 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/csv.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    11236 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/output/geojson.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    26913 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/gml32.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     9189 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/results.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6113 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/utils.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4603 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/output/xmlschema.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/parsers/
--rw-rw-r--   0 jan       (1000) jan       (1000)      290 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4864 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/base.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/parsers/fes20/
--rw-rw-r--   0 jan       (1000) jan       (1000)      624 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     9747 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/expressions.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3507 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/filters.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     8726 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/functions.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2863 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/identifiers.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    23601 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/operators.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    10083 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/query.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2176 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/fes20/sorting.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/parsers/gml/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1462 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/gml/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1065 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/parsers/gml/base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3171 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/gml/geometries.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3553 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/parsers/tags.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1038 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/parsers/values.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/queries/
--rw-rw-r--   0 jan       (1000) jan       (1000)      892 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7146 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/adhoc.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5943 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7095 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/queries/stored.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.696781 django-gisserver-1.2.6/gisserver/static/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/static/gisserver/
--rw-rw-r--   0 jan       (1000) jan       (1000)      163 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/static/gisserver/index.css
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.696781 django-gisserver-1.2.6/gisserver/templates/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/templates/gisserver/
--rw-rw-r--   0 jan       (1000) jan       (1000)      866 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/index.html
--rw-rw-r--   0 jan       (1000) jan       (1000)      993 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/service_description.html
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.700781 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1041 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)     8675 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)      636 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml
--rw-rw-r--   0 jan       (1000) jan       (1000)      538 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_field.html
--rw-rw-r--   0 jan       (1000) jan       (1000)      788 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_type.html
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/gisserver/templatetags/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templatetags/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      204 2022-09-07 09:58:17.000000 django-gisserver-1.2.6/gisserver/templatetags/gisserver_tags.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    34202 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/types.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    13252 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/gisserver/views.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      496 2023-06-07 10:52:10.704781 django-gisserver-1.2.6/setup.cfg
--rwxrwxr-x   0 jan       (1000) jan       (1000)     2471 2023-06-07 10:50:30.000000 django-gisserver-1.2.6/setup.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/
+-rw-rw-r--   0 lars      (1000) lars      (1000)    13086 2023-06-08 09:05:07.000000 django-gisserver-1.2.7/CHANGES.md
+-rw-rw-r--   0 lars      (1000) lars      (1000)    16725 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/LICENSE
+-rw-rw-r--   0 lars      (1000) lars      (1000)      227 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/MANIFEST.in
+-rw-rw-r--   0 lars      (1000) lars      (1000)     5349 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/PKG-INFO
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4027 2023-05-03 13:46:37.000000 django-gisserver-1.2.7/README.md
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/django_gisserver.egg-info/
+-rw-rw-r--   0 lars      (1000) lars      (1000)     5349 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/PKG-INFO
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1915 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)        1 2023-01-11 09:33:57.000000 django-gisserver-1.2.7/django_gisserver.egg-info/not-zip-safe
+-rw-rw-r--   0 lars      (1000) lars      (1000)      180 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/requires.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)       10 2023-06-08 09:12:21.000000 django-gisserver-1.2.7/django_gisserver.egg-info/top_level.txt
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/
+-rw-rw-r--   0 lars      (1000) lars      (1000)       40 2023-06-08 09:05:27.000000 django-gisserver-1.2.7/gisserver/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     2108 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/conf.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     5329 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/db.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4596 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/exceptions.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    32232 2023-05-03 09:52:03.000000 django-gisserver-1.2.7/gisserver/features.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    12619 2023-05-08 12:47:05.000000 django-gisserver-1.2.7/gisserver/geometries.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/operations/
+-rw-rw-r--   0 lars      (1000) lars      (1000)        0 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/operations/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    17012 2023-06-08 09:02:34.000000 django-gisserver-1.2.7/gisserver/operations/base.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    18635 2023-06-08 09:02:49.000000 django-gisserver-1.2.7/gisserver/operations/wfs20.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/output/
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1950 2023-05-08 12:47:05.000000 django-gisserver-1.2.7/gisserver/output/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     7954 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/base.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1542 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/buffer.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     6198 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/csv.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    11236 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/geojson.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    26913 2023-05-03 13:37:23.000000 django-gisserver-1.2.7/gisserver/output/gml32.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     9189 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/results.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     6113 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/utils.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4603 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/output/xmlschema.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/parsers/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      290 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4864 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/base.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/parsers/fes20/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      624 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     9747 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/expressions.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     3507 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/filters.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     8726 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/functions.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     2863 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/identifiers.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    23601 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/operators.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    10083 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/query.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     2176 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/fes20/sorting.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/parsers/gml/
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1462 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/gml/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1065 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/gml/base.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     3171 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/gml/geometries.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     3553 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/tags.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1038 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/parsers/values.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/queries/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      892 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     7146 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/adhoc.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     5943 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/base.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)     7095 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/queries/stored.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/static/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/static/gisserver/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      163 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/static/gisserver/index.css
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/gisserver/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      866 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/index.html
+-rw-rw-r--   0 lars      (1000) lars      (1000)      993 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/service_description.html
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.138926 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/
+-rw-rw-r--   0 lars      (1000) lars      (1000)     1041 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml
+-rw-rw-r--   0 lars      (1000) lars      (1000)     8675 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml
+-rw-rw-r--   0 lars      (1000) lars      (1000)      636 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml
+-rw-rw-r--   0 lars      (1000) lars      (1000)      538 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_field.html
+-rw-rw-r--   0 lars      (1000) lars      (1000)      788 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_type.html
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/gisserver/templatetags/
+-rw-rw-r--   0 lars      (1000) lars      (1000)        0 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templatetags/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)      204 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/templatetags/gisserver_tags.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    34202 2023-01-11 08:47:11.000000 django-gisserver-1.2.7/gisserver/types.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    13252 2023-06-08 08:38:15.000000 django-gisserver-1.2.7/gisserver/views.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)      496 2023-06-08 09:12:21.142926 django-gisserver-1.2.7/setup.cfg
+-rwxrwxr-x   0 lars      (1000) lars      (1000)     2471 2023-05-08 12:47:05.000000 django-gisserver-1.2.7/setup.py
```

### Comparing `django-gisserver-1.2.6/CHANGES.md` & `django-gisserver-1.2.7/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2023-06-08 (1.2.7)
+
+* WFS endpoints now accept a GML version number in their OUTPUTFORMAT.
+
 # 2023-06-07 (1.2.6)
 
 * Workaround for FME doing a DescribeFeatureType with the wrong outputformat.
 * Dropped support for Django versions < 3.2 and Python < 3.9.
 * Minor optimizations.
 
 # 2023-01-11 (1.2.5)
```

### Comparing `django-gisserver-1.2.6/LICENSE` & `django-gisserver-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/PKG-INFO` & `django-gisserver-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-gisserver
-Version: 1.2.6
+Version: 1.2.7
 Summary: Django speaking WFS 2.0 (exposing GeoDjango model fields)
 Home-page: https://github.com/amsterdam/django-gisserver
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Mozilla Public License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -153,9 +152,7 @@
 Much of this software is then published as Open Source so that other municipalities,
 organizations and citizens can use the software as a basis and inspiration to develop
 similar software themselves. The Municipality of Amsterdam considers it important that
 software developed with public money is also publicly available.
 
 This package is initially developed by the City of Amsterdam, but the tools
 and concepts created in this project can be used in any city.
-
-
```

### Comparing `django-gisserver-1.2.6/README.md` & `django-gisserver-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/django_gisserver.egg-info/PKG-INFO` & `django-gisserver-1.2.7/django_gisserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-gisserver
-Version: 1.2.6
+Version: 1.2.7
 Summary: Django speaking WFS 2.0 (exposing GeoDjango model fields)
 Home-page: https://github.com/amsterdam/django-gisserver
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Mozilla Public License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -153,9 +152,7 @@
 Much of this software is then published as Open Source so that other municipalities,
 organizations and citizens can use the software as a basis and inspiration to develop
 similar software themselves. The Municipality of Amsterdam considers it important that
 software developed with public money is also publicly available.
 
 This package is initially developed by the City of Amsterdam, but the tools
 and concepts created in this project can be used in any city.
-
-
```

### Comparing `django-gisserver-1.2.6/django_gisserver.egg-info/SOURCES.txt` & `django-gisserver-1.2.7/django_gisserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/conf.py` & `django-gisserver-1.2.7/gisserver/conf.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/db.py` & `django-gisserver-1.2.7/gisserver/db.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/exceptions.py` & `django-gisserver-1.2.7/gisserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/features.py` & `django-gisserver-1.2.7/gisserver/features.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/geometries.py` & `django-gisserver-1.2.7/gisserver/geometries.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/operations/base.py` & `django-gisserver-1.2.7/gisserver/operations/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,18 @@
         self.subtype = self.extra.get("subtype")
         self.renderer_class = renderer_class
         self.title = title
         self._max_page_size = max_page_size
 
     def matches(self, value):
         """Test whether the 'value' is matched by this object."""
+        if self.content_type == "application/gml+xml":
+            # Allow "application/gml+xml; version=3.2" as sent by FME.
+            # TODO rewrite this matching code in a clean way.
+            value = value.split("; ", 1)[0]
         return self.content_type == value or self.subtype == value
 
     @property
     def identifier(self):
         """The identifier to use in templates as OUTPUTFORMAT input value."""
         return self.subtype or self.content_type
```

### Comparing `django-gisserver-1.2.6/gisserver/operations/wfs20.py` & `django-gisserver-1.2.7/gisserver/operations/wfs20.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,23 @@
 SAFE_VERSION = re.compile(r"\A[0-9.]+\Z")
 RE_SAFE_FILENAME = re.compile(r"\A[A-Za-z0-9]+[A-Za-z0-9.]*")  # no dot at the start.
 
 
 class GetCapabilities(WFSMethod):
     """ "This operation returns map features, and available operations this WFS server supports."""
 
-    output_formats = [OutputFormat("text/xml")]
+    output_formats = [
+        OutputFormat(
+            "application/gml+xml",
+            version="3.2",
+            renderer_class=output.gml32_value_renderer,
+            title="GML",
+        ),
+        OutputFormat("text/xml"),
+    ]
     xml_template_name = "get_capabilities.xml"
 
     def get_parameters(self):
         # Not calling super, as this differs slightly (e.g. no output formats)
         return [
             Parameter(
                 "service",
@@ -140,16 +148,19 @@
     """
 
     output_formats = [
         OutputFormat("XMLSCHEMA", renderer_class=output.XMLSchemaRenderer),
         # At least one version of FME seems to sends a DescribeFeatureType
         # request with this output format. Do what mapserver does and just
         # send it XML Schema.
-        OutputFormat("application/gml+xml; version=3.2",
-                     renderer_class=output.XMLSchemaRenderer)
+        OutputFormat(
+            "application/gml+xml",
+            version="3.2",
+            renderer_class=output.XMLSchemaRenderer,
+        )
         # OutputFormat("text/xml", subtype="gml/3.1.1"),
     ]
 
     def get_context_data(self, typeNames, **params):
         if self.view.KVP.get("TYPENAMES") == "" or self.view.KVP.get("TYPENAME") == "":
             # Using TYPENAMES= does result in an error.
             raise MissingParameterValue("typeNames", "Empty TYPENAMES parameter")
@@ -437,15 +448,15 @@
             charset="utf-8",
             renderer_class=output.geojson_renderer,
             title="GeoJSON",
         ),
         OutputFormat(
             # Alias needed to make ESRI ArcGIS online accept the WFS.
             # It does not recognize the "subtype" as an alias.
-            "GEOJSON",
+            "geojson",
             renderer_class=output.geojson_renderer,
         ),
         OutputFormat(
             "text/csv",
             subtype="csv",
             charset="utf-8",
             renderer_class=output.csv_renderer,
@@ -459,14 +470,20 @@
 class GetPropertyValue(BaseWFSGetDataMethod):
     """This returns a limited set of properties of the feature.
     It works almost identical to GetFeature, except that it returns a single field.
     """
 
     output_formats = [
         OutputFormat(
+            "application/gml+xml",
+            version="3.2",
+            renderer_class=output.gml32_value_renderer,
+            title="GML",
+        ),
+        OutputFormat(
             "text/xml", subtype="gml/3.2", renderer_class=output.gml32_value_renderer
         ),
     ]
 
     parameters = BaseWFSGetDataMethod.parameters + [
         Parameter("valueReference", required=True, parser=fes20.ValueReference)
     ]
```

### Comparing `django-gisserver-1.2.6/gisserver/output/__init__.py` & `django-gisserver-1.2.7/gisserver/output/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/base.py` & `django-gisserver-1.2.7/gisserver/output/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/buffer.py` & `django-gisserver-1.2.7/gisserver/output/buffer.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/csv.py` & `django-gisserver-1.2.7/gisserver/output/csv.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/geojson.py` & `django-gisserver-1.2.7/gisserver/output/geojson.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/gml32.py` & `django-gisserver-1.2.7/gisserver/output/gml32.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/results.py` & `django-gisserver-1.2.7/gisserver/output/results.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/utils.py` & `django-gisserver-1.2.7/gisserver/output/utils.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/output/xmlschema.py` & `django-gisserver-1.2.7/gisserver/output/xmlschema.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/base.py` & `django-gisserver-1.2.7/gisserver/parsers/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/__init__.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/expressions.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/expressions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/filters.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/filters.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/functions.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/functions.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/identifiers.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/identifiers.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/operators.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/operators.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/query.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/query.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/fes20/sorting.py` & `django-gisserver-1.2.7/gisserver/parsers/fes20/sorting.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/gml/__init__.py` & `django-gisserver-1.2.7/gisserver/parsers/gml/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/gml/base.py` & `django-gisserver-1.2.7/gisserver/parsers/gml/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/gml/geometries.py` & `django-gisserver-1.2.7/gisserver/parsers/gml/geometries.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/tags.py` & `django-gisserver-1.2.7/gisserver/parsers/tags.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/parsers/values.py` & `django-gisserver-1.2.7/gisserver/parsers/values.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/queries/__init__.py` & `django-gisserver-1.2.7/gisserver/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/queries/adhoc.py` & `django-gisserver-1.2.7/gisserver/queries/adhoc.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/queries/base.py` & `django-gisserver-1.2.7/gisserver/queries/base.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/queries/stored.py` & `django-gisserver-1.2.7/gisserver/queries/stored.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/index.html` & `django-gisserver-1.2.7/gisserver/templates/gisserver/index.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/service_description.html` & `django-gisserver-1.2.7/gisserver/templates/gisserver/service_description.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml` & `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/describe_stored_queries.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml` & `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/get_capabilities.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml` & `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/2.0.0/list_stored_queries.xml`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_field.html` & `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_field.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/templates/gisserver/wfs/feature_type.html` & `django-gisserver-1.2.7/gisserver/templates/gisserver/wfs/feature_type.html`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/types.py` & `django-gisserver-1.2.7/gisserver/types.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/gisserver/views.py` & `django-gisserver-1.2.7/gisserver/views.py`

 * *Files identical despite different names*

### Comparing `django-gisserver-1.2.6/setup.py` & `django-gisserver-1.2.7/setup.py`

 * *Files identical despite different names*

