# Comparing `tmp/Avlos-0.5.4.tar.gz` & `tmp/Avlos-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Avlos-0.5.4.tar", last modified: Tue Apr 18 14:55:49 2023, max compression
+gzip compressed data, was "Avlos-0.5.5.tar", last modified: Thu Jun  8 19:26:09 2023, max compression
```

## Comparing `Avlos-0.5.4.tar` & `Avlos-0.5.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.270426 Avlos-0.5.4/
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.257436 Avlos-0.5.4/Avlos.egg-info/
--rw-r--r--   0 yanconst   (501) staff       (20)      245 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     1857 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/SOURCES.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/dependency_links.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       44 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/entry_points.txt
--rw-r--r--   0 yanconst   (501) staff       (20)       47 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/requires.txt
--rw-r--r--   0 yanconst   (501) staff       (20)        6 2023-04-18 14:55:49.000000 Avlos-0.5.4/Avlos.egg-info/top_level.txt
--rw-r--r--   0 yanconst   (501) staff       (20)     5224 2022-06-25 18:06:56.000000 Avlos-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 yanconst   (501) staff       (20)     1067 2022-06-25 18:06:56.000000 Avlos-0.5.4/LICENSE
--rw-r--r--   0 yanconst   (501) staff       (20)      247 2022-11-12 18:59:54.000000 Avlos-0.5.4/MANIFEST.in
--rw-r--r--   0 yanconst   (501) staff       (20)      245 2023-04-18 14:55:49.270274 Avlos-0.5.4/PKG-INFO
--rw-r--r--   0 yanconst   (501) staff       (20)     5674 2023-03-30 21:32:01.000000 Avlos-0.5.4/README.md
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.259503 Avlos-0.5.4/avlos/
--rw-r--r--   0 yanconst   (501) staff       (20)       41 2022-09-09 17:01:49.000000 Avlos-0.5.4/avlos/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)      656 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/bitmask_field.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1920 2022-10-02 15:27:43.000000 Avlos-0.5.4/avlos/channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1490 2022-09-09 17:01:49.000000 Avlos-0.5.4/avlos/cli.py
--rw-r--r--   0 yanconst   (501) staff       (20)      699 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/counter.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2656 2023-01-05 20:43:17.000000 Avlos-0.5.4/avlos/datatypes.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.260681 Avlos-0.5.4/avlos/definitions/
--rw-r--r--   0 yanconst   (501) staff       (20)      417 2022-12-03 10:33:47.000000 Avlos-0.5.4/avlos/definitions/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1842 2023-01-01 23:15:33.000000 Avlos-0.5.4/avlos/definitions/remote_attribute.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1955 2022-12-25 09:07:18.000000 Avlos-0.5.4/avlos/definitions/remote_bitmask.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1891 2023-01-13 21:25:11.000000 Avlos-0.5.4/avlos/definitions/remote_enum.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2493 2023-01-01 21:13:12.000000 Avlos-0.5.4/avlos/definitions/remote_function.py
--rw-r--r--   0 yanconst   (501) staff       (20)     5450 2022-12-25 09:07:04.000000 Avlos-0.5.4/avlos/definitions/remote_node.py
--rw-r--r--   0 yanconst   (501) staff       (20)      821 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/definitions/remote_root_node.py
--rw-r--r--   0 yanconst   (501) staff       (20)      679 2022-06-11 09:57:19.000000 Avlos-0.5.4/avlos/deserializer.py
--rw-r--r--   0 yanconst   (501) staff       (20)      649 2023-01-13 21:06:58.000000 Avlos-0.5.4/avlos/enum_field.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.261618 Avlos-0.5.4/avlos/generators/
--rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-05-24 22:21:47.000000 Avlos-0.5.4/avlos/generators/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1730 2023-01-13 21:33:59.000000 Avlos-0.5.4/avlos/generators/filters.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1345 2023-01-13 21:34:39.000000 Avlos-0.5.4/avlos/generators/generator_c.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3945 2023-03-19 14:59:37.000000 Avlos-0.5.4/avlos/generators/generator_cpp.py
--rw-r--r--   0 yanconst   (501) staff       (20)      593 2022-06-14 22:21:34.000000 Avlos-0.5.4/avlos/generators/generator_dbc.py
--rw-r--r--   0 yanconst   (501) staff       (20)      591 2022-06-14 22:21:34.000000 Avlos-0.5.4/avlos/generators/generator_rst.py
--rw-r--r--   0 yanconst   (501) staff       (20)      327 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/json_codec.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.262635 Avlos-0.5.4/avlos/mixins/
--rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-05-24 22:21:47.000000 Avlos-0.5.4/avlos/mixins/__init__.py
--rw-r--r--   0 yanconst   (501) staff       (20)      514 2023-01-01 00:32:03.000000 Avlos-0.5.4/avlos/mixins/comm_node.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1057 2023-01-02 13:54:26.000000 Avlos-0.5.4/avlos/mixins/impex_node.py
--rw-r--r--   0 yanconst   (501) staff       (20)      151 2022-12-03 10:33:47.000000 Avlos-0.5.4/avlos/mixins/meta_node.py
--rw-r--r--   0 yanconst   (501) staff       (20)      618 2022-10-02 15:27:43.000000 Avlos-0.5.4/avlos/mixins/named_node.py
--rw-r--r--   0 yanconst   (501) staff       (20)     1757 2022-09-09 17:01:49.000000 Avlos-0.5.4/avlos/processor.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.266466 Avlos-0.5.4/avlos/templates/
--rw-r--r--   0 yanconst   (501) staff       (20)     2580 2023-01-13 20:26:34.000000 Avlos-0.5.4/avlos/templates/device.cpp.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     1147 2022-12-15 21:27:06.000000 Avlos-0.5.4/avlos/templates/device.dbc.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     2979 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/templates/device.hpp.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     1133 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/templates/docs.rst.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     3114 2023-01-05 20:43:17.000000 Avlos-0.5.4/avlos/templates/fw_endpoints.c.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     1657 2023-01-13 21:37:06.000000 Avlos-0.5.4/avlos/templates/fw_endpoints.h.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     7421 2023-04-18 14:43:38.000000 Avlos-0.5.4/avlos/templates/helpers.hpp.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     3024 2023-03-19 14:59:37.000000 Avlos-0.5.4/avlos/templates/remote_object.cpp.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)     2115 2023-03-30 21:32:01.000000 Avlos-0.5.4/avlos/templates/remote_object.hpp.jinja
--rw-r--r--   0 yanconst   (501) staff       (20)      844 2022-06-25 18:06:56.000000 Avlos-0.5.4/avlos/unit_field.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.267198 Avlos-0.5.4/example/
--rw-r--r--   0 yanconst   (501) staff       (20)      145 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/README.md
--rw-r--r--   0 yanconst   (501) staff       (20)      328 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/avlos_config.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)      536 2022-09-09 17:01:49.000000 Avlos-0.5.4/example/device.yaml
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.267353 Avlos-0.5.4/example/docs/
--rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/docs/index.rst
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.267462 Avlos-0.5.4/example/fw/
--rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-25 18:06:56.000000 Avlos-0.5.4/example/fw/main.c
--rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-04-18 14:55:49.270468 Avlos-0.5.4/setup.cfg
--rw-r--r--   0 yanconst   (501) staff       (20)      725 2023-04-18 14:43:38.000000 Avlos-0.5.4/setup.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.269067 Avlos-0.5.4/tests/
--rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-11 10:04:29.000000 Avlos-0.5.4/tests/__init__.py
-drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-04-18 14:55:49.270064 Avlos-0.5.4/tests/definition/
--rw-r--r--   0 yanconst   (501) staff       (20)      692 2023-01-13 20:26:34.000000 Avlos-0.5.4/tests/definition/avlos_config.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)      396 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_bitmask.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     2042 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_missing_version.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)      162 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_name.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)      290 2022-09-09 17:01:49.000000 Avlos-0.5.4/tests/definition/bad_device_unit.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)     2570 2023-01-13 20:57:07.000000 Avlos-0.5.4/tests/definition/good_device.yaml
--rw-r--r--   0 yanconst   (501) staff       (20)      709 2022-12-13 21:19:54.000000 Avlos-0.5.4/tests/dummy_channel.py
--rw-r--r--   0 yanconst   (501) staff       (20)      926 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_counter.py
--rw-r--r--   0 yanconst   (501) staff       (20)     2899 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_deserialization.py
--rw-r--r--   0 yanconst   (501) staff       (20)      589 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_functions.py
--rw-r--r--   0 yanconst   (501) staff       (20)     4138 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_generation.py
--rw-r--r--   0 yanconst   (501) staff       (20)      977 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_impex.py
--rw-r--r--   0 yanconst   (501) staff       (20)     3611 2023-03-30 21:32:01.000000 Avlos-0.5.4/tests/test_remote_objects.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.167142 Avlos-0.5.5/
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.158204 Avlos-0.5.5/Avlos.egg-info/
+-rw-r--r--   0 yanconst   (501) staff       (20)      245 2023-06-08 19:26:09.000000 Avlos-0.5.5/Avlos.egg-info/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     1857 2023-06-08 19:26:09.000000 Avlos-0.5.5/Avlos.egg-info/SOURCES.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        1 2023-06-08 19:26:09.000000 Avlos-0.5.5/Avlos.egg-info/dependency_links.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       44 2023-06-08 19:26:09.000000 Avlos-0.5.5/Avlos.egg-info/entry_points.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)       47 2023-06-08 19:26:09.000000 Avlos-0.5.5/Avlos.egg-info/requires.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)        6 2023-06-08 19:26:09.000000 Avlos-0.5.5/Avlos.egg-info/top_level.txt
+-rw-r--r--   0 yanconst   (501) staff       (20)     5224 2022-06-25 18:06:56.000000 Avlos-0.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 yanconst   (501) staff       (20)     1067 2022-06-25 18:06:56.000000 Avlos-0.5.5/LICENSE
+-rw-r--r--   0 yanconst   (501) staff       (20)      247 2022-11-12 18:59:54.000000 Avlos-0.5.5/MANIFEST.in
+-rw-r--r--   0 yanconst   (501) staff       (20)      245 2023-06-08 19:26:09.166977 Avlos-0.5.5/PKG-INFO
+-rw-r--r--   0 yanconst   (501) staff       (20)     5674 2023-03-30 21:32:01.000000 Avlos-0.5.5/README.md
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.160048 Avlos-0.5.5/avlos/
+-rw-r--r--   0 yanconst   (501) staff       (20)       41 2022-09-09 17:01:49.000000 Avlos-0.5.5/avlos/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      656 2023-03-30 21:32:01.000000 Avlos-0.5.5/avlos/bitmask_field.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1920 2022-10-02 15:27:43.000000 Avlos-0.5.5/avlos/channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1490 2022-09-09 17:01:49.000000 Avlos-0.5.5/avlos/cli.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      699 2023-03-30 21:32:01.000000 Avlos-0.5.5/avlos/counter.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2656 2023-01-05 20:43:17.000000 Avlos-0.5.5/avlos/datatypes.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.161183 Avlos-0.5.5/avlos/definitions/
+-rw-r--r--   0 yanconst   (501) staff       (20)      417 2022-12-03 10:33:47.000000 Avlos-0.5.5/avlos/definitions/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1842 2023-01-01 23:15:33.000000 Avlos-0.5.5/avlos/definitions/remote_attribute.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1955 2022-12-25 09:07:18.000000 Avlos-0.5.5/avlos/definitions/remote_bitmask.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1891 2023-01-13 21:25:11.000000 Avlos-0.5.5/avlos/definitions/remote_enum.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2493 2023-01-01 21:13:12.000000 Avlos-0.5.5/avlos/definitions/remote_function.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     5450 2022-12-25 09:07:04.000000 Avlos-0.5.5/avlos/definitions/remote_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      821 2023-03-30 21:32:01.000000 Avlos-0.5.5/avlos/definitions/remote_root_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      679 2022-06-11 09:57:19.000000 Avlos-0.5.5/avlos/deserializer.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      649 2023-01-13 21:06:58.000000 Avlos-0.5.5/avlos/enum_field.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.162069 Avlos-0.5.5/avlos/generators/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-05-24 22:21:47.000000 Avlos-0.5.5/avlos/generators/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1730 2023-01-13 21:33:59.000000 Avlos-0.5.5/avlos/generators/filters.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1345 2023-01-13 21:34:39.000000 Avlos-0.5.5/avlos/generators/generator_c.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3945 2023-03-19 14:59:37.000000 Avlos-0.5.5/avlos/generators/generator_cpp.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      593 2022-06-14 22:21:34.000000 Avlos-0.5.5/avlos/generators/generator_dbc.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      591 2022-06-14 22:21:34.000000 Avlos-0.5.5/avlos/generators/generator_rst.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      327 2023-03-30 21:32:01.000000 Avlos-0.5.5/avlos/json_codec.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.162760 Avlos-0.5.5/avlos/mixins/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-05-24 22:21:47.000000 Avlos-0.5.5/avlos/mixins/__init__.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      514 2023-01-01 00:32:03.000000 Avlos-0.5.5/avlos/mixins/comm_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1057 2023-01-02 13:54:26.000000 Avlos-0.5.5/avlos/mixins/impex_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      151 2022-12-03 10:33:47.000000 Avlos-0.5.5/avlos/mixins/meta_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      618 2022-10-02 15:27:43.000000 Avlos-0.5.5/avlos/mixins/named_node.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     1757 2022-09-09 17:01:49.000000 Avlos-0.5.5/avlos/processor.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.164083 Avlos-0.5.5/avlos/templates/
+-rw-r--r--   0 yanconst   (501) staff       (20)     2594 2023-06-08 19:00:25.000000 Avlos-0.5.5/avlos/templates/device.cpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     1147 2022-12-15 21:27:06.000000 Avlos-0.5.5/avlos/templates/device.dbc.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     3039 2023-06-08 19:02:24.000000 Avlos-0.5.5/avlos/templates/device.hpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     1133 2023-03-30 21:32:01.000000 Avlos-0.5.5/avlos/templates/docs.rst.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     3114 2023-01-05 20:43:17.000000 Avlos-0.5.5/avlos/templates/fw_endpoints.c.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     1657 2023-01-13 21:37:06.000000 Avlos-0.5.5/avlos/templates/fw_endpoints.h.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     7477 2023-06-08 19:02:49.000000 Avlos-0.5.5/avlos/templates/helpers.hpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     3045 2023-06-08 19:02:58.000000 Avlos-0.5.5/avlos/templates/remote_object.cpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)     2175 2023-06-08 19:02:12.000000 Avlos-0.5.5/avlos/templates/remote_object.hpp.jinja
+-rw-r--r--   0 yanconst   (501) staff       (20)      844 2022-06-25 18:06:56.000000 Avlos-0.5.5/avlos/unit_field.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.164550 Avlos-0.5.5/example/
+-rw-r--r--   0 yanconst   (501) staff       (20)      145 2022-06-25 18:06:56.000000 Avlos-0.5.5/example/README.md
+-rw-r--r--   0 yanconst   (501) staff       (20)      328 2022-06-25 18:06:56.000000 Avlos-0.5.5/example/avlos_config.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      536 2022-09-09 17:01:49.000000 Avlos-0.5.5/example/device.yaml
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.164725 Avlos-0.5.5/example/docs/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-25 18:06:56.000000 Avlos-0.5.5/example/docs/index.rst
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.164841 Avlos-0.5.5/example/fw/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-25 18:06:56.000000 Avlos-0.5.5/example/fw/main.c
+-rw-r--r--   0 yanconst   (501) staff       (20)       38 2023-06-08 19:26:09.167186 Avlos-0.5.5/setup.cfg
+-rw-r--r--   0 yanconst   (501) staff       (20)      725 2023-06-08 19:24:30.000000 Avlos-0.5.5/setup.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.165957 Avlos-0.5.5/tests/
+-rw-r--r--   0 yanconst   (501) staff       (20)        0 2022-06-11 10:04:29.000000 Avlos-0.5.5/tests/__init__.py
+drwxr-xr-x   0 yanconst   (501) staff       (20)        0 2023-06-08 19:26:09.166791 Avlos-0.5.5/tests/definition/
+-rw-r--r--   0 yanconst   (501) staff       (20)      692 2023-01-13 20:26:34.000000 Avlos-0.5.5/tests/definition/avlos_config.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      396 2022-09-09 17:01:49.000000 Avlos-0.5.5/tests/definition/bad_device_bitmask.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     2042 2022-09-09 17:01:49.000000 Avlos-0.5.5/tests/definition/bad_device_missing_version.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      162 2022-09-09 17:01:49.000000 Avlos-0.5.5/tests/definition/bad_device_name.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      290 2022-09-09 17:01:49.000000 Avlos-0.5.5/tests/definition/bad_device_unit.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)     2570 2023-01-13 20:57:07.000000 Avlos-0.5.5/tests/definition/good_device.yaml
+-rw-r--r--   0 yanconst   (501) staff       (20)      709 2022-12-13 21:19:54.000000 Avlos-0.5.5/tests/dummy_channel.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      926 2023-03-30 21:32:01.000000 Avlos-0.5.5/tests/test_counter.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     2899 2023-03-30 21:32:01.000000 Avlos-0.5.5/tests/test_deserialization.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      589 2023-03-30 21:32:01.000000 Avlos-0.5.5/tests/test_functions.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     4138 2023-03-30 21:32:01.000000 Avlos-0.5.5/tests/test_generation.py
+-rw-r--r--   0 yanconst   (501) staff       (20)      977 2023-03-30 21:32:01.000000 Avlos-0.5.5/tests/test_impex.py
+-rw-r--r--   0 yanconst   (501) staff       (20)     3611 2023-03-30 21:32:01.000000 Avlos-0.5.5/tests/test_remote_objects.py
```

### Comparing `Avlos-0.5.4/Avlos.egg-info/SOURCES.txt` & `Avlos-0.5.5/Avlos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/CODE_OF_CONDUCT.md` & `Avlos-0.5.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/LICENSE` & `Avlos-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/README.md` & `Avlos-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/bitmask_field.py` & `Avlos-0.5.5/avlos/bitmask_field.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/channel.py` & `Avlos-0.5.5/avlos/channel.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/cli.py` & `Avlos-0.5.5/avlos/cli.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/counter.py` & `Avlos-0.5.5/avlos/counter.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/datatypes.py` & `Avlos-0.5.5/avlos/datatypes.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/definitions/remote_attribute.py` & `Avlos-0.5.5/avlos/definitions/remote_attribute.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/definitions/remote_bitmask.py` & `Avlos-0.5.5/avlos/definitions/remote_bitmask.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/definitions/remote_enum.py` & `Avlos-0.5.5/avlos/definitions/remote_enum.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/definitions/remote_function.py` & `Avlos-0.5.5/avlos/definitions/remote_function.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/definitions/remote_node.py` & `Avlos-0.5.5/avlos/definitions/remote_node.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/definitions/remote_root_node.py` & `Avlos-0.5.5/avlos/definitions/remote_root_node.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/deserializer.py` & `Avlos-0.5.5/avlos/deserializer.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/enum_field.py` & `Avlos-0.5.5/avlos/enum_field.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/generators/filters.py` & `Avlos-0.5.5/avlos/generators/filters.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/generators/generator_c.py` & `Avlos-0.5.5/avlos/generators/generator_c.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/generators/generator_cpp.py` & `Avlos-0.5.5/avlos/generators/generator_cpp.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/generators/generator_dbc.py` & `Avlos-0.5.5/avlos/generators/generator_dbc.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/generators/generator_rst.py` & `Avlos-0.5.5/avlos/generators/generator_rst.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/mixins/comm_node.py` & `Avlos-0.5.5/avlos/mixins/comm_node.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/mixins/impex_node.py` & `Avlos-0.5.5/avlos/mixins/impex_node.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/mixins/named_node.py` & `Avlos-0.5.5/avlos/mixins/named_node.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/processor.py` & `Avlos-0.5.5/avlos/processor.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/templates/device.cpp.jinja` & `Avlos-0.5.5/avlos/templates/device.cpp.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 */
 
 {%- macro getter_byval(attr) -%}
 {{attr.dtype.c_name}} {{ device_name | capitalize_first }}::get_{{attr.name}}(void)
 {
     {{attr.dtype.c_name}} value = 0;
     this->send({{attr.ep_id}}, this->_data, 0, true);
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), this->delay_us_value)) 
     {
         read_le(&value, this->_data);
     }
     return value;
 }
 {%- endmacro %}
 
 {%- macro getter_char(attr) -%}
 void {{ device_name | capitalize_first }}::get_{{attr.name}}(char out_value[])
 {
     this->send({{attr.ep_id}}, this->_data, 0, true);
     this->_dlc = 0;
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), this->delay_us_value)) 
     {
         memcpy(out_value, this->_data, this->_dlc);
     }
 }
 {%- endmacro %}
 
 {%- macro setter_byval(attr) -%}
