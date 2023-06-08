# Comparing `tmp/galaxy-util-22.5.0.dev3.tar.gz` & `tmp/galaxy-util-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-util-22.5.0.dev3.tar", last modified: Mon Mar  6 18:35:32 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/util/dist/.tmp-74k4aili/galaxy-util-23.0.1.tar", last modified: Thu Jun  8 17:37:41 2023, max compression
```

## Comparing `galaxy-util-22.5.0.dev3.tar` & `galaxy-util-23.0.1.tar`

### file list

```diff
@@ -1,88 +1,96 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.521865 galaxy-util-22.5.0.dev3/
--rw-r--r--   0 mvandenb   (501) staff       (20)      923 2023-02-17 09:03:53.000000 galaxy-util-22.5.0.dev3/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)      152 2023-03-06 18:30:39.000000 galaxy-util-22.5.0.dev3/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2302 2023-03-06 18:35:32.522003 galaxy-util-22.5.0.dev3/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      293 2023-03-06 18:30:39.000000 galaxy-util-22.5.0.dev3/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.493897 galaxy-util-22.5.0.dev3/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.495349 galaxy-util-22.5.0.dev3/galaxy/exceptions/
--rw-r--r--   0 mvandenb   (501) staff       (20)     7702 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/exceptions/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5294 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/exceptions/error_codes.json
--rw-r--r--   0 mvandenb   (501) staff       (20)     1910 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/exceptions/error_codes.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.516185 galaxy-util-22.5.0.dev3/galaxy/util/
--rw-r--r--   0 mvandenb   (501) staff       (20)    59489 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      872 2022-11-16 11:10:40.000000 galaxy-util-22.5.0.dev3/galaxy/util/aliaspickler.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5715 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/bool_expressions.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1086 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/bunch.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1881 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/bytesize.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5938 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/checkers.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6129 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/commands.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    12891 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/compression_utils.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.516963 galaxy-util-22.5.0.dev3/galaxy/util/custom_logging/
--rw-r--r--   0 mvandenb   (501) staff       (20)      413 2022-11-16 11:10:40.000000 galaxy-util-22.5.0.dev3/galaxy/util/custom_logging/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1377 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/custom_logging/fluent_log.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7819 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/dbkeys.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2316 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/dictifiable.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        9 2022-02-02 10:06:09.000000 galaxy-util-22.5.0.dev3/galaxy/util/docutils_template.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      225 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/dynamic.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1542 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/expressions.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1935 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/facts.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2606 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/filelock.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5616 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/form_builder.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2006 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/hash_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8119 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/heartbeat.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      873 2022-11-16 11:10:40.000000 galaxy-util-22.5.0.dev3/galaxy/util/image_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4961 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/inflection.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7172 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/json.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5780 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/jstree.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1628 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/lazy_process.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1525 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/monitors.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2549 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/odict.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1708 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/oset.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.518119 galaxy-util-22.5.0.dev3/galaxy/util/path/
--rw-r--r--   0 mvandenb   (501) staff       (20)    15788 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/path/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      204 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/path/ntpath.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      208 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/path/posixpath.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3761 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/permutations.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4756 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/plugin_config.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7384 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/properties.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1503 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/renamed_temporary_file.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      632 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/resources.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    18155 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/rules_dsl.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    11738 2022-11-16 11:10:40.000000 galaxy-util-22.5.0.dev3/galaxy/util/rules_dsl_spec.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     3710 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/sanitize_html.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3654 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/script.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3499 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/search.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4616 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/simplegraph.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      619 2022-11-16 11:10:40.000000 galaxy-util-22.5.0.dev3/galaxy/util/sleeper.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1671 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/sockets.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      557 2022-02-02 10:06:09.000000 galaxy-util-22.5.0.dev3/galaxy/util/specs.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      745 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/sqlite.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1735 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/submodules.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1362 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/task.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5669 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/template.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.519688 galaxy-util-22.5.0.dev3/galaxy/util/tool_shed/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-util-22.5.0.dev3/galaxy/util/tool_shed/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    20331 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/tool_shed/common_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      930 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/tool_shed/encoding_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3430 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/tool_shed/xml_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      216 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/tool_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6755 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/topsort.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1001 2022-11-16 11:10:40.000000 galaxy-util-22.5.0.dev3/galaxy/util/ucsc.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1115 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/validation.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6668 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/galaxy/util/watcher.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    11803 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/xml_macros.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2824 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/yaml_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3020 2023-03-06 18:30:38.000000 galaxy-util-22.5.0.dev3/galaxy/util/zipstream.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      117 2023-03-06 18:34:50.000000 galaxy-util-22.5.0.dev3/galaxy/version.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2023-03-06 18:35:32.521527 galaxy-util-22.5.0.dev3/galaxy_util.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     2302 2023-03-06 18:35:32.000000 galaxy-util-22.5.0.dev3/galaxy_util.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     2039 2023-03-06 18:35:32.000000 galaxy-util-22.5.0.dev3/galaxy_util.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2023-03-06 18:35:32.000000 galaxy-util-22.5.0.dev3/galaxy_util.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      168 2023-03-06 18:35:32.000000 galaxy-util-22.5.0.dev3/galaxy_util.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2023-03-06 18:35:32.000000 galaxy-util-22.5.0.dev3/galaxy_util.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       81 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/pyproject.toml
--rw-r--r--   0 mvandenb   (501) staff       (20)     1361 2023-03-06 18:35:32.522649 galaxy-util-22.5.0.dev3/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)       17 2022-12-08 11:44:37.000000 galaxy-util-22.5.0.dev3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-util-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/exceptions/error_codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/exceptions/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    61298 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/aliaspickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/bool_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/bytesize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/compression_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/util/custom_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/custom_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/custom_logging/fluent_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/dbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/dictifiable.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/docutils_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/drs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/form_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/hash_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/inflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/jstree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/lazy_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/odict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/oset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/util/path/
+-rw-r--r--   0 runner    (1001) docker     (123)    16902 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/path/ntpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/path/posixpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/permutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/renamed_temporary_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/rules_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/rules_dsl_spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/sanitize_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/simplegraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/util/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/tool_shed/common_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/tool_shed/encoding_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/tool_shed/tool_shed_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/tool_shed/xml_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/tool_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/topsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/ucsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy/util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/xml_macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/yaml_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/util/zipstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/galaxy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/galaxy_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-08 17:37:41.000000 galaxy-util-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 17:37:04.000000 galaxy-util-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-util-22.5.0.dev3/HISTORY.rst` & `galaxy-util-23.0.1/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 History
 -------
 
 .. to_doc
 
----------------------
-22.5.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
 
+=========
+Bug fixes
+=========
 
----------------------
+* Replace httpbin service with pytest-httpserver by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16042 <https://github.com/galaxyproject/galaxy/pull/16042>`_
+
+-------------------
 22.1.2 (2022-12-08)
----------------------
+-------------------
 
 * Pin packaging dependency to < 22, fixes ``LegacyVersion`` import errors
 * Add missing pyparsing dependency
 
----------------------
+-------------------
 22.1.1 (2022-08-22)
----------------------
+-------------------
 
 * First release from the 22.01 branch of Galaxy
 
----------------------
+-------------------
 21.1.0 (2021-03-19)
----------------------
+-------------------
 
 * First release from the 21.01 branch of Galaxy.
 
----------------------
+-------------------
 20.9.1 (2020-10-28)
----------------------
+-------------------
+
 
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-03)
----------------------
+-------------------
 
 * First release from 20.05 branch of Galaxy.
 
----------------------
+-------------------
 19.9.0 (2019-11-21)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
```

### Comparing `galaxy-util-22.5.0.dev3/LICENSE` & `galaxy-util-23.0.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-util-22.5.0.dev3/PKG-INFO` & `galaxy-util-23.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-util
-Version: 22.5.0.dev3
+Version: 23.0.1
 Summary: Galaxy generic utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: jstree
 Provides-Extra: template
@@ -33,64 +34,69 @@
 
 
 Overview
 --------
 
 The Galaxy_ utilities module.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
 History
 -------
 
 .. to_doc
 
----------------------
-22.5.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
 
+=========
+Bug fixes
+=========
 
----------------------
+* Replace httpbin service with pytest-httpserver by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16042 <https://github.com/galaxyproject/galaxy/pull/16042>`_
+
+-------------------
 22.1.2 (2022-12-08)
----------------------
+-------------------
 
 * Pin packaging dependency to < 22, fixes ``LegacyVersion`` import errors
 * Add missing pyparsing dependency
 
----------------------
+-------------------
 22.1.1 (2022-08-22)
----------------------
+-------------------
 
 * First release from the 22.01 branch of Galaxy
 
----------------------
+-------------------
 21.1.0 (2021-03-19)
----------------------
+-------------------
 
 * First release from the 21.01 branch of Galaxy.
 
----------------------
+-------------------
 20.9.1 (2020-10-28)
----------------------
+-------------------
+
 
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-03)
----------------------
+-------------------
 
 * First release from 20.05 branch of Galaxy.
 
