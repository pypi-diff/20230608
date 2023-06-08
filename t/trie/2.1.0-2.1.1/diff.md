# Comparing `tmp/trie-2.1.0.tar.gz` & `tmp/trie-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trie-2.1.0.tar", last modified: Fri Dec  9 21:31:19 2022, max compression
+gzip compressed data, was "trie-2.1.1.tar", last modified: Thu Jun  8 21:03:51 2023, max compression
```

## Comparing `trie-2.1.0.tar` & `trie-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,50 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-09 21:31:19.511567 trie-2.1.0/
--rw-r--r--   0 eve        (501) staff       (20)     1090 2022-12-07 19:02:40.000000 trie-2.1.0/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      171 2022-12-09 20:33:42.000000 trie-2.1.0/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)    17486 2022-12-09 21:31:19.511421 trie-2.1.0/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)    16415 2022-12-07 19:02:43.000000 trie-2.1.0/README.md
--rw-r--r--   0 eve        (501) staff       (20)       38 2022-12-09 21:31:19.511597 trie-2.1.0/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     2304 2022-12-09 21:30:24.000000 trie-2.1.0/setup.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-09 21:31:19.510105 trie-2.1.0/trie/
--rw-r--r--   0 eve        (501) staff       (20)      174 2022-12-07 19:02:48.000000 trie-2.1.0/trie/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    12812 2022-12-08 22:22:28.000000 trie-2.1.0/trie/binary.py
--rw-r--r--   0 eve        (501) staff       (20)     5609 2022-12-08 22:22:28.000000 trie-2.1.0/trie/branches.py
--rw-r--r--   0 eve        (501) staff       (20)      889 2022-12-07 19:02:43.000000 trie-2.1.0/trie/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     9413 2022-12-08 22:22:28.000000 trie-2.1.0/trie/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    13169 2022-12-08 22:22:28.000000 trie-2.1.0/trie/fog.py
--rw-r--r--   0 eve        (501) staff       (20)    29576 2022-12-08 22:22:28.000000 trie-2.1.0/trie/hexary.py
--rw-r--r--   0 eve        (501) staff       (20)     7229 2022-12-08 22:22:28.000000 trie-2.1.0/trie/iter.py
--rw-r--r--   0 eve        (501) staff       (20)    12522 2022-12-08 22:22:28.000000 trie-2.1.0/trie/smt.py
--rw-r--r--   0 eve        (501) staff       (20)     4626 2022-12-08 22:22:28.000000 trie-2.1.0/trie/typing.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-09 21:31:19.511146 trie-2.1.0/trie/utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 19:02:43.000000 trie-2.1.0/trie/utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1504 2022-12-08 22:22:28.000000 trie-2.1.0/trie/utils/binaries.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-09 21:31:19.511254 trie-2.1.0/trie/utils/compat/
--rw-r--r--   0 eve        (501) staff       (20)      246 2022-12-08 22:22:28.000000 trie-2.1.0/trie/utils/compat/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2224 2022-12-08 22:22:28.000000 trie-2.1.0/trie/utils/db.py
--rw-r--r--   0 eve        (501) staff       (20)     2666 2022-12-08 22:22:28.000000 trie-2.1.0/trie/utils/nibbles.py
--rw-r--r--   0 eve        (501) staff       (20)     6463 2022-12-08 22:22:28.000000 trie-2.1.0/trie/utils/nodes.py
--rw-r--r--   0 eve        (501) staff       (20)     1409 2022-12-08 22:22:28.000000 trie-2.1.0/trie/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-09 21:31:19.510675 trie-2.1.0/trie.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)    17486 2022-12-09 21:31:19.000000 trie-2.1.0/trie.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)      511 2022-12-09 21:31:19.000000 trie-2.1.0/trie.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-12-09 21:31:19.000000 trie-2.1.0/trie.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-12-09 21:31:19.000000 trie-2.1.0/trie.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)      479 2022-12-09 21:31:19.000000 trie-2.1.0/trie.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)        5 2022-12-09 21:31:19.000000 trie-2.1.0/trie.egg-info/top_level.txt
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:03:51.640249 trie-2.1.1/
+-rw-r--r--   0 eve        (501) staff       (20)     1095 2023-06-08 20:58:09.000000 trie-2.1.1/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-06-08 20:58:09.000000 trie-2.1.1/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)    18099 2023-06-08 21:03:51.640037 trie-2.1.1/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)    17147 2023-06-08 20:58:09.000000 trie-2.1.1/README.md
+-rw-r--r--   0 eve        (501) staff       (20)     1196 2023-06-08 20:58:09.000000 trie-2.1.1/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-08 21:03:51.640286 trie-2.1.1/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     2478 2023-06-08 21:03:46.000000 trie-2.1.1/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:03:51.636377 trie-2.1.1/tests/
+-rw-r--r--   0 eve        (501) staff       (20)     4459 2023-06-08 20:58:09.000000 trie-2.1.1/tests/test_bin_trie.py
+-rw-r--r--   0 eve        (501) staff       (20)      692 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_binaries_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     8734 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_branches_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1101 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     6470 2023-06-08 20:58:09.000000 trie-2.1.1/tests/test_exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)     8211 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_fog.py
+-rw-r--r--   0 eve        (501) staff       (20)    35901 2023-06-08 20:58:09.000000 trie-2.1.1/tests/test_hexary_trie.py
+-rw-r--r--   0 eve        (501) staff       (20)    21187 2023-06-08 20:58:09.000000 trie-2.1.1/tests/test_hexary_trie_walk.py
+-rw-r--r--   0 eve        (501) staff       (20)     4889 2023-06-08 20:58:09.000000 trie-2.1.1/tests/test_iter.py
+-rw-r--r--   0 eve        (501) staff       (20)      352 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_nibbles_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     6687 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_nodes_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1310 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_proof.py
+-rw-r--r--   0 eve        (501) staff       (20)     2199 2023-06-08 20:58:09.000000 trie-2.1.1/tests/test_smt.py
+-rw-r--r--   0 eve        (501) staff       (20)     1705 2022-12-08 22:22:28.000000 trie-2.1.1/tests/test_typing.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:03:51.638454 trie-2.1.1/trie/
+-rw-r--r--   0 eve        (501) staff       (20)      174 2022-12-07 19:02:48.000000 trie-2.1.1/trie/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    12812 2022-12-08 22:22:28.000000 trie-2.1.1/trie/binary.py
+-rw-r--r--   0 eve        (501) staff       (20)     5609 2022-12-08 22:22:28.000000 trie-2.1.1/trie/branches.py
+-rw-r--r--   0 eve        (501) staff       (20)      889 2022-12-07 19:02:43.000000 trie-2.1.1/trie/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     9411 2023-06-08 20:58:09.000000 trie-2.1.1/trie/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    13168 2023-06-08 20:58:09.000000 trie-2.1.1/trie/fog.py
+-rw-r--r--   0 eve        (501) staff       (20)    29582 2023-06-08 20:58:09.000000 trie-2.1.1/trie/hexary.py
+-rw-r--r--   0 eve        (501) staff       (20)     7229 2022-12-08 22:22:28.000000 trie-2.1.1/trie/iter.py
+-rw-r--r--   0 eve        (501) staff       (20)    12522 2022-12-08 22:22:28.000000 trie-2.1.1/trie/smt.py
+-rw-r--r--   0 eve        (501) staff       (20)     4626 2022-12-08 22:22:28.000000 trie-2.1.1/trie/typing.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:03:51.639648 trie-2.1.1/trie/utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 19:02:43.000000 trie-2.1.1/trie/utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1504 2022-12-08 22:22:28.000000 trie-2.1.1/trie/utils/binaries.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:03:51.639774 trie-2.1.1/trie/utils/compat/
+-rw-r--r--   0 eve        (501) staff       (20)      246 2022-12-08 22:22:28.000000 trie-2.1.1/trie/utils/compat/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2224 2022-12-08 22:22:28.000000 trie-2.1.1/trie/utils/db.py
+-rw-r--r--   0 eve        (501) staff       (20)     2666 2022-12-08 22:22:28.000000 trie-2.1.1/trie/utils/nibbles.py
+-rw-r--r--   0 eve        (501) staff       (20)     6463 2022-12-08 22:22:28.000000 trie-2.1.1/trie/utils/nodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1326 2023-06-08 20:58:09.000000 trie-2.1.1/trie/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 21:03:51.639100 trie-2.1.1/trie.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)    18099 2023-06-08 21:03:51.000000 trie-2.1.1/trie.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)      863 2023-06-08 21:03:51.000000 trie-2.1.1/trie.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 21:03:51.000000 trie-2.1.1/trie.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 21:03:50.000000 trie-2.1.1/trie.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)      562 2023-06-08 21:03:51.000000 trie-2.1.1/trie.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)        5 2023-06-08 21:03:51.000000 trie-2.1.1/trie.egg-info/top_level.txt
```

### Comparing `trie-2.1.0/LICENSE` & `trie-2.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 The Ethereum Foundation
+Copyright (c) 2017-2023 The Ethereum Foundation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `trie-2.1.0/PKG-INFO` & `trie-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 Metadata-Version: 2.1
 Name: trie
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python implementation of the Ethereum Trie structure
 Home-page: https://github.com/ethereum/py-trie
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum blockchain evm trie merkle
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python Implementation of the Ethereum Trie structure
 
-[![PyPI](https://img.shields.io/pypi/v/trie.svg)](https://pypi.org/project/trie/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/trie.svg)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
+[![Build Status](https://circleci.com/gh/ethereum/py-trie.svg?style=shield)](https://circleci.com/gh/ethereum/py-trie)
+[![PyPI version](https://badge.fury.io/py/trie.svg)](https://badge.fury.io/py/trie)
+[![Python versions](https://img.shields.io/pypi/pyversions/trie.svg)](https://pypi.python.org/pypi/trie)
 
 > This library and repository was previously located at [pipermerriam/py-trie](https://github.com/pipermerriam/py-trie). It was transferred to the Ethereum foundation GitHub in
 > November 2017 and renamed to `py-trie`.
 
 ## Installation
 
 ```sh