```

### Comparing `Avlos-0.5.4/avlos/templates/device.dbc.jinja` & `Avlos-0.5.5/avlos/templates/device.dbc.jinja`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/templates/device.hpp.jinja` & `Avlos-0.5.5/avlos/templates/device.hpp.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 };
 {%- endfor %}
 
 class {{ device_name | capitalize_first }} : Node
 {
     public:
 
-        {{ device_name | capitalize_first }}(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb):
-            Node(_can_node_id, _send_cb, _recv_cb, _delay_us_cb) 
+        {{ device_name | capitalize_first }}(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb, uint32_t _delay_us_value):
+            Node(_can_node_id, _send_cb, _recv_cb, _delay_us_cb, _delay_us_value) 
 {%- if instance.remote_attributes %}
     {%- for attr in instance.remote_attributes.values() %}
         {%- if attr.remote_attributes %}
-            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb, _delay_us_cb)
+            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb, _delay_us_cb, _delay_us_value)
         {%- endif %}
     {%- endfor %}
 {%- endif %} {};
 
     {%- if instance.remote_attributes %}
         {%- for attr in instance.remote_attributes.values() %}
             {%- if attr.remote_attributes %}
```

### Comparing `Avlos-0.5.4/avlos/templates/docs.rst.jinja` & `Avlos-0.5.5/avlos/templates/docs.rst.jinja`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/templates/fw_endpoints.c.jinja` & `Avlos-0.5.5/avlos/templates/fw_endpoints.c.jinja`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/templates/fw_endpoints.h.jinja` & `Avlos-0.5.5/avlos/templates/fw_endpoints.h.jinja`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/avlos/templates/helpers.hpp.jinja` & `Avlos-0.5.5/avlos/templates/helpers.hpp.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,30 @@
 #define CAN_EP_SIZE (12)
 #define CAN_EP_MASK ((1 << CAN_EP_SIZE) - 1)
 #define CAN_SEQ_SIZE (9)
 #define CAN_SEQ_MASK (((1 << CAN_SEQ_SIZE) - 1) << CAN_EP_SIZE)
 #define CAN_DEV_SIZE (8)
 #define CAN_DEV_MASK (((1 << CAN_DEV_SIZE) - 1) << (CAN_EP_SIZE + CAN_SEQ_SIZE))
 