----------------------
+-------------------
 19.9.0 (2019-11-21)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/exceptions/__init__.py` & `galaxy-util-23.0.1/galaxy/exceptions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Reflecting Galaxy's origins as a web application, these exceptions tend to be a
 bit web-oriented. However this module is a dependency of modules and tools that
 have nothing to do with the web - keep this in mind when defining exception names
 and messages.
 """
 
-from ..exceptions.error_codes import (
+from .error_codes import (
     error_codes_by_name,
     ErrorCode,
 )
 
 
 class MessageException(Exception):
     """Most generic Galaxy exception - indicates merely that some exceptional condition happened."""
@@ -55,14 +55,24 @@
 class ObjectInvalid(Exception):
     """Accessed object store ID is invalid"""
 
 
 # Please keep the exceptions ordered by status code
 
 
+class AcceptedRetryLater(MessageException):
+    status_code = 202
+    err_code = error_codes_by_name["ACCEPTED_RETRY_LATER"]
+    retry_after: int
+
+    def __init__(self, msg, retry_after=60):
+        super().__init__(msg)
+        self.retry_after = retry_after
+
+
 class NoContentException(MessageException):
     status_code = 204
     err_code = error_codes_by_name["NO_CONTENT_GENERIC"]
 
 
 class ActionInputError(MessageException):
     status_code = 400
@@ -195,29 +205,28 @@
 class ObjectNotFound(MessageException):
     """Accessed object was not found"""
 
     status_code = 404
     err_code = error_codes_by_name["USER_OBJECT_NOT_FOUND"]
 
 
+class Conflict(MessageException):
+    status_code = 409
+    err_code = error_codes_by_name["CONFLICT"]
+
+
 class DeprecatedMethod(MessageException):
     """
     Method (or a particular form/arg signature) has been removed and won't be available later
     """
 
-    status_code = 404
-    # TODO:?? 410 Gone?
+    status_code = 410
     err_code = error_codes_by_name["DEPRECATED_API_CALL"]
 
 
-class Conflict(MessageException):
-    status_code = 409
-    err_code = error_codes_by_name["CONFLICT"]
-
-
 class ConfigurationError(Exception):
     status_code = 500
     err_code = error_codes_by_name["CONFIG_ERROR"]
 
 
 class InconsistentDatabase(MessageException):
     status_code = 500
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/exceptions/error_codes.json` & `galaxy-util-23.0.1/galaxy/exceptions/error_codes.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9473684210526315%*

 * *Differences: {'28': "{'name': 'CONFLICT', 'code': 409001, 'message': 'Database conflict prevented fulfilling "*

 * *       "the request.'}",*

 * * '29': "{'name': 'DEPRECATED_API_CALL', 'code': 410001, 'message': 'This API method or call "*

 * *       "signature has been deprecated and is no longer available'}",*

 * * 'insert': "[(1, OrderedDict([('name', 'ACCEPTED_RETRY_LATER'), ('code', 202001), ('message', "*

 * *           "'Galaxy has accepted this request and is processing. A retry-after header indicates to "*

 * *           "the client when t […]*

```diff
@@ -1,14 +1,19 @@
 [
     {
         "code": 0,
         "message": "Unknown error occurred while processing request.",
         "name": "UNKNOWN"
     },
     {
+        "code": 202001,
+        "message": "Galaxy has accepted this request and is processing. A retry-after header indicates to the client when to retry.",
+        "name": "ACCEPTED_RETRY_LATER"
+    },
+    {
         "code": 204001,
         "message": "Galaxy has no content to associate with this request.",
         "name": "NO_CONTENT_GENERIC"
     },
     {
         "code": 400001,
         "message": "User does not have permissions to run jobs as another user.",
@@ -131,24 +136,24 @@
     },
     {
         "code": 404001,
         "message": "No such object found.",
         "name": "USER_OBJECT_NOT_FOUND"
     },
     {
-        "code": 404002,
-        "message": "This API method or call signature has been deprecated and is no longer available",
-        "name": "DEPRECATED_API_CALL"
-    },
-    {
         "code": 409001,
         "message": "Database conflict prevented fulfilling the request.",
         "name": "CONFLICT"
     },
     {
+        "code": 410001,
+        "message": "This API method or call signature has been deprecated and is no longer available",
+        "name": "DEPRECATED_API_CALL"
+    },
+    {
         "code": 500001,
         "message": "Internal server error.",
         "name": "INTERNAL_SERVER_ERROR"
     },
     {
         "code": 500002,
         "message": "Inconsistent database prevented fulfilling the request.",
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/exceptions/error_codes.py` & `galaxy-util-23.0.1/galaxy/exceptions/error_codes.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/__init__.py` & `galaxy-util-23.0.1/galaxy/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,27 +19,34 @@
 import stat
 import string
 import sys
 import tempfile
 import textwrap
 import threading
 import time
-import typing
 import unicodedata
 import xml.dom.minidom
-from datetime import datetime
+from datetime import (
+    datetime,
+    timezone,
+)
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from hashlib import md5
 from os.path import relpath
-from pathlib import Path
 from typing import (
     Any,
+    Iterable,
+    Iterator,
+    List,
     Optional,
     overload,
+    Tuple,
+    TypeVar,
+    Union,
 )
 from urllib.parse import (
     urlencode,
     urlparse,
     urlsplit,
     urlunsplit,
 )
@@ -58,32 +65,45 @@
 except ImportError:
     # For Pulsar on Windows (which does not use the function that uses grp)
     grp = None  # type: ignore[assignment]
 LXML_AVAILABLE = True
 try:
     from lxml import etree
     from lxml.etree import _Element as Element
+
+    # lxml.etree.ElementTree is a function that returns a new instance of the
+    # lxml.etree._ElementTree class. This class doesn't have a proper
+    # __init__() method, so we can add a __new__() constructor that mimicks
+    # xml.etree.ElementTree.ElementTree initialization.
+    class ElementTree(etree._ElementTree):
+        def __new__(cls, element=None, file=None) -> etree.ElementTree:
+            return etree.ElementTree(element, file=file)
+
 except ImportError:
     LXML_AVAILABLE = False
     import xml.etree.ElementTree as etree  # type: ignore[assignment,no-redef]
-    from xml.etree.ElementTree import Element  # noqa: F401  # type: ignore[assignment,no-redef]
+    from xml.etree.ElementTree import (  # type: ignore[assignment]
+        Element,
+        ElementTree,
+    )
 
 try:
     import docutils.core as docutils_core
     import docutils.writers.html4css1 as docutils_html4css1
 except ImportError:
     docutils_core = None  # type: ignore[assignment]
     docutils_html4css1 = None  # type: ignore[assignment]
 
 from .custom_logging import get_logger
 from .inflection import Inflector
 from .path import (  # noqa: F401
     safe_contains,
     safe_makedirs,
     safe_relpath,
+    StrPath,
 )
 
 try:
     shlex_join = shlex.join  # type: ignore[attr-defined]
 except AttributeError:
     # Python < 3.8
     def shlex_join(split_command):
@@ -247,15 +267,15 @@
     while True:
         data = fp.read(chunk_size)
         if not data:
             break
         yield data
 
 
-def chunk_iterable(it: typing.Iterable, size: int = 1000):
+def chunk_iterable(it: Iterable, size: int = 1000) -> Iterator[tuple]:
     """
     Break an iterable into chunks of ``size`` elements.
 
     >>> list(chunk_iterable([1, 2, 3, 4, 5, 6, 7], 3))
     [(1, 2, 3), (4, 5, 6), (7,)]
     """
     it = iter(it)
@@ -274,15 +294,15 @@
     >>> len(set(ids))
     1000
     """
     random_bits = str(random.getrandbits(KEY_SIZE)).encode("UTF-8")
     return md5(random_bits).hexdigest()
 
 
-def parse_xml(fname: typing.Union[str, Path], strip_whitespace=True, remove_comments=True):
+def parse_xml(fname: StrPath, strip_whitespace=True, remove_comments=True) -> ElementTree:
     """Returns a parsed xml tree"""
     parser = None
     if remove_comments and LXML_AVAILABLE:
         # If using stdlib etree comments are always removed,
         # but lxml doesn't do this by default
         parser = etree.XMLParser(remove_comments=remove_comments)
     try:
@@ -301,36 +321,36 @@
         raise
     except etree.ParseError:
         log.exception("Error parsing file %s", fname)
         raise
     return tree
 
 
-def parse_xml_string(xml_string, strip_whitespace=True):
+def parse_xml_string(xml_string: str, strip_whitespace: bool = True) -> Element:
     try:
-        tree = etree.fromstring(xml_string)
+        elem = etree.fromstring(xml_string)
     except ValueError as e:
         if "strings with encoding declaration are not supported" in unicodify(e):
-            tree = etree.fromstring(xml_string.encode("utf-8"))
+            elem = etree.fromstring(xml_string.encode("utf-8"))
         else:
             raise e
     if strip_whitespace:
-        for elem in tree.iter("*"):
-            if elem.text is not None:
-                elem.text = elem.text.strip()
-            if elem.tail is not None:
-                elem.tail = elem.tail.strip()
-    return tree
+        for sub_elem in elem.iter("*"):
+            if sub_elem.text is not None:
+                sub_elem.text = sub_elem.text.strip()
+            if sub_elem.tail is not None:
+                sub_elem.tail = sub_elem.tail.strip()
+    return elem
 
 
-def parse_xml_string_to_etree(xml_string, strip_whitespace=True):
-    return etree.ElementTree(parse_xml_string(xml_string=xml_string, strip_whitespace=strip_whitespace))
+def parse_xml_string_to_etree(xml_string: str, strip_whitespace: bool = True) -> ElementTree:
+    return ElementTree(parse_xml_string(xml_string=xml_string, strip_whitespace=strip_whitespace))
 
 
-def xml_to_string(elem, pretty=False):
+def xml_to_string(elem: Element, pretty: bool = False) -> str:
     """
     Returns a string from an xml tree.
     """
     try:
         if elem is not None:
             xml_str = etree.tostring(elem, encoding="unicode")
         else:
@@ -776,15 +796,15 @@
     slug_base = re.sub(r"[^a-zA-Z0-9\-]", "", slug_base)
     # Remove trailing '-'.
     if slug_base.endswith("-"):
         slug_base = slug_base[:-1]
     return slug_base
 
 
-def which(file):
+def which(file: str) -> Optional[str]:
     # http://stackoverflow.com/questions/5226958/which-equivalent-function-in-python
     for path in os.environ["PATH"].split(":"):
         if os.path.exists(path + "/" + file):
             return path + "/" + file
 
     return None
 
@@ -1008,15 +1028,15 @@
         elif obj in falsy:
             return False
         else:
             raise ValueError(f"String is not true/false: {obj!r}")
     return bool(obj)
 
 
-def string_as_bool(string: typing.Any) -> bool:
+def string_as_bool(string: Any) -> bool:
     if str(string).lower() in ("true", "yes", "on", "1"):
         return True
     else:
         return False
 
 
 def string_as_bool_or_none(string):
@@ -1034,15 +1054,40 @@
         return True
     elif string in ["none", "null"]:
         return None
     else:
         return False
 
 
