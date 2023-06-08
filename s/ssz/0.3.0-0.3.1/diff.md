# Comparing `tmp/ssz-0.3.0.tar.gz` & `tmp/ssz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssz-0.3.0.tar", last modified: Tue Aug 23 03:07:40 2022, max compression
+gzip compressed data, was "ssz-0.3.1.tar", last modified: Thu Jun  8 21:09:44 2023, max compression
```

## Comparing `ssz-0.3.0.tar` & `ssz-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,56 @@
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.121901 ssz-0.3.0/
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/.tox/
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/.tox/lint/
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/.tox/lint/lib/
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/.tox/lint/lib/python3.8/
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/.tox/lint/lib/python3.8/site-packages/
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/.tox/lint/lib/python3.8/site-packages/pyrsistent/
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     7188 2022-08-18 21:10:23.000000 ssz-0.3.0/.tox/lint/lib/python3.8/site-packages/pyrsistent/__init__.pyi
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)    10409 2022-08-18 21:10:23.000000 ssz-0.3.0/.tox/lint/lib/python3.8/site-packages/pyrsistent/typing.pyi
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1090 2022-08-18 21:04:44.000000 ssz-0.3.0/LICENSE
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      160 2022-08-18 21:04:44.000000 ssz-0.3.0/MANIFEST.in
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     4003 2022-08-23 03:07:40.121901 ssz-0.3.0/PKG-INFO
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     2953 2022-08-18 21:04:44.000000 ssz-0.3.0/README.md
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1116 2022-08-18 21:04:44.000000 ssz-0.3.0/pyproject.toml
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)        9 2022-08-18 18:45:11.000000 ssz-0.3.0/requirements-docs.txt
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)       38 2022-08-23 03:07:40.121901 ssz-0.3.0/setup.cfg
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     2721 2022-08-23 03:07:23.000000 ssz-0.3.0/setup.py
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.117901 ssz-0.3.0/ssz/
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      674 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/__init__.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     3474 2022-08-18 19:47:08.000000 ssz-0.3.0/ssz/abc.py
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.121901 ssz-0.3.0/ssz/cache/
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)       42 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/cache/__init__.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1363 2022-08-18 19:47:08.000000 ssz-0.3.0/ssz/cache/cache.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1195 2022-08-18 21:04:44.000000 ssz-0.3.0/ssz/cache/utils.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1031 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/codec.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      564 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/constants.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      341 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/exceptions.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      374 2022-08-18 19:47:08.000000 ssz-0.3.0/ssz/hash.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)    13105 2022-08-18 19:47:08.000000 ssz-0.3.0/ssz/hash_tree.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)    12474 2022-08-18 21:04:44.000000 ssz-0.3.0/ssz/hashable_container.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      711 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/hashable_list.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)    14861 2022-08-18 21:04:44.000000 ssz-0.3.0/ssz/hashable_structure.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      849 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/hashable_vector.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)        0 2022-08-18 21:04:44.000000 ssz-0.3.0/ssz/py.typed
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.121901 ssz-0.3.0/ssz/sedes/
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1847 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/__init__.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1936 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/base.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     5982 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/basic.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     3581 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/bitlist.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     2477 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/bitvector.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1125 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/boolean.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      951 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/byte.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1900 2022-08-23 03:05:38.000000 ssz-0.3.0/ssz/sedes/byte_list.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     2002 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/byte_vector.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     6580 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/container.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     6175 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/list.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)    13836 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/serializable.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1957 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/signed_serializable.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1493 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/uint.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     5343 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/sedes/vector.py
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.121901 ssz-0.3.0/ssz/tools/
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      149 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/tools/__init__.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      708 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/tools/codec.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     3822 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/tools/dump.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     4324 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/tools/parse.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      300 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/tree_hash.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      327 2022-08-18 18:45:11.000000 ssz-0.3.0/ssz/typing.py
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     6691 2022-08-18 19:47:08.000000 ssz-0.3.0/ssz/utils.py
-drwxrwxr-x   0 jcarver   (1000) jcarver   (1001)        0 2022-08-23 03:07:40.121901 ssz-0.3.0/ssz.egg-info/
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     4003 2022-08-23 03:07:39.000000 ssz-0.3.0/ssz.egg-info/PKG-INFO
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)     1080 2022-08-23 03:07:40.000000 ssz-0.3.0/ssz.egg-info/SOURCES.txt
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)        1 2022-08-23 03:07:39.000000 ssz-0.3.0/ssz.egg-info/dependency_links.txt
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)        1 2022-08-23 03:07:39.000000 ssz-0.3.0/ssz.egg-info/not-zip-safe
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)      731 2022-08-23 03:07:39.000000 ssz-0.3.0/ssz.egg-info/requires.txt
--rw-rw-r--   0 jcarver   (1000) jcarver   (1001)        4 2022-08-23 03:07:39.000000 ssz-0.3.0/ssz.egg-info/top_level.txt
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:09:44.108898 ssz-0.3.1/
+-rw-r--r--   0 eve        (501) staff       (20)     1095 2023-06-08 21:05:34.000000 ssz-0.3.1/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-06-08 21:05:34.000000 ssz-0.3.1/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     3170 2023-06-08 21:09:44.108731 ssz-0.3.1/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     2214 2023-06-08 21:05:34.000000 ssz-0.3.1/README.md
+-rw-r--r--   0 eve        (501) staff       (20)     1203 2023-06-08 21:05:34.000000 ssz-0.3.1/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-08 21:09:44.108939 ssz-0.3.1/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     2538 2023-06-08 21:09:31.000000 ssz-0.3.1/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:09:44.104486 ssz-0.3.1/ssz/
+-rw-r--r--   0 eve        (501) staff       (20)      674 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3474 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/abc.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:09:44.105583 ssz-0.3.1/ssz/cache/
+-rw-r--r--   0 eve        (501) staff       (20)       42 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/cache/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1363 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/cache/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     1195 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/cache/utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1031 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/codec.py
+-rw-r--r--   0 eve        (501) staff       (20)      564 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      341 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)      374 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/hash.py
+-rw-r--r--   0 eve        (501) staff       (20)    13105 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/hash_tree.py
+-rw-r--r--   0 eve        (501) staff       (20)    12474 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/hashable_container.py
+-rw-r--r--   0 eve        (501) staff       (20)      711 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/hashable_list.py
+-rw-r--r--   0 eve        (501) staff       (20)    14861 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/hashable_structure.py
+-rw-r--r--   0 eve        (501) staff       (20)      849 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/hashable_vector.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:09:44.107790 ssz-0.3.1/ssz/sedes/
+-rw-r--r--   0 eve        (501) staff       (20)     1847 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1936 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     5982 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/basic.py
+-rw-r--r--   0 eve        (501) staff       (20)     3580 2023-06-08 21:05:34.000000 ssz-0.3.1/ssz/sedes/bitlist.py
+-rw-r--r--   0 eve        (501) staff       (20)     2477 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/bitvector.py
+-rw-r--r--   0 eve        (501) staff       (20)     1125 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/boolean.py
+-rw-r--r--   0 eve        (501) staff       (20)      951 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/byte.py
+-rw-r--r--   0 eve        (501) staff       (20)     1900 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/byte_list.py
+-rw-r--r--   0 eve        (501) staff       (20)     2002 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/byte_vector.py
+-rw-r--r--   0 eve        (501) staff       (20)     6580 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/container.py
+-rw-r--r--   0 eve        (501) staff       (20)     6175 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/list.py
+-rw-r--r--   0 eve        (501) staff       (20)    13836 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/serializable.py
+-rw-r--r--   0 eve        (501) staff       (20)     1957 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/signed_serializable.py
+-rw-r--r--   0 eve        (501) staff       (20)     1493 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/uint.py
+-rw-r--r--   0 eve        (501) staff       (20)     5343 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/sedes/vector.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:09:44.108486 ssz-0.3.1/ssz/tools/
+-rw-r--r--   0 eve        (501) staff       (20)      149 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/tools/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      708 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/tools/codec.py
+-rw-r--r--   0 eve        (501) staff       (20)     3822 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/tools/dump.py
+-rw-r--r--   0 eve        (501) staff       (20)     4324 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/tools/parse.py
+-rw-r--r--   0 eve        (501) staff       (20)      300 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/tree_hash.py
+-rw-r--r--   0 eve        (501) staff       (20)      327 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/typing.py
+-rw-r--r--   0 eve        (501) staff       (20)     6691 2023-04-19 17:04:52.000000 ssz-0.3.1/ssz/utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:09:44.105172 ssz-0.3.1/ssz.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     3170 2023-06-08 21:09:43.000000 ssz-0.3.1/ssz.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)      936 2023-06-08 21:09:44.000000 ssz-0.3.1/ssz.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 21:09:43.000000 ssz-0.3.1/ssz.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 21:09:43.000000 ssz-0.3.1/ssz.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)      597 2023-06-08 21:09:43.000000 ssz-0.3.1/ssz.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)        4 2023-06-08 21:09:43.000000 ssz-0.3.1/ssz.egg-info/top_level.txt
```

### Comparing `ssz-0.3.0/LICENSE` & `ssz-0.3.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 The Ethereum Foundation
+Copyright (c) 2018-2023 The Ethereum Foundation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ssz-0.3.0/PKG-INFO` & `ssz-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: ssz
-Version: 0.3.0
+Version: 0.3.1
 Summary: ssz: Python implementation of the Simple Serialization encoding and decoding
 Home-page: https://github.com/ethereum/py-ssz
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: yaml
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
+Provides-Extra: yaml
 License-File: LICENSE
 
 # py-ssz
 