-pip install trie
+python -m pip install trie
 ```
 
-## Development
+## Developer Setup
 
-```sh
-pip install -e .[dev]
-```
+If you would like to hack on py-trie, please check out the [Snake Charmers
+Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+for information on how we do:
 
-### Running the tests
+- Testing
+- Pull Requests
+- Code Style
+- Documentation
 
-You can run the tests with:
+### Development Environment Setup
+
+You can set up your dev environment with:
 
 ```sh
-pytest tests
+git clone git@github.com:ethereum/py-trie.git
+cd py-trie
+virtualenv -p python3 venv
+. venv/bin/activate
+python -m pip install -e ".[dev]"
 ```
 
-Or you can install `tox` to run the full test suite.
-
-### Releasing
-
-Pandoc is required for transforming the markdown README to the proper format to
-render correctly on pypi.
+## Running the tests
 
-For Debian-like systems:
+You can run the tests with:
 
 ```sh
-apt install pandoc
+git submodule update --init --recursive
+pytest tests
 ```
 
-Or on OSX:
-
-```sh
-brew install pandoc
-```
+### Release setup
 
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
-To issue the next version in line, use bumpversion and specify which part to bump,
-like `bumpversion minor` or `bumpversion devnum`.
+To issue the next version in line, specify which part to bump,
+like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
+master branch, except when releasing a beta (in which case the beta is released from master,
+and the previous stable branch is released from said branch).
 
 If you are in a beta version, `bumpversion stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `bumpversion --new-version 4.0.0-alpha.1 devnum`
 
 ## Usage