-#define RECV_DELAY_US (160.0f)
-
 typedef void (*send_callback)(uint32_t arbitration_id, uint8_t *data, uint8_t dlc, bool rtr);
 typedef bool (*recv_callback)(uint32_t *arbitration_id, uint8_t *data, uint8_t *dlc);
 typedef void (*delay_us_callback)(uint32_t us);
 
 class Node {
     public:
 
-    Node(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb):
-        can_node_id(_can_node_id), send_cb(_send_cb), recv_cb(_recv_cb), delay_us_cb(_delay_us_cb) {}
+    Node(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb, uint32_t _delay_us_value):
+        can_node_id(_can_node_id), send_cb(_send_cb), recv_cb(_recv_cb), delay_us_cb(_delay_us_cb), delay_us_value(_delay_us_value) {}
 
     protected:
     uint8_t can_node_id;
     send_callback send_cb;
     recv_callback recv_cb;
     delay_us_callback delay_us_cb;
+    uint32_t delay_us_value;
     uint8_t _data[8];
     uint8_t _dlc;
     uint32_t get_arbitration_id(uint32_t cmd_id)
     {
         return ((this->can_node_id << (CAN_EP_SIZE + CAN_SEQ_SIZE)) & CAN_DEV_MASK) | (cmd_id & CAN_EP_MASK);
     }
     void send(uint8_t cmd_id, uint8_t *data, uint8_t data_size, bool rtr)
```

### Comparing `Avlos-0.5.4/avlos/templates/remote_object.cpp.jinja` & `Avlos-0.5.5/avlos/templates/remote_object.cpp.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 */
 
 {%- macro getter_byval(attr) -%}
 {{attr.dtype.c_name}} {{ instance.name | capitalize_first }}_::get_{{attr.name}}(void)
 {
     {{attr.dtype.c_name}} value = 0;
     this->send({{attr.ep_id}}, this->_data, 0, true);
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), this->delay_us_value)) 
     {
         read_le(&value, this->_data);
     }
     return value;
 }
 {%- endmacro %}
 
 {%- macro getter_char(attr) -%}
 void {{ instance.name | capitalize_first }}_::get_{{attr.name}}(char out_value[])
 {
     this->send({{attr.ep_id}}, this->_data, 0, true);
     this->_dlc = 0;
-    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    if (this->recv({{attr.ep_id}}, this->_data, &(this->_dlc), this->delay_us_value)) 
     {
         memcpy(out_value, this->_data, this->_dlc);
     }
 }
 {%- endmacro %}
 
 {%- macro setter_byval(attr) -%}