-def listify(item, do_strip=False) -> typing.List[typing.Any]:
+ItemType = TypeVar("ItemType")
+
+
+@overload
+def listify(item: Union[None, Literal[False]], do_strip: bool = False) -> List:
+    ...
+
+
+@overload
+def listify(item: str, do_strip: bool = False) -> List[str]:
+    ...
+
+
+@overload
+def listify(item: Union[List[ItemType], Tuple[ItemType, ...]], do_strip: bool = False) -> List[ItemType]:
+    ...
+
+
+# Unfortunately we cannot use ItemType .. -> List[ItemType] in the next overload
+# because then that would also match Union types.
+@overload
+def listify(item: Any, do_strip: bool = False) -> List:
+    ...
+
+
+def listify(item: Any, do_strip: bool = False) -> List:
     """
     Make a single item a single item list.
 
     If *item* is a string, it is split on comma (``,``) characters to produce the list. Optionally, if *do_strip* is
     true, any extra whitespace around the split items is stripped.
 
     If *item* is a list it is returned unchanged. If *item* is a tuple, it is converted to a list and returned. If
@@ -1053,17 +1098,15 @@
     :type  do_strip:    bool
     :param do_strip:    strip whitespaces from around split items, if set to ``True``
     :rtype:             list
     :returns:           The input as a list
     """
     if not item:
         return []
-    elif isinstance(item, list):
-        return item
-    elif isinstance(item, tuple):
+    elif isinstance(item, (list, tuple)):
         return list(item)
     elif isinstance(item, str) and item.count(","):
         if do_strip:
             return [token.strip() for token in item.split(",")]
         else:
             return item.split(",")
     else:
@@ -1622,18 +1665,23 @@
 
 #  Don't use these two directly, prefer method version that "works" with packaged Galaxy.
 galaxy_root_path = os.path.join(__path__[0], os.pardir, os.pardir, os.pardir)  # type: ignore[name-defined]
 galaxy_samples_path = os.path.join(__path__[0], os.pardir, "config", "sample")  # type: ignore[name-defined]
 
 
 def galaxy_directory():
-    root_path = os.path.abspath(galaxy_root_path)
-    if os.path.basename(root_path) == "packages":
-        root_path = os.path.abspath(os.path.join(root_path, ".."))
-    return root_path
+    path = galaxy_root_path
+    if in_packages():
+        path = os.path.join(galaxy_root_path, "..")
+    return os.path.abspath(path)
+
+
+def in_packages():
+    # Normalize first; otherwise basename will be `..`
+    return os.path.basename(os.path.normpath(galaxy_root_path)) == "packages"
 
 
 def galaxy_samples_directory():
     return os.path.join(galaxy_directory(), "lib", "galaxy", "config", "sample")
 
 
 def config_directories_from_setting(directories_setting, galaxy_root=galaxy_root_path):
@@ -1757,14 +1805,25 @@
     False
     """
     if allow_list is None:
         allow_list = ("http://", "https://", "ftp://")
     return any(uri.startswith(scheme) for scheme in allow_list)
 
 
+def check_github_api_response_rate_limit(response):
+    if response.status_code == 403 and "API rate limit exceeded" in response.json()["message"]:
+        # It can take tens of minutes before the rate limit window resets
+        message = "GitHub API rate limit exceeded."
+        rate_limit_reset_UTC_timestamp = response.headers.get("X-RateLimit-Reset")
+        if rate_limit_reset_UTC_timestamp:
+            rate_limit_reset_datetime = datetime.fromtimestamp(int(rate_limit_reset_UTC_timestamp), tz=timezone.utc)
+            message += f" The rate limit window will reset at {rate_limit_reset_datetime.isoformat()}."
+        raise Exception(message)
+
+
 def download_to_file(url, dest_file_path, timeout=30, chunk_size=2**20):
     """Download a URL to a file in chunks."""
     with requests.get(url, timeout=timeout, stream=True) as r, open(dest_file_path, "wb") as f:
         for chunk in r.iter_content(chunk_size):
             if chunk:
                 f.write(chunk)
 
@@ -1842,13 +1901,7 @@
             message = self.template
         log_message = message + f" ({self.elapsed * 1000:0.3f} ms)"
         return log_message
 
     @property
     def elapsed(self):
         return time.time() - self.begin
-
-
-if __name__ == "__main__":
-    import doctest
-
-    doctest.testmod(sys.modules[__name__], verbose=False)
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/aliaspickler.py` & `galaxy-util-23.0.1/galaxy/util/aliaspickler.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/bool_expressions.py` & `galaxy-util-23.0.1/galaxy/util/bool_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.args = token[0][0::2]
 
     def __str__(self):
         sep = f" {self.reprsymbol} "
         return f"({sep.join(map(str, self.args))})"
 
     def __bool__(self):
-        return self.evalop(bool(a) for a in self.args)
+        return self.evalop(bool(a) for a in self.args)  # type: ignore[misc,call-arg]
 
     __nonzero__ = __bool__
 
 
 class BoolAnd(BoolBinaryOperation):
     """Represents the `AND` boolean operation."""
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/bunch.py` & `galaxy-util-23.0.1/galaxy/util/bunch.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/bytesize.py` & `galaxy-util-23.0.1/galaxy/util/bytesize.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/checkers.py` & `galaxy-util-23.0.1/galaxy/util/checkers.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/commands.py` & `galaxy-util-23.0.1/galaxy/util/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Generic I/O and shell processing code used by Galaxy tool dependencies."""
 import logging
 import os
 import shlex
 import subprocess
 import sys as _sys
 import tempfile
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Union,
+)
 
 from galaxy.util import (
     unicodify,
     which,
 )
 
 log = logging.getLogger(__name__)
@@ -44,35 +51,37 @@
         if err:
             err = unicodify(err)
             sys.stderr.write(err)
             err = None
     return out, err
 
 
-def shell(cmds, env=None, **kwds):
+def shell(cmds: Union[List[str], str], env: Optional[Dict[str, str]] = None, **kwds: Dict[str, Any]) -> int:
     """Run shell commands with `shell_process` and wait."""
     sys = kwds.get("sys", _sys)
     assert sys is not None
     p = shell_process(cmds, env, **kwds)
     if redirecting_io(sys=sys):
         redirect_aware_commmunicate(p, sys=sys)
         exit = p.returncode
         return exit
     else:
         return p.wait()
 
 
-def shell_process(cmds, env=None, **kwds):
+def shell_process(
+    cmds: Union[List[str], str], env: Optional[Dict[str, str]] = None, **kwds: Dict[str, Any]
+) -> subprocess.Popen:
     """A high-level method wrapping subprocess.Popen.
 
     Handles details such as environment extension and in process I/O
     redirection.
     """
     sys = kwds.get("sys", _sys)
-    popen_kwds = dict()
+    popen_kwds: Dict[str, Any] = dict()
     if isinstance(cmds, str):
         log.warning("Passing program arguments as a string may be a security hazard if combined with untrusted input")
         popen_kwds["shell"] = True
     if kwds.get("stdout", None) is None and redirecting_io(sys=sys):
         popen_kwds["stdout"] = subprocess.PIPE
     if kwds.get("stderr", None) is None and redirecting_io(sys=sys):
         popen_kwds["stderr"] = subprocess.PIPE
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/compression_utils.py` & `galaxy-util-23.0.1/galaxy/util/compression_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import bz2
 import gzip
 import io
 import logging
 import os
 import tarfile
+import tempfile
 import zipfile
 from typing import (
     Any,
     cast,
     Generator,
     IO,
     Iterable,
@@ -16,15 +17,18 @@
     overload,
     Tuple,
     Union,
 )
 
 from typing_extensions import Literal
 
-from galaxy.util.path import safe_relpath
+from galaxy.util.path import (
+    safe_relpath,
+    StrPath,
+)
 from .checkers import (
     is_bz2,
     is_gzip,
 )
 
 log = logging.getLogger(__name__)
 
@@ -145,26 +149,39 @@
             if line and line[0] != "#":
                 yield line.split(sep)
 
 
 ArchiveMemberType = Union[tarfile.TarInfo, zipfile.ZipInfo]
 
 
-class CompressedFile:
+def decompress_bytes_to_directory(content: bytes) -> str:
+    temp_directory = tempfile.mkdtemp()
+    with tempfile.NamedTemporaryFile(delete=False) as fp:
+        fp.write(content)
+        fp.close()
+        return CompressedFile(fp.name).extract(temp_directory)
+
 
+def decompress_path_to_directory(path: str) -> str:
+    temp_directory = tempfile.mkdtemp()
+    return CompressedFile(path).extract(temp_directory)
+
+
+class CompressedFile:
     archive: Union[tarfile.TarFile, zipfile.ZipFile]
 
     @staticmethod
-    def can_decompress(file_path: str) -> bool:
+    def can_decompress(file_path: StrPath) -> bool:
         return tarfile.is_tarfile(file_path) or zipfile.is_zipfile(file_path)
 
-    def __init__(self, file_path: str, mode: str = "r") -> None:
+    def __init__(self, file_path: StrPath, mode: str = "r") -> None:
+        file_path_str = str(file_path)
         if tarfile.is_tarfile(file_path):
             self.file_type = "tar"
-        elif zipfile.is_zipfile(file_path) and not file_path.endswith(".jar"):
+        elif zipfile.is_zipfile(file_path) and not file_path_str.endswith(".jar"):
             self.file_type = "zip"
         self.file_name = os.path.splitext(os.path.basename(file_path))[0]
         if self.file_name.endswith(".tar"):
             self.file_name = os.path.splitext(self.file_name)[0]
         self.type = self.file_type
         method = f"open_{self.file_type}"
         if hasattr(self, method):
@@ -195,15 +212,15 @@
                 and all(self.getname(item).startswith(common_prefix + os.sep) for item in contents if self.isfile(item))
             ):
                 common_prefix += os.sep
             if not common_prefix.endswith(os.sep):
                 common_prefix = ""
         return common_prefix
 
-    def extract(self, path: str) -> str:
+    def extract(self, path: StrPath) -> str:
         """Determine the path to which the archive should be extracted."""
         contents = self.getmembers()
         extraction_path = path
         common_prefix_dir = self.common_prefix_dir
         if len(contents) == 1:
             # The archive contains a single file, return the extraction path.
             if self.isfile(contents[0]):