@@ -384,9 +386,7 @@
 >>> # get_witness_for_key_prefix function
 >>> get_witness_for_key_prefix(t.db, t.root_hash, b'key1') # equivalent to `get_branch(t.db, t.root_hash, b'key1')`
 (b'\x00\x82\x1a\xd9^L|38J\xed\xf31S\xb2\x97A\x8dy\x91RJ\x92\xf5ZC\xb4\x99T&;!\x9f\xa9!\xa2\xfe;', b"\x01*\xaccxH\x89\x08}\x93|\xda\xb9\r\x9b\x82\x8b\xb2Y\xbc\x10\xb9\x88\xf40\xef\xed\x8b'\x13\xbc\xa5\xccYGb\xc2\x8db\x88lPs@)\x86v\xd7B\xf7\xd3X\x93\xc9\xf0\xfd\xae\xe0`j#\x0b\xca;\xf8", b'\x00\x11\x8aEL3\x839E\xbd\xc4G\xd1xj\x0fxWu\xcb\xf6\xf3\xf2\x8e7!M\xca\x1c/\xd7\x7f\xed\xc6', b'\x02value1')
 >>> get_witness_for_key_prefix(t.db, t.root_hash, b'key') # this will include additional nodes of b'key2'
 (b'\x00\x82\x1a\xd9^L|38J\xed\xf31S\xb2\x97A\x8dy\x91RJ\x92\xf5ZC\xb4\x99T&;!\x9f\xa9!\xa2\xfe;', b"\x01*\xaccxH\x89\x08}\x93|\xda\xb9\r\x9b\x82\x8b\xb2Y\xbc\x10\xb9\x88\xf40\xef\xed\x8b'\x13\xbc\xa5\xccYGb\xc2\x8db\x88lPs@)\x86v\xd7B\xf7\xd3X\x93\xc9\xf0\xfd\xae\xe0`j#\x0b\xca;\xf8", b'\x00\x11\x8aEL3\x839E\xbd\xc4G\xd1xj\x0fxWu\xcb\xf6\xf3\xf2\x8e7!M\xca\x1c/\xd7\x7f\xed\xc6', b'\x02value1', b'\x00\x10O\xa9\x0b\x1c!_`<\xb5^\x98D\x89\x17\x148\xac\xda&\xb3P\xf6\x06[\x1b9\xc09\xbas\x85\xf5', b'\x02value2')
 >>> get_witness_for_key_prefix(t.db, t.root_hash, b'') # this will return the whole trie
 ```
-
-
```