@@ -86,15 +86,15 @@
 
     this->send({{attr.ep_id}}, this->_data, data_len, false);
     {%- endif %}
 
     {%- if attr.dtype.c_name != "void" %}
     {{attr.dtype.c_name}} value = 0;
     this->send(17, this->_data, 0, true);
-    if (this->recv(17, this->_data, &(this->_dlc), RECV_DELAY_US)) 
+    if (this->recv(17, this->_data, &(this->_dlc), this->delay_us_value)) 
     {
         read_le(&value, this->_data);
     }
     return value;
     {%- endif %}
 }
             {%- endif %}
```

### Comparing `Avlos-0.5.4/avlos/templates/remote_object.hpp.jinja` & `Avlos-0.5.5/avlos/templates/remote_object.hpp.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     {%- endfor %}
 {%- endif %}
 
 class {{ instance.name | capitalize_first }}_ : Node
 {
     public:
 
-        {{ instance.name | capitalize_first }}_(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb):
-            Node(_can_node_id, _send_cb, _recv_cb, _delay_us_cb) 
+        {{ instance.name | capitalize_first }}_(uint8_t _can_node_id, send_callback _send_cb, recv_callback _recv_cb, delay_us_callback _delay_us_cb, uint32_t _delay_us_value):
+            Node(_can_node_id, _send_cb, _recv_cb, _delay_us_cb, _delay_us_value) 
 {%- if instance.remote_attributes %}
     {%- for attr in instance.remote_attributes.values() %}
         {%- if attr.remote_attributes %}
-            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb, _delay_us_cb)
+            , {{attr.name}}(_can_node_id, _send_cb, _recv_cb, _delay_us_cb, _delay_us_value)
         {%- endif %}
     {%- endfor %}
 {%- endif %} {};
 
     {%- if instance.remote_attributes %}
         {%- for attr in instance.remote_attributes.values() %}
             {%- if attr.remote_attributes %}