@@ -304,22 +321,22 @@
         return False
 
     def isfile(self, member: ArchiveMemberType) -> bool:
         if not self.isdir(member):
             return True
         return False
 
-    def open_tar(self, filepath: str, mode: str) -> tarfile.TarFile:
+    def open_tar(self, filepath: StrPath, mode: str) -> tarfile.TarFile:
         return tarfile.open(filepath, mode, errorlevel=0)
 
-    def open_zip(self, filepath: str, mode: str) -> zipfile.ZipFile:
+    def open_zip(self, filepath: StrPath, mode: str) -> zipfile.ZipFile:
         mode = cast(Literal["a", "r", "w", "x"], mode)
         return zipfile.ZipFile(filepath, mode)
 
-    def zipfile_ok(self, path_to_archive: str) -> bool:
+    def zipfile_ok(self, path_to_archive: StrPath) -> bool:
         """
         This function is a bit pedantic and not functionally necessary.  It checks whether there is
         no file pointing outside of the extraction, because ZipFile.extractall() has some potential
         security holes.  See python zipfile documentation for more details.
         """
         basename = os.path.realpath(os.path.dirname(path_to_archive))
         zip_archive = zipfile.ZipFile(path_to_archive)
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/custom_logging/fluent_log.py` & `galaxy-util-23.0.1/galaxy/util/custom_logging/fluent_log.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/dbkeys.py` & `galaxy-util-23.0.1/galaxy/util/dbkeys.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/dictifiable.py` & `galaxy-util-23.0.1/galaxy/util/dictifiable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import datetime
 import uuid
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Optional,
+)
 
 
 def dict_for(obj, **kwds):
     # Create dict to represent item.
     return dict(model_class=obj.__class__.__name__, **kwds)
 
 
 class Dictifiable:
     """Mixin that enables objects to be converted to dictionaries. This is useful
     when for sharing objects across boundaries, such as the API, tool scripts,
     and JavaScript code."""
 
-    def to_dict(self, view="collection", value_mapper=None):
+    def to_dict(self, view: str = "collection", value_mapper: Optional[Dict[str, Callable]] = None) -> Dict[str, Any]:
         """
         Return item dictionary.
         """
 
         if not value_mapper:
             value_mapper = {}
 
@@ -25,16 +31,17 @@
             Recursive helper function to get item values.
             """
             # FIXME: why use exception here? Why not look for key in value_mapper
             # first and then default to to_dict?
             try:
                 return item.to_dict(view=view, value_mapper=value_mapper)
             except Exception:
+                assert value_mapper is not None
                 if key in value_mapper:
-                    return value_mapper.get(key)(item)
+                    return value_mapper[key](item)
                 if type(item) == datetime.datetime:
                     return item.isoformat()
                 elif type(item) == uuid.UUID:
                     return str(item)
                 # Leaving this for future reference, though we may want a more
                 # generic way to handle special type mappings going forward.
                 # If the item is of a class that needs to be 'stringified' before being put into a JSON data structure
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/expressions.py` & `galaxy-util-23.0.1/galaxy/util/expressions.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/facts.py` & `galaxy-util-23.0.1/galaxy/util/facts.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/filelock.py` & `galaxy-util-23.0.1/galaxy/util/filelock.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/form_builder.py` & `galaxy-util-23.0.1/galaxy/util/form_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -195,15 +195,7 @@
         d["type"] = "select"
         d["data"] = [{"label": "New History", "value": "new"}]
         if self.user and self.security:
             for a in self.user.histories:
                 if not a.deleted:
                     d["data"].append({"label": a.name, "value": self.security.encode_id(a.id)})
         return d
-
-
-def get_suite():
-    """Get unittest suite for this module"""
-    import doctest
-    import sys
-
-    return doctest.DocTestSuite(sys.modules[__name__])
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/heartbeat.py` & `galaxy-util-23.0.1/galaxy/util/heartbeat.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/image_util.py` & `galaxy-util-23.0.1/galaxy/util/image_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/inflection.py` & `galaxy-util-23.0.1/galaxy/util/inflection.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/json.py` & `galaxy-util-23.0.1/galaxy/util/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from collections.abc import (
     Iterable,
     Mapping,
     Sequence,
 )
 from decimal import Decimal
 
-from ..util import unicodify
+from . import unicodify
 
 __all__ = ("safe_dumps", "validate_jsonrpc_request", "validate_jsonrpc_response", "jsonrpc_request", "jsonrpc_response")
 
 log = logging.getLogger(__name__)
 
 to_json_string = json.dumps
 from_json_string = json.loads
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/jstree.py` & `galaxy-util-23.0.1/galaxy/util/jstree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,154 +1,152 @@
 import copy
 import os
 from collections import namedtuple
 
 import dictobj
 
-Path = namedtuple('Path', ('path', 'id', 'options'))
+Path = namedtuple("Path", ("path", "id", "options"))
 
 
 class Node(dictobj.DictionaryObject):
-  """
-  Copyright 2012 "Grim Apps"
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-  Helper class written by William Grim - grimwm
-  Original repo: https://github.com/grimwm/py-jstree
-  Code adjusted according to the idea of Frank Blechschmidt - FraBle
-  Thank you!
-  ************************
-  This class exists as a helper to the JSTree.  Its "jsonData" method can
-  generate sub-tree JSON without putting the logic directly into the JSTree.
-
-  This data structure is only semi-immutable.  The JSTree uses a directly
-  iterative (i.e. no stack is managed) builder pattern to construct a
-  tree out of paths.  Therefore, the children are not known in advance, and
-  we have to keep the children attribute mutable.
-  """
-
-  def __init__(self, path, oid, **kwargs):
-    """
-    kwargs allows users to pass arbitrary information into a Node that
-    will later be output in jsonData().  It allows for more advanced
-    configuration than the default path handling that JSTree currently allows.
-    For example, users may want to pass "attr" or some other valid jsTree options.
-
-    Example:
-      >>> node = Node('a', None)
-      >>> assert node._items == {'text': 'a', 'children': dictobj.MutableDictionaryObject({})}
-      >>> assert node.jsonData() == {'text': 'a'}
-
-      >>> node = Node('a', 1)
-      >>> assert node._items == {'text': 'a', 'children': dictobj.MutableDictionaryObject({}), 'li_attr': dictobj.DictionaryObject({'id': 1}), 'id': 1}
-      >>> assert node.jsonData() == {'text': 'a', 'id': 1, 'li_attr': {'id': 1}}
-
-      >>> node = Node('a', 5, icon="folder", state = {'opened': True})
-      >>> assert node._items == {'text': 'a', 'id': 5, 'state': dictobj.DictionaryObject({'opened': True}), 'children': dictobj.MutableDictionaryObject({}), 'li_attr': dictobj.DictionaryObject({'id': 5}), 'icon': 'folder'}
-      >>> assert node.jsonData() == {'text': 'a', 'state': {'opened': True}, 'id': 5, 'li_attr': {'id': 5}, 'icon': 'folder'}
     """
-    super().__init__()
+    Copyright 2012 "Grim Apps"
 
-    children = kwargs.get('children', {})
-    if len([key for key in children if not isinstance(children[key], Node)]):
-      raise TypeError(
-        f"One or more children were not instances of '{Node.__name__}'")
-    if 'children' in kwargs:
-      del kwargs['children']
-    self._items['children'] = dictobj.MutableDictionaryObject(children)
-
-    if oid is not None:
-      li_attr = kwargs.get('li_attr', {})
-      li_attr['id'] = oid
-      kwargs['li_attr'] = li_attr
-      self._items['id'] = oid
-
-    self._items.update(dictobj.DictionaryObject(**kwargs))
-    self._items['text'] = path
-
-  def jsonData(self):
-    children = [self.children[k].jsonData() for k in sorted(self.children)]
-    output = {}
-    for k in self._items:
-      if 'children' == k:
-        continue
-      if isinstance(self._items[k], dictobj.DictionaryObject):
-        output[k] = self._items[k].asdict()
-      else:
-        output[k] = self._items[k]
-    if len(children):
-      output['children'] = children
-    return output
+     Licensed under the Apache License, Version 2.0 (the "License");
+     you may not use this file except in compliance with the License.
+     You may obtain a copy of the License at
+
+         http://www.apache.org/licenses/LICENSE-2.0
+
+     Unless required by applicable law or agreed to in writing, software
+     distributed under the License is distributed on an "AS IS" BASIS,
+     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+     See the License for the specific language governing permissions and
+     limitations under the License.
+
+    Helper class written by William Grim - grimwm
+    Original repo: https://github.com/grimwm/py-jstree
+    Code adjusted according to the idea of Frank Blechschmidt - FraBle
+    Thank you!
+    ************************
+    This class exists as a helper to the JSTree.  Its "jsonData" method can
+    generate sub-tree JSON without putting the logic directly into the JSTree.
+
+    This data structure is only semi-immutable.  The JSTree uses a directly
+    iterative (i.e. no stack is managed) builder pattern to construct a
+    tree out of paths.  Therefore, the children are not known in advance, and
+    we have to keep the children attribute mutable.
+    """
+
+    def __init__(self, path, oid, **kwargs):
+        """
+        kwargs allows users to pass arbitrary information into a Node that
+        will later be output in jsonData().  It allows for more advanced
+        configuration than the default path handling that JSTree currently allows.
+        For example, users may want to pass "attr" or some other valid jsTree options.
+
+        Example:
+          >>> node = Node('a', None)
+          >>> assert node._items == {'text': 'a', 'children': dictobj.MutableDictionaryObject({})}
+          >>> assert node.jsonData() == {'text': 'a'}
+
+          >>> node = Node('a', 1)
+          >>> assert node._items == {'text': 'a', 'children': dictobj.MutableDictionaryObject({}), 'li_attr': dictobj.DictionaryObject({'id': 1}), 'id': 1}
+          >>> assert node.jsonData() == {'text': 'a', 'id': 1, 'li_attr': {'id': 1}}
+
+          >>> node = Node('a', 5, icon="folder", state = {'opened': True})
+          >>> assert node._items == {'text': 'a', 'id': 5, 'state': dictobj.DictionaryObject({'opened': True}), 'children': dictobj.MutableDictionaryObject({}), 'li_attr': dictobj.DictionaryObject({'id': 5}), 'icon': 'folder'}
+          >>> assert node.jsonData() == {'text': 'a', 'state': {'opened': True}, 'id': 5, 'li_attr': {'id': 5}, 'icon': 'folder'}
+        """
+        super().__init__()
+
+        children = kwargs.get("children", {})
+        if len([key for key in children if not isinstance(children[key], Node)]):
+            raise TypeError(f"One or more children were not instances of '{Node.__name__}'")
+        if "children" in kwargs:
+            del kwargs["children"]
+        self._items["children"] = dictobj.MutableDictionaryObject(children)
+
+        if oid is not None:
+            li_attr = kwargs.get("li_attr", {})
+            li_attr["id"] = oid
+            kwargs["li_attr"] = li_attr
+            self._items["id"] = oid
+
+        self._items.update(dictobj.DictionaryObject(**kwargs))
+        self._items["text"] = path
+
+    def jsonData(self):
+        children = [self.children[k].jsonData() for k in sorted(self.children)]
+        output = {}
+        for k in self._items:
+            if "children" == k:
+                continue
+            if isinstance(self._items[k], dictobj.DictionaryObject):
+                output[k] = self._items[k].asdict()
+            else:
+                output[k] = self._items[k]
+        if len(children):
+            output["children"] = children
+        return output
 
 
 class JSTree(dictobj.DictionaryObject):