### Comparing `trie-2.1.0/README.md` & `trie-2.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 # Python Implementation of the Ethereum Trie structure
 
-[![PyPI](https://img.shields.io/pypi/v/trie.svg)](https://pypi.org/project/trie/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/trie.svg)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
+[![Build Status](https://circleci.com/gh/ethereum/py-trie.svg?style=shield)](https://circleci.com/gh/ethereum/py-trie)
+[![PyPI version](https://badge.fury.io/py/trie.svg)](https://badge.fury.io/py/trie)
+[![Python versions](https://img.shields.io/pypi/pyversions/trie.svg)](https://pypi.python.org/pypi/trie)
 
 > This library and repository was previously located at [pipermerriam/py-trie](https://github.com/pipermerriam/py-trie). It was transferred to the Ethereum foundation GitHub in
 > November 2017 and renamed to `py-trie`.
 
 ## Installation
 
 ```sh
-pip install trie
+python -m pip install trie
 ```
 
-## Development
+## Developer Setup
 
-```sh
-pip install -e .[dev]
-```
+If you would like to hack on py-trie, please check out the [Snake Charmers
+Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+for information on how we do:
 
-### Running the tests
+- Testing
+- Pull Requests
+- Code Style
+- Documentation
 
-You can run the tests with:
+### Development Environment Setup
+
+You can set up your dev environment with:
 
 ```sh
-pytest tests
+git clone git@github.com:ethereum/py-trie.git
+cd py-trie
+virtualenv -p python3 venv
+. venv/bin/activate
+python -m pip install -e ".[dev]"
 ```
 
-Or you can install `tox` to run the full test suite.
-
-### Releasing
+## Running the tests
 
-Pandoc is required for transforming the markdown README to the proper format to
-render correctly on pypi.
-
-For Debian-like systems:
+You can run the tests with:
 
 ```sh
-apt install pandoc
+git submodule update --init --recursive
+pytest tests
 ```
 
-Or on OSX:
-
-```sh
-brew install pandoc
-```
+### Release setup
 
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
-To issue the next version in line, use bumpversion and specify which part to bump,
-like `bumpversion minor` or `bumpversion devnum`.
+To issue the next version in line, specify which part to bump,
+like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
+master branch, except when releasing a beta (in which case the beta is released from master,
+and the previous stable branch is released from said branch).
 
 If you are in a beta version, `bumpversion stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `bumpversion --new-version 4.0.0-alpha.1 devnum`
 
 ## Usage
```

### Comparing `trie-2.1.0/setup.py` & `trie-2.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,82 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 
 extras_require = {
     "test": [
+        "pytest>=7.0.0",
+        "pytest-xdist>=2.4.0",
         "hypothesis>=6.56.4,<7",
         "pycryptodome",
-        "pytest-xdist>=2.4.0,<3",
-        "tox==3.14.6",
-        "pytest>=6.2.5",
     ],
     "lint": [
-        "black>=22",
-        "flake8==5.0.4",
+        "flake8==6.0.0",  # flake8 claims semver but adds new warnings at minor releases, leave it pinned.
+        "flake8-bugbear==23.3.23",  # flake8-bugbear does not follow semver, leave it pinned.
         "isort>=5.10.1",
+        "black>=23",
+    ],
+    "docs": [
+        "towncrier>=21,<22",
     ],
     "dev": [
-        "bumpversion>=0.5.3,<1",
+        "bumpversion>=0.5.3",
+        "pytest-watch>=4.1.0",
+        "tox>=4.0.0",
+        "build>=0.9.0",
         "wheel",
         "twine",
         "eth-hash>=0.1.0,<1.0.0",
     ],
 }
 
 extras_require["dev"] = (
-    extras_require["dev"] + extras_require["test"] + extras_require["lint"]
+    extras_require["dev"]
+    + extras_require["test"]
+    + extras_require["lint"]
+    + extras_require["docs"]
 )
 
 with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="trie",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="2.1.0",
+    version="2.1.1",
     description="""Python implementation of the Ethereum Trie structure""",
     long_description_markdown_filename="README.md",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/py-trie",
     include_package_data=True,
     py_modules=["trie"],
     python_requires=">=3.7,<4",
     install_requires=[
-        "eth-hash>=0.1.0,<1.0.0",
-        "eth-utils>=2.0.0,<3.0.0",
+        "eth-hash>=0.1.0",
+        "eth-utils>=2.0.0",
         "hexbytes>=0.2.0",
-        "rlp>=3,<4",
-        "sortedcontainers>=2.1.0,<3",
+        "rlp>=3",
+        "sortedcontainers>=2.1.0",
         "typing-extensions>=4.0.0,<5; python_version < '3.8'",
     ],
     extras_require=extras_require,
     license="MIT",
     zip_safe=False,
     keywords="ethereum blockchain evm trie merkle",
     packages=find_packages(exclude=["tests", "tests.*"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
-        "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Topic :: Software Development",
-        "Topic :: Utilities",
     ],
 )
```

### Comparing `trie-2.1.0/trie/binary.py` & `trie-2.1.1/trie/binary.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/branches.py` & `trie-2.1.1/trie/branches.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/constants.py` & `trie-2.1.1/trie/constants.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/exceptions.py` & `trie-2.1.1/trie/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         self,
         missing_node_hash: Hash32,
         root_hash: Hash32,
         requested_key: bytes,
         prefix: Nibbles = None,
         *args,
     ):
-
         if not isinstance(missing_node_hash, bytes):
             raise TypeError(
                 "Missing node hash must be bytes, was: %r" % missing_node_hash
             )
         elif not isinstance(root_hash, bytes):
             raise TypeError("Root hash must be bytes, was: %r" % root_hash)
         elif not isinstance(requested_key, bytes):
@@ -179,15 +178,14 @@
     def __init__(
         self,
         nibbles_traversed: NibblesInput,
         node: HexaryTrieNode,
         untraversed_tail: NibblesInput,
         *args,
     ) -> None:
-
         super().__init__(
             Nibbles(nibbles_traversed),
             node,
             Nibbles(untraversed_tail),
             *args,
         )
         self._simulated_node = self._make_simulated_node()
```

### Comparing `trie-2.1.0/trie/fog.py` & `trie-2.1.1/trie/fog.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,14 @@
 
     def add(
         self,
         node_prefix_input: NibblesInput,
         trie_node: HexaryTrieNode,
         sub_segments: Sequence[NibblesInput],
     ) -> None:
-
         """
         Add a new cached node body for each of the sub segments supplied. Later cache
         lookups will be in the form of get(node_prefix + sub_segments[0]).
 
         :param node_prefix: the path from the root to the cached node
         :param trie_node: the body to cache
         :param sub_segments: all of the children of the parent which should be made
```

### Comparing `trie-2.1.0/trie/hexary.py` & `trie-2.1.1/trie/hexary.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
             trie._set_raw_node(node)
 
         with trie.at_root(root_hash) as proven_snapshot:
             try:
                 return proven_snapshot.get(key)
             except MissingTrieNode as e:
                 raise BadTrieProof(
-                    "Missing proof node with hash {}".format(e.missing_node_hash)
+                    f"Missing proof node with hash {e.missing_node_hash}"
                 )
 
     def get_proof(self, key):
         validate_is_bytes(key)
 
         node = self.get_node(self.root_hash)
         trie_key = bytes_to_nibbles(key)
@@ -618,15 +618,15 @@
             # inserted recently, so this hack allows us to use an LRU-cached
             # implementation of _node_to_db_mapping(), which improves the performance of
             # _prune_node() significantly.
             return self._cached_create_node_to_db_mapping(tuplify(node))
         else:
             return self._create_node_to_db_mapping(node)
 
-    @functools.lru_cache(4096)
+    @functools.lru_cache(4096)  # noqa: B019
     def _cached_create_node_to_db_mapping(self, node):
         if isinstance(node, tuple):
             node = listify(node)
         return self._create_node_to_db_mapping(node)
 
     def _create_node_to_db_mapping(self, node):
         validate_is_node(node)
```

### Comparing `trie-2.1.0/trie/iter.py` & `trie-2.1.1/trie/iter.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/smt.py` & `trie-2.1.1/trie/smt.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/typing.py` & `trie-2.1.1/trie/typing.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/utils/binaries.py` & `trie-2.1.1/trie/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/utils/db.py` & `trie-2.1.1/trie/utils/db.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/utils/nibbles.py` & `trie-2.1.1/trie/utils/nibbles.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/utils/nodes.py` & `trie-2.1.1/trie/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `trie-2.1.0/trie/validation.py` & `trie-2.1.1/trie/validation.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,24 +6,20 @@
 from trie.exceptions import (
     ValidationError,
 )
 
 
 def validate_is_bytes(value):
     if not isinstance(value, bytes):
-        raise ValidationError(
-            "Value is not of type `bytes`: got '{0}'".format(type(value))
-        )
+        raise ValidationError(f"Value is not of type `bytes`: got '{type(value)}'")
 
 
 def validate_length(value, length):
     if len(value) != length:
-        raise ValidationError(
-            "Value is of length {0}.  Must be {1}".format(len(value), length)
-        )
+        raise ValidationError(f"Value is of length {len(value)}.  Must be {length}")
 
 
 def validate_is_node(node):
     if node == BLANK_NODE:
         return
     elif len(node) == 2:
         key, value = node
@@ -39,15 +35,15 @@
                 continue
             elif isinstance(sub_node, list):
                 validate_is_node(sub_node)
             else:
                 validate_is_bytes(sub_node)
                 validate_length(sub_node, 32)
     else:
-        raise ValidationError("Invalid Node: {0}".format(node))
+        raise ValidationError(f"Invalid Node: {node}")
 
 
 def validate_is_bin_node(node):
     if node == BLANK_HASH or node[0] in BINARY_TRIE_NODE_TYPES:
         return
     else:
-        raise ValidationError("Invalid Node: {0}".format(node))
+        raise ValidationError(f"Invalid Node: {node}")
```

### Comparing `trie-2.1.0/trie.egg-info/PKG-INFO` & `trie-2.1.1/trie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 Metadata-Version: 2.1
 Name: trie
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python implementation of the Ethereum Trie structure
 Home-page: https://github.com/ethereum/py-trie
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum blockchain evm trie merkle
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python Implementation of the Ethereum Trie structure
 
-[![PyPI](https://img.shields.io/pypi/v/trie.svg)](https://pypi.org/project/trie/)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/trie.svg)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
+[![Build Status](https://circleci.com/gh/ethereum/py-trie.svg?style=shield)](https://circleci.com/gh/ethereum/py-trie)
+[![PyPI version](https://badge.fury.io/py/trie.svg)](https://badge.fury.io/py/trie)
+[![Python versions](https://img.shields.io/pypi/pyversions/trie.svg)](https://pypi.python.org/pypi/trie)
 
 > This library and repository was previously located at [pipermerriam/py-trie](https://github.com/pipermerriam/py-trie). It was transferred to the Ethereum foundation GitHub in
 > November 2017 and renamed to `py-trie`.
 
 ## Installation
 
 ```sh
-pip install trie
+python -m pip install trie
 ```
 
-## Development
+## Developer Setup
 
-```sh
-pip install -e .[dev]
-```
+If you would like to hack on py-trie, please check out the [Snake Charmers
+Tactical Manual](https://github.com/ethereum/snake-charmers-tactical-manual)
+for information on how we do:
 
-### Running the tests
+- Testing
+- Pull Requests
+- Code Style
+- Documentation
 
-You can run the tests with:
+### Development Environment Setup
+
+You can set up your dev environment with:
 
 ```sh
-pytest tests
+git clone git@github.com:ethereum/py-trie.git
+cd py-trie
+virtualenv -p python3 venv
+. venv/bin/activate
+python -m pip install -e ".[dev]"
 ```
 
-Or you can install `tox` to run the full test suite.
-
-### Releasing
-
-Pandoc is required for transforming the markdown README to the proper format to
-render correctly on pypi.
+## Running the tests
 
-For Debian-like systems:
+You can run the tests with:
 
 ```sh
-apt install pandoc
+git submodule update --init --recursive
+pytest tests
 ```
 
-Or on OSX:
-
-```sh
-brew install pandoc
-```
+### Release setup
 
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
-To issue the next version in line, use bumpversion and specify which part to bump,
-like `bumpversion minor` or `bumpversion devnum`.
+To issue the next version in line, specify which part to bump,
+like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
+master branch, except when releasing a beta (in which case the beta is released from master,
+and the previous stable branch is released from said branch).
 
 If you are in a beta version, `bumpversion stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `bumpversion --new-version 4.0.0-alpha.1 devnum`
 
 ## Usage
@@ -384,9 +386,7 @@
 >>> # get_witness_for_key_prefix function
 >>> get_witness_for_key_prefix(t.db, t.root_hash, b'key1') # equivalent to `get_branch(t.db, t.root_hash, b'key1')`
 (b'\x00\x82\x1a\xd9^L|38J\xed\xf31S\xb2\x97A\x8dy\x91RJ\x92\xf5ZC\xb4\x99T&;!\x9f\xa9!\xa2\xfe;', b"\x01*\xaccxH\x89\x08}\x93|\xda\xb9\r\x9b\x82\x8b\xb2Y\xbc\x10\xb9\x88\xf40\xef\xed\x8b'\x13\xbc\xa5\xccYGb\xc2\x8db\x88lPs@)\x86v\xd7B\xf7\xd3X\x93\xc9\xf0\xfd\xae\xe0`j#\x0b\xca;\xf8", b'\x00\x11\x8aEL3\x839E\xbd\xc4G\xd1xj\x0fxWu\xcb\xf6\xf3\xf2\x8e7!M\xca\x1c/\xd7\x7f\xed\xc6', b'\x02value1')
 >>> get_witness_for_key_prefix(t.db, t.root_hash, b'key') # this will include additional nodes of b'key2'
 (b'\x00\x82\x1a\xd9^L|38J\xed\xf31S\xb2\x97A\x8dy\x91RJ\x92\xf5ZC\xb4\x99T&;!\x9f\xa9!\xa2\xfe;', b"\x01*\xaccxH\x89\x08}\x93|\xda\xb9\r\x9b\x82\x8b\xb2Y\xbc\x10\xb9\x88\xf40\xef\xed\x8b'\x13\xbc\xa5\xccYGb\xc2\x8db\x88lPs@)\x86v\xd7B\xf7\xd3X\x93\xc9\xf0\xfd\xae\xe0`j#\x0b\xca;\xf8", b'\x00\x11\x8aEL3\x839E\xbd\xc4G\xd1xj\x0fxWu\xcb\xf6\xf3\xf2\x8e7!M\xca\x1c/\xd7\x7f\xed\xc6', b'\x02value1', b'\x00\x10O\xa9\x0b\x1c!_`<\xb5^\x98D\x89\x17\x148\xac\xda&\xb3P\xf6\x06[\x1b9\xc09\xbas\x85\xf5', b'\x02value2')
 >>> get_witness_for_key_prefix(t.db, t.root_hash, b'') # this will return the whole trie
 ```
-
-
```