-[![Join the chat at https://gitter.im/ethereum/py-ssz](https://badges.gitter.im/ethereum/py-ssz.svg)](https://gitter.im/ethereum/py-ssz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/py-ssz.svg?style=shield)](https://circleci.com/gh/ethereum/py-ssz)
 [![PyPI version](https://badge.fury.io/py/ssz.svg)](https://badge.fury.io/py/ssz)
 [![Python versions](https://img.shields.io/pypi/pyversions/ssz.svg)](https://pypi.python.org/pypi/ssz)
-[![Docs build](https://readthedocs.org/projects/ssz/badge/?version=latest)](http://ssz.readthedocs.io/en/latest/?badge=latest)
+[![Docs build](https://readthedocs.org/projects/ssz/badge/?version=latest)](https://ssz.readthedocs.io/en/latest/?badge=latest)
+   
 
 
 Python implementation of the Simple Serialization encoding and decoding
 
 Read more in the [documentation on ReadTheDocs](https://ssz.readthedocs.io/). [View the change log](https://ssz.readthedocs.io/en/latest/release_notes.html).
 
 ## Quickstart
@@ -63,51 +62,19 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:ethereum/py-ssz.git
 cd py-ssz
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 ssz/ tests/ -c "clear; flake8 ssz tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on py-ssz failed'" ../tests ../ssz
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ssz-0.3.0/README.md` & `ssz-0.3.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # py-ssz
 
-[![Join the chat at https://gitter.im/ethereum/py-ssz](https://badges.gitter.im/ethereum/py-ssz.svg)](https://gitter.im/ethereum/py-ssz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/py-ssz.svg?style=shield)](https://circleci.com/gh/ethereum/py-ssz)
 [![PyPI version](https://badge.fury.io/py/ssz.svg)](https://badge.fury.io/py/ssz)
 [![Python versions](https://img.shields.io/pypi/pyversions/ssz.svg)](https://pypi.python.org/pypi/ssz)
-[![Docs build](https://readthedocs.org/projects/ssz/badge/?version=latest)](http://ssz.readthedocs.io/en/latest/?badge=latest)
+[![Docs build](https://readthedocs.org/projects/ssz/badge/?version=latest)](https://ssz.readthedocs.io/en/latest/?badge=latest)
+   
 
 
 Python implementation of the Simple Serialization encoding and decoding
 
 Read more in the [documentation on ReadTheDocs](https://ssz.readthedocs.io/). [View the change log](https://ssz.readthedocs.io/en/latest/release_notes.html).
 
 ## Quickstart
@@ -33,51 +34,19 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:ethereum/py-ssz.git
 cd py-ssz
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 ssz/ tests/ -c "clear; flake8 ssz tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on py-ssz failed'" ../tests ../ssz
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ssz-0.3.0/pyproject.toml` & `ssz-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 [tool.towncrier]
-# Read https://github.com/ethereum/py-ssz/newsfragments/README.md for instructions
+# Read https://github.com/ethereum/py-ssz/blob/master/newsfragments/README.md for instructions
 package = "ssz"
 filename = "docs/release_notes.rst"
 directory = "newsfragments"
 underlines = ["-", "~", "^"]
 title_format = "py-ssz v{version} ({project_date})"
 issue_format = "`#{issue} <https://github.com/ethereum/py-ssz/issues/{issue}>`__"
 
 [[tool.towncrier.type]]
-directory = "feature"
-name = "Features"
+directory = "breaking"
+name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "bugfix"
 name = "Bugfixes"
 showcontent = true
 
 [[tool.towncrier.type]]
-directory = "performance"
-name = "Performance improvements"
+directory = "deprecation"
+name = "Deprecations"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "doc"
 name = "Improved Documentation"
 showcontent = true
 
 [[tool.towncrier.type]]
-directory = "removal"
-name = "Deprecations and Removals"
+directory = "feature"
+name = "Features"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "internal"
 name = "Internal Changes - for py-ssz Contributors"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
-name = "Miscellaneous changes"
+name = "Miscellaneous Changes"
 showcontent = false
 
 [[tool.towncrier.type]]
-directory = "breaking"
-name = "Breaking changes"
+directory = "performance"
+name = "Performance Improvements"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "removal"
+name = "Removals"
 showcontent = true
```

### Comparing `ssz-0.3.0/setup.py` & `ssz-0.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [
-        "pytest>=6.2.5,<7",
-        "pytest-xdist>=2.4.0,<3",
-        "tox==3.14.6",
+        "pytest>=7.0.0",
+        "pytest-xdist>=2.4.0",
         "hypothesis==4.54.0",
-        "mypy-extensions>=0.4.1,<1.0.0",
-    ],
-    "yaml": [
-        "ruamel.yaml==0.15.87",
+        "mypy-extensions>=0.4.1",
     ],
     "lint": [
-        "black>=22.6.0,<23",
         "flake8==3.7.9",
         "isort>=5.10.1,<6",
-        "pydocstyle>=5.0.0,<6",
+        "pydocstyle>=6.0.0",
+        "black>=23",
     ],
     "doc": [
-        "Sphinx>=1.6.5,<2",
-        "sphinx_rtd_theme>=0.1.9,<1",
-        "Jinja2<3",
-        "MarkupSafe<2",
+        "sphinx>=5.0.0",
+        "sphinx_rtd_theme>=1.0.0",
         "towncrier>=21,<22",
     ],
     "dev": [
-        "bumpversion>=0.5.3,<1",
+        "bumpversion>=0.5.3",
+        "pytest-watch>=4.1.0",
+        "tox>=4.0.0",
+        "build>=0.9.0",
         "wheel",
         "twine",
         "ipython",
-        "pre-commit==1.18.3",
-        "pytest-watch>=4.1.0,<5",
+    ],
+    "yaml": [
+        "ruamel.yaml>=0.17.0",
     ],
 }
 
 extras_require["dev"] = (
     extras_require["dev"]
     + extras_require["test"]
     + extras_require["lint"]
@@ -47,24 +45,24 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="ssz",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="0.3.0",
+    version="0.3.1",
     description="""ssz: Python implementation of the Simple Serialization encoding and decoding""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/py-ssz",
     include_package_data=True,
     install_requires=[
-        "eth-utils>=1,<2",
+        "eth-utils>=2",
         "lru-dict>=1.1.6",
         # When updating to a newer version of pyrsistent, please check that the interface
         # `transform` expects has not changed (see https://github.com/tobgu/pyrsistent/issues/180)
         "pyrsistent>=0.16.0,<0.17",
     ],
     setup_requires=[],
     python_requires=">=3.7, <4",
@@ -76,17 +74,15 @@
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ssz": ["py.typed"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
-        "Operating System :: MacOS",
-        "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: Implementation :: PyPy",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ssz-0.3.0/ssz/__init__.py` & `ssz-0.3.1/ssz/__init__.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/abc.py` & `ssz-0.3.1/ssz/abc.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/cache/cache.py` & `ssz-0.3.1/ssz/cache/cache.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/cache/utils.py` & `ssz-0.3.1/ssz/cache/utils.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/codec.py` & `ssz-0.3.1/ssz/codec.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/constants.py` & `ssz-0.3.1/ssz/constants.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/hash_tree.py` & `ssz-0.3.1/ssz/hash_tree.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/hashable_container.py` & `ssz-0.3.1/ssz/hashable_container.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/hashable_list.py` & `ssz-0.3.1/ssz/hashable_list.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/hashable_structure.py` & `ssz-0.3.1/ssz/hashable_structure.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/hashable_vector.py` & `ssz-0.3.1/ssz/hashable_vector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/__init__.py` & `ssz-0.3.1/ssz/sedes/__init__.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/base.py` & `ssz-0.3.1/ssz/sedes/base.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/basic.py` & `ssz-0.3.1/ssz/sedes/basic.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/bitlist.py` & `ssz-0.3.1/ssz/sedes/bitlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         return bytes(serialized_bytearray)
 
     #
     # Deserialization
     #
     @to_tuple
     def deserialize(self, data: bytes) -> Tuple[bool, ...]:
-
         # Length of data should be larger than 1
         if len(data) < 1:
             raise DeserializationError(
                 f"Cannot deserialize empty bytes string as Bitlist[{self.max_bit_count}] "
             )
 
         #   Last byte in bytes should be >= 1, if not data is not a serialised bitlist.
```

### Comparing `ssz-0.3.0/ssz/sedes/bitvector.py` & `ssz-0.3.1/ssz/sedes/bitvector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/boolean.py` & `ssz-0.3.1/ssz/sedes/boolean.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/byte.py` & `ssz-0.3.1/ssz/sedes/byte.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/byte_list.py` & `ssz-0.3.1/ssz/sedes/byte_list.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/byte_vector.py` & `ssz-0.3.1/ssz/sedes/byte_vector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/container.py` & `ssz-0.3.1/ssz/sedes/container.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/list.py` & `ssz-0.3.1/ssz/sedes/list.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/serializable.py` & `ssz-0.3.1/ssz/sedes/serializable.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/signed_serializable.py` & `ssz-0.3.1/ssz/sedes/signed_serializable.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/uint.py` & `ssz-0.3.1/ssz/sedes/uint.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/sedes/vector.py` & `ssz-0.3.1/ssz/sedes/vector.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/tools/codec.py` & `ssz-0.3.1/ssz/tools/codec.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/tools/dump.py` & `ssz-0.3.1/ssz/tools/dump.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/tools/parse.py` & `ssz-0.3.1/ssz/tools/parse.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz/utils.py` & `ssz-0.3.1/ssz/utils.py`

 * *Files identical despite different names*

### Comparing `ssz-0.3.0/ssz.egg-info/PKG-INFO` & `ssz-0.3.1/ssz.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: ssz
-Version: 0.3.0
+Version: 0.3.1
 Summary: ssz: Python implementation of the Simple Serialization encoding and decoding
 Home-page: https://github.com/ethereum/py-ssz
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: yaml
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
+Provides-Extra: yaml
 License-File: LICENSE
 
 # py-ssz
 
-[![Join the chat at https://gitter.im/ethereum/py-ssz](https://badges.gitter.im/ethereum/py-ssz.svg)](https://gitter.im/ethereum/py-ssz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/py-ssz.svg?style=shield)](https://circleci.com/gh/ethereum/py-ssz)
 [![PyPI version](https://badge.fury.io/py/ssz.svg)](https://badge.fury.io/py/ssz)
 [![Python versions](https://img.shields.io/pypi/pyversions/ssz.svg)](https://pypi.python.org/pypi/ssz)
-[![Docs build](https://readthedocs.org/projects/ssz/badge/?version=latest)](http://ssz.readthedocs.io/en/latest/?badge=latest)
+[![Docs build](https://readthedocs.org/projects/ssz/badge/?version=latest)](https://ssz.readthedocs.io/en/latest/?badge=latest)
+   
 
 
 Python implementation of the Simple Serialization encoding and decoding
 
 Read more in the [documentation on ReadTheDocs](https://ssz.readthedocs.io/). [View the change log](https://ssz.readthedocs.io/en/latest/release_notes.html).
 
 ## Quickstart
@@ -63,51 +62,19 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:ethereum/py-ssz.git
 cd py-ssz
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 ssz/ tests/ -c "clear; flake8 ssz tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on py-ssz failed'" ../tests ../ssz
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ssz-0.3.0/ssz.egg-info/SOURCES.txt` & `ssz-0.3.1/ssz.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements-docs.txt
 setup.py
-.tox/lint/lib/python3.8/site-packages/pyrsistent/__init__.pyi
-.tox/lint/lib/python3.8/site-packages/pyrsistent/typing.pyi
 ssz/__init__.py
 ssz/abc.py
 ssz/codec.py
 ssz/constants.py
 ssz/exceptions.py
 ssz/hash.py
 ssz/hash_tree.py
```