-  """
-  An immutable dictionary-like object that converts a list of "paths"
-  into a tree structure suitable for jQuery's jsTree.
-  """
-
-  def __init__(self, paths, **kwargs):
     """
-    Take a list of paths and put them into a tree.  Paths with the same prefix should
-    be at the same level in the tree.
-
-    kwargs may be standard jsTree options used at all levels in the tree.  These will be outputted
-    in the JSON.
-
+    An immutable dictionary-like object that converts a list of "paths"
+    into a tree structure suitable for jQuery's jsTree.
     """
-    if len([p for p in paths if not isinstance(p, Path)]):
-      raise TypeError(
-        f"All paths must be instances of '{Path.__name__}'")
-
-    super().__init__()
-
-    root = Node('', None, **kwargs)
-    for path in sorted(paths):
-      curr = root
-      subpaths = path.path.split(os.path.sep)
-      for i, subpath in enumerate(subpaths):
-        if subpath not in curr.children:
-          opt = copy.deepcopy(kwargs)
-          if len(subpaths) - 1 == i:
-            oid = path.id
-            opt.update(path.options) if path.options is not None else None
-          else:
-            oid = None
-          curr.children[subpath] = Node(subpath, oid, **opt)
-          # oid = path.id if len(subpaths) - 1 == i else None
-          # curr.children[subpath] = Node(subpath, oid, **kwargs)
-        curr = curr.children[subpath]
-    self._items['_root'] = root
 
-  def pretty(self, root=None, depth=0, spacing=2):
-    """
-    Create a "pretty print" represenation of the tree with customized indentation at each
-    level of the tree.
-    """
-    if root is None:
-      root = self._root
-    fmt = "%s%s/" if root.children else "%s%s"
-    s = fmt % (" " * depth * spacing, root.text)
-    for child in root.children:
-      child = root.children[child]
-      s += f"\n{self.pretty(child, depth + 1, spacing)}"
-    return s
+    def __init__(self, paths, **kwargs):
+        """
+        Take a list of paths and put them into a tree.  Paths with the same prefix should
+        be at the same level in the tree.
+
+        kwargs may be standard jsTree options used at all levels in the tree.  These will be outputted
+        in the JSON.
+
+        """
+        if len([p for p in paths if not isinstance(p, Path)]):
+            raise TypeError(f"All paths must be instances of '{Path.__name__}'")
+
+        super().__init__()
+
+        root = Node("", None, **kwargs)
+        for path in sorted(paths):
+            curr = root
+            subpaths = path.path.split(os.path.sep)
+            for i, subpath in enumerate(subpaths):
+                if subpath not in curr.children:
+                    opt = copy.deepcopy(kwargs)
+                    if len(subpaths) - 1 == i:
+                        oid = path.id
+                        opt.update(path.options) if path.options is not None else None
+                    else:
+                        oid = None
+                    curr.children[subpath] = Node(subpath, oid, **opt)
+                    # oid = path.id if len(subpaths) - 1 == i else None
+                    # curr.children[subpath] = Node(subpath, oid, **kwargs)
+                curr = curr.children[subpath]
+        self._items["_root"] = root
+
+    def pretty(self, root=None, depth=0, spacing=2):
+        """
+        Create a "pretty print" represenation of the tree with customized indentation at each
+        level of the tree.
+        """
+        if root is None:
+            root = self._root
+        fmt = "%s%s/" if root.children else "%s%s"
+        s = fmt % (" " * depth * spacing, root.text)
+        for child in root.children:
+            child = root.children[child]
+            s += f"\n{self.pretty(child, depth + 1, spacing)}"
+        return s
+
+    def jsonData(self):
+        """
+        Returns a copy of the internal tree in a JSON-friendly format,
+        ready for consumption by jsTree.  The data is represented as a
+        list of dictionaries, each of which are our internal nodes.
 
-  def jsonData(self):
-    """
-    Returns a copy of the internal tree in a JSON-friendly format,
-    ready for consumption by jsTree.  The data is represented as a
-    list of dictionaries, each of which are our internal nodes.
-
-    """
-    return [self._root.children[k].jsonData() for k in sorted(self._root.children)]
+        """
+        return [self._root.children[k].jsonData() for k in sorted(self._root.children)]
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/lazy_process.py` & `galaxy-util-23.0.1/galaxy/util/lazy_process.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/monitors.py` & `galaxy-util-23.0.1/galaxy/util/monitors.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/odict.py` & `galaxy-util-23.0.1/galaxy/util/odict.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         item = dict
         self._keys = []
         if isinstance(item, dict_alias):
             UserDict.__init__(self, item)
         else:
             UserDict.__init__(self, None)
         if isinstance(item, list):
-            for (key, value) in item:
+            for key, value in item:
                 self[key] = value
 
     def __delitem__(self, key):
         UserDict.__delitem__(self, key)
         self._keys.remove(key)
 
     def __setitem__(self, key, item):
@@ -68,15 +68,15 @@
 
     def setdefault(self, key, failobj=None):
         if key not in self._keys:
             self._keys.append(key)
         return UserDict.setdefault(self, key, failobj)
 
     def update(self, dict):
-        for (key, val) in dict.items():
+        for key, val in dict.items():
             self.__setitem__(key, val)
 
     def values(self):
         return map(self.get, self._keys)
 
     def iterkeys(self):
         return iter(self._keys)
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/oset.py` & `galaxy-util-23.0.1/galaxy/util/oset.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/path/__init__.py` & `galaxy-util-23.0.1/galaxy/util/path/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import types
 from functools import partial
 from itertools import starmap
 from operator import getitem
 from os import (
     extsep,
     makedirs,
+    PathLike,
     stat,
     walk,
 )
 from os.path import (
     abspath,
     basename,
     dirname,
@@ -23,51 +24,74 @@
     isabs,
     islink,
     join,
     normpath,
     pardir,
     realpath,
     relpath,
+    sep as separator,
 )
-from os.path import sep as separator
 from pathlib import Path
+from typing import (
+    AnyStr,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    TYPE_CHECKING,
+    Union,
+)
 
 try:
     from grp import getgrgid
 except ImportError:
     getgrgid = None  # type: ignore[assignment]
 
 try:
     from pwd import getpwuid
 except ImportError:
     getpwuid = None  # type: ignore[assignment]
 
 import galaxy.util
 
+# Stable in Python 3.10 path types
+if TYPE_CHECKING:
+    StrPath = Union[str, PathLike[str]]
+    BytesPath = Union[bytes, PathLike[bytes]]
+    GenericPath = Union[AnyStr, PathLike[AnyStr]]
+    StrOrBytesPath = Union[str, bytes, PathLike[str], PathLike[bytes]]
+else:
+    StrPath = Union[str, PathLike]
+    BytesPath = Union[bytes, PathLike]
+    GenericPath = Union[AnyStr, PathLike]
+    StrOrBytesPath = Union[str, bytes, PathLike, PathLike]
+
+AllowListT = Optional[List[GenericPath]]
+
 WALK_MAX_DIRS = 10000
 
 log = logging.getLogger(__name__)
 
 
-def safe_path(path, allowlist=None):
+def safe_path(path: GenericPath, allowlist: AllowListT = None):
     """Ensure that a the absolute location of the path (after following symlinks) is either itself or on the allowlist
     of acceptable locations.
 
     This function does not perform an existence check, thus, if the path does not exist, ``True`` is returned.
 
     :type path:         string
     :param path:        a path to check
     :type allowlist:    comma separated list of strings
     :param allowlist:   list of acceptable locations
     :return:            ``True`` if ``path`` resolves to itself or a allowlisted location
     """
     return any(__contains(dirname(path), path, allowlist=allowlist))
 
 