```

### Comparing `Avlos-0.5.4/avlos/unit_field.py` & `Avlos-0.5.5/avlos/unit_field.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/example/device.yaml` & `Avlos-0.5.5/example/device.yaml`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/setup.py` & `Avlos-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="Avlos",
-    version="0.5.4",
+    version="0.5.5",
     description="Avlos Remote Object Templating System",
     author="Yannis Chatzikonstantinou",
     author_email="yannis@tinymovr.com",
     url="https://www.tinymovr.com",
     packages=find_packages(include=["avlos", "avlos.*"]),
     include_package_data=True,
     python_requires=">=3.9",
```

### Comparing `Avlos-0.5.4/tests/definition/avlos_config.yaml` & `Avlos-0.5.5/tests/definition/avlos_config.yaml`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/definition/bad_device_missing_version.yaml` & `Avlos-0.5.5/tests/definition/bad_device_missing_version.yaml`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/definition/good_device.yaml` & `Avlos-0.5.5/tests/definition/good_device.yaml`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/dummy_channel.py` & `Avlos-0.5.5/tests/dummy_channel.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/test_counter.py` & `Avlos-0.5.5/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/test_deserialization.py` & `Avlos-0.5.5/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/test_functions.py` & `Avlos-0.5.5/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/test_generation.py` & `Avlos-0.5.5/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/test_impex.py` & `Avlos-0.5.5/tests/test_impex.py`

 * *Files identical despite different names*

### Comparing `Avlos-0.5.4/tests/test_remote_objects.py` & `Avlos-0.5.5/tests/test_remote_objects.py`

 * *Files identical despite different names*