-def safe_contains(prefix, path, allowlist=None, real=None):
+def safe_contains(prefix: GenericPath, path: GenericPath, allowlist: AllowListT = None, real=None):
     """Ensure a path is contained within another path.
 
     Given any two filesystem paths, ensure that ``path`` is contained in ``prefix``. If ``path`` exists (either as an
     absolute path or relative to ``prefix``), it is canonicalized with :func:`os.path.realpath` to ensure it is not a
     symbolic link that points outside of ``prefix``. If it is a symbolic link and ``allowlist`` is set, the symbolic link
     may also point inside a ``allowlist`` path.
 
@@ -90,23 +114,23 @@
 class _SafeContainsDirectoryChecker:
     def __init__(self, dirpath, prefix, allowlist=None):
         self.allowlist = allowlist
         self.dirpath = dirpath
         self.prefix = prefix
         self.real_dirpath = realpath(join(prefix, dirpath))
 
-    def check(self, filename):
+    def check(self, filename: GenericPath) -> bool:
         dirpath_path = join(self.real_dirpath, filename)
         if islink(dirpath_path):
             return safe_contains(self.prefix, filename, allowlist=self.allowlist)
         else:
             return safe_contains(self.prefix, filename, allowlist=self.allowlist, real=dirpath_path)
 
 
-def safe_makedirs(path):
+def safe_makedirs(path: GenericPath) -> None:
     """Safely make a directory, do not fail if it already exists or is created during execution.
 
     :type path:     string
     :param path:    a directory to create
     """
     # prechecking for existence is faster than try/except
     if not exists(path):
@@ -115,15 +139,15 @@
         except OSError as e:
             # reviewing the source for Python 2.7, this would only ever happen for the last path element anyway so no
             # need to recurse - this exception means the last part of the path was already in existence.
             if e.errno != errno.EEXIST:
                 raise
 
 
-def safe_relpath(path):
+def safe_relpath(path: GenericPath) -> bool:
     """Determine whether a relative path references a path outside its root.
 
     This is a path computation: the filesystem is not accessed to confirm the existence or nature of ``path``.
 
     :type path:     string
     :param path:    a path to check
     :rtype:         bool
@@ -148,15 +172,15 @@
     """
     for i, elems in enumerate(walk(path, followlinks=bool(allowlist)), start=1):
         dirpath, dirnames, filenames = elems
         _check = _SafeContainsDirectoryChecker(dirpath, path, allowlist=allowlist).check
 
         if allowlist and i % WALK_MAX_DIRS == 0:
             raise RuntimeError(
-                "Breaking out of walk of %s after %s iterations (most likely infinite symlink recursion) at: %s"
+                "Breaking out of walk of %r after %s iterations (most likely infinite symlink recursion) at: %r"
                 % (path, WALK_MAX_DIRS, dirpath)
             )
         _prefix = partial(join, dirpath)
 
         prune = False
         for dname in dirnames:
             if not _check(join(dirpath, dname)):
@@ -172,15 +196,15 @@
                 break
         if prune:
             filenames = map(basename, filter(_check, map(_prefix, filenames)))
 
         yield (dirpath, dirnames, filenames)
 
 
-def unsafe_walk(path, allowlist=None, username=None):
+def unsafe_walk(path: GenericPath, allowlist: AllowListT = None, username: Optional[str] = None):
     """Walk a path and ensure that none of its contents are symlinks outside the path.
 
     It is assumed that ``path`` itself has already been validated e.g. with :func:`safe_relpath` or
     :func:`safe_contains`. This function is most useful for the case where you want to test whether a directory contains
     safe paths, but do not want to actually walk the safe contents.
 
     :type path:         string
@@ -196,15 +220,15 @@
         if username and is_safe:
             is_safe = full_path_permission_for_user(path, walked_path, username=username, skip_prefix=True)
         if not is_safe:
             unsafe_paths.append(walked_path)
     return unsafe_paths
 
 
-def __path_permission_for_user(path, username):
+def __path_permission_for_user(path: GenericPath, username: str) -> bool:
     """
     :type path:         string
     :param path:        a directory or file to check
     :type username:     string
     :param username:    a username matching the systems username
     """
     if getpwuid is None or getgrgid is None:
@@ -223,15 +247,15 @@
         or (file_owner == username and owner_permissions >= 4)
         or (username in group_members and group_permissions >= 4)
     ):
         return True
     return False
 
 
-def full_path_permission_for_user(prefix, path, username, skip_prefix=False):
+def full_path_permission_for_user(prefix, path, username: str, skip_prefix=False):
     """
     Assuming username is identical to the os username, this checks that the
     given user can read the specified path by checking the file permission
     and each parent directory permission.
 
     :type prefix:       string
     :param prefix:      a directory under which ``path`` is to be checked
@@ -256,29 +280,29 @@
             if not __path_permission_for_user(parent_path, username):
                 can_read = False
             depth += 1
             parent_path = dirname(parent_path)
     return can_read
 
 
-def joinext(root, ext):
+def joinext(root: str, ext: str) -> str:
     """
     Roughly the reverse of os.path.splitext.
 
     :type  root: string
     :param root: part of the filename before the extension
     :type  root: string
     :param ext: the extension
     :rtype: string
     :returns: ``root`` joined with ``ext`` separated by a single ``os.extsep``
     """
     return extsep.join((root.rstrip(extsep), ext.lstrip(extsep)))
 
 
-def has_ext(path, ext, aliases=False, ignore=None):
+def has_ext(path: AnyStr, ext: str, aliases=False, ignore=None):
     """
     Determine whether ``path`` has extension ``ext``
 
     :type     path: string
     :param    path: Path to check
     :type      ext: string
     :param     ext: Extension to check
@@ -293,15 +317,15 @@
     root, _ext = __splitext_ignore(path, ignore=ignore)
     if aliases:
         return _ext in extensions[ext]
     else:
         return _ext == ext
 
 
-def get_ext(path, ignore=None, canonicalize=True):
+def get_ext(path: AnyStr, ignore=None, canonicalize=True) -> str:
     """
     Return the extension of ``path``
 
     :type          path: string
     :param         path: Path to check
     :type        ignore: string
     :param       ignore: Ignore this extension at the end of the path (e.g. ``sample``)
@@ -331,15 +355,15 @@
     def __missing__(self, key):
         for v in self.values():
             if key in v:
                 self[key] = v
                 return v
         raise KeyError(key)
 
-    def canonicalize(self, ext):
+    def canonicalize(self, ext: str) -> str:
         # shouldn't raise an IndexError because it should raise a KeyError first
         return self[ext][0]
 
 
 extensions = Extensions(
     {
         "ini": ["ini"],
@@ -369,57 +393,59 @@
         galaxy.util.commands.execute(cmd)
         return True
     except galaxy.util.commands.CommandLineException as e:
         log.warning(f"Changing ownership of {description} {path} failed: {galaxy.util.unicodify(e)}")
         return False
 
 
-def __listify(item):
+def __listify(item) -> Union[list, tuple]:
     """A non-splitting version of :func:`galaxy.util.listify`."""
     if not item:
         return []
     elif isinstance(item, list) or isinstance(item, tuple):
         return item
     else:
         return [item]
 
 
 # helpers
 
 
-def __walk(path):
+def __walk(path: GenericPath) -> Iterator[GenericPath]:
     for dirpath, dirnames, filenames in walk(path):
         for name in dirnames:
             yield join(dirpath, name)
         for name in filenames:
             yield join(dirpath, name)
 
 
-def __contains(prefix, path, allowlist=None, real=None):
+def __contains(
+    prefix: GenericPath, path: GenericPath, allowlist: AllowListT = None, real: Optional[GenericPath] = None
+):
     real = real or realpath(join(prefix, path))
     yield not relpath(real, prefix).startswith(pardir)
     for aldir in allowlist or []:
         # a path is under the allowlist if the relative path between it and the allowlist does not have to go up (..)
         yield not relpath(real, aldir).startswith(pardir)
 
 
-def __ext_strip_sep(ext):
+def __ext_strip_sep(ext: str) -> str:
     return ext.lstrip(extsep)
 
 
-def __splitext_no_sep(path):
-    path = galaxy.util.unicodify(path)
-    return (path.rsplit(extsep, 1) + [""])[0:2]
+def __splitext_no_sep(path: AnyStr) -> List[str]:
+    path_as_str = galaxy.util.unicodify(path)
+    return (path_as_str.rsplit(extsep, 1) + [""])[0:2]
 
 
-def __splitext_ignore(path, ignore=None):
+def __splitext_ignore(path: AnyStr, ignore: Optional[Union[List[str], Tuple[str]]] = None) -> Tuple[str, str]:
     # note: unlike os.path.splitext this strips extsep from ext
-    ignore = map(__ext_strip_sep, __listify(ignore))
+    ignore_map = map(__ext_strip_sep, __listify(ignore))
     root, ext = __splitext_no_sep(path)
-    if ext in ignore:
+    if ext in ignore_map:
         new_path = path[0 : (-len(ext) - 1)]
         root, ext = __splitext_no_sep(new_path)
 
     return (root, ext)
 
 
 # cross-platform support
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/permutations.py` & `galaxy-util-23.0.1/galaxy/util/permutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,48 +2,55 @@
 and tools. This module is meant to capture some general permutation logic that
 can be applicable for both cases but will only be used in the newer tools case
 first.
 
 Maybe this doesn't make sense and maybe much of this stuff could be replaced
 with itertools product and permutations. These are open questions.
 """
+from typing import (
+    Dict,
+    TypeVar,
+)
 
 from galaxy.exceptions import MessageException
 from galaxy.util.bunch import Bunch
 
 input_classification = Bunch(
     SINGLE="single",
     MATCHED="matched",
     MULTIPLIED="multiplied",
 )
 
+# generic type of splitting input dictionary
+T = TypeVar("T")
+
 
 class InputMatchedException(MessageException):
     """Indicates problem matching inputs while building up inputs
     permutations."""
 
 
-def expand_multi_inputs(inputs, classifier, key_filter=None):
+def expand_multi_inputs(inputs: Dict[str, T], classifier, key_filter=None):
     key_filter = key_filter or (lambda x: True)
 
     single_inputs, matched_multi_inputs, multiplied_multi_inputs = __split_inputs(inputs, classifier, key_filter)
 
     # Build up every combination of inputs to be run together.
     input_combos = __extend_with_matched_combos(single_inputs, matched_multi_inputs)
     input_combos = __extend_with_multiplied_combos(input_combos, multiplied_multi_inputs)
 
     return input_combos
 
 
-def __split_inputs(inputs, classifier, key_filter):
+def __split_inputs(inputs: Dict[str, T], classifier, key_filter):
     key_filter = key_filter or (lambda x: True)
 
-    single_inputs = {}
-    matched_multi_inputs = {}
-    multiplied_multi_inputs = {}
+    single_inputs: Dict[str, T] = {}
+    matched_multi_inputs: Dict[str, T] = {}
+    multiplied_multi_inputs: Dict[str, T] = {}
 
     for input_key in filter(key_filter, inputs):
         input_type, expanded_val = classifier(input_key)
         if input_type == input_classification.SINGLE:
             single_inputs[input_key] = expanded_val
         elif input_type == input_classification.MATCHED:
             matched_multi_inputs[input_key] = expanded_val
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/plugin_config.py` & `galaxy-util-23.0.1/galaxy/util/plugin_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/properties.py` & `galaxy-util-23.0.1/galaxy/util/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,56 @@
 """ Module used to blend ini, environment, and explicit dictionary properties
 to determine application configuration. Some hard coded defaults for Galaxy but
 this should be reusable by tool shed and pulsar as well.
 """
 import os
 import os.path
 import sys
-from configparser import ConfigParser
+from configparser import (
+    BasicInterpolation,
+    ConfigParser,
+    InterpolationError,
+)
 from functools import partial
 from itertools import (
     product,
     starmap,
 )
+from typing import (
+    cast,
+    Iterable,
+    Optional,
+)
 
 import yaml
 
 from galaxy.exceptions import InvalidFileFormatError
 from galaxy.util.path import (
     extensions,
     has_ext,
     joinext,
 )
 
 
+def get_from_env(key: str, prefixes: Iterable[str], default: Optional[str] = None):
+    """
+    Return first available value for prefix+key set in the environment, or default.
+    An empty prefix is ignored.
+
+    Useful when we need to check against multiple prefixes sequentially,
+    returning the first available value.
+    """
+    for prefix in prefixes:
+        if prefix:
+            value = os.getenv(f"{prefix}{key}")
+            if value:
+                return value
+    return default
+
+
 def find_config_file(names, exts=None, dirs=None, include_samples=False):
     """Locate a config file in multiple directories, with multiple extensions.
 
     >>> from shutil import rmtree
     >>> from tempfile import mkdtemp
     >>> def touch(d, f):
     ...     open(os.path.join(d, f), 'w').close()
@@ -125,55 +150,53 @@
 def _read_from_yaml_file(path):
     with open(path) as f:
         return yaml.safe_load(f)
 
 
 def nice_config_parser(path):
     parser = NicerConfigParser(path, defaults=__default_properties(path))
-    parser.optionxform = str  # Don't lower-case keys
     with open(path) as f:
         parser.read_file(f)
     return parser
 
 
+class _InterpolateWrapper(BasicInterpolation):
+    def before_get(self, parser, section, option, value, defaults):
+        try:
+            return super().before_get(parser, section, option, value, defaults)
+        except InterpolationError:
+            e = cast(InterpolationError, sys.exc_info()[1])
+            args = list(e.args)
+            args[0] = f"Error in file {parser.filename}: {e}"
+            e.args = tuple(args)
+            e.message = args[0]
+            raise
+
+
 class NicerConfigParser(ConfigParser):
     def __init__(self, filename, *args, **kw):
+        kw["interpolation"] = _InterpolateWrapper()
         ConfigParser.__init__(self, *args, **kw)
         self.filename = filename
-        self._interpolation = self.InterpolateWrapper(self._interpolation)
+
+    def optionxform(self, optionstr: str) -> str:
+        # Don't lower-case keys
+        return str(super().optionxform(optionstr))
 
     def defaults(self):
         """Return the defaults, with their values interpolated (with the
         defaults dict itself)
 
         Mainly to support defaults using values such as %(here)s
         """
-        defaults = ConfigParser.defaults(self).copy()
+        defaults = dict(ConfigParser.defaults(self))
         for key, val in defaults.items():
             defaults[key] = self.get("DEFAULT", key) or val
         return defaults
 
-    class InterpolateWrapper:
-        def __init__(self, original):
-            self._original = original
-
-        def __getattr__(self, name):
-            return getattr(self._original, name)
-
-        def before_get(self, parser, section, option, value, defaults):
-            try:
-                return self._original.before_get(parser, section, option, value, defaults)
-            except Exception:
-                e = sys.exc_info()[1]
-                args = list(e.args)
-                args[0] = f"Error in file {parser.filename}: {e}"
-                e.args = tuple(args)
-                e.message = args[0]
-                raise
-
 
 def _running_from_source():
     paths = ["run.sh", "lib/galaxy/__init__.py", "scripts/common_startup.sh"]
     return all(map(os.path.exists, paths))
 
 
 running_from_source = _running_from_source()
@@ -191,15 +214,15 @@
 
 
 def __get_all_configs(dirs, names):
     return list(filter(os.path.exists, starmap(os.path.join, product(dirs, names))))
 
 
 def __find_config_files(names, exts=None, dirs=None, include_samples=False):
-    sample_names = []
+    sample_names: Iterable[str] = []
     if isinstance(names, str):
         names = [names]
     if not dirs:
         dirs = [os.getcwd()]
     if exts:
         # add exts to names, converts back into a list because it's going to be small and we might consume names twice
         names = list(starmap(joinext, product(names, exts)))
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/renamed_temporary_file.py` & `galaxy-util-23.0.1/galaxy/util/renamed_temporary_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Safely write file to temporary file and then move file into place."""
 # Copied from https://stackoverflow.com/a/12007885.
 import os
 import tempfile
 
+from galaxy.util.path import StrOrBytesPath
+
 
 class RenamedTemporaryFile:
     """
     A temporary file object which will be renamed to the specified
     path on exit.
     """
 
-    def __init__(self, final_path, **kwargs):
+    final_path: StrOrBytesPath
+
+    def __init__(self, final_path: StrOrBytesPath, **kwargs):
         """
         >>> dir = tempfile.mkdtemp()
         >>> with RenamedTemporaryFile(os.path.join(dir, 'test.txt'), mode="w") as out:
         ...     _ = out.write('bla')
         """
         tmpfile_dir = kwargs.pop("dir", None)
 
@@ -23,15 +27,15 @@
 
         if tmpfile_dir is None:
             tmpfile_dir = os.path.dirname(final_path)
 
         self.tmpfile = tempfile.NamedTemporaryFile(dir=tmpfile_dir, delete=False, **kwargs)
         self.final_path = final_path
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str):
         """
         Delegate attribute access to the underlying temporary file object.
         """
         return getattr(self.tmpfile, attr)
 
     def __enter__(self):
         self.tmpfile.__enter__()
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/resources.py` & `galaxy-util-23.0.1/galaxy/util/resources.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 """Provide a consistent interface into and utilities for importlib file resources.
 """
 try:
+    from importlib.abc import Traversable  # type: ignore[attr-defined]
     from importlib.resources import files  # type: ignore[attr-defined]
 except ImportError:
     # Python < 3.9
     from importlib_resources import files  # type: ignore[no-redef]
+    from importlib_resources.abc import Traversable  # type: ignore[no-redef]
 
 
-def resource_string(package_or_requirement, resource_name):
+def resource_path(package_or_requirement, resource_name):
     """
     Return specified resource as a string.
 
     Replacement function for pkg_resources.resource_string, but returns unicode string instead of bytestring.
     """
-    return files(package_or_requirement).joinpath(resource_name).read_text()
+    return files(package_or_requirement).joinpath(resource_name)
+
+
+def resource_string(package_or_requirement, resource_name) -> str:
+    """
+    Return specified resource as a string.
+
+    Replacement function for pkg_resources.resource_string, but returns unicode string instead of bytestring.
+    """
+    return resource_path(package_or_requirement, resource_name).read_text()
 
 
 __all__ = (
     "files",
     "resource_string",
+    "resource_path",
+    "Traversable",
 )
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/rules_dsl.py` & `galaxy-util-23.0.1/galaxy/util/rules_dsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,16 @@
         return result
 
     new_data = list(map(new_row, data))
     return new_data
 
 
 class BaseRuleDefinition(metaclass=abc.ABCMeta):
-    @abc.abstractproperty
+    @property
+    @abc.abstractmethod
     def rule_type(self):
         """Short string describing type of rule (plugin class) to use."""
 
     @abc.abstractmethod
     def validate_rule(self, rule):
         """Validate dictified rule definition of this type."""
 
@@ -446,15 +447,15 @@
             return a_val
 
         sorted_data = sorted(sortable, key=sort_func)
 
         new_data = []
         new_sources = []
 
-        for (row, source) in sorted_data:
+        for row, source in sorted_data:
             new_data.append(row)
             new_sources.append(source)
 
         return new_data, new_sources
 
 
 class SwapColumnsRuleDefinition(BaseRuleDefinition):
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/rules_dsl_spec.yml` & `galaxy-util-23.0.1/galaxy/util/rules_dsl_spec.yml`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/sanitize_html.py` & `galaxy-util-23.0.1/galaxy/util/sanitize_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,9 +248,9 @@
     "xml:lang",
 ]
 
 
 def sanitize_html(htmlSource, allow_data_urls=False):
     kwd = dict(tags=_acceptable_elements, attributes=_acceptable_attributes, strip=True)
     if allow_data_urls:
-        kwd["protocols"] = bleach.ALLOWED_PROTOCOLS + ["data"]
+        kwd["protocols"] = list(bleach.ALLOWED_PROTOCOLS) + ["data"]
     return bleach.clean(unicodify(htmlSource), **kwd)
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/script.py` & `galaxy-util-23.0.1/galaxy/util/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/search.py` & `galaxy-util-23.0.1/galaxy/util/search.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/simplegraph.py` & `galaxy-util-23.0.1/galaxy/util/simplegraph.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/sleeper.py` & `galaxy-util-23.0.1/galaxy/util/sleeper.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/sockets.py` & `galaxy-util-23.0.1/galaxy/util/sockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 import socket
 import sys
 
 from galaxy.util import commands
 
 
-def get_ip():
+def get_ip() -> str:
     if sys.platform == "darwin":
         # If we're on OSX it is likely that the docker host is localhost.
         return socket.gethostbyname(socket.gethostname())
     # This method assumes that the ip with default route is the ip we want to return
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         # doesn't even have to be reachable
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/specs.py` & `galaxy-util-23.0.1/galaxy/util/specs.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/sqlite.py` & `galaxy-util-23.0.1/galaxy/util/sqlite.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/submodules.py` & `galaxy-util-23.0.1/galaxy/util/submodules.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/task.py` & `galaxy-util-23.0.1/galaxy/util/task.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/template.py` & `galaxy-util-23.0.1/galaxy/util/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # Skip libpasteurize fixers, which make sure code is py2 and py3 compatible.
 # This is not needed, we only translate code on py3.
 myfixes = [f for f in myfixes if not f.startswith("libpasteurize")]
 refactoring_tool = RefactoringTool(myfixes, {"print_function": True})
 
 
 class FixedModuleCodeCompiler(Compiler):
-
     module_code = None
 
     def getModuleCode(self):
         self._moduleDef = self.module_code
         return self._moduleDef
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/tool_shed/encoding_util.py` & `galaxy-util-23.0.1/galaxy/util/tool_shed/encoding_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/topsort.py` & `galaxy-util-23.0.1/galaxy/util/topsort.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/ucsc.py` & `galaxy-util-23.0.1/galaxy/util/ucsc.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/validation.py` & `galaxy-util-23.0.1/galaxy/util/validation.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/watcher.py` & `galaxy-util-23.0.1/galaxy/util/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/xml_macros.py` & `galaxy-util-23.0.1/galaxy/util/xml_macros.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,22 +127,22 @@
     expand tokens in element and (recursively) in its children
     replacements of text attributes and attribute values are
     possible
     """
     value = element.text
     if value:
         new_value = _expand_tokens_str(element.text, tokens)
-        if not (new_value is value):
+        if new_value is not value:
             element.text = new_value
     for key, value in element.attrib.items():
         new_value = _expand_tokens_str(value, tokens)
-        if not (new_value is value):
+        if new_value is not value:
             element.attrib[key] = new_value
         new_key = _expand_tokens_str(key, tokens)
-        if not (new_key is key):
+        if new_key is not key:
             element.attrib[new_key] = element.attrib[key]
             del element.attrib[key]
     # recursively expand in childrens
     _expand_tokens(list(element), tokens)
 
 
 def _expand_tokens_str(s, tokens):
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/yaml_util.py` & `galaxy-util-23.0.1/galaxy/util/yaml_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import yaml
 from yaml.constructor import ConstructorError
 
 try:
     from yaml import CSafeLoader as SafeLoader
 except ImportError:
-    from yaml import SafeLoader  # type: ignore[misc]
+    from yaml import SafeLoader  # type: ignore[misc, assignment]
 
 
 log = logging.getLogger(__name__)
 
 
 class OrderedLoader(SafeLoader):
     # This class was pulled out of ordered_load() for the sake of
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy/util/zipstream.py` & `galaxy-util-23.0.1/galaxy/util/zipstream.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 import os
 import zlib
+from typing import (
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Set,
+)
 from urllib.parse import quote
 
 import zipstream
 
 from .path import safe_walk
 
 CRC32_MIN = 1444
 CRC32_MAX = 1459
 
 
 class ZipstreamWrapper:
-    def __init__(self, archive_name=None, upstream_mod_zip=False, upstream_gzip=False):
+    def __init__(
+        self, archive_name: Optional[str] = None, upstream_mod_zip: bool = False, upstream_gzip: bool = False
+    ) -> None:
         self.upstream_mod_zip = upstream_mod_zip
         self.archive_name = archive_name
         if not self.upstream_mod_zip:
             self.archive = zipstream.ZipFile(
                 allowZip64=True, compression=zipstream.ZIP_STORED if upstream_gzip else zipstream.ZIP_DEFLATED
             )
-        self.files = []
-        self.directories = set()
+        self.files: List[str] = []
+        self.directories: Set[str] = set()
         self.size = 0
 
-    def response(self):
+    def response(self) -> Iterator[bytes]:
         if self.upstream_mod_zip:
             dir_lines = [f"0 0 @directory {directory}" for directory in self.directories]
             yield "\n".join(dir_lines + self.files).encode()
         else:
             yield from iter(self.archive)
 
-    def get_headers(self):
+    def get_headers(self) -> Dict[str, str]:
         headers = {}
         if self.archive_name:
             headers["Content-Disposition"] = f'attachment; filename="{self.archive_name}.zip"'
         if self.upstream_mod_zip:
             headers["X-Archive-Files"] = "zip"
         else:
             headers["Content-Type"] = "application/x-zip-compressed"
         return headers
 
-    def add_path(self, path, archive_name):
+    def add_path(self, path: str, archive_name: str) -> None:
         size = int(os.stat(path).st_size)
         if self.upstream_mod_zip:
             # calculating crc32 would defeat the point of using mod-zip, but if we ever calculate hashsums we should consider this
             crc32 = "-"
             # We do have to calculate the crc32 for files that are between 1444 and 1459 bytes in size, xref: https://github.com/evanmiller/mod_zip/issues/44#issuecomment-656660686
             # Oddly that seems to be only true for usegalaxy.org (nginx version 1.12.2), and works fine locally (nginx 1.19.10).
             # May have been fixed in nginx 1.17.0
@@ -55,15 +64,15 @@
             if head:
                 self.directories.add(head)
             self.files.append(line)
         else:
             self.size += size
             self.archive.write(path, archive_name)
 
-    def write(self, path, archive_name=None):
+    def write(self, path: str, archive_name: Optional[str] = None) -> None:
         if os.path.isdir(path):
             pardir = os.path.join(path, os.pardir)
             for root, directories, files in safe_walk(path):
                 for directory in directories:
                     dir_path = os.path.join(root, directory)
                     self.add_path(dir_path, os.path.relpath(dir_path, pardir))
                 for file in files:
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy_util.egg-info/PKG-INFO` & `galaxy-util-23.0.1/galaxy_util.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-util
-Version: 22.5.0.dev3
+Version: 23.0.1
 Summary: Galaxy generic utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: jstree
 Provides-Extra: template
@@ -33,64 +34,69 @@
 
 
 Overview
 --------
 
 The Galaxy_ utilities module.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
 History
 -------
 
 .. to_doc
 
----------------------
-22.5.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
 
+=========
+Bug fixes
+=========
 
----------------------
+* Replace httpbin service with pytest-httpserver by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16042 <https://github.com/galaxyproject/galaxy/pull/16042>`_
+
+-------------------
 22.1.2 (2022-12-08)
----------------------
+-------------------
 
 * Pin packaging dependency to < 22, fixes ``LegacyVersion`` import errors
 * Add missing pyparsing dependency
 
----------------------
+-------------------
 22.1.1 (2022-08-22)
----------------------
+-------------------
 
 * First release from the 22.01 branch of Galaxy
 
----------------------
+-------------------
 21.1.0 (2021-03-19)
----------------------
+-------------------
 
 * First release from the 21.01 branch of Galaxy.
 
----------------------
+-------------------
 20.9.1 (2020-10-28)
----------------------
+-------------------
+
 
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-03)
----------------------
+-------------------
 
 * First release from 20.05 branch of Galaxy.
 
----------------------
+-------------------
 19.9.0 (2019-11-21)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
```

### Comparing `galaxy-util-22.5.0.dev3/galaxy_util.egg-info/SOURCES.txt` & `galaxy-util-23.0.1/galaxy_util.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.rst
 dev-requirements.txt
 pyproject.toml
 setup.cfg
 test-requirements.txt
 galaxy/__init__.py
+galaxy/py.typed
 galaxy/version.py
 galaxy/exceptions/__init__.py
 galaxy/exceptions/error_codes.json
 galaxy/exceptions/error_codes.py
 galaxy/util/__init__.py
 galaxy/util/aliaspickler.py
 galaxy/util/bool_expressions.py
@@ -18,26 +19,28 @@
 galaxy/util/bytesize.py
 galaxy/util/checkers.py
 galaxy/util/commands.py
 galaxy/util/compression_utils.py
 galaxy/util/dbkeys.py
 galaxy/util/dictifiable.py
 galaxy/util/docutils_template.txt
+galaxy/util/drs.py
 galaxy/util/dynamic.py
 galaxy/util/expressions.py
 galaxy/util/facts.py
 galaxy/util/filelock.py
 galaxy/util/form_builder.py
 galaxy/util/hash_util.py
 galaxy/util/heartbeat.py
 galaxy/util/image_util.py
 galaxy/util/inflection.py
 galaxy/util/json.py
 galaxy/util/jstree.py
 galaxy/util/lazy_process.py
+galaxy/util/markdown.py
 galaxy/util/monitors.py
 galaxy/util/odict.py
 galaxy/util/oset.py
 galaxy/util/permutations.py
 galaxy/util/plugin_config.py
 galaxy/util/properties.py
 galaxy/util/renamed_temporary_file.py
@@ -51,29 +54,33 @@
 galaxy/util/sleeper.py
 galaxy/util/sockets.py
 galaxy/util/specs.py
 galaxy/util/sqlite.py
 galaxy/util/submodules.py
 galaxy/util/task.py
 galaxy/util/template.py
+galaxy/util/themes.py
 galaxy/util/tool_version.py
 galaxy/util/topsort.py
 galaxy/util/ucsc.py
+galaxy/util/unittest.py
 galaxy/util/validation.py
 galaxy/util/watcher.py
 galaxy/util/xml_macros.py
 galaxy/util/yaml_util.py
 galaxy/util/zipstream.py
 galaxy/util/custom_logging/__init__.py
 galaxy/util/custom_logging/fluent_log.py
 galaxy/util/path/__init__.py
 galaxy/util/path/ntpath.py
 galaxy/util/path/posixpath.py
 galaxy/util/tool_shed/__init__.py
 galaxy/util/tool_shed/common_util.py
 galaxy/util/tool_shed/encoding_util.py
+galaxy/util/tool_shed/tool_shed_registry.py
 galaxy/util/tool_shed/xml_util.py
+galaxy/util/unittest_utils/__init__.py
 galaxy_util.egg-info/PKG-INFO
 galaxy_util.egg-info/SOURCES.txt
 galaxy_util.egg-info/dependency_links.txt
 galaxy_util.egg-info/requires.txt
 galaxy_util.egg-info/top_level.txt
```

### Comparing `galaxy-util-22.5.0.dev3/setup.cfg` & `galaxy-util-23.0.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy generic utilities
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-util
 url = https://github.com/galaxyproject/galaxy
-version = 22.5.0.dev3
+version = 23.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	bleach
 	boltons
 	docutils
```

