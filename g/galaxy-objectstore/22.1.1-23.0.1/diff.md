# Comparing `tmp/galaxy-objectstore-22.1.1.tar.gz` & `tmp/galaxy-objectstore-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-objectstore-22.1.1.tar", last modified: Mon Aug 22 19:45:55 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/objectstore/dist/.tmp-jdkak610/galaxy-objectstore-23.0.1.tar", last modified: Thu Jun  8 17:40:15 2023, max compression
```

## Comparing `galaxy-objectstore-22.1.1.tar` & `galaxy-objectstore-23.0.1.tar`

### file list

```diff
@@ -1,47 +1,30 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.613267 galaxy-objectstore-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      540 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-objectstore-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       29 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1921 2022-08-22 19:45:55.613406 galaxy-objectstore-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      341 2022-03-24 19:47:11.000000 galaxy-objectstore-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.606237 galaxy-objectstore-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.608625 galaxy-objectstore-22.1.1/galaxy/objectstore/
--rw-r--r--   0 mvandenb   (501) staff       (20)    46619 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    25344 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/azure_blob.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    32651 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/cloud.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    28374 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/irods.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    16936 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/pithos.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3021 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/pulsar.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33209 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/s3.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2910 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/s3_multipart_upload.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.608876 galaxy-objectstore-22.1.1/galaxy/objectstore/unittest_utils/
--rw-r--r--   0 mvandenb   (501) staff       (20)     2680 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/galaxy/objectstore/unittest_utils/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      440 2022-08-22 19:45:29.000000 galaxy-objectstore-22.1.1/galaxy/project_galaxy_objectstore.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.610587 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1921 2022-08-22 19:45:54.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1135 2022-08-22 19:45:55.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:54.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:45:54.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:54.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       19 2022-08-22 19:45:54.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:54.000000 galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       19 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.611318 galaxy-objectstore-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:55.619773 galaxy-objectstore-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2717 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-objectstore-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.611570 galaxy-objectstore-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-objectstore-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:55.612979 galaxy-objectstore-22.1.1/tests/objectstore/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:14.000000 galaxy-objectstore-22.1.1/tests/objectstore/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      440 2022-03-24 19:47:14.000000 galaxy-objectstore-22.1.1/tests/objectstore/irods_object_store_conf.xml
--rw-r--r--   0 mvandenb   (501) staff       (20)      446 2022-03-24 19:47:14.000000 galaxy-objectstore-22.1.1/tests/objectstore/irods_object_store_conf_no_auth.xml
--rw-r--r--   0 mvandenb   (501) staff       (20)      454 2022-03-24 19:47:14.000000 galaxy-objectstore-22.1.1/tests/objectstore/irods_object_store_conf_no_extra_dir.xml
--rw-r--r--   0 mvandenb   (501) staff       (20)     1904 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/tests/objectstore/test_irods.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    32857 2022-08-22 19:45:28.000000 galaxy-objectstore-22.1.1/tests/objectstore/test_objectstore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-objectstore-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/
+-rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31799 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/irods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/pithos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/s3_multipart_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/objectstore/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-08 17:40:15.000000 galaxy-objectstore-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-objectstore-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-objectstore-22.1.1/HISTORY.rst` & `galaxy-objectstore-23.0.1/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-.. :changelog:
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.2.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.9.1 (2021-03-01)
----------------------
-
+-------------------
 
+* Second release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
```

### Comparing `galaxy-objectstore-22.1.1/LICENSE` & `galaxy-objectstore-23.0.1/LICENSE`

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

### Comparing `galaxy-objectstore-22.1.1/PKG-INFO` & `galaxy-objectstore-23.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 Metadata-Version: 2.1
 Name: galaxy-objectstore
-Version: 22.1.1
-Summary: Galaxy Objectstore Framework and Plugins
+Version: 23.0.1
+Summary: Galaxy objectstore framework and plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-objectstore.svg
    :target: https://pypi.org/project/galaxy-objectstore/
 
 
 Overview
 --------
 
 The Galaxy_ object store framework and default implementations.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.2.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
-
----------------------
+-------------------
 20.9.1 (2021-03-01)
----------------------
-
+-------------------
 
+* Second release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
-
-
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/__init__.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,34 +8,45 @@
 import abc
 import logging
 import os
 import random
 import shutil
 import threading
 import time
-from typing import Any, Dict, List, Type
+from typing import (
+    Any,
+    Dict,
+    List,
+    Tuple,
+    Type,
+)
 
 import yaml
 
-from galaxy.exceptions import ObjectInvalid, ObjectNotFound
+from galaxy.exceptions import (
+    ObjectInvalid,
+    ObjectNotFound,
+)
 from galaxy.util import (
     asbool,
     directory_hash_id,
     force_symlink,
     parse_xml,
     umask_fix_perms,
 )
 from galaxy.util.bunch import Bunch
 from galaxy.util.path import (
     safe_makedirs,
     safe_relpath,
 )
 from galaxy.util.sleeper import Sleeper
 
-NO_SESSION_ERROR_MESSAGE = "Attempted to 'create' object store entity in configuration with no database session present."
+NO_SESSION_ERROR_MESSAGE = (
+    "Attempted to 'create' object store entity in configuration with no database session present."
+)
 
 log = logging.getLogger(__name__)
 
 
 class ObjectStore(metaclass=abc.ABCMeta):
 
     """ObjectStore interface.
@@ -82,15 +93,17 @@
 
     @abc.abstractmethod
     def exists(self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None):
         """Return True if the object identified by `obj` exists, False otherwise."""
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def create(self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False):
+    def create(
+        self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False
+    ):
         """
         Mark the object (`obj`) as existing in the store, but with no content.
 
         This method will create a proper directory structure for
         the file if the directory does not already exist.
         """
         raise NotImplementedError()
@@ -110,52 +123,83 @@
         Return size of the object identified by `obj`.
 
         If the object does not exist, return 0.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def delete(self, obj, entire_dir=False, base_dir=None, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False):
+    def delete(
+        self,
+        obj,
+        entire_dir=False,
+        base_dir=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+    ):
         """
         Delete the object identified by `obj`.
 
         :type entire_dir: boolean
         :param entire_dir: If True, delete the entire directory pointed to by
                            extra_dir. For safety reasons, this option applies
                            only for and in conjunction with the extra_dir or
                            obj_dir options.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def get_data(self, obj, start=0, count=-1, base_dir=None, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False):
+    def get_data(
+        self,
+        obj,
+        start=0,
+        count=-1,
+        base_dir=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+    ):
         """
         Fetch `count` bytes of data offset by `start` bytes using `obj.id`.
 
         If the object does not exist raises `ObjectNotFound`.
 
         :type start: int
         :param start: Set the position to start reading the dataset file
 
         :type count: int
         :param count: Read at most `count` bytes from the dataset
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def get_filename(self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False):
+    def get_filename(
+        self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False
+    ):
         """
         Get the expected filename with absolute path for object with id `obj.id`.
 
         This can be used to access the contents of the object.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def update_from_file(self, obj, base_dir=None, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False, file_name=None, create=False):
+    def update_from_file(
+        self,
+        obj,
+        base_dir=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        file_name=None,
+        create=False,
+    ):
         """
         Inform the store that the file associated with `obj.id` has been updated.
 
         If `file_name` is provided, update from that file instead of the
         default.
         If the object does not exist raises `ObjectNotFound`.
 
@@ -209,14 +253,18 @@
     def get_store_by(self, obj):
         """Return how object is stored (by 'uuid', 'id', or None if not yet saved).
 
         Certain Galaxy remote data features aren't available if objects are stored by 'id'.
         """
         raise NotImplementedError()
 
+    @abc.abstractmethod
+    def to_dict(self) -> Dict[str, Any]:
+        raise NotImplementedError
+
 
 class BaseObjectStore(ObjectStore):
     store_by: str
     store_type: str
 
     def __init__(self, config, config_dict=None, **kwargs):
         """
@@ -233,25 +281,33 @@
         """
         if config_dict is None:
             config_dict = {}
         self.running = True
         self.config = config
         self.check_old_style = config.object_store_check_old_style
         extra_dirs = {}
-        extra_dirs['job_work'] = config.jobs_directory
-        extra_dirs['temp'] = config.new_file_path
-        extra_dirs.update({
-            e['type']: e['path'] for e in config_dict.get('extra_dirs', [])})
+        extra_dirs["job_work"] = config.jobs_directory
+        extra_dirs["temp"] = config.new_file_path
+        extra_dirs.update({e["type"]: e["path"] for e in config_dict.get("extra_dirs", [])})
         self.extra_dirs = extra_dirs
 
+    def start(self):
+        """
+        Call all postfork function(s) here. These functions spawn a thread.
+        We register start(self) with app, so app starts the threads. Override
+        this function in subclasses, as needed.
+        """
+
     def shutdown(self):
         """Close any connections for this ObjectStore."""
         self.running = False
 
-    def file_ready(self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False):
+    def file_ready(
+        self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False
+    ):
         """
         Check if a file corresponding to a dataset is ready to be used.
 
         Return True if so, False otherwise
         """
         return True
 
@@ -270,17 +326,17 @@
         return clazz(config, config_dict, **kwd)
 
     def to_dict(self):
         extra_dirs = []
         for extra_dir_type, extra_dir_path in self.extra_dirs.items():
             extra_dirs.append({"type": extra_dir_type, "path": extra_dir_path})
         return {
-            'config': config_to_dict(self.config),
-            'extra_dirs': extra_dirs,
-            'type': self.store_type,
+            "config": config_to_dict(self.config),
+            "extra_dirs": extra_dirs,
+            "type": self.store_type,
         }
 
     def _get_object_id(self, obj):
         if hasattr(obj, self.store_by):
             obj_id = getattr(obj, self.store_by)
             if obj_id is None:
                 obj.flush()
@@ -291,51 +347,51 @@
             # job working directories.
             return obj.id
 
     def _invoke(self, delegate, obj=None, **kwargs):
         return self.__getattribute__(f"_{delegate}")(obj=obj, **kwargs)
 
     def exists(self, obj, **kwargs):
-        return self._invoke('exists', obj, **kwargs)
+        return self._invoke("exists", obj, **kwargs)
 
     def create(self, obj, **kwargs):
-        return self._invoke('create', obj, **kwargs)
+        return self._invoke("create", obj, **kwargs)
 
     def empty(self, obj, **kwargs):
-        return self._invoke('empty', obj, **kwargs)
+        return self._invoke("empty", obj, **kwargs)
 
     def size(self, obj, **kwargs):
-        return self._invoke('size', obj, **kwargs)
+        return self._invoke("size", obj, **kwargs)
 
     def delete(self, obj, **kwargs):
-        return self._invoke('delete', obj, **kwargs)
+        return self._invoke("delete", obj, **kwargs)
 
     def get_data(self, obj, **kwargs):
-        return self._invoke('get_data', obj, **kwargs)
+        return self._invoke("get_data", obj, **kwargs)
 
     def get_filename(self, obj, **kwargs):
-        return self._invoke('get_filename', obj, **kwargs)
+        return self._invoke("get_filename", obj, **kwargs)
 
     def update_from_file(self, obj, **kwargs):
-        return self._invoke('update_from_file', obj, **kwargs)
+        return self._invoke("update_from_file", obj, **kwargs)
 
     def get_object_url(self, obj, **kwargs):
-        return self._invoke('get_object_url', obj, **kwargs)
+        return self._invoke("get_object_url", obj, **kwargs)
 
     def get_concrete_store_name(self, obj):
-        return self._invoke('get_concrete_store_name', obj)
+        return self._invoke("get_concrete_store_name", obj)
 
     def get_concrete_store_description_markdown(self, obj):
-        return self._invoke('get_concrete_store_description_markdown', obj)
+        return self._invoke("get_concrete_store_description_markdown", obj)
 
     def get_store_usage_percent(self):
-        return self._invoke('get_store_usage_percent')
+        return self._invoke("get_store_usage_percent")
 
     def get_store_by(self, obj, **kwargs):
-        return self._invoke('get_store_by', obj, **kwargs)
+        return self._invoke("get_store_by", obj, **kwargs)
 
 
 class ConcreteObjectStore(BaseObjectStore):
     """Subclass of ObjectStore for stores that don't delegate (non-nested).
 
     Currently only adds store_by functionality. Which doesn't make
     sense for the delegating object stores.
@@ -390,15 +446,16 @@
     >>> obj = Bunch(id=1)
     >>> s = DiskObjectStore(Bunch(umask=0o077, jobs_directory=file_path, new_file_path=file_path, object_store_check_old_style=False), dict(files_dir=file_path))
     >>> s.create(obj)
     >>> s.exists(obj)
     True
     >>> assert s.get_filename(obj) == file_path + '/000/dataset_1.dat'
     """
-    store_type = 'disk'
+
+    store_type = "disk"
 
     def __init__(self, config, config_dict):
         """
         :type config: object
         :param config: An object, most likely populated from
             `galaxy/config.ini`, having the same attributes needed by
             :class:`ObjectStore` plus:
@@ -416,54 +473,80 @@
         self.file_path = os.path.abspath(config_dict.get("files_dir") or config.file_path)
 
     @classmethod
     def parse_xml(clazz, config_xml):
         extra_dirs = []
         config_dict = {}
         if config_xml is not None:
-            store_by = config_xml.attrib.get('store_by', None)
+            store_by = config_xml.attrib.get("store_by", None)
             if store_by is not None:
-                config_dict['store_by'] = store_by
-            name = config_xml.attrib.get('name', None)
+                config_dict["store_by"] = store_by
+            name = config_xml.attrib.get("name", None)
             if name is not None:
-                config_dict['name'] = name
+                config_dict["name"] = name
             for e in config_xml:
-                if e.tag == 'files_dir':
-                    config_dict["files_dir"] = e.get('path')
-                elif e.tag == 'description':
+                if e.tag == "files_dir":
+                    config_dict["files_dir"] = e.get("path")
+                elif e.tag == "description":
                     config_dict["description"] = e.text
                 else:
-                    extra_dirs.append({"type": e.get('type'), "path": e.get('path')})
+                    extra_dirs.append({"type": e.get("type"), "path": e.get("path")})
 
         config_dict["extra_dirs"] = extra_dirs
         return config_dict
 
     def to_dict(self):
         as_dict = super().to_dict()
         as_dict["files_dir"] = self.file_path
         return as_dict
 
-    def __get_filename(self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False):
+    def __get_filename(
+        self, obj, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False
+    ):
         """
         Return the absolute path for the file corresponding to the `obj.id`.
 
         This is regardless of whether or not the file exists.
         """
-        path = self._construct_path(obj, base_dir=base_dir, dir_only=dir_only, extra_dir=extra_dir,
-                                    extra_dir_at_root=extra_dir_at_root, alt_name=alt_name,
-                                    obj_dir=False, old_style=True)
+        path = self._construct_path(
+            obj,
+            base_dir=base_dir,
+            dir_only=dir_only,
+            extra_dir=extra_dir,
+            extra_dir_at_root=extra_dir_at_root,
+            alt_name=alt_name,
+            obj_dir=False,
+            old_style=True,
+        )
         # For backward compatibility: check the old style root path first;
         # otherwise construct hashed path.
         if not os.path.exists(path):
-            return self._construct_path(obj, base_dir=base_dir, dir_only=dir_only, extra_dir=extra_dir,
-                                        extra_dir_at_root=extra_dir_at_root, alt_name=alt_name)
+            return self._construct_path(
+                obj,
+                base_dir=base_dir,
+                dir_only=dir_only,
+                extra_dir=extra_dir,
+                extra_dir_at_root=extra_dir_at_root,
+                alt_name=alt_name,
+            )
 
     # TODO: rename to _disk_path or something like that to avoid conflicts with
     # children that'll use the local_extra_dirs decorator, e.g. S3
-    def _construct_path(self, obj, old_style=False, base_dir=None, dir_only=False, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False, **kwargs):
+    def _construct_path(
+        self,
+        obj,
+        old_style=False,
+        base_dir=None,
+        dir_only=False,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        **kwargs,
+    ):
         """
         Construct the absolute path for accessing the object identified by `obj.id`.
 
         :type base_dir: string
         :param base_dir: A key in self.extra_dirs corresponding to the base
                          directory in which this object should be created, or
                          None to specify the default directory.
@@ -489,20 +572,20 @@
             hash id (e.g., /files/dataset_10.dat (old) vs.
             /files/000/dataset_10.dat (new))
         """
         base = os.path.abspath(self.extra_dirs.get(base_dir, self.file_path))
         # extra_dir should never be constructed from provided data but just
         # make sure there are no shenannigans afoot
         if extra_dir and extra_dir != os.path.normpath(extra_dir):
-            log.warning('extra_dir is not normalized: %s', extra_dir)
+            log.warning("extra_dir is not normalized: %s", extra_dir)
             raise ObjectInvalid("The requested object is invalid")
         # ensure that any parent directory references in alt_name would not
         # result in a path not contained in the directory path constructed here
         if alt_name and not safe_relpath(alt_name):
-            log.warning('alt_name would locate path outside dir: %s', alt_name)
+            log.warning("alt_name would locate path outside dir: %s", alt_name)
             raise ObjectInvalid("The requested object is invalid")
         obj_id = self._get_object_id(obj)
         if old_style:
             if extra_dir is not None:
                 path = os.path.join(base, extra_dir)
             else:
                 path = base
@@ -516,15 +599,17 @@
             if extra_dir is not None:
                 if extra_dir_at_root:
                     rel_path = os.path.join(extra_dir, rel_path)
                 else:
                     rel_path = os.path.join(rel_path, extra_dir)
             path = os.path.join(base, rel_path)
         if not dir_only:
-            assert obj_id is not None, f"The effective dataset identifier consumed by object store [{self.store_by}] must be set before a path can be constructed."
+            assert (
+                obj_id is not None
+            ), f"The effective dataset identifier consumed by object store [{self.store_by}] must be set before a path can be constructed."
             path = os.path.join(path, alt_name if alt_name else f"dataset_{obj_id}.dat")
         return os.path.abspath(path)
 
     def _exists(self, obj, **kwargs):
         """Override `ObjectStore`'s stub and check on disk."""
         if self.check_old_style:
             path = self._construct_path(obj, old_style=True, **kwargs)
@@ -534,21 +619,21 @@
                 return True
         return os.path.exists(self._construct_path(obj, **kwargs))
 
     def _create(self, obj, **kwargs):
         """Override `ObjectStore`'s stub by creating any files and folders on disk."""
         if not self._exists(obj, **kwargs):
             path = self._construct_path(obj, **kwargs)
-            dir_only = kwargs.get('dir_only', False)
+            dir_only = kwargs.get("dir_only", False)
             # Create directory if it does not exist
             dir = path if dir_only else os.path.dirname(path)
             safe_makedirs(dir)
             # Create the file if it does not exist
             if not dir_only:
-                open(path, 'w').close()  # Should be rb?
+                open(path, "w").close()  # Should be rb?
                 umask_fix_perms(path, self.config.umask, 0o666)
 
     def _empty(self, obj, **kwargs):
         """Override `ObjectStore`'s stub by checking file size on disk."""
         return self.size(obj, **kwargs) == 0
 
     def _size(self, obj, **kwargs):
@@ -570,25 +655,27 @@
                 return 0
         else:
             return 0
 
     def _delete(self, obj, entire_dir=False, **kwargs):
         """Override `ObjectStore`'s stub; delete the file or folder on disk."""
         path = self._get_filename(obj, **kwargs)
-        extra_dir = kwargs.get('extra_dir', None)
-        obj_dir = kwargs.get('obj_dir', False)
+        extra_dir = kwargs.get("extra_dir", None)
+        obj_dir = kwargs.get("obj_dir", False)
         try:
             if entire_dir and (extra_dir or obj_dir):
                 shutil.rmtree(path)
                 return True
-            if self._exists(obj, **kwargs):
-                os.remove(path)
-                return True
+            os.remove(path)
+            return True
+        except FileNotFoundError:
+            # Absolutely possible that a delete request races, but that's "fine".
+            return True
         except OSError as ex:
-            log.critical(f'{self.__get_filename(obj, **kwargs)} delete error {ex}')
+            log.critical(f"{self.__get_filename(obj, **kwargs)} delete error {ex}")
         return False
 
     def _get_data(self, obj, start=0, count=-1, **kwargs):
         """Override `ObjectStore`'s stub; retrieve data directly from disk."""
         data_file = open(self._get_filename(obj, **kwargs))  # Should be rb?
         data_file.seek(start)
         content = data_file.read(count)
@@ -611,15 +698,15 @@
         path = self._construct_path(obj, **kwargs)
         if not os.path.exists(path):
             raise ObjectNotFound
         return path
 
     def _update_from_file(self, obj, file_name=None, create=False, **kwargs):
         """`create` parameter is not used in this implementation."""
-        preserve_symlinks = kwargs.pop('preserve_symlinks', False)
+        preserve_symlinks = kwargs.pop("preserve_symlinks", False)
         # FIXME: symlinks and the object store model may not play well together
         # these should be handled better, e.g. registering the symlink'd file
         # as an object
         if create:
             self._create(obj, **kwargs)
         if file_name and self._exists(obj, **kwargs):
             try:
@@ -630,15 +717,15 @@
                     shutil.copy(file_name, path)
                     umask_fix_perms(path, self.config.umask, 0o666)
             except shutil.SameFileError:
                 # That's ok, we need to ignore this so that remote object stores can update
                 # the remote object from the cache file path
                 pass
             except OSError as ex:
-                log.critical(f'Error copying {file_name} to {self.__get_filename(obj, **kwargs)}: {ex}')
+                log.critical(f"Error copying {file_name} to {self.__get_filename(obj, **kwargs)}: {ex}")
                 raise ex
 
     def _get_object_url(self, obj, **kwargs):
         """
         Override `ObjectStore`'s stub.
 
         Returns `None`, we have no URLs.
@@ -668,95 +755,97 @@
         """For each backend, shuts them down."""
         for store in self.backends.values():
             store.shutdown()
         super().shutdown()
 
     def _exists(self, obj, **kwargs):
         """Determine if the `obj` exists in any of the backends."""
-        return self._call_method('_exists', obj, False, False, **kwargs)
+        return self._call_method("_exists", obj, False, False, **kwargs)
 
     def file_ready(self, obj, **kwargs):
         """Determine if the file for `obj` is ready to be used by any of the backends."""
-        return self._call_method('file_ready', obj, False, False, **kwargs)
+        return self._call_method("file_ready", obj, False, False, **kwargs)
 
     def _create(self, obj, **kwargs):
         """Create a backing file in a random backend."""
         random.choice(list(self.backends.values())).create(obj, **kwargs)
 
     def _empty(self, obj, **kwargs):
         """For the first backend that has this `obj`, determine if it is empty."""
-        return self._call_method('_empty', obj, True, False, **kwargs)
+        return self._call_method("_empty", obj, True, False, **kwargs)
 
     def _size(self, obj, **kwargs):
         """For the first backend that has this `obj`, return its size."""
-        return self._call_method('_size', obj, 0, False, **kwargs)
+        return self._call_method("_size", obj, 0, False, **kwargs)
 
     def _delete(self, obj, **kwargs):
         """For the first backend that has this `obj`, delete it."""
-        return self._call_method('_delete', obj, False, False, **kwargs)
+        return self._call_method("_delete", obj, False, False, **kwargs)
 
     def _get_data(self, obj, **kwargs):
         """For the first backend that has this `obj`, get data from it."""
-        return self._call_method('_get_data', obj, ObjectNotFound, True, **kwargs)
+        return self._call_method("_get_data", obj, ObjectNotFound, True, **kwargs)
 
     def _get_filename(self, obj, **kwargs):
         """For the first backend that has this `obj`, get its filename."""
-        return self._call_method('_get_filename', obj, ObjectNotFound, True, **kwargs)
+        return self._call_method("_get_filename", obj, ObjectNotFound, True, **kwargs)
 
     def _update_from_file(self, obj, **kwargs):
         """For the first backend that has this `obj`, update it from the given file."""
-        if kwargs.get('create', False):
+        if kwargs.get("create", False):
             self._create(obj, **kwargs)
-            kwargs['create'] = False
-        return self._call_method('_update_from_file', obj, ObjectNotFound, True, **kwargs)
+            kwargs["create"] = False
+        return self._call_method("_update_from_file", obj, ObjectNotFound, True, **kwargs)
 
     def _get_object_url(self, obj, **kwargs):
         """For the first backend that has this `obj`, get its URL."""
-        return self._call_method('_get_object_url', obj, None, False, **kwargs)
+        return self._call_method("_get_object_url", obj, None, False, **kwargs)
 
     def _get_concrete_store_name(self, obj):
-        return self._call_method('_get_concrete_store_name', obj, None, False)
+        return self._call_method("_get_concrete_store_name", obj, None, False)
 
     def _get_concrete_store_description_markdown(self, obj):
-        return self._call_method('_get_concrete_store_description_markdown', obj, None, False)
+        return self._call_method("_get_concrete_store_description_markdown", obj, None, False)
 
     def _get_store_by(self, obj):
-        return self._call_method('_get_store_by', obj, None, False)
+        return self._call_method("_get_store_by", obj, None, False)
 
     def _repr_object_for_exception(self, obj):
         try:
             # there are a few objects in python that don't have __class__
             obj_id = self._get_object_id(obj)
-            return f'{obj.__class__.__name__}({self.store_by}={obj_id})'
+            return f"{obj.__class__.__name__}({self.store_by}={obj_id})"
         except AttributeError:
             return str(obj)
 
-    def _call_method(self, method, obj, default, default_is_exception,
-            **kwargs):
+    def _call_method(self, method, obj, default, default_is_exception, **kwargs):
         """Check all children object stores for the first one with the dataset."""
         for store in self.backends.values():
             if store.exists(obj, **kwargs):
                 return store.__getattribute__(method)(obj, **kwargs)
         if default_is_exception:
-            raise default('objectstore, _call_method failed: %s on %s, kwargs: %s'
-                          % (method, self._repr_object_for_exception(obj), str(kwargs)))
+            raise default(
+                "objectstore, _call_method failed: %s on %s, kwargs: %s"
+                % (method, self._repr_object_for_exception(obj), str(kwargs))
+            )
         else:
             return default
 
 
 class DistributedObjectStore(NestedObjectStore):
 
     """
     ObjectStore that defers to a list of backends.
 
     When getting objects the first store where the object exists is used.
     When creating objects they are created in a store selected randomly, but
     with weighting.
     """
-    store_type = 'distributed'
+
+    store_type = "distributed"
 
     def __init__(self, config, config_dict, fsmon=False):
         """
         :type config: object
         :param config: An object, most likely populated from
             `galaxy/config.ini`, having the same attributes needed by
             :class:`NestedObjectStore` plus:
@@ -806,29 +895,29 @@
             log.info("Filesystem space monitor started")
 
     @classmethod
     def parse_xml(clazz, config_xml, legacy=False):
         if legacy:
             backends_root = config_xml
         else:
-            backends_root = config_xml.find('backends')
+            backends_root = config_xml.find("backends")
 
         backends: List[Dict[str, Any]] = []
         config_dict = {
-            'search_for_missing': asbool(backends_root.get('search_for_missing', True)),
-            'global_max_percent_full': float(backends_root.get('maxpctfull', 0)),
-            'backends': backends,
+            "search_for_missing": asbool(backends_root.get("search_for_missing", True)),
+            "global_max_percent_full": float(backends_root.get("maxpctfull", 0)),
+            "backends": backends,
         }
 
-        for b in [e for e in backends_root if e.tag == 'backend']:
+        for b in [e for e in backends_root if e.tag == "backend"]:
             store_id = b.get("id")
             store_weight = int(b.get("weight", 1))
-            store_maxpctfull = float(b.get('maxpctfull', 0))
+            store_maxpctfull = float(b.get("maxpctfull", 0))
             store_type = b.get("type", "disk")
-            store_by = b.get('store_by', None)
+            store_by = b.get("store_by", None)
 
             objectstore_class, _ = type_to_object_store_class(store_type)
             backend_config_dict = objectstore_class.parse_xml(b)
             backend_config_dict["id"] = store_id
             backend_config_dict["weight"] = store_weight
             backend_config_dict["max_percent_full"] = store_maxpctfull
             backend_config_dict["type"] = store_type
@@ -839,24 +928,25 @@
         return config_dict
 
     @classmethod
     def from_xml(clazz, config, config_xml, fsmon=False):
         legacy = False
         if config_xml is None:
             distributed_config = config.distributed_object_store_config_file
-            assert distributed_config is not None, \
-                "distributed object store ('object_store = distributed') " \
-                "requires a config file, please set one in " \
+            assert distributed_config is not None, (
+                "distributed object store ('object_store = distributed') "
+                "requires a config file, please set one in "
                 "'distributed_object_store_config_file')"
+            )
 
-            log.debug('Loading backends for distributed object store from %s', distributed_config)
+            log.debug("Loading backends for distributed object store from %s", distributed_config)
             config_xml = parse_xml(distributed_config).getroot()
             legacy = True
         else:
-            log.debug('Loading backends for distributed object store from %s', config_xml.get('id'))
+            log.debug("Loading backends for distributed object store from %s", config_xml.get("id"))
 
         config_dict = clazz.parse_xml(config_xml, legacy=legacy)
         return clazz(config, config_dict, fsmon=fsmon)
 
     def to_dict(self) -> Dict[str, Any]:
         as_dict = super().to_dict()
         as_dict["global_max_percent_full"] = self.global_max_percent_full
@@ -891,80 +981,92 @@
     def _create(self, obj, **kwargs):
         """The only method in which obj.object_store_id may be None."""
         if obj.object_store_id is None or not self._exists(obj, **kwargs):
             if obj.object_store_id is None or obj.object_store_id not in self.backends:
                 try:
                     obj.object_store_id = random.choice(self.weighted_backend_ids)
                 except IndexError:
-                    raise ObjectInvalid('objectstore.create, could not generate '
-                                        'obj.object_store_id: %s, kwargs: %s'
-                                        % (str(obj), str(kwargs)))
-                log.debug("Selected backend '%s' for creation of %s %s"
-                          % (obj.object_store_id, obj.__class__.__name__, obj.id))
+                    raise ObjectInvalid(
+                        "objectstore.create, could not generate "
+                        "obj.object_store_id: %s, kwargs: %s" % (str(obj), str(kwargs))
+                    )
+                log.debug(
+                    "Selected backend '%s' for creation of %s %s"
+                    % (obj.object_store_id, obj.__class__.__name__, obj.id)
+                )
             else:
-                log.debug("Using preferred backend '%s' for creation of %s %s"
-                          % (obj.object_store_id, obj.__class__.__name__, obj.id))
+                log.debug(
+                    "Using preferred backend '%s' for creation of %s %s"
+                    % (obj.object_store_id, obj.__class__.__name__, obj.id)
+                )
             self.backends[obj.object_store_id].create(obj, **kwargs)
 
     def _call_method(self, method, obj, default, default_is_exception, **kwargs):
         object_store_id = self.__get_store_id_for(obj, **kwargs)
         if object_store_id is not None:
             return self.backends[object_store_id].__getattribute__(method)(obj, **kwargs)
         if default_is_exception:
-            raise default('objectstore, _call_method failed: %s on %s, kwargs: %s'
-                          % (method, self._repr_object_for_exception(obj), str(kwargs)))
+            raise default(
+                "objectstore, _call_method failed: %s on %s, kwargs: %s"
+                % (method, self._repr_object_for_exception(obj), str(kwargs))
+            )
         else:
             return default
 
     def __get_store_id_for(self, obj, **kwargs):
         if obj.object_store_id is not None:
             if obj.object_store_id in self.backends:
                 return obj.object_store_id
             else:
-                log.warning('The backend object store ID (%s) for %s object with ID %s is invalid'
-                            % (obj.object_store_id, obj.__class__.__name__, obj.id))
+                log.warning(
+                    "The backend object store ID (%s) for %s object with ID %s is invalid"
+                    % (obj.object_store_id, obj.__class__.__name__, obj.id)
+                )
         elif self.search_for_missing:
             # if this instance has been switched from a non-distributed to a
             # distributed object store, or if the object's store id is invalid,
             # try to locate the object
             for id, store in self.backends.items():
                 if store.exists(obj, **kwargs):
-                    log.warning(f"{obj.__class__.__name__} object with ID {obj.id} found in backend object store with ID {id}")
+                    log.warning(
+                        f"{obj.__class__.__name__} object with ID {obj.id} found in backend object store with ID {id}"
+                    )
                     obj.object_store_id = id
                     return id
         return None
 
 
 class HierarchicalObjectStore(NestedObjectStore):
 
     """
     ObjectStore that defers to a list of backends.
 
     When getting objects the first store where the object exists is used.
     When creating objects only the first store is used.
     """
-    store_type = 'hierarchical'
+
+    store_type = "hierarchical"
 
     def __init__(self, config, config_dict, fsmon=False):
         """The default constructor. Extends `NestedObjectStore`."""
         super().__init__(config, config_dict)
 
         backends: Dict[int, ObjectStore] = {}
         for order, backend_def in enumerate(config_dict["backends"]):
             backends[order] = build_object_store_from_config(config, config_dict=backend_def, fsmon=fsmon)
 
         self.backends = backends
 
     @classmethod
     def parse_xml(clazz, config_xml):
         backends_list = []
-        for b in sorted(config_xml.find('backends'), key=lambda b: int(b.get('order'))):
-            store_type = b.get("type")
+        for backend in sorted(config_xml.find("backends"), key=lambda b: int(b.get("order"))):
+            store_type = backend.get("type")
             objectstore_class, _ = type_to_object_store_class(store_type)
-            backend_config_dict = objectstore_class.parse_xml(b)
+            backend_config_dict = objectstore_class.parse_xml(backend)
             backend_config_dict["type"] = store_type
             backends_list.append(backend_config_dict)
 
         return {"backends": backends_list}
 
     def to_dict(self):
         as_dict = super().to_dict()
@@ -983,42 +1085,48 @@
         return False
 
     def _create(self, obj, **kwargs):
         """Call the primary object store."""
         self.backends[0].create(obj, **kwargs)
 
 
-def type_to_object_store_class(store, fsmon=False):
-    objectstore_class: Type[ObjectStore]
+def type_to_object_store_class(store: str, fsmon: bool = False) -> Tuple[Type[BaseObjectStore], Dict[str, Any]]:
+    objectstore_class: Type[BaseObjectStore]
     objectstore_constructor_kwds = {}
-    if store == 'disk':
+    if store == "disk":
         objectstore_class = DiskObjectStore
-    elif store == 's3':
+    elif store == "s3":
         from .s3 import S3ObjectStore
+
         objectstore_class = S3ObjectStore
-    elif store == 'cloud':
+    elif store == "cloud":
         from .cloud import Cloud
+
         objectstore_class = Cloud
-    elif store == 'swift':
+    elif store == "swift":
         from .s3 import SwiftObjectStore
+
         objectstore_class = SwiftObjectStore
-    elif store == 'distributed':
+    elif store == "distributed":
         objectstore_class = DistributedObjectStore
         objectstore_constructor_kwds["fsmon"] = fsmon
-    elif store == 'hierarchical':
+    elif store == "hierarchical":
         objectstore_class = HierarchicalObjectStore
         objectstore_constructor_kwds["fsmon"] = fsmon
-    elif store == 'irods':
+    elif store == "irods":
         from .irods import IRODSObjectStore
+
         objectstore_class = IRODSObjectStore
-    elif store == 'azure_blob':
+    elif store == "azure_blob":
         from .azure_blob import AzureBlobObjectStore
+
         objectstore_class = AzureBlobObjectStore
-    elif store == 'pithos':
+    elif store == "pithos":
         from .pithos import PithosObjectStore
+
         objectstore_class = PithosObjectStore
     else:
         raise Exception(f"Unrecognized object store definition: {store}")
     # Disable the Pulsar object store for now until it receives some attention
     # elif store == 'pulsar':
     #    from .pulsar import PulsarObjectStore
     #    return PulsarObjectStore(config=config, config_xml=config_xml)
@@ -1033,117 +1141,127 @@
     Will use the `object_store_config_file` attribute of the `config` object to
     configure a new object store from the specified XML file.
 
     Or you can specify the object store type in the `object_store` attribute of
     the `config` object. Currently 'disk', 's3', 'swift', 'distributed',
     'hierarchical', 'irods', and 'pulsar' are supported values.
     """
-    from_object = 'xml'
+    from_object = "xml"
 
-    if config is None and config_dict is not None and 'config' in config_dict:
+    if config is None and config_dict is not None and "config" in config_dict:
         # Build a config object from to_dict of an ObjectStore.
         config = Bunch(**config_dict["config"])
     elif config is None:
-        raise Exception("build_object_store_from_config sent None as config parameter and one cannot be recovered from config_dict")
+        raise Exception(
+            "build_object_store_from_config sent None as config parameter and one cannot be recovered from config_dict"
+        )
 
     if config_xml is None and config_dict is None:
         config_file = config.object_store_config_file
         if os.path.exists(config_file):
             if config_file.endswith(".xml") or config_file.endswith(".xml.sample"):
                 # This is a top level invocation of build_object_store_from_config, and
                 # we have an object_store_conf.xml -- read the .xml and build
                 # accordingly
                 config_xml = parse_xml(config.object_store_config_file).getroot()
-                store = config_xml.get('type')
+                store = config_xml.get("type")
             else:
                 with open(config_file) as f:
                     config_dict = yaml.safe_load(f)
-                from_object = 'dict'
-                store = config_dict.get('type')
+                from_object = "dict"
+                store = config_dict.get("type")
         else:
             store = config.object_store
     elif config_xml is not None:
-        store = config_xml.get('type')
+        store = config_xml.get("type")
     elif config_dict is not None:
-        from_object = 'dict'
-        store = config_dict.get('type')
+        from_object = "dict"
+        store = config_dict.get("type")
 
     objectstore_class, objectstore_constructor_kwds = type_to_object_store_class(store, fsmon=fsmon)
-    if from_object == 'xml':
+    if from_object == "xml":
         return objectstore_class.from_xml(config=config, config_xml=config_xml, **objectstore_constructor_kwds)
     else:
         return objectstore_class(config=config, config_dict=config_dict, **objectstore_constructor_kwds)
 
 
 def local_extra_dirs(func):
     """Non-local plugin decorator using local directories for the extra_dirs (job_work and temp)."""
 
     def wraps(self, *args, **kwargs):
-        if kwargs.get('base_dir', None) is None:
+        if kwargs.get("base_dir", None) is None:
             return func(self, *args, **kwargs)
         else:
             for c in self.__class__.__mro__:
-                if c.__name__ == 'DiskObjectStore':
+                if c.__name__ == "DiskObjectStore":
                     return getattr(c, func.__name__)(self, *args, **kwargs)
-            raise Exception("Could not call DiskObjectStore's %s method, does your "
-                            "Object Store plugin inherit from DiskObjectStore?"
-                            % func.__name__)
+            raise Exception(
+                "Could not call DiskObjectStore's %s method, does your "
+                "Object Store plugin inherit from DiskObjectStore?" % func.__name__
+            )
+
     return wraps
 
 
 def convert_bytes(bytes):
     """A helper function used for pretty printing disk usage."""
     if bytes is None:
         bytes = 0
     bytes = float(bytes)
 
     if bytes >= 1099511627776:
         terabytes = bytes / 1099511627776
-        size = f'{terabytes:.2f}TB'
+        size = f"{terabytes:.2f}TB"
     elif bytes >= 1073741824:
         gigabytes = bytes / 1073741824
-        size = f'{gigabytes:.2f}GB'
+        size = f"{gigabytes:.2f}GB"
     elif bytes >= 1048576:
         megabytes = bytes / 1048576
-        size = f'{megabytes:.2f}MB'
+        size = f"{megabytes:.2f}MB"
     elif bytes >= 1024:
         kilobytes = bytes / 1024
-        size = f'{kilobytes:.2f}KB'
+        size = f"{kilobytes:.2f}KB"
     else:
-        size = f'{bytes:.2f}b'
+        size = f"{bytes:.2f}b"
     return size
 
 
 def config_to_dict(config):
-    """Dict-ify the portion of a config object consumed by the ObjectStore class and its subclasses.
-    """
+    """Dict-ify the portion of a config object consumed by the ObjectStore class and its subclasses."""
     return {
-        'object_store_check_old_style': config.object_store_check_old_style,
-        'file_path': config.file_path,
-        'umask': config.umask,
-        'jobs_directory': config.jobs_directory,
-        'new_file_path': config.new_file_path,
-        'object_store_cache_path': config.object_store_cache_path,
-        'gid': config.gid,
+        "object_store_check_old_style": config.object_store_check_old_style,
+        "file_path": config.file_path,
+        "umask": config.umask,
+        "jobs_directory": config.jobs_directory,
+        "new_file_path": config.new_file_path,
+        "object_store_cache_path": config.object_store_cache_path,
+        "gid": config.gid,
     }
 
 
 class ObjectStorePopulator:
-    """ Small helper for interacting with the object store and making sure all
+    """Small helper for interacting with the object store and making sure all
     datasets from a job end up with the same object_store_id.
     """
 
-    def __init__(self, app, user):
-        self.object_store = app.object_store
+    def __init__(self, has_object_store, user):
+        if hasattr(has_object_store, "object_store"):
+            object_store = has_object_store.object_store
+        else:
+            object_store = has_object_store
+        self.object_store = object_store
         self.object_store_id = None
         self.user = user
 
     def set_object_store_id(self, data):
+        self.set_dataset_object_store_id(data.dataset)
+
+    def set_dataset_object_store_id(self, dataset):
         # Create an empty file immediately.  The first dataset will be
         # created in the "default" store, all others will be created in
         # the same store as the first.
-        data.dataset.object_store_id = self.object_store_id
+        dataset.object_store_id = self.object_store_id
         try:
-            self.object_store.create(data.dataset)
+            self.object_store.create(dataset)
         except ObjectInvalid:
-            raise Exception('Unable to create output dataset: object store is full')
-        self.object_store_id = data.dataset.object_store_id  # these will be the same thing after the first output
+            raise Exception("Unable to create output dataset: object store is full")
+        self.object_store_id = dataset.object_store_id  # these will be the same thing after the first output
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/azure_blob.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/azure_blob.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,102 +15,105 @@
     from azure.storage.blob import BlockBlobService
     from azure.storage.blob.models import Blob
 except ImportError:
     BlockBlobService = None
 
 from galaxy.exceptions import (
     ObjectInvalid,
-    ObjectNotFound
+    ObjectNotFound,
 )
 from galaxy.util import (
     directory_hash_id,
     umask_fix_perms,
     unlink,
 )
 from galaxy.util.path import safe_relpath
 from galaxy.util.sleeper import Sleeper
-from ..objectstore import (
+from . import (
     ConcreteObjectStore,
     convert_bytes,
 )
 
-NO_BLOBSERVICE_ERROR_MESSAGE = ("ObjectStore configured, but no azure.storage.blob dependency available."
-                                "Please install and properly configure azure.storage.blob or modify Object Store configuration.")
+NO_BLOBSERVICE_ERROR_MESSAGE = (
+    "ObjectStore configured, but no azure.storage.blob dependency available."
+    "Please install and properly configure azure.storage.blob or modify Object Store configuration."
+)
 
 log = logging.getLogger(__name__)
 
 
 def parse_config_xml(config_xml):
     try:
-        auth_xml = config_xml.findall('auth')[0]
+        auth_xml = config_xml.findall("auth")[0]
 
-        account_name = auth_xml.get('account_name')
-        account_key = auth_xml.get('account_key')
+        account_name = auth_xml.get("account_name")
+        account_key = auth_xml.get("account_key")
 
-        container_xml = config_xml.find('container')
-        container_name = container_xml.get('name')
-        max_chunk_size = int(container_xml.get('max_chunk_size', 250))  # currently unused
+        container_xml = config_xml.find("container")
+        container_name = container_xml.get("name")
+        max_chunk_size = int(container_xml.get("max_chunk_size", 250))  # currently unused
 
-        c_xml = config_xml.findall('cache')[0]
-        cache_size = float(c_xml.get('size', -1))
-        staging_path = c_xml.get('path', None)
+        c_xml = config_xml.findall("cache")[0]
+        cache_size = float(c_xml.get("size", -1))
+        staging_path = c_xml.get("path", None)
 
-        tag, attrs = 'extra_dir', ('type', 'path')
+        tag, attrs = "extra_dir", ("type", "path")
         extra_dirs = config_xml.findall(tag)
         if not extra_dirs:
-            msg = f'No {tag} element in XML tree'
+            msg = f"No {tag} element in XML tree"
             log.error(msg)
             raise Exception(msg)
         extra_dirs = [{k: e.get(k) for k in attrs} for e in extra_dirs]
         return {
-            'auth': {
-                'account_name': account_name,
-                'account_key': account_key,
+            "auth": {
+                "account_name": account_name,
+                "account_key": account_key,
             },
-            'container': {
-                'name': container_name,
-                'max_chunk_size': max_chunk_size,
+            "container": {
+                "name": container_name,
+                "max_chunk_size": max_chunk_size,
             },
-            'cache': {
-                'size': cache_size,
-                'path': staging_path,
+            "cache": {
+                "size": cache_size,
+                "path": staging_path,
             },
-            'extra_dirs': extra_dirs,
+            "extra_dirs": extra_dirs,
         }
     except Exception:
         # Toss it back up after logging, we can't continue loading at this point.
         log.exception("Malformed ObjectStore Configuration XML -- unable to continue")
         raise
 
 
 class AzureBlobObjectStore(ConcreteObjectStore):
     """
     Object store that stores objects as blobs in an Azure Blob Container. A local
     cache exists that is used as an intermediate location for files between
     Galaxy and Azure.
     """
-    store_type = 'azure_blob'
+
+    store_type = "azure_blob"
 
     def __init__(self, config, config_dict):
         super().__init__(config, config_dict)
 
         self.transfer_progress = 0
 
         auth_dict = config_dict["auth"]
         container_dict = config_dict["container"]
         cache_dict = config_dict["cache"]
 
-        self.account_name = auth_dict.get('account_name')
-        self.account_key = auth_dict.get('account_key')
+        self.account_name = auth_dict.get("account_name")
+        self.account_key = auth_dict.get("account_key")
 
-        self.container_name = container_dict.get('name')
-        self.max_chunk_size = container_dict.get('max_chunk_size', 250)  # currently unused
+        self.container_name = container_dict.get("name")
+        self.max_chunk_size = container_dict.get("max_chunk_size", 250)  # currently unused
 
-        self.cache_size = cache_dict.get('size', -1)
-        self.staging_path = cache_dict.get('path') or self.config.object_store_cache_path
+        self.cache_size = cache_dict.get("size", -1)
+        self.staging_path = cache_dict.get("path") or self.config.object_store_cache_path
 
         self._initialize()
 
     def _initialize(self):
         if BlockBlobService is None:
             raise Exception(NO_BLOBSERVICE_ERROR_MESSAGE)
 
@@ -124,28 +127,30 @@
             self.sleeper = Sleeper()
             self.cache_monitor_thread = threading.Thread(target=self.__cache_monitor)
             self.cache_monitor_thread.start()
             log.info("Cache cleaner manager started")
 
     def to_dict(self):
         as_dict = super().to_dict()
-        as_dict.update({
-            'auth': {
-                'account_name': self.account_name,
-                'account_key': self.account_key,
-            },
-            'container': {
-                'name': self.container_name,
-                'max_chunk_size': self.max_chunk_size,
-            },
-            'cache': {
-                'size': self.cache_size,
-                'path': self.staging_path,
+        as_dict.update(
+            {
+                "auth": {
+                    "account_name": self.account_name,
+                    "account_key": self.account_key,
+                },
+                "container": {
+                    "name": self.container_name,
+                    "max_chunk_size": self.max_chunk_size,
+                },
+                "cache": {
+                    "size": self.cache_size,
+                    "path": self.staging_path,
+                },
             }
-        })
+        )
         return as_dict
 
     ###################
     # Private Methods #
     ###################
 
     # config_xml is an ElementTree object.
@@ -154,25 +159,35 @@
         return parse_config_xml(config_xml)
 
     def _configure_connection(self):
         log.debug("Configuring Connection")
         self.account = CloudStorageAccount(self.account_name, self.account_key)
         self.service = self.account.create_block_blob_service()
 
-    def _construct_path(self, obj, base_dir=None, dir_only=None, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False, **kwargs):
+    def _construct_path(
+        self,
+        obj,
+        base_dir=None,
+        dir_only=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        **kwargs,
+    ):
         # extra_dir should never be constructed from provided data but just
         # make sure there are no shenannigans afoot
         if extra_dir and extra_dir != os.path.normpath(extra_dir):
-            log.warning('extra_dir is not normalized: %s', extra_dir)
+            log.warning("extra_dir is not normalized: %s", extra_dir)
             raise ObjectInvalid("The requested object is invalid")
         # ensure that any parent directory references in alt_name would not
         # result in a path not contained in the directory path constructed here
         if alt_name:
             if not safe_relpath(alt_name):
-                log.warning('alt_name would locate path outside dir: %s', alt_name)
+                log.warning("alt_name would locate path outside dir: %s", alt_name)
                 raise ObjectInvalid("The requested object is invalid")
             # alt_name can contain parent directory references, but S3 will not
             # follow them, so if they are valid we normalize them out
             alt_name = os.path.normpath(alt_name)
 
         rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
 
@@ -194,15 +209,15 @@
 
         if not dir_only:
             rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
 
         return rel_path
 
     def _fix_permissions(self, rel_path):
-        """ Set permissions on rel_path"""
+        """Set permissions on rel_path"""
         for basedir, _, files in os.walk(rel_path):
             umask_fix_perms(basedir, self.config.umask, 0o777, self.config.gid)
             for filename in files:
                 path = os.path.join(basedir, filename)
                 # Ignore symlinks
                 if os.path.islink(path):
                     continue
@@ -234,15 +249,15 @@
             exists = self.service.exists(self.container_name, rel_path)
         except AzureHttpError:
             log.exception("Trouble checking existence of Azure blob '%s'", rel_path)
             return False
         return exists
 
     def _in_cache(self, rel_path):
-        """ Check if the given dataset is in the local cache. """
+        """Check if the given dataset is in the local cache."""
         cache_path = self._get_cache_path(rel_path)
         return os.path.exists(cache_path)
 
     def _pull_into_cache(self, rel_path):
         # Ensure the cache directory structure exists (e.g., dataset_#_files/)
         rel_path_dir = os.path.dirname(rel_path)
         if not os.path.exists(self._get_cache_path(rel_path_dir)):
@@ -256,20 +271,26 @@
         self.transfer_progress = float(complete) / float(total) * 100  # in percent
 
     def _download(self, rel_path):
         local_destination = self._get_cache_path(rel_path)
         try:
             log.debug("Pulling '%s' into cache to %s", rel_path, local_destination)
             if self.cache_size > 0 and self._get_size_in_azure(rel_path) > self.cache_size:
-                log.critical("File %s is larger (%s) than the cache size (%s). Cannot download.",
-                             rel_path, self._get_size_in_azure(rel_path), self.cache_size)
+                log.critical(
+                    "File %s is larger (%s) than the cache size (%s). Cannot download.",
+                    rel_path,
+                    self._get_size_in_azure(rel_path),
+                    self.cache_size,
+                )
                 return False
             else:
                 self.transfer_progress = 0  # Reset transfer progress counter
-                self.service.get_blob_to_path(self.container_name, rel_path, local_destination, progress_callback=self._transfer_cb)
+                self.service.get_blob_to_path(
+                    self.container_name, rel_path, local_destination, progress_callback=self._transfer_cb
+                )
                 return True
         except AzureHttpError:
             log.exception("Problem downloading '%s' from Azure", rel_path)
         return False
 
     def _push_to_os(self, rel_path, source_file=None, from_string=None):
         """
@@ -279,32 +300,52 @@
         If ``from_string`` is provided, set contents of the file to the value of
         the string.
         """
         try:
             source_file = source_file or self._get_cache_path(rel_path)
 
             if not os.path.exists(source_file):
-                log.error("Tried updating blob '%s' from source file '%s', but source file does not exist.", rel_path, source_file)
+                log.error(
+                    "Tried updating blob '%s' from source file '%s', but source file does not exist.",
+                    rel_path,
+                    source_file,
+                )
                 return False
 
             if os.path.getsize(source_file) == 0:
-                log.debug("Wanted to push file '%s' to azure blob '%s' but its size is 0; skipping.", source_file, rel_path)
+                log.debug(
+                    "Wanted to push file '%s' to azure blob '%s' but its size is 0; skipping.", source_file, rel_path
+                )
                 return True
 
             if from_string:
-                self.service.create_blob_from_text(self.container_name, rel_path, from_string, progress_callback=self._transfer_cb)
+                self.service.create_blob_from_text(
+                    self.container_name, rel_path, from_string, progress_callback=self._transfer_cb
+                )
                 log.debug("Pushed data from string '%s' to blob '%s'", from_string, rel_path)
             else:
                 start_time = datetime.now()
-                log.debug("Pushing cache file '%s' of size %s bytes to '%s'", source_file, os.path.getsize(source_file), rel_path)
+                log.debug(
+                    "Pushing cache file '%s' of size %s bytes to '%s'",
+                    source_file,
+                    os.path.getsize(source_file),
+                    rel_path,
+                )
                 self.transfer_progress = 0  # Reset transfer progress counter
-                self.service.create_blob_from_path(self.container_name, rel_path, source_file, progress_callback=self._transfer_cb)
+                self.service.create_blob_from_path(
+                    self.container_name, rel_path, source_file, progress_callback=self._transfer_cb
+                )
                 end_time = datetime.now()
-                log.debug("Pushed cache file '%s' to blob '%s' (%s bytes transfered in %s sec)",
-                          source_file, rel_path, os.path.getsize(source_file), end_time - start_time)
+                log.debug(
+                    "Pushed cache file '%s' to blob '%s' (%s bytes transfered in %s sec)",
+                    source_file,
+                    rel_path,
+                    os.path.getsize(source_file),
+                    end_time - start_time,
+                )
             return True
 
         except AzureHttpError:
             log.exception("Trouble pushing to Azure Blob '%s' from file '%s'", rel_path, source_file)
         return False
 
     ##################
@@ -315,16 +356,16 @@
         in_cache = in_azure = False
         rel_path = self._construct_path(obj, **kwargs)
 
         in_cache = self._in_cache(rel_path)
         in_azure = self._in_azure(rel_path)
         # log.debug("~~~~~~ File '%s' exists in cache: %s; in azure: %s" % (rel_path, in_cache, in_azure))
         # dir_only does not get synced so shortcut the decision
-        dir_only = kwargs.get('dir_only', False)
-        base_dir = kwargs.get('base_dir', None)
+        dir_only = kwargs.get("dir_only", False)
+        base_dir = kwargs.get("base_dir", None)
         if dir_only:
             if in_cache or in_azure:
                 return True
             # for JOB_WORK directory
             elif base_dir:
                 if not os.path.exists(rel_path):
                     os.makedirs(rel_path, exist_ok=True)
@@ -355,22 +396,20 @@
                 return True
             else:
                 log.debug("Waiting for dataset %s to transfer from OS: %s/%s", rel_path, local_size, remote_size)
 
         return False
 
     def _create(self, obj, **kwargs):
-
         if not self._exists(obj, **kwargs):
-
             # Pull out locally used fields
-            extra_dir = kwargs.get('extra_dir', None)
-            extra_dir_at_root = kwargs.get('extra_dir_at_root', False)
-            dir_only = kwargs.get('dir_only', False)
-            alt_name = kwargs.get('alt_name', None)
+            extra_dir = kwargs.get("extra_dir", None)
+            extra_dir_at_root = kwargs.get("extra_dir_at_root", False)
+            dir_only = kwargs.get("dir_only", False)
+            alt_name = kwargs.get("alt_name", None)
 
             # Construct hashed path
             rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
 
             # Optionally append extra_dir
             if extra_dir is not None:
                 if extra_dir_at_root:
@@ -387,22 +426,22 @@
             # flat namespace), do so for consistency with the regular file system
             # S3 folders are marked by having trailing '/' so add it now
             # s3_dir = '%s/' % rel_path
             # self._push_to_os(s3_dir, from_string='')
             # If instructed, create the dataset in cache & in S3
             if not dir_only:
                 rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
-                open(os.path.join(self.staging_path, rel_path), 'w').close()
-                self._push_to_os(rel_path, from_string='')
+                open(os.path.join(self.staging_path, rel_path), "w").close()
+                self._push_to_os(rel_path, from_string="")
 
     def _empty(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             return bool(self._size(obj, **kwargs) > 0)
         else:
-            raise ObjectNotFound(f'objectstore.empty, object does not exist: {str(obj)}, kwargs: {str(kwargs)}')
+            raise ObjectNotFound(f"objectstore.empty, object does not exist: {str(obj)}, kwargs: {str(kwargs)}")
 
     def _size(self, obj, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
         if self._in_cache(rel_path):
             try:
                 return os.path.getsize(self._get_cache_path(rel_path))
             except OSError as ex:
@@ -410,18 +449,18 @@
         elif self._exists(obj, **kwargs):
             return self._get_size_in_azure(rel_path)
         log.warning("Did not find dataset '%s', returning 0 for size", rel_path)
         return 0
 
     def _delete(self, obj, entire_dir=False, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
-        extra_dir = kwargs.get('extra_dir', None)
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        extra_dir = kwargs.get("extra_dir", None)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         try:
             if base_dir and dir_only and obj_dir:
                 # Remove temporary data in JOB_WORK directory
                 shutil.rmtree(os.path.abspath(rel_path))
                 return True
 
             # For the case of extra_files, because we don't have a reference to
@@ -442,15 +481,15 @@
                 if self._in_azure(rel_path):
                     log.debug("Deleting from Azure: %s", rel_path)
                     self.service.delete_blob(self.container_name, rel_path)
                     return True
         except AzureHttpError:
             log.exception("Could not delete blob '%s' from Azure", rel_path)
         except OSError:
-            log.exception('%s delete error', self._get_filename(obj, **kwargs))
+            log.exception("%s delete error", self._get_filename(obj, **kwargs))
         return False
 
     def _get_data(self, obj, start=0, count=-1, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
         # Check cache first and get file if not there
         if not self._in_cache(rel_path):
             self._pull_into_cache(rel_path)
@@ -459,17 +498,17 @@
         data_file.seek(start)
         content = data_file.read(count)
         data_file.close()
         return content
 
     def _get_filename(self, obj, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
 
         # for JOB_WORK directory
         if base_dir and dir_only and obj_dir:
             return os.path.abspath(rel_path)
 
         cache_path = self._get_cache_path(rel_path)
         # S3 does not recognize directories as files so cannot check if those exist.
@@ -490,15 +529,15 @@
             else:
                 if self._pull_into_cache(rel_path):
                     return cache_path
         # For the case of retrieving a directory only, return the expected path
         # even if it does not exist.
         # if dir_only:
         #     return cache_path
-        raise ObjectNotFound(f'objectstore.get_filename, no cache_path: {str(obj)}, kwargs: {str(kwargs)}')
+        raise ObjectNotFound(f"objectstore.get_filename, no cache_path: {str(obj)}, kwargs: {str(kwargs)}")
 
     def _update_from_file(self, obj, file_name=None, create=False, **kwargs):
         if create is True:
             self._create(obj, **kwargs)
         elif self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
             # Chose whether to use the dataset file itself or an alternate file
@@ -515,15 +554,17 @@
                     log.exception("Trouble copying source file '%s' to cache '%s'", source_file, cache_file)
             else:
                 source_file = self._get_cache_path(rel_path)
 
             self._push_to_os(rel_path, source_file)
 
         else:
-            raise ObjectNotFound(f'objectstore.update_from_file, object does not exist: {str(obj)}, kwargs: {str(kwargs)}')
+            raise ObjectNotFound(
+                f"objectstore.update_from_file, object does not exist: {str(obj)}, kwargs: {str(kwargs)}"
+            )
 
     def _get_object_url(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
             try:
                 url = self.service.make_blob_url(container_name=self.container_name, blob_name=rel_path)
                 return url
@@ -555,16 +596,19 @@
                     file_tuple = last_access_time, filepath, file_size
                     file_list.append(file_tuple)
             # Sort the file list (based on access time)
             file_list.sort()
             # Initiate cleaning once within 10% of the defined cache size?
             cache_limit = self.cache_size * 0.9
             if total_size > cache_limit:
-                log.info("Initiating cache cleaning: current cache size: %s; clean until smaller than: %s",
-                         convert_bytes(total_size), convert_bytes(cache_limit))
+                log.info(
+                    "Initiating cache cleaning: current cache size: %s; clean until smaller than: %s",
+                    convert_bytes(total_size),
+                    convert_bytes(cache_limit),
+                )
                 # How much to delete? If simply deleting up to the cache-10% limit,
                 # is likely to be deleting frequently and may run the risk of hitting
                 # the limit - maybe delete additional #%?
                 # For now, delete enough to leave at least 10% of the total cache free
                 delete_this_much = total_size - cache_limit
                 # Keep deleting datasets from file_list until deleted_amount does not
                 # exceed delete_this_much; start deleting from the front of the file list,
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/cloud.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,41 +8,50 @@
 import os.path
 import shutil
 import subprocess
 import threading
 import time
 from datetime import datetime
 
-from galaxy.exceptions import ObjectInvalid, ObjectNotFound
+from galaxy.exceptions import (
+    ObjectInvalid,
+    ObjectNotFound,
+)
 from galaxy.util import (
     directory_hash_id,
     safe_relpath,
     umask_fix_perms,
     unlink,
 )
 from galaxy.util.sleeper import Sleeper
+from . import (
+    ConcreteObjectStore,
+    convert_bytes,
+)
 from .s3 import parse_config_xml
-from ..objectstore import ConcreteObjectStore, convert_bytes
+
 try:
-    from cloudbridge.factory import CloudProviderFactory, ProviderList
+    from cloudbridge.factory import (
+        CloudProviderFactory,
+        ProviderList,
+    )
     from cloudbridge.interfaces.exceptions import InvalidNameException
 except ImportError:
     CloudProviderFactory = None
     ProviderList = None
 
 log = logging.getLogger(__name__)
 
 NO_CLOUDBRIDGE_ERROR_MESSAGE = (
     "Cloud ObjectStore is configured, but no CloudBridge dependency available."
     "Please install CloudBridge or modify ObjectStore configuration."
 )
 
 
 class CloudConfigMixin:
-
     def _config_to_dict(self):
         return {
             "provider": self.provider,
             "auth": self.credentials,
             "bucket": {
                 "name": self.bucket_name,
                 "use_reduced_redundancy": self.use_rr,
@@ -54,62 +63,63 @@
                 "is_secure": self.is_secure,
                 "conn_path": self.conn_path,
             },
             "cache": {
                 "size": self.cache_size,
                 "path": self.staging_path,
             },
-            'enable_cache_monitor': False,
+            "enable_cache_monitor": False,
         }
 
 
 class Cloud(ConcreteObjectStore, CloudConfigMixin):
     """
     Object store that stores objects as items in an cloud storage. A local
     cache exists that is used as an intermediate location for files between
     Galaxy and the cloud storage.
     """
-    store_type = 'cloud'
+
+    store_type = "cloud"
 
     def __init__(self, config, config_dict):
         super().__init__(config, config_dict)
         self.transfer_progress = 0
 
-        bucket_dict = config_dict['bucket']
-        connection_dict = config_dict.get('connection', {})
-        cache_dict = config_dict['cache']
-        self.enable_cache_monitor = config_dict.get('enable_cache_monitor', True)
+        bucket_dict = config_dict["bucket"]
+        connection_dict = config_dict.get("connection", {})
+        cache_dict = config_dict["cache"]
+        self.enable_cache_monitor = config_dict.get("enable_cache_monitor", True)
 
         self.provider = config_dict["provider"]
         self.credentials = config_dict["auth"]
-        self.bucket_name = bucket_dict.get('name')
-        self.use_rr = bucket_dict.get('use_reduced_redundancy', False)
-        self.max_chunk_size = bucket_dict.get('max_chunk_size', 250)
-
-        self.host = connection_dict.get('host', None)
-        self.port = connection_dict.get('port', 6000)
-        self.multipart = connection_dict.get('multipart', True)
-        self.is_secure = connection_dict.get('is_secure', True)
-        self.conn_path = connection_dict.get('conn_path', '/')
+        self.bucket_name = bucket_dict.get("name")
+        self.use_rr = bucket_dict.get("use_reduced_redundancy", False)
+        self.max_chunk_size = bucket_dict.get("max_chunk_size", 250)
+
+        self.host = connection_dict.get("host", None)
+        self.port = connection_dict.get("port", 6000)
+        self.multipart = connection_dict.get("multipart", True)
+        self.is_secure = connection_dict.get("is_secure", True)
+        self.conn_path = connection_dict.get("conn_path", "/")
 
-        self.cache_size = cache_dict.get('size', -1)
-        self.staging_path = cache_dict.get('path') or self.config.object_store_cache_path
+        self.cache_size = cache_dict.get("size", -1)
+        self.staging_path = cache_dict.get("path") or self.config.object_store_cache_path
 
         self._initialize()
 
     def _initialize(self):
         if CloudProviderFactory is None:
             raise Exception(NO_CLOUDBRIDGE_ERROR_MESSAGE)
 
         self.conn = self._get_connection(self.provider, self.credentials)
         self.bucket = self._get_bucket(self.bucket_name)
         self.start_cache_monitor()
         # Test if 'axel' is available for parallel download and pull the key into cache
         try:
-            subprocess.call('axel')
+            subprocess.call("axel")
             self.use_axel = True
         except OSError:
             self.use_axel = False
 
     def start_cache_monitor(self):
         # Clean cache only if value is set in galaxy.ini
         if self.cache_size != -1 and self.enable_cache_monitor:
@@ -121,22 +131,23 @@
             self.cache_monitor_thread.start()
             log.info("Cache cleaner manager started")
 
     @staticmethod
     def _get_connection(provider, credentials):
         log.debug(f"Configuring `{provider}` Connection")
         if provider == "aws":
-            config = {"aws_access_key": credentials["access_key"],
-                      "aws_secret_key": credentials["secret_key"]}
+            config = {"aws_access_key": credentials["access_key"], "aws_secret_key": credentials["secret_key"]}
             connection = CloudProviderFactory().create_provider(ProviderList.AWS, config)
         elif provider == "azure":
-            config = {"azure_subscription_id": credentials["subscription_id"],
-                      "azure_client_id": credentials["client_id"],
-                      "azure_secret": credentials["secret"],
-                      "azure_tenant": credentials["tenant"]}
+            config = {
+                "azure_subscription_id": credentials["subscription_id"],
+                "azure_client_id": credentials["client_id"],
+                "azure_secret": credentials["secret"],
+                "azure_tenant": credentials["tenant"],
+            }
             connection = CloudProviderFactory().create_provider(ProviderList.AZURE, config)
         elif provider == "google":
             config = {"gcp_service_creds_file": credentials["credentials_file"]}
             connection = CloudProviderFactory().create_provider(ProviderList.GCP, config)
         else:
             raise Exception(f"Unsupported provider `{provider}`.")
 
@@ -189,53 +200,47 @@
             # Read any provider-specific configuration.
             auth_element = config_xml.findall("auth")[0]
             missing_config = []
             if provider == "aws":
                 akey = auth_element.get("access_key")
                 skey = auth_element.get("secret_key")
 
-                config["auth"] = {
-                    "access_key": akey,
-                    "secret_key": skey}
+                config["auth"] = {"access_key": akey, "secret_key": skey}
             elif provider == "azure":
                 sid = auth_element.get("subscription_id")
                 if sid is None:
                     missing_config.append("subscription_id")
                 cid = auth_element.get("client_id")
                 if cid is None:
                     missing_config.append("client_id")
                 sec = auth_element.get("secret")
                 if sec is None:
                     missing_config.append("secret")
                 ten = auth_element.get("tenant")
                 if ten is None:
                     missing_config.append("tenant")
-                config["auth"] = {
-                    "subscription_id": sid,
-                    "client_id": cid,
-                    "secret": sec,
-                    "tenant": ten}
+                config["auth"] = {"subscription_id": sid, "client_id": cid, "secret": sec, "tenant": ten}
             elif provider == "google":
                 cre = auth_element.get("credentials_file")
                 if not os.path.isfile(cre):
                     msg = f"The following file specified for GCP credentials not found: {cre}"
                     log.error(msg)
                     raise OSError(msg)
                 if cre is None:
                     missing_config.append("credentials_file")
-                config["auth"] = {
-                    "credentials_file": cre}
+                config["auth"] = {"credentials_file": cre}
             else:
                 msg = f"Unsupported provider `{provider}`."
                 log.error(msg)
                 raise Exception(msg)
 
             if len(missing_config) > 0:
-                msg = "The following configuration required for {} cloud backend " \
-                      "are missing: {}".format(provider, missing_config)
+                msg = "The following configuration required for {} cloud backend " "are missing: {}".format(
+                    provider, missing_config
+                )
                 log.error(msg)
                 raise Exception(msg)
             else:
                 return config
         except Exception:
             log.exception("Malformed ObjectStore Configuration XML -- unable to continue")
             raise
@@ -262,26 +267,29 @@
                     file_tuple = last_access_time, filepath, file_size
                     file_list.append(file_tuple)
             # Sort the file list (based on access time)
             file_list.sort()
             # Initiate cleaning once within 10% of the defined cache size?
             cache_limit = self.cache_size * 0.9
             if total_size > cache_limit:
-                log.info("Initiating cache cleaning: current cache size: %s; clean until smaller than: %s",
-                         convert_bytes(total_size), convert_bytes(cache_limit))
+                log.info(
+                    "Initiating cache cleaning: current cache size: %s; clean until smaller than: %s",
+                    convert_bytes(total_size),
+                    convert_bytes(cache_limit),
+                )
                 # How much to delete? If simply deleting up to the cache-10% limit,
                 # is likely to be deleting frequently and may run the risk of hitting
                 # the limit - maybe delete additional #%?
                 # For now, delete enough to leave at least 10% of the total cache free
                 delete_this_much = total_size - cache_limit
                 self.__clean_cache(file_list, delete_this_much)
             self.sleeper.sleep(30)  # Test cache size every 30 seconds?
 
     def __clean_cache(self, file_list, delete_this_much):
-        """ Keep deleting files from the file_list until the size of the deleted
+        """Keep deleting files from the file_list until the size of the deleted
         files is greater than the value in delete_this_much parameter.
 
         :type file_list: list
         :param file_list: List of candidate files that can be deleted. This method
             will start deleting files from the beginning of the list so the list
             should be sorted accordingly. The list must contains 3-element tuples,
             positioned as follows: position 0 holds file last accessed timestamp
@@ -323,36 +331,45 @@
         except Exception:
             # These two generic exceptions will be replaced by specific exceptions
             # once proper exceptions are exposed by CloudBridge.
             log.exception(f"Could not get bucket '{bucket_name}'")
         raise Exception
 
     def _fix_permissions(self, rel_path):
-        """ Set permissions on rel_path"""
+        """Set permissions on rel_path"""
         for basedir, _, files in os.walk(rel_path):
             umask_fix_perms(basedir, self.config.umask, 0o777, self.config.gid)
             for filename in files:
                 path = os.path.join(basedir, filename)
                 # Ignore symlinks
                 if os.path.islink(path):
                     continue
                 umask_fix_perms(path, self.config.umask, 0o666, self.config.gid)
 
-    def _construct_path(self, obj, base_dir=None, dir_only=None, extra_dir=None, extra_dir_at_root=False, alt_name=None,
-                        obj_dir=False, **kwargs):
+    def _construct_path(
+        self,
+        obj,
+        base_dir=None,
+        dir_only=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        **kwargs,
+    ):
         # extra_dir should never be constructed from provided data but just
         # make sure there are no shenannigans afoot
         if extra_dir and extra_dir != os.path.normpath(extra_dir):
-            log.warning('extra_dir is not normalized: %s', extra_dir)
+            log.warning("extra_dir is not normalized: %s", extra_dir)
             raise ObjectInvalid("The requested object is invalid")
         # ensure that any parent directory references in alt_name would not
         # result in a path not contained in the directory path constructed here
         if alt_name:
             if not safe_relpath(alt_name):
-                log.warning('alt_name would locate path outside dir: %s', alt_name)
+                log.warning("alt_name would locate path outside dir: %s", alt_name)
                 raise ObjectInvalid("The requested object is invalid")
             # alt_name can contain parent directory references, but S3 will not
             # follow them, so if they are valid we normalize them out
             alt_name = os.path.normpath(alt_name)
         rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
         if extra_dir is not None:
             if extra_dir_at_root:
@@ -364,15 +381,15 @@
         if obj_dir:
             rel_path = os.path.join(rel_path, str(self._get_object_id(obj)))
         if base_dir:
             base = self.extra_dirs.get(base_dir)
             return os.path.join(base, rel_path)
 
         # S3 folders are marked by having trailing '/' so add it now
-        rel_path = f'{rel_path}/'
+        rel_path = f"{rel_path}/"
 
         if not dir_only:
             rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
         return rel_path
 
     def _get_cache_path(self, rel_path):
         return os.path.abspath(os.path.join(self.staging_path, rel_path))
@@ -389,30 +406,30 @@
             log.exception("Could not get size of key '%s' from S3", rel_path)
             return -1
 
     def _key_exists(self, rel_path):
         exists = False
         try:
             # A hackish way of testing if the rel_path is a folder vs a file
-            is_dir = rel_path[-1] == '/'
+            is_dir = rel_path[-1] == "/"
             if is_dir:
                 keyresult = self.bucket.objects.list(prefix=rel_path)
                 if len(keyresult) > 0:
                     exists = True
                 else:
                     exists = False
             else:
                 exists = True if self.bucket.objects.get(rel_path) is not None else False
         except Exception:
             log.exception("Trouble checking existence of S3 key '%s'", rel_path)
             return False
         return exists
 
     def _in_cache(self, rel_path):
-        """ Check if the given dataset is in the local cache and return True if so. """
+        """Check if the given dataset is in the local cache and return True if so."""
         # log.debug("------ Checking cache for rel_path %s" % rel_path)
         cache_path = self._get_cache_path(rel_path)
         return os.path.exists(cache_path)
 
     def _pull_into_cache(self, rel_path):
         # Ensure the cache directory structure exists (e.g., dataset_#_files/)
         rel_path_dir = os.path.dirname(rel_path)
@@ -428,16 +445,20 @@
 
     def _download(self, rel_path):
         try:
             log.debug("Pulling key '%s' into cache to %s", rel_path, self._get_cache_path(rel_path))
             key = self.bucket.objects.get(rel_path)
             # Test if cache is large enough to hold the new file
             if self.cache_size > 0 and key.size > self.cache_size:
-                log.critical("File %s is larger (%s) than the cache size (%s). Cannot download.",
-                             rel_path, key.size, self.cache_size)
+                log.critical(
+                    "File %s is larger (%s) than the cache size (%s). Cannot download.",
+                    rel_path,
+                    key.size,
+                    self.cache_size,
+                )
                 return False
             if self.use_axel:
                 log.debug("Parallel pulled key '%s' into cache to %s", rel_path, self._get_cache_path(rel_path))
                 ncores = multiprocessing.cpu_count()
                 url = key.generate_url(7200)
                 ret_code = subprocess.call(f"axel -a -n {ncores} '{url}'")
                 if ret_code == 0:
@@ -460,73 +481,90 @@
         If ``from_string`` is provided, set contents of the file to the value of
         the string.
         """
         try:
             source_file = source_file if source_file else self._get_cache_path(rel_path)
             if os.path.exists(source_file):
                 if os.path.getsize(source_file) == 0 and (self.bucket.objects.get(rel_path) is not None):
-                    log.debug("Wanted to push file '%s' to S3 key '%s' but its size is 0; skipping.", source_file,
-                              rel_path)
+                    log.debug(
+                        "Wanted to push file '%s' to S3 key '%s' but its size is 0; skipping.", source_file, rel_path
+                    )
                     return True
                 if from_string:
                     if not self.bucket.objects.get(rel_path):
                         created_obj = self.bucket.objects.create(rel_path)
                         created_obj.upload(source_file)
                     else:
                         self.bucket.objects.get(rel_path).upload(source_file)
                     log.debug("Pushed data from string '%s' to key '%s'", from_string, rel_path)
                 else:
                     start_time = datetime.now()
-                    log.debug("Pushing cache file '%s' of size %s bytes to key '%s'", source_file,
-                              os.path.getsize(source_file), rel_path)
+                    log.debug(
+                        "Pushing cache file '%s' of size %s bytes to key '%s'",
+                        source_file,
+                        os.path.getsize(source_file),
+                        rel_path,
+                    )
                     self.transfer_progress = 0  # Reset transfer progress counter
                     if not self.bucket.objects.get(rel_path):
                         created_obj = self.bucket.objects.create(rel_path)
                         created_obj.upload_from_file(source_file)
                     else:
                         self.bucket.objects.get(rel_path).upload_from_file(source_file)
 
                     end_time = datetime.now()
-                    log.debug("Pushed cache file '%s' to key '%s' (%s bytes transfered in %s sec)",
-                              source_file, rel_path, os.path.getsize(source_file), end_time - start_time)
+                    log.debug(
+                        "Pushed cache file '%s' to key '%s' (%s bytes transfered in %s sec)",
+                        source_file,
+                        rel_path,
+                        os.path.getsize(source_file),
+                        end_time - start_time,
+                    )
                 return True
             else:
-                log.error("Tried updating key '%s' from source file '%s', but source file does not exist.",
-                          rel_path, source_file)
+                log.error(
+                    "Tried updating key '%s' from source file '%s', but source file does not exist.",
+                    rel_path,
+                    source_file,
+                )
         except Exception:
             log.exception("Trouble pushing S3 key '%s' from file '%s'", rel_path, source_file)
         return False
 
     def file_ready(self, obj, **kwargs):
         """
         A helper method that checks if a file corresponding to a dataset is
         ready and available to be used. Return ``True`` if so, ``False`` otherwise.
         """
         rel_path = self._construct_path(obj, **kwargs)
         # Make sure the size in cache is available in its entirety
         if self._in_cache(rel_path):
             if os.path.getsize(self._get_cache_path(rel_path)) == self._get_size_in_cloud(rel_path):
                 return True
-            log.debug("Waiting for dataset %s to transfer from OS: %s/%s", rel_path,
-                      os.path.getsize(self._get_cache_path(rel_path)), self._get_size_in_cloud(rel_path))
+            log.debug(
+                "Waiting for dataset %s to transfer from OS: %s/%s",
+                rel_path,
+                os.path.getsize(self._get_cache_path(rel_path)),
+                self._get_size_in_cloud(rel_path),
+            )
         return False
 
     def _exists(self, obj, **kwargs):
         in_cache = False
         rel_path = self._construct_path(obj, **kwargs)
 
         # Check cache
         if self._in_cache(rel_path):
             in_cache = True
         # Check cloud
         in_cloud = self._key_exists(rel_path)
         # log.debug("~~~~~~ File '%s' exists in cache: %s; in s3: %s" % (rel_path, in_cache, in_s3))
         # dir_only does not get synced so shortcut the decision
-        dir_only = kwargs.get('dir_only', False)
-        base_dir = kwargs.get('base_dir', None)
+        dir_only = kwargs.get("dir_only", False)
+        base_dir = kwargs.get("base_dir", None)
         if dir_only:
             if in_cache or in_cloud:
                 return True
             # for JOB_WORK directory
             elif base_dir:
                 if not os.path.exists(rel_path):
                     os.makedirs(rel_path, exist_ok=True)
@@ -541,20 +579,19 @@
         elif in_cloud:
             return True
         else:
             return False
 
     def _create(self, obj, **kwargs):
         if not self._exists(obj, **kwargs):
-
             # Pull out locally used fields
-            extra_dir = kwargs.get('extra_dir', None)
-            extra_dir_at_root = kwargs.get('extra_dir_at_root', False)
-            dir_only = kwargs.get('dir_only', False)
-            alt_name = kwargs.get('alt_name', None)
+            extra_dir = kwargs.get("extra_dir", None)
+            extra_dir_at_root = kwargs.get("extra_dir_at_root", False)
+            dir_only = kwargs.get("dir_only", False)
+            alt_name = kwargs.get("alt_name", None)
 
             # Construct hashed path
             rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
 
             # Optionally append extra_dir
             if extra_dir is not None:
                 if extra_dir_at_root:
@@ -565,23 +602,22 @@
             # Create given directory in cache
             cache_dir = os.path.join(self.staging_path, rel_path)
             if not os.path.exists(cache_dir):
                 os.makedirs(cache_dir, exist_ok=True)
 
             if not dir_only:
                 rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
-                open(os.path.join(self.staging_path, rel_path), 'w').close()
-                self._push_to_os(rel_path, from_string='')
+                open(os.path.join(self.staging_path, rel_path), "w").close()
+                self._push_to_os(rel_path, from_string="")
 
     def _empty(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             return bool(self._size(obj, **kwargs) > 0)
         else:
-            raise ObjectNotFound('objectstore.empty, object does not exist: %s, kwargs: %s'
-                                 % (str(obj), str(kwargs)))
+            raise ObjectNotFound(f"objectstore.empty, object does not exist: {obj}, kwargs: {kwargs}")
 
     def _size(self, obj, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
         if self._in_cache(rel_path):
             try:
                 return os.path.getsize(self._get_cache_path(rel_path))
             except OSError as ex:
@@ -589,18 +625,18 @@
         elif self._exists(obj, **kwargs):
             return self._get_size_in_cloud(rel_path)
         log.warning("Did not find dataset '%s', returning 0 for size", rel_path)
         return 0
 
     def _delete(self, obj, entire_dir=False, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
-        extra_dir = kwargs.get('extra_dir', None)
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        extra_dir = kwargs.get("extra_dir", None)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         try:
             # Remove temparory data in JOB_WORK directory
             if base_dir and dir_only and obj_dir:
                 shutil.rmtree(os.path.abspath(rel_path))
                 return True
 
             # For the case of extra_files, because we don't have a reference to
@@ -622,15 +658,15 @@
                     key = self.bucket.objects.get(rel_path)
                     log.debug("Deleting key %s", key.name)
                     key.delete()
                     return True
         except Exception:
             log.exception("Could not delete key '%s' from cloud", rel_path)
         except OSError:
-            log.exception('%s delete error', self._get_filename(obj, **kwargs))
+            log.exception("%s delete error", self._get_filename(obj, **kwargs))
         return False
 
     def _get_data(self, obj, start=0, count=-1, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
         # Check cache first and get file if not there
         if not self._in_cache(rel_path):
             self._pull_into_cache(rel_path)
@@ -638,17 +674,17 @@
         data_file = open(self._get_cache_path(rel_path))
         data_file.seek(start)
         content = data_file.read(count)
         data_file.close()
         return content
 
     def _get_filename(self, obj, **kwargs):
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         rel_path = self._construct_path(obj, **kwargs)
 
         # for JOB_WORK directory
         if base_dir and dir_only and obj_dir:
             return os.path.abspath(rel_path)
 
         cache_path = self._get_cache_path(rel_path)
@@ -670,16 +706,15 @@
             else:
                 if self._pull_into_cache(rel_path):
                     return cache_path
         # For the case of retrieving a directory only, return the expected path
         # even if it does not exist.
         # if dir_only:
         #     return cache_path
-        raise ObjectNotFound('objectstore.get_filename, no cache_path: %s, kwargs: %s'
-                             % (str(obj), str(kwargs)))
+        raise ObjectNotFound(f"objectstore.get_filename, no cache_path: {obj}, kwargs: {kwargs}")
         # return cache_path # Until the upload tool does not explicitly create the dataset, return expected path
 
     def _update_from_file(self, obj, file_name=None, create=False, **kwargs):
         if create:
             self._create(obj, **kwargs)
         if self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
@@ -696,16 +731,15 @@
                 except OSError:
                     log.exception("Trouble copying source file '%s' to cache '%s'", source_file, cache_file)
             else:
                 source_file = self._get_cache_path(rel_path)
             # Update the file on cloud
             self._push_to_os(rel_path, source_file)
         else:
-            raise ObjectNotFound('objectstore.update_from_file, object does not exist: %s, kwargs: %s'
-                                 % (str(obj), str(kwargs)))
+            raise ObjectNotFound(f"objectstore.update_from_file, object does not exist: {obj}, kwargs: {kwargs}")
 
     def _get_object_url(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
             try:
                 key = self.bucket.objects.get(rel_path)
                 return key.generate_url(expires_in=86400)  # 24hrs
@@ -714,12 +748,12 @@
         return None
 
     def _get_store_usage_percent(self):
         return 0.0
 
     def shutdown(self):
         self.running = False
-        thread = getattr(self, 'cache_monitor_thread', None)
+        thread = getattr(self, "cache_monitor_thread", None)
         if thread:
             log.debug("Shutting down thread")
             self.sleeper.wake()
             thread.join(5)
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/irods.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/irods.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,269 +1,351 @@
 """
 Object Store plugin for the Integrated Rule-Oriented Data System (iRODS)
 """
 import logging
 import os
 import shutil
+import threading
 from datetime import datetime
 from pathlib import Path
 
 try:
     import irods
     import irods.keywords as kw
-    from irods.exception import CollectionDoesNotExist
-    from irods.exception import DataObjectDoesNotExist
+    from irods.exception import (
+        CollectionDoesNotExist,
+        DataObjectDoesNotExist,
+    )
     from irods.session import iRODSSession
 except ImportError:
     irods = None
 
-from galaxy.exceptions import ObjectInvalid, ObjectNotFound
+from galaxy.exceptions import (
+    ObjectInvalid,
+    ObjectNotFound,
+)
 from galaxy.util import (
     directory_hash_id,
     ExecutionTimer,
     umask_fix_perms,
     unlink,
 )
 from galaxy.util.path import safe_relpath
-from ..objectstore import DiskObjectStore
+from . import DiskObjectStore
 
-IRODS_IMPORT_MESSAGE = ('The Python irods package is required to use this feature, please install it')
+IRODS_IMPORT_MESSAGE = "The Python irods package is required to use this feature, please install it"
 # 1 MB
 CHUNK_SIZE = 2**20
 log = logging.getLogger(__name__)
 logging.getLogger("irods.connection").setLevel(logging.INFO)  # irods logging generates gigabytes of logs
 
 
 def _config_xml_error(tag):
-    msg = f'No {tag} element in config XML tree'
+    msg = f"No {tag} element in config XML tree"
     raise Exception(msg)
 
 
 def _config_dict_error(key):
-    msg = 'No {key} key in config dictionary'.forma(key=key)
+    msg = "No {key} key in config dictionary".forma(key=key)
     raise Exception(msg)
 
 
 def parse_config_xml(config_xml):
     try:
-        a_xml = config_xml.findall('auth')
+        a_xml = config_xml.findall("auth")
         if not a_xml:
-            _config_xml_error('auth')
-        username = a_xml[0].get('username')
-        password = a_xml[0].get('password')
+            _config_xml_error("auth")
+        username = a_xml[0].get("username")
+        password = a_xml[0].get("password")
 
-        r_xml = config_xml.findall('resource')
+        r_xml = config_xml.findall("resource")
         if not r_xml:
-            _config_xml_error('resource')
-        resource_name = r_xml[0].get('name')
+            _config_xml_error("resource")
+        resource_name = r_xml[0].get("name")
 
-        z_xml = config_xml.findall('zone')
+        z_xml = config_xml.findall("zone")
         if not z_xml:
-            _config_xml_error('zone')
-        zone_name = z_xml[0].get('name')
+            _config_xml_error("zone")
+        zone_name = z_xml[0].get("name")
 
-        c_xml = config_xml.findall('connection')
+        c_xml = config_xml.findall("connection")
         if not c_xml:
-            _config_xml_error('connection')
-        host = c_xml[0].get('host', None)
-        port = int(c_xml[0].get('port', 0))
-        timeout = int(c_xml[0].get('timeout', 30))
-        refresh_time = int(c_xml[0].get('refresh_time', 300))
+            _config_xml_error("connection")
+        host = c_xml[0].get("host", None)
+        port = int(c_xml[0].get("port", 0))
+        timeout = int(c_xml[0].get("timeout", 30))
+        refresh_time = int(c_xml[0].get("refresh_time", 300))
+        connection_pool_monitor_interval = int(c_xml[0].get("connection_pool_monitor_interval", -1))
 
-        c_xml = config_xml.findall('cache')
+        c_xml = config_xml.findall("cache")
         if not c_xml:
-            _config_xml_error('cache')
-        cache_size = float(c_xml[0].get('size', -1))
-        staging_path = c_xml[0].get('path', None)
+            _config_xml_error("cache")
+        cache_size = float(c_xml[0].get("size", -1))
+        staging_path = c_xml[0].get("path", None)
 
-        attrs = ('type', 'path')
-        e_xml = config_xml.findall('extra_dir')
+        attrs = ("type", "path")
+        e_xml = config_xml.findall("extra_dir")
         if not e_xml:
-            _config_xml_error('extra_dir')
+            _config_xml_error("extra_dir")
         extra_dirs = [{k: e.get(k) for k in attrs} for e in e_xml]
 
         return {
-            'auth': {
-                'username': username,
-                'password': password,
-            },
-            'resource': {
-                'name': resource_name,
-            },
-            'zone': {
-                'name': zone_name,
-            },
-            'connection': {
-                'host': host,
-                'port': port,
-                'timeout': timeout,
-                'refresh_time': refresh_time,
-            },
-            'cache': {
-                'size': cache_size,
-                'path': staging_path,
+            "auth": {
+                "username": username,
+                "password": password,
+            },
+            "resource": {
+                "name": resource_name,
+            },
+            "zone": {
+                "name": zone_name,
+            },
+            "connection": {
+                "host": host,
+                "port": port,
+                "timeout": timeout,
+                "refresh_time": refresh_time,
+                "connection_pool_monitor_interval": connection_pool_monitor_interval,
+            },
+            "cache": {
+                "size": cache_size,
+                "path": staging_path,
             },
-            'extra_dirs': extra_dirs,
+            "extra_dirs": extra_dirs,
         }
     except Exception:
         # Toss it back up after logging, we can't continue loading at this point.
         log.exception("Malformed iRODS ObjectStore Configuration XML -- unable to continue.")
         raise
 
 
 class CloudConfigMixin:
-
     def _config_to_dict(self):
         return {
-            'auth': {
-                'username': self.username,
-                'password': self.password,
-            },
-            'resource': {
-                'name': self.resource,
-            },
-            'zone': {
-                'name': self.zone,
-            },
-            'connection': {
-                'host': self.host,
-                'port': self.port,
-                'timeout': self.timeout,
-                'refresh_time': self.refresh_time,
-            },
-            'cache': {
-                'size': self.cache_size,
-                'path': self.staging_path,
-            }
+            "auth": {
+                "username": self.username,
+                "password": self.password,
+            },
+            "resource": {
+                "name": self.resource,
+            },
+            "zone": {
+                "name": self.zone,
+            },
+            "connection": {
+                "host": self.host,
+                "port": self.port,
+                "timeout": self.timeout,
+                "refresh_time": self.refresh_time,
+                "connection_pool_monitor_interval": self.connection_pool_monitor_interval,
+            },
+            "cache": {
+                "size": self.cache_size,
+                "path": self.staging_path,
+            },
         }
 
 
 class IRODSObjectStore(DiskObjectStore, CloudConfigMixin):
     """
     Object store that stores files as data objects in an iRODS Zone. A local cache
     exists that is used as an intermediate location for files between Galaxy and iRODS.
     """
 
-    store_type = 'irods'
+    store_type = "irods"
 
     def __init__(self, config, config_dict):
         ipt_timer = ExecutionTimer()
         super().__init__(config, config_dict)
 
-        auth_dict = config_dict.get('auth')
+        auth_dict = config_dict.get("auth")
         if auth_dict is None:
-            _config_dict_error('auth')
+            _config_dict_error("auth")
 
-        self.username = auth_dict.get('username')
+        self.username = auth_dict.get("username")
         if self.username is None:
-            _config_dict_error('auth->username')
-        self.password = auth_dict.get('password')
+            _config_dict_error("auth->username")
+        self.password = auth_dict.get("password")
         if self.password is None:
-            _config_dict_error('auth->password')
+            _config_dict_error("auth->password")
 
-        resource_dict = config_dict['resource']
+        resource_dict = config_dict["resource"]
         if resource_dict is None:
-            _config_dict_error('resource')
-        self.resource = resource_dict.get('name')
+            _config_dict_error("resource")
+        self.resource = resource_dict.get("name")
         if self.resource is None:
-            _config_dict_error('resource->name')
+            _config_dict_error("resource->name")
 
-        zone_dict = config_dict['zone']
+        zone_dict = config_dict["zone"]
         if zone_dict is None:
-            _config_dict_error('zone')
-        self.zone = zone_dict.get('name')
+            _config_dict_error("zone")
+        self.zone = zone_dict.get("name")
         if self.zone is None:
-            _config_dict_error('zone->name')
+            _config_dict_error("zone->name")
 
-        connection_dict = config_dict['connection']
+        connection_dict = config_dict["connection"]
         if connection_dict is None:
-            _config_dict_error('connection')
-        self.host = connection_dict.get('host')
+            _config_dict_error("connection")
+        self.host = connection_dict.get("host")
         if self.host is None:
-            _config_dict_error('connection->host')
-        self.port = connection_dict.get('port')
+            _config_dict_error("connection->host")
+        self.port = connection_dict.get("port")
         if self.port is None:
-            _config_dict_error('connection->port')
-        self.timeout = connection_dict.get('timeout')
+            _config_dict_error("connection->port")
+        self.timeout = connection_dict.get("timeout")
         if self.timeout is None:
-            _config_dict_error('connection->timeout')
-        self.refresh_time = connection_dict.get('refresh_time')
+            _config_dict_error("connection->timeout")
+        self.refresh_time = connection_dict.get("refresh_time")
         if self.refresh_time is None:
-            _config_dict_error('connection->refresh_time')
+            _config_dict_error("connection->refresh_time")
+        self.connection_pool_monitor_interval = connection_dict.get("connection_pool_monitor_interval")
+        if self.connection_pool_monitor_interval is None:
+            _config_dict_error("connection->connection_pool_monitor_interval")
 
-        cache_dict = config_dict['cache']
+        cache_dict = config_dict["cache"]
         if cache_dict is None:
-            _config_dict_error('cache')
-        self.cache_size = cache_dict.get('size', -1)
+            _config_dict_error("cache")
+        self.cache_size = cache_dict.get("size", -1)
         if self.cache_size is None:
-            _config_dict_error('cache->size')
-        self.staging_path = cache_dict.get('path') or self.config.object_store_cache_path
+            _config_dict_error("cache->size")
+        self.staging_path = cache_dict.get("path") or self.config.object_store_cache_path
         if self.staging_path is None:
-            _config_dict_error('cache->path')
+            _config_dict_error("cache->path")
 
-        extra_dirs = {e['type']: e['path'] for e in config_dict.get('extra_dirs', [])}
+        extra_dirs = {e["type"]: e["path"] for e in config_dict.get("extra_dirs", [])}
         if not extra_dirs:
-            _config_dict_error('extra_dirs')
+            _config_dict_error("extra_dirs")
         self.extra_dirs.update(extra_dirs)
 
         if irods is None:
             raise Exception(IRODS_IMPORT_MESSAGE)
 
         self.home = f"/{self.zone}/home/{self.username}"
 
         if irods is None:
             raise Exception(IRODS_IMPORT_MESSAGE)
 
-        self.session = iRODSSession(host=self.host, port=self.port, user=self.username, password=self.password, zone=self.zone, refresh_time=self.refresh_time)
+        self.session = iRODSSession(
+            host=self.host,
+            port=self.port,
+            user=self.username,
+            password=self.password,
+            zone=self.zone,
+            refresh_time=self.refresh_time,
+        )
         # Set connection timeout
         self.session.connection_timeout = self.timeout
+
+        if self.connection_pool_monitor_interval != -1:
+            # This Event object is initialized to False
+            # It is set to True in shutdown(), causing
+            # the connection pool monitor thread to return/terminate
+            self.stop_connection_pool_monitor_event = threading.Event()
+            self.connection_pool_monitor_thread = None
+
         log.debug("irods_pt __init__: %s", ipt_timer)
 
     def shutdown(self):
         # This call will cleanup all the connections in the connection pool
         # OSError sometimes happens on GitHub Actions, after the test has successfully completed. Ignore it if it happens.
         ipt_timer = ExecutionTimer()
         try:
             self.session.cleanup()
         except OSError:
             pass
+
+        if self.connection_pool_monitor_interval != -1:
+            # Set to True so the connection pool monitor thread will return/terminate
+            self.stop_connection_pool_monitor_event.set()
+            if self.connection_pool_monitor_thread is not None:
+                self.connection_pool_monitor_thread.join(5)
+
         log.debug("irods_pt shutdown: %s", ipt_timer)
 
     @classmethod
     def parse_xml(cls, config_xml):
         return parse_config_xml(config_xml)
 
+    def start_connection_pool_monitor(self):
+        self.connection_pool_monitor_thread = threading.Thread(
+            target=self._connection_pool_monitor,
+            args=(),
+            kwargs={
+                "refresh_time": self.refresh_time,
+                "connection_pool_monitor_interval": self.connection_pool_monitor_interval,
+                "stop_connection_pool_monitor_event": self.stop_connection_pool_monitor_event,
+            },
+            name="ConnectionPoolMonitorThread",
+            daemon=True,
+        )
+        self.connection_pool_monitor_thread.start()
+        log.info("Connection pool monitor started")
+
+    def start(self):
+        if self.connection_pool_monitor_interval != -1:
+            self.start_connection_pool_monitor()
+
+    def _connection_pool_monitor(self, *args, **kwargs):
+        refresh_time = kwargs["refresh_time"]
+        connection_pool_monitor_interval = kwargs["connection_pool_monitor_interval"]
+        stop_connection_pool_monitor_event = kwargs["stop_connection_pool_monitor_event"]
+
+        while not stop_connection_pool_monitor_event.is_set():
+            curr_time = datetime.now()
+            idle_connection_set = self.session.pool.idle.copy()
+            for conn in idle_connection_set:
+                # If the connection was created more than 'refresh_time'
+                # seconds ago, release the connection (as its stale)
+                if (curr_time - conn.create_time).total_seconds() > refresh_time:
+                    log.debug(
+                        "Idle connection with id {} was created more than {} seconds ago. Releasing the connection.".format(
+                            id(conn), refresh_time
+                        )
+                    )
+                    self.session.pool.release_connection(conn, True)
+            stop_connection_pool_monitor_event.wait(connection_pool_monitor_interval)
+
     def to_dict(self):
         as_dict = super().to_dict()
         as_dict.update(self._config_to_dict())
         return as_dict
 
     def _fix_permissions(self, rel_path):
-        """ Set permissions on rel_path"""
+        """Set permissions on rel_path"""
         for basedir, _, files in os.walk(rel_path):
             umask_fix_perms(basedir, self.config.umask, 0o777, self.config.gid)
             for filename in files:
                 path = os.path.join(basedir, filename)
                 # Ignore symlinks
                 if os.path.islink(path):
                     continue
                 umask_fix_perms(path, self.config.umask, 0o666, self.config.gid)
 
-    def _construct_path(self, obj, base_dir=None, dir_only=None, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False, **kwargs):
+    def _construct_path(
+        self,
+        obj,
+        base_dir=None,
+        dir_only=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        **kwargs,
+    ):
         ipt_timer = ExecutionTimer()
         # extra_dir should never be constructed from provided data but just
         # make sure there are no shenanigans afoot
         if extra_dir and extra_dir != os.path.normpath(extra_dir):
-            log.warning('extra_dir is not normalized: %s', extra_dir)
+            log.warning("extra_dir is not normalized: %s", extra_dir)
             raise ObjectInvalid("The requested object is invalid")
         # ensure that any parent directory references in alt_name would not
         # result in a path not contained in the directory path constructed here
         if alt_name:
             if not safe_relpath(alt_name):
-                log.warning('alt_name would locate path outside dir: %s', alt_name)
+                log.warning("alt_name would locate path outside dir: %s", alt_name)
                 raise ObjectInvalid("The requested object is invalid")
             # alt_name can contain parent directory references, but S3 will not
             # follow them, so if they are valid we normalize them out
             alt_name = os.path.normpath(alt_name)
         rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
         if extra_dir is not None:
             if extra_dir_at_root:
@@ -290,16 +372,16 @@
     # rel_path is file or folder?
     def _get_size_in_irods(self, rel_path):
         ipt_timer = ExecutionTimer()
         p = Path(rel_path)
         data_object_name = p.stem + p.suffix
         subcollection_name = p.parent
 
-        collection_path = f"{self.home}/{str(subcollection_name)}"
-        data_object_path = f"{collection_path}/{str(data_object_name)}"
+        collection_path = f"{self.home}/{subcollection_name}"
+        data_object_path = f"{collection_path}/{data_object_name}"
         options = {kw.DEST_RESC_NAME_KW: self.resource}
 
         try:
             data_obj = self.session.data_objects.get(data_object_path, **options)
             return data_obj.__sizeof__()
         except (DataObjectDoesNotExist, CollectionDoesNotExist):
             log.warning("Collection or data object (%s) does not exist", data_object_path)
@@ -310,29 +392,29 @@
     # rel_path is file or folder?
     def _data_object_exists(self, rel_path):
         ipt_timer = ExecutionTimer()
         p = Path(rel_path)
         data_object_name = p.stem + p.suffix
         subcollection_name = p.parent
 
-        collection_path = f"{self.home}/{str(subcollection_name)}"
-        data_object_path = f"{collection_path}/{str(data_object_name)}"
+        collection_path = f"{self.home}/{subcollection_name}"
+        data_object_path = f"{collection_path}/{data_object_name}"
         options = {kw.DEST_RESC_NAME_KW: self.resource}
 
         try:
             self.session.data_objects.get(data_object_path, **options)
             return True
         except (DataObjectDoesNotExist, CollectionDoesNotExist):
             log.debug("Collection or data object (%s) does not exist", data_object_path)
             return False
         finally:
             log.debug("irods_pt _data_object_exists: %s", ipt_timer)
 
     def _in_cache(self, rel_path):
-        """ Check if the given dataset is in the local cache and return True if so. """
+        """Check if the given dataset is in the local cache and return True if so."""
         cache_path = self._get_cache_path(rel_path)
         return os.path.exists(cache_path)
 
     def _pull_into_cache(self, rel_path):
         ipt_timer = ExecutionTimer()
         # Ensure the cache directory structure exists (e.g., dataset_#_files/)
         rel_path_dir = os.path.dirname(rel_path)
@@ -348,16 +430,16 @@
         ipt_timer = ExecutionTimer()
         log.debug("Pulling data object '%s' into cache to %s", rel_path, self._get_cache_path(rel_path))
 
         p = Path(rel_path)
         data_object_name = p.stem + p.suffix
         subcollection_name = p.parent
 
-        collection_path = f"{self.home}/{str(subcollection_name)}"
-        data_object_path = f"{collection_path}/{str(data_object_name)}"
+        collection_path = f"{self.home}/{subcollection_name}"
+        data_object_path = f"{collection_path}/{data_object_name}"
         options = {kw.DEST_RESC_NAME_KW: self.resource}
 
         try:
             cache_path = self._get_cache_path(rel_path)
             self.session.data_objects.get(data_object_path, cache_path, **options)
             log.debug("Pulled data object '%s' into cache to %s", rel_path, cache_path)
             return True
@@ -378,58 +460,74 @@
         """
         ipt_timer = ExecutionTimer()
         p = Path(rel_path)
         data_object_name = p.stem + p.suffix
         subcollection_name = p.parent
 
         source_file = source_file if source_file else self._get_cache_path(rel_path)
-        options = {kw.FORCE_FLAG_KW: '', kw.DEST_RESC_NAME_KW: self.resource}
+        options = {kw.FORCE_FLAG_KW: "", kw.DEST_RESC_NAME_KW: self.resource}
 
         if not os.path.exists(source_file):
-            log.error("Tried updating key '%s' from source file '%s', but source file does not exist.", rel_path, source_file)
+            log.error(
+                "Tried updating key '%s' from source file '%s', but source file does not exist.", rel_path, source_file
+            )
             return False
 
         # Check if the data object exists in iRODS
-        collection_path = f"{self.home}/{str(subcollection_name)}"
-        data_object_path = f"{collection_path}/{str(data_object_name)}"
+        collection_path = f"{self.home}/{subcollection_name}"
+        data_object_path = f"{collection_path}/{data_object_name}"
         exists = False
 
         try:
             exists = self.session.data_objects.exists(data_object_path)
 
             if os.path.getsize(source_file) == 0 and exists:
-                log.debug("Wanted to push file '%s' to iRODS collection '%s' but its size is 0; skipping.", source_file, rel_path)
+                log.debug(
+                    "Wanted to push file '%s' to iRODS collection '%s' but its size is 0; skipping.",
+                    source_file,
+                    rel_path,
+                )
                 return True
 
             # Create sub-collection first
             self.session.collections.create(collection_path, recurse=True, **options)
 
             if from_string:
                 # Create data object
                 data_obj = self.session.data_objects.create(data_object_path, self.resource, **options)
 
                 # Save 'from_string' as a file
-                with data_obj.open('w') as data_obj_fp:
+                with data_obj.open("w") as data_obj_fp:
                     data_obj_fp.write(from_string)
 
                 # Add file containing 'from_string' to the irods collection, since
                 # put() expects a file as input. Get file name from data object's 'desc' field
                 self.session.data_objects.put(data_obj.desc, f"{collection_path}/", **options)
 
                 log.debug("Pushed data from string '%s' to collection '%s'", from_string, data_object_path)
             else:
                 start_time = datetime.now()
-                log.debug("Pushing cache file '%s' of size %s bytes to collection '%s'", source_file, os.path.getsize(source_file), rel_path)
+                log.debug(
+                    "Pushing cache file '%s' of size %s bytes to collection '%s'",
+                    source_file,
+                    os.path.getsize(source_file),
+                    rel_path,
+                )
 
                 # Add the source file to the irods collection
                 self.session.data_objects.put(source_file, data_object_path, **options)
 
                 end_time = datetime.now()
-                log.debug("Pushed cache file '%s' to collection '%s' (%s bytes transfered in %s sec)",
-                        source_file, rel_path, os.path.getsize(source_file), (end_time - start_time).total_seconds())
+                log.debug(
+                    "Pushed cache file '%s' to collection '%s' (%s bytes transfered in %s sec)",
+                    source_file,
+                    rel_path,
+                    os.path.getsize(source_file),
+                    (end_time - start_time).total_seconds(),
+                )
             return True
         finally:
             log.debug("irods_pt _push_to_irods: %s", ipt_timer)
 
     def file_ready(self, obj, **kwargs):
         """
         A helper method that checks if a file corresponding to a dataset is
@@ -438,48 +536,52 @@
         ipt_timer = ExecutionTimer()
         rel_path = self._construct_path(obj, **kwargs)
         # Make sure the size in cache is available in its entirety
         if self._in_cache(rel_path):
             if os.path.getsize(self._get_cache_path(rel_path)) == self._get_size_in_irods(rel_path):
                 log.debug("irods_pt _file_ready: %s", ipt_timer)
                 return True
-            log.debug("Waiting for dataset %s to transfer from OS: %s/%s", rel_path,
-                      os.path.getsize(self._get_cache_path(rel_path)), self._get_size_in_irods(rel_path))
+            log.debug(
+                "Waiting for dataset %s to transfer from OS: %s/%s",
+                rel_path,
+                os.path.getsize(self._get_cache_path(rel_path)),
+                self._get_size_in_irods(rel_path),
+            )
         log.debug("irods_pt _file_ready: %s", ipt_timer)
         return False
 
     def _exists(self, obj, **kwargs):
         ipt_timer = ExecutionTimer()
         rel_path = self._construct_path(obj, **kwargs)
 
         # Check cache and irods
         if self._in_cache(rel_path) or self._data_object_exists(rel_path):
             log.debug("irods_pt _exists: %s", ipt_timer)
             return True
 
         # dir_only does not get synced so shortcut the decision
-        dir_only = kwargs.get('dir_only', False)
-        base_dir = kwargs.get('base_dir', None)
+        dir_only = kwargs.get("dir_only", False)
+        base_dir = kwargs.get("base_dir", None)
         if dir_only and base_dir:
             # for JOB_WORK directory
             if not os.path.exists(rel_path):
                 os.makedirs(rel_path, exist_ok=True)
             log.debug("irods_pt _exists: %s", ipt_timer)
             return True
         log.debug("irods_pt _exists: %s", ipt_timer)
         return False
 
     def _create(self, obj, **kwargs):
         ipt_timer = ExecutionTimer()
         if not self._exists(obj, **kwargs):
             # Pull out locally used fields
-            extra_dir = kwargs.get('extra_dir', None)
-            extra_dir_at_root = kwargs.get('extra_dir_at_root', False)
-            dir_only = kwargs.get('dir_only', False)
-            alt_name = kwargs.get('alt_name', None)
+            extra_dir = kwargs.get("extra_dir", None)
+            extra_dir_at_root = kwargs.get("extra_dir_at_root", False)
+            dir_only = kwargs.get("dir_only", False)
+            alt_name = kwargs.get("alt_name", None)
 
             # Construct hashed path
             rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
 
             # Optionally append extra_dir
             if extra_dir is not None:
                 if extra_dir_at_root:
@@ -490,24 +592,23 @@
             # Create given directory in cache
             cache_dir = os.path.join(self.staging_path, rel_path)
             if not os.path.exists(cache_dir):
                 os.makedirs(cache_dir, exist_ok=True)
 
             if not dir_only:
                 rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
-                open(os.path.join(self.staging_path, rel_path), 'w').close()
-                self._push_to_irods(rel_path, from_string='')
+                open(os.path.join(self.staging_path, rel_path), "w").close()
+                self._push_to_irods(rel_path, from_string="")
         log.debug("irods_pt _create: %s", ipt_timer)
 
     def _empty(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             return bool(self._size(obj, **kwargs) > 0)
         else:
-            raise ObjectNotFound('objectstore.empty, object does not exist: %s, kwargs: %s'
-                                 % (str(obj), str(kwargs)))
+            raise ObjectNotFound(f"objectstore.empty, object does not exist: {obj}, kwargs: {kwargs}")
 
     def _size(self, obj, **kwargs):
         ipt_timer = ExecutionTimer()
         rel_path = self._construct_path(obj, **kwargs)
         if self._in_cache(rel_path):
             try:
                 return os.path.getsize(self._get_cache_path(rel_path))
@@ -521,18 +622,18 @@
         log.warning("Did not find dataset '%s', returning 0 for size", rel_path)
         log.debug("irods_pt _size: %s", ipt_timer)
         return 0
 
     def _delete(self, obj, entire_dir=False, **kwargs):
         ipt_timer = ExecutionTimer()
         rel_path = self._construct_path(obj, **kwargs)
-        extra_dir = kwargs.get('extra_dir', None)
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        extra_dir = kwargs.get("extra_dir", None)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
 
         options = {kw.DEST_RESC_NAME_KW: self.resource}
 
         try:
             # Remove temparory data in JOB_WORK directory
             if base_dir and dir_only and obj_dir:
                 shutil.rmtree(os.path.abspath(rel_path))
@@ -541,15 +642,15 @@
             # For the case of extra_files, because we don't have a reference to
             # individual files we need to remove the entire directory structure
             # with all the files in it. This is easy for the local file system,
             # but requires iterating through each individual key in irods and deleing it.
             if entire_dir and extra_dir:
                 shutil.rmtree(self._get_cache_path(rel_path), ignore_errors=True)
 
-                col_path = f"{self.home}/{str(rel_path)}"
+                col_path = f"{self.home}/{rel_path}"
                 col = None
                 try:
                     col = self.session.collections.get(col_path)
                 except CollectionDoesNotExist:
                     log.warning("Collection (%s) does not exist!", col_path)
                     return False
 
@@ -569,27 +670,27 @@
                 # Delete from cache first
                 unlink(self._get_cache_path(rel_path), ignore_errors=True)
                 # Delete from irods as well
                 p = Path(rel_path)
                 data_object_name = p.stem + p.suffix
                 subcollection_name = p.parent
 
-                collection_path = f"{self.home}/{str(subcollection_name)}"
-                data_object_path = f"{collection_path}/{str(data_object_name)}"
+                collection_path = f"{self.home}/{subcollection_name}"
+                data_object_path = f"{collection_path}/{data_object_name}"
 
                 try:
                     data_obj = self.session.data_objects.get(data_object_path, **options)
                     # remove object
                     data_obj.unlink(force=True)
                     return True
                 except (DataObjectDoesNotExist, CollectionDoesNotExist):
                     log.info("Collection or data object (%s) does not exist", data_object_path)
                     return True
         except OSError:
-            log.exception('%s delete error', self._get_filename(obj, **kwargs))
+            log.exception("%s delete error", self._get_filename(obj, **kwargs))
         finally:
             log.debug("irods_pt _delete: %s", ipt_timer)
         return False
 
     def _get_data(self, obj, start=0, count=-1, **kwargs):
         ipt_timer = ExecutionTimer()
         rel_path = self._construct_path(obj, **kwargs)
@@ -602,17 +703,17 @@
         content = data_file.read(count)
         data_file.close()
         log.debug("irods_pt _get_data: %s", ipt_timer)
         return content
 
     def _get_filename(self, obj, **kwargs):
         ipt_timer = ExecutionTimer()
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         rel_path = self._construct_path(obj, **kwargs)
 
         # for JOB_WORK directory
         if base_dir and dir_only and obj_dir:
             log.debug("irods_pt _get_filename: %s", ipt_timer)
             return os.path.abspath(rel_path)
 
@@ -639,16 +740,15 @@
                     log.debug("irods_pt _get_filename: %s", ipt_timer)
                     return cache_path
         # For the case of retrieving a directory only, return the expected path
         # even if it does not exist.
         # if dir_only:
         #     return cache_path
         log.debug("irods_pt _get_filename: %s", ipt_timer)
-        raise ObjectNotFound('objectstore.get_filename, no cache_path: %s, kwargs: %s'
-                             % (str(obj), str(kwargs)))
+        raise ObjectNotFound(f"objectstore.get_filename, no cache_path: {obj}, kwargs: {kwargs}")
         # return cache_path # Until the upload tool does not explicitly create the dataset, return expected path
 
     def _update_from_file(self, obj, file_name=None, create=False, **kwargs):
         ipt_timer = ExecutionTimer()
         if create:
             self._create(obj, **kwargs)
         if self._exists(obj, **kwargs):
@@ -667,27 +767,26 @@
                     log.exception("Trouble copying source file '%s' to cache '%s'", source_file, cache_file)
             else:
                 source_file = self._get_cache_path(rel_path)
             # Update the file on iRODS
             self._push_to_irods(rel_path, source_file)
         else:
             log.debug("irods_pt _update_from_file: %s", ipt_timer)
-            raise ObjectNotFound('objectstore.update_from_file, object does not exist: %s, kwargs: %s'
-                                 % (str(obj), str(kwargs)))
+            raise ObjectNotFound(f"objectstore.update_from_file, object does not exist: {obj}, kwargs: {kwargs}")
         log.debug("irods_pt _update_from_file: %s", ipt_timer)
 
     # Unlike S3, url is not really applicable to iRODS
     def _get_object_url(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
 
             p = Path(rel_path)
             data_object_name = p.stem + p.suffix
             subcollection_name = p.parent
 
-            collection_path = f"{self.home}/{str(subcollection_name)}"
-            data_object_path = f"{collection_path}/{str(data_object_name)}"
+            collection_path = f"{self.home}/{subcollection_name}"
+            data_object_path = f"{collection_path}/{data_object_name}"
 
             return data_object_path
 
     def _get_store_usage_percent(self):
         return 0.0
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/pithos.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/pithos.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,159 +8,175 @@
 
 try:
     from kamaki.clients import (
         astakos,
         Client as KamakiClient,
         ClientError,
         pithos,
-        utils
+        utils,
     )
 except ImportError:
     KamakiClient = None
 
 from galaxy.exceptions import (
     ObjectInvalid,
-    ObjectNotFound
+    ObjectNotFound,
 )
 from galaxy.util import (
     directory_hash_id,
     umask_fix_perms,
 )
 from galaxy.util.path import safe_relpath
-from ..objectstore import ConcreteObjectStore
+from . import ConcreteObjectStore
 
 NO_KAMAKI_ERROR_MESSAGE = (
     "ObjectStore configured, but no kamaki.clients dependency available."
     "Please install and properly configure kamaki.clients or modify Object "
-    "Store configuration.")
+    "Store configuration."
+)
 
 log = logging.getLogger(__name__)
 
 
 def parse_config_xml(config_xml):
     """Parse and validate config_xml, return dict for convenience
     :param config_xml: (lxml.etree.Element) root of XML subtree
     :returns: (dict) according to syntax
     :raises: various XML parse errors
     """
     r = dict()
     try:
         for tag, required_attrs, optional_attrs in (
-                ('auth', ('url', 'token', ), ('ca_certs', 'ignore_ssl', )),
-                ('container', ('name', ), ('project', )), ):
+            (
+                "auth",
+                (
+                    "url",
+                    "token",
+                ),
+                (
+                    "ca_certs",
+                    "ignore_ssl",
+                ),
+            ),
+            ("container", ("name",), ("project",)),
+        ):
             element = config_xml.findall(tag)[0]
             required = tuple((k, element.get(k)) for k in required_attrs)
             for k, v in required:
                 if not v:
-                    msg = f'No value for {tag}:{k} in XML tree'
+                    msg = f"No value for {tag}:{k} in XML tree"
                     log.error(msg)
                     raise Exception(msg)
             optional = tuple((k, element.get(k)) for k in optional_attrs)
             r[tag] = dict(required + optional)
 
         # Extract extra_dir
-        tag, attrs = 'extra_dir', ('type', 'path')
+        tag, attrs = "extra_dir", ("type", "path")
         extra_dirs = config_xml.findall(tag)
         if not extra_dirs:
-            msg = f'No {tag} element in XML tree'
+            msg = f"No {tag} element in XML tree"
             log.error(msg)
             raise Exception(msg)
-        r['extra_dirs'] = [
-            {k: e.get(k) for k in attrs} for e in extra_dirs]
-        if 'job_work' not in (d['type'] for d in r['extra_dirs']):
+        r["extra_dirs"] = [{k: e.get(k) for k in attrs} for e in extra_dirs]
+        if "job_work" not in (d["type"] for d in r["extra_dirs"]):
             msg = f'No value for {tag}:type="job_work" in XML tree'
             log.error(msg)
             raise Exception(msg)
     except Exception:
-        log.exception(
-            "Malformed PithosObjectStore Configuration XML -- "
-            "unable to continue")
+        log.exception("Malformed PithosObjectStore Configuration XML -- " "unable to continue")
         raise
     return r
 
 
 class PithosObjectStore(ConcreteObjectStore):
     """
     Object store that stores objects as items in a Pithos+ container.
     Cache is ignored for the time being.
     """
-    store_type = 'pithos'
+
+    store_type = "pithos"
 
     def __init__(self, config, config_dict):
         super().__init__(config, config_dict)
         self.staging_path = self.config.file_path
-        log.info('Parse config_xml for pithos object store')
+        log.info("Parse config_xml for pithos object store")
         self.config_dict = config_dict
         log.debug(self.config_dict)
 
         self._initialize()
 
     def _initialize(self):
         if KamakiClient is None:
             raise Exception(NO_KAMAKI_ERROR_MESSAGE)
 
-        log.info('Authenticate Synnefo account')
+        log.info("Authenticate Synnefo account")
         self._authenticate()
-        log.info('Initialize Pithos+ client')
+        log.info("Initialize Pithos+ client")
         self._init_pithos()
 
     @classmethod
     def parse_xml(clazz, config_xml):
         return parse_config_xml(config_xml)
 
     def to_dict(self):
         as_dict = super().to_dict()
         as_dict.update(self.config_dict)
         return as_dict
 
     def _authenticate(self):
-        auth = self.config_dict['auth']
-        url, token = auth['url'], auth['token']
-        ca_certs = auth.get('ca_certs')
+        auth = self.config_dict["auth"]
+        url, token = auth["url"], auth["token"]
+        ca_certs = auth.get("ca_certs")
         if ca_certs:
             utils.https.patch_with_certs(ca_certs)
-        elif auth.get('ignore_ssl').lower() in ('true', 'yes', 'on'):
+        elif auth.get("ignore_ssl").lower() in ("true", "yes", "on"):
             utils.https.patch_ignore_ssl()
         self.astakos = astakos.AstakosClient(url, token)
 
     def _init_pithos(self):
-        uuid, token = self.astakos.user_term('id'), self.astakos.token
+        uuid, token = self.astakos.user_term("id"), self.astakos.token
         service_type = pithos.PithosClient.service_type
         pithos_url = self.astakos.get_endpoint_url(service_type)
-        container = self.config_dict['container']['name']
+        container = self.config_dict["container"]["name"]
         self.pithos = pithos.PithosClient(pithos_url, token, uuid, container)
 
         # Create container if not exist, or reassign to named project
-        project = self.config_dict['container'].get('project', None)
+        project = self.config_dict["container"].get("project", None)
         try:
             c = self.pithos.get_container_info()
         except ClientError as ce:
-            if ce.status not in (404, ):
+            if ce.status not in (404,):
                 raise
             c = self.pithos.create_container(project_id=project)
             return
-        if project and c.get('x-container-policy-project') != project:
+        if project and c.get("x-container-policy-project") != project:
             self.pithos.reassign_container(project)
 
     def _construct_path(
-            self, obj,
-            base_dir=None, dir_only=None, extra_dir=None,
-            extra_dir_at_root=False, alt_name=None, obj_dir=False, **kwargs):
+        self,
+        obj,
+        base_dir=None,
+        dir_only=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        **kwargs,
+    ):
         """Construct path from object and parameters"""
         # param extra_dir: should never be constructed from provided data but
         # just make sure there are no shenannigans afoot
         if extra_dir and extra_dir != os.path.normpath(extra_dir):
-            log.warning(f'extra_dir is not normalized: {extra_dir}')
+            log.warning(f"extra_dir is not normalized: {extra_dir}")
             raise ObjectInvalid("The requested object is invalid")
         # ensure that any parent directory references in alt_name would not
         # result in a path not contained in the directory path constructed here
         if alt_name:
             if not safe_relpath(alt_name):
-                log.warning(
-                    f'alt_name would locate path outside dir: {alt_name}')
+                log.warning(f"alt_name would locate path outside dir: {alt_name}")
                 raise ObjectInvalid("The requested object is invalid")
             # alt_name can contain parent directory references, but S3 will not
             # follow them, so if they are valid we normalize them out
             alt_name = os.path.normpath(alt_name)
         rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
         if extra_dir is not None:
             if extra_dir_at_root:
@@ -172,42 +188,41 @@
         if obj_dir:
             rel_path = os.path.join(rel_path, str(self._get_object_id(obj)))
         if base_dir:
             base = self.extra_dirs.get(base_dir)
             return os.path.join(base, rel_path)
 
         # Pithos+ folders are marked by having trailing '/' so add it now
-        rel_path = f'{rel_path}/'
+        rel_path = f"{rel_path}/"
 
         if not dir_only:
-            an = alt_name if alt_name else f'dataset_{self._get_object_id(obj)}.dat'
+            an = alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat"
             rel_path = os.path.join(rel_path, an)
         return rel_path
 
     def _get_cache_path(self, rel_path):
         return os.path.abspath(os.path.join(self.staging_path, rel_path))
 
     def _in_cache(self, rel_path):
         """Check if the given dataset is in the local cache and return True if
-           so.
+        so.
         """
         cache_path = self._get_cache_path(rel_path)
         return os.path.exists(cache_path)
 
     def _fix_permissions(self, rel_path):
-        """ Set permissions on rel_path"""
+        """Set permissions on rel_path"""
         for basedir, _, files in os.walk(rel_path):
             umask_fix_perms(basedir, self.config.umask, 0o777, self.config.gid)
             for filename in files:
                 path = os.path.join(basedir, filename)
                 # Ignore symlinks
                 if os.path.islink(path):
                     continue
-                umask_fix_perms(
-                    path, self.config.umask, 0o666, self.config.gid)
+                umask_fix_perms(path, self.config.umask, 0o666, self.config.gid)
 
     def _pull_into_cache(self, rel_path):
         # Ensure the cache directory structure exists (e.g., dataset_#_files/)
         rel_path_dir = os.path.dirname(rel_path)
         rel_cache_path_dir = self._get_cache_path(rel_path_dir)
         if not os.path.exists(rel_cache_path_dir):
             os.makedirs(self._get_cache_path(rel_path_dir), exist_ok=True)
@@ -224,21 +239,21 @@
         :returns: weather the file exists remotely or in cache
         """
         path = self._construct_path(obj, **kwargs)
         try:
             self.pithos.get_object_info(path)
             return True
         except ClientError as ce:
-            if ce.status not in (404, ):
+            if ce.status not in (404,):
                 raise
 
         in_cache = self._in_cache(path)
-        dir_only = kwargs.get('dir_only', False)
+        dir_only = kwargs.get("dir_only", False)
         if dir_only:
-            base_dir = kwargs.get('base_dir', None)
+            base_dir = kwargs.get("base_dir", None)
             if in_cache:
                 return True
             elif base_dir:  # for JOB_WORK directory
                 if not os.path.exists(path):
                     os.makedirs(path, exist_ok=True)
                 return True
             return False
@@ -251,18 +266,18 @@
             return True
         return False
 
     def _create(self, obj, **kwargs):
         """Touch a file (aka create empty), if it doesn't exist"""
         if not self._exists(obj, **kwargs):
             # Pull out locally used fields
-            extra_dir = kwargs.get('extra_dir', None)
-            extra_dir_at_root = kwargs.get('extra_dir_at_root', False)
-            dir_only = kwargs.get('dir_only', False)
-            alt_name = kwargs.get('alt_name', None)
+            extra_dir = kwargs.get("extra_dir", None)
+            extra_dir_at_root = kwargs.get("extra_dir_at_root", False)
+            dir_only = kwargs.get("dir_only", False)
+            alt_name = kwargs.get("alt_name", None)
 
             # Construct hashed path
             rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
 
             # Optionally append extra_dir
             if extra_dir is not None:
                 if extra_dir_at_root:
@@ -272,85 +287,81 @@
 
             # Create given directory in cache
             cache_dir = os.path.join(self.staging_path, rel_path)
             if not os.path.exists(cache_dir):
                 os.makedirs(cache_dir, exist_ok=True)
 
             if dir_only:
-                self.pithos.upload_from_string(
-                    rel_path, '', content_type='application/directory')
+                self.pithos.upload_from_string(rel_path, "", content_type="application/directory")
             else:
-                rel_path = os.path.join(
-                    rel_path,
-                    alt_name if alt_name else f'dataset_{self._get_object_id(obj)}.dat')
+                rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
                 new_file = os.path.join(self.staging_path, rel_path)
-                open(new_file, 'w').close()
-                self.pithos.upload_from_string(rel_path, '')
+                open(new_file, "w").close()
+                self.pithos.upload_from_string(rel_path, "")
 
     def _empty(self, obj, **kwargs):
         """
         :returns: weather the object has content
         :raises ObjectNotFound:
         """
         if not self._exists(obj, **kwargs):
-            raise ObjectNotFound(
-                f'objectstore.empty, object does not exist: {obj}, kwargs: {kwargs}')
+            raise ObjectNotFound(f"objectstore.empty, object does not exist: {obj}, kwargs: {kwargs}")
         return bool(self._size(obj, **kwargs))
 
     def _size(self, obj, **kwargs):
         """
         :returns: The size of the object, or 0 if it doesn't exist (sorry for
             that, not our fault, the ObjectStore interface is like that some
             times)
         """
         path = self._construct_path(obj, **kwargs)
         if self._in_cache(path):
             try:
                 return os.path.getsize(self._get_cache_path(path))
             except OSError as ex:
                 log.warning(
-                    'Could not get size of file {path} in local cache,'
-                    'will try Pithos. Error: {err}'.format(path=path, err=ex))
+                    "Could not get size of file {path} in local cache,"
+                    "will try Pithos. Error: {err}".format(path=path, err=ex)
+                )
         try:
             file = self.pithos.get_object_info(path)
         except ClientError as ce:
-            if ce.status not in (404, ):
+            if ce.status not in (404,):
                 raise
             return 0
-        return int(file['content-length'])
+        return int(file["content-length"])
 
     def _delete(self, obj, **kwargs):
         """Delete the object
         :returns: weather the object was deleted
         """
         path = self._construct_path(obj, **kwargs)
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         try:
             if all((base_dir, dir_only, obj_dir)):
                 shutil.rmtree(os.path.abspath(path))
                 return True
             cache_path = self._get_cache_path(path)
 
-            entire_dir = kwargs.get('entire_dir', False)
-            extra_dir = kwargs.get('extra_dir', False)
+            entire_dir = kwargs.get("entire_dir", False)
+            extra_dir = kwargs.get("extra_dir", False)
             if entire_dir and extra_dir:
                 shutil.rmtree(cache_path)
-                log.debug(f'On Pithos: delete -r {path}/')
-                self.pithos.del_object(path, delimiter='/')
+                log.debug(f"On Pithos: delete -r {path}/")
+                self.pithos.del_object(path, delimiter="/")
                 return True
             else:
                 os.unlink(cache_path)
                 self.pithos.del_object(path)
         except OSError:
-            log.exception(
-                f'{self._get_filename(obj, **kwargs)} delete error')
+            log.exception(f"{self._get_filename(obj, **kwargs)} delete error")
         except ClientError as ce:
-            log.exception(f'Could not delete {path} from Pithos, {ce}')
+            log.exception(f"Could not delete {path} from Pithos, {ce}")
         return False
 
     def _get_data(self, obj, start=0, count=-1, **kwargs):
         """Fetch (e.g., download) data
         :param start: Chunk of data starts here
         :param count: Fetch at most as many data, fetch all if negative
         """
@@ -363,17 +374,17 @@
         data_file.seek(start)
         content = data_file.read(count)
         data_file.close()
         return content
 
     def _get_filename(self, obj, **kwargs):
         """Get the expected filename with absolute path"""
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         path = self._construct_path(obj, **kwargs)
 
         # for JOB_WORK directory
         if base_dir and dir_only and obj_dir:
             return os.path.abspath(path)
         cache_path = self._get_cache_path(path)
         if dir_only:
@@ -382,60 +393,60 @@
             return cache_path
         if self._in_cache(path):
             return cache_path
         elif self._exists(obj, **kwargs):
             if not dir_only:
                 self._pull_into_cache(path)
                 return cache_path
-        raise ObjectNotFound(
-            f'objectstore.get_filename, no cache_path: {obj}, kwargs: {kwargs}')
+        raise ObjectNotFound(f"objectstore.get_filename, no cache_path: {obj}, kwargs: {kwargs}")
 
     def _update_from_file(self, obj, **kwargs):
         """Update the store when a file is updated"""
-        if kwargs.get('create'):
+        if kwargs.get("create"):
             self._create(obj, **kwargs)
         if not self._exists(obj, **kwargs):
             raise ObjectNotFound(
-                'objectstore.update_from_file, object does not exist: {obj}, '
-                'kwargs: {kwargs}'.format(obj=obj, kwargs=kwargs))
+                "objectstore.update_from_file, object does not exist: {obj}, "
+                "kwargs: {kwargs}".format(obj=obj, kwargs=kwargs)
+            )
 
         path = self._construct_path(obj, **kwargs)
         cache_path = self._get_cache_path(path)
-        file_name = kwargs.get('file_name')
+        file_name = kwargs.get("file_name")
         if file_name:
             source_path = os.path.abspath(file_name)
             try:
                 if source_path != cache_path:
                     shutil.copy2(source_path, cache_path)
                 self._fix_permissions(cache_path)
             except OSError:
                 log.exception(
                     'Trouble copying source file "{source}" to cache "{cache}"'
-                    ''.format(source=source_path, cache=cache_path))
+                    "".format(source=source_path, cache=cache_path)
+                )
         else:
             with open(cache_path) as f:
                 self.pithos.upload_object(obj, f)
 
     def _get_object_url(self, obj, **kwargs):
         """
         :returns: URL for direct access, None if no object
         """
         if self._exists(obj, **kwargs):
             path = self._construct_path(obj, **kwargs)
             try:
                 return self.pithos.publish_object(path)
             except ClientError as ce:
-                log.exception(
-                    f'Trouble generating URL for dataset "{path}"')
-                log.exception(f'Kamaki: {ce}')
+                log.exception(f'Trouble generating URL for dataset "{path}"')
+                log.exception(f"Kamaki: {ce}")
         return None
 
     def _get_store_usage_percent(self):
         """
         :returns: percentage indicating how full the store is
         """
         quotas = self.astakos.get_quotas()
-        project = self.config_dict['container']['project']
-        pithos_quotas = quotas[project]['pithos.diskspace']
-        usage = pithos_quotas['usage']
-        limit = min(pithos_quotas['limit'], pithos_quotas['project_limit'])
+        project = self.config_dict["container"]["project"]
+        pithos_quotas = quotas[project]["pithos.diskspace"]
+        usage = pithos_quotas["usage"]
+        limit = min(pithos_quotas["limit"], pithos_quotas["project_limit"])
         return (100.0 * usage) / limit
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/pulsar.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/pulsar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..objectstore import BaseObjectStore
+from . import BaseObjectStore
 
 try:
     from pulsar.client.manager import ObjectStoreClientManager
 except ImportError:
     ObjectStoreClientManager = None
 
 
@@ -55,15 +55,15 @@
     def _get_store_usage_percent(self):
         return self.pulsar_client.get_store_usage_percent()
 
     def _get_object_url(self, obj, extra_dir=None, extra_dir_at_root=False, alt_name=None):
         return None
 
     def __build_kwds(self, obj, **kwds):
-        kwds['object_id'] = obj.id
+        kwds["object_id"] = obj.id
         return kwds
 
     def __build_pulsar_client(self, config_xml):
         if ObjectStoreClientManager is None:
             raise Exception("Pulsar client code not available, cannot use this module.")
         url = config_xml.get("url")
         private_token = config_xml.get("private_token", None)
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/s3.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,186 +15,195 @@
     import boto
     from boto.exception import S3ResponseError
     from boto.s3.connection import S3Connection
     from boto.s3.key import Key
 except ImportError:
     boto = None  # type: ignore[assignment]
 
-from galaxy.exceptions import ObjectInvalid, ObjectNotFound
+from galaxy.exceptions import (
+    ObjectInvalid,
+    ObjectNotFound,
+)
 from galaxy.util import (
     directory_hash_id,
     string_as_bool,
     umask_fix_perms,
     unlink,
     which,
 )
 from galaxy.util.path import safe_relpath
 from galaxy.util.sleeper import Sleeper
+from . import (
+    ConcreteObjectStore,
+    convert_bytes,
+)
 from .s3_multipart_upload import multipart_upload
-from ..objectstore import ConcreteObjectStore, convert_bytes
 
-NO_BOTO_ERROR_MESSAGE = ("S3/Swift object store configured, but no boto dependency available."
-                         "Please install and properly configure boto or modify object store configuration.")
+NO_BOTO_ERROR_MESSAGE = (
+    "S3/Swift object store configured, but no boto dependency available."
+    "Please install and properly configure boto or modify object store configuration."
+)
 
 log = logging.getLogger(__name__)
-logging.getLogger('boto').setLevel(logging.INFO)  # Otherwise boto is quite noisy
+logging.getLogger("boto").setLevel(logging.INFO)  # Otherwise boto is quite noisy
 
 
 def parse_config_xml(config_xml):
     try:
-        a_xml = config_xml.findall('auth')[0]
-        access_key = a_xml.get('access_key')
-        secret_key = a_xml.get('secret_key')
-
-        b_xml = config_xml.findall('bucket')[0]
-        bucket_name = b_xml.get('name')
-        use_rr = string_as_bool(b_xml.get('use_reduced_redundancy', "False"))
-        max_chunk_size = int(b_xml.get('max_chunk_size', 250))
+        a_xml = config_xml.findall("auth")[0]
+        access_key = a_xml.get("access_key")
+        secret_key = a_xml.get("secret_key")
+
+        b_xml = config_xml.findall("bucket")[0]
+        bucket_name = b_xml.get("name")
+        use_rr = string_as_bool(b_xml.get("use_reduced_redundancy", "False"))
+        max_chunk_size = int(b_xml.get("max_chunk_size", 250))
 
-        cn_xml = config_xml.findall('connection')
+        cn_xml = config_xml.findall("connection")
         if not cn_xml:
             cn_xml = {}
         else:
             cn_xml = cn_xml[0]
 
-        host = cn_xml.get('host', None)
-        port = int(cn_xml.get('port', 6000))
-        multipart = string_as_bool(cn_xml.get('multipart', 'True'))
-        is_secure = string_as_bool(cn_xml.get('is_secure', 'True'))
-        conn_path = cn_xml.get('conn_path', '/')
+        host = cn_xml.get("host", None)
+        port = int(cn_xml.get("port", 6000))
+        multipart = string_as_bool(cn_xml.get("multipart", "True"))
+        is_secure = string_as_bool(cn_xml.get("is_secure", "True"))
+        conn_path = cn_xml.get("conn_path", "/")
 
-        c_xml = config_xml.findall('cache')[0]
-        cache_size = float(c_xml.get('size', -1))
+        c_xml = config_xml.findall("cache")[0]
+        cache_size = float(c_xml.get("size", -1))
 
-        staging_path = c_xml.get('path', None)
+        staging_path = c_xml.get("path", None)
 
-        tag, attrs = 'extra_dir', ('type', 'path')
+        tag, attrs = "extra_dir", ("type", "path")
         extra_dirs = config_xml.findall(tag)
         if not extra_dirs:
-            msg = f'No {tag} element in XML tree'
+            msg = f"No {tag} element in XML tree"
             log.error(msg)
             raise Exception(msg)
         extra_dirs = [{k: e.get(k) for k in attrs} for e in extra_dirs]
 
         return {
-            'auth': {
-                'access_key': access_key,
-                'secret_key': secret_key,
+            "auth": {
+                "access_key": access_key,
+                "secret_key": secret_key,
             },
-            'bucket': {
-                'name': bucket_name,
-                'use_reduced_redundancy': use_rr,
-                'max_chunk_size': max_chunk_size,
+            "bucket": {
+                "name": bucket_name,
+                "use_reduced_redundancy": use_rr,
+                "max_chunk_size": max_chunk_size,
             },
-            'connection': {
-                'host': host,
-                'port': port,
-                'multipart': multipart,
-                'is_secure': is_secure,
-                'conn_path': conn_path,
+            "connection": {
+                "host": host,
+                "port": port,
+                "multipart": multipart,
+                "is_secure": is_secure,
+                "conn_path": conn_path,
             },
-            'cache': {
-                'size': cache_size,
-                'path': staging_path,
+            "cache": {
+                "size": cache_size,
+                "path": staging_path,
             },
-            'extra_dirs': extra_dirs,
+            "extra_dirs": extra_dirs,
         }
     except Exception:
         # Toss it back up after logging, we can't continue loading at this point.
         log.exception("Malformed ObjectStore Configuration XML -- unable to continue")
         raise
 
 
 class CloudConfigMixin:
-
     def _config_to_dict(self):
         return {
-            'auth': {
-                'access_key': self.access_key,
-                'secret_key': self.secret_key,
+            "auth": {
+                "access_key": self.access_key,
+                "secret_key": self.secret_key,
             },
-            'bucket': {
-                'name': self.bucket,
-                'use_reduced_redundancy': self.use_rr,
+            "bucket": {
+                "name": self.bucket,
+                "use_reduced_redundancy": self.use_rr,
             },
-            'connection': {
-                'host': self.host,
-                'port': self.port,
-                'multipart': self.multipart,
-                'is_secure': self.is_secure,
-                'conn_path': self.conn_path,
+            "connection": {
+                "host": self.host,
+                "port": self.port,
+                "multipart": self.multipart,
+                "is_secure": self.is_secure,
+                "conn_path": self.conn_path,
             },
-            'cache': {
-                'size': self.cache_size,
-                'path': self.staging_path,
+            "cache": {
+                "size": self.cache_size,
+                "path": self.staging_path,
             },
-            'enable_cache_monitor': False,
+            "enable_cache_monitor": False,
         }
 
 
 class S3ObjectStore(ConcreteObjectStore, CloudConfigMixin):
     """
     Object store that stores objects as items in an AWS S3 bucket. A local
     cache exists that is used as an intermediate location for files between
     Galaxy and S3.
     """
-    store_type = 's3'
+
+    store_type = "s3"
 
     def __init__(self, config, config_dict):
         super().__init__(config, config_dict)
 
         self.transfer_progress = 0
 
-        auth_dict = config_dict['auth']
-        bucket_dict = config_dict['bucket']
-        connection_dict = config_dict.get('connection', {})
-        cache_dict = config_dict['cache']
-        self.enable_cache_monitor = config_dict.get('enable_cache_monitor', True)
-
-        self.access_key = auth_dict.get('access_key')
-        self.secret_key = auth_dict.get('secret_key')
-
-        self.bucket = bucket_dict.get('name')
-        self.use_rr = bucket_dict.get('use_reduced_redundancy', False)
-        self.max_chunk_size = bucket_dict.get('max_chunk_size', 250)
-
-        self.host = connection_dict.get('host', None)
-        self.port = connection_dict.get('port', 6000)
-        self.multipart = connection_dict.get('multipart', True)
-        self.is_secure = connection_dict.get('is_secure', True)
-        self.conn_path = connection_dict.get('conn_path', '/')
+        auth_dict = config_dict["auth"]
+        bucket_dict = config_dict["bucket"]
+        connection_dict = config_dict.get("connection", {})
+        cache_dict = config_dict["cache"]
+        self.enable_cache_monitor = config_dict.get("enable_cache_monitor", True)
+
+        self.access_key = auth_dict.get("access_key")
+        self.secret_key = auth_dict.get("secret_key")
+
+        self.bucket = bucket_dict.get("name")
+        self.use_rr = bucket_dict.get("use_reduced_redundancy", False)
+        self.max_chunk_size = bucket_dict.get("max_chunk_size", 250)
+
+        self.host = connection_dict.get("host", None)
+        self.port = connection_dict.get("port", 6000)
+        self.multipart = connection_dict.get("multipart", True)
+        self.is_secure = connection_dict.get("is_secure", True)
+        self.conn_path = connection_dict.get("conn_path", "/")
 
-        self.cache_size = cache_dict.get('size', -1)
-        self.staging_path = cache_dict.get('path') or self.config.object_store_cache_path
+        self.cache_size = cache_dict.get("size", -1)
+        self.staging_path = cache_dict.get("path") or self.config.object_store_cache_path
 
-        extra_dirs = {
-            e['type']: e['path'] for e in config_dict.get('extra_dirs', [])}
+        extra_dirs = {e["type"]: e["path"] for e in config_dict.get("extra_dirs", [])}
         self.extra_dirs.update(extra_dirs)
 
         self._initialize()
 
     def _initialize(self):
         if boto is None:
             raise Exception(NO_BOTO_ERROR_MESSAGE)
 
         # for multipart upload
-        self.s3server = {'access_key': self.access_key,
-                         'secret_key': self.secret_key,
-                         'is_secure': self.is_secure,
-                         'max_chunk_size': self.max_chunk_size,
-                         'host': self.host,
-                         'port': self.port,
-                         'use_rr': self.use_rr,
-                         'conn_path': self.conn_path}
+        self.s3server = {
+            "access_key": self.access_key,
+            "secret_key": self.secret_key,
+            "is_secure": self.is_secure,
+            "max_chunk_size": self.max_chunk_size,
+            "host": self.host,
+            "port": self.port,
+            "use_rr": self.use_rr,
+            "conn_path": self.conn_path,
+        }
 
         self._configure_connection()
         self._bucket = self._get_bucket(self.bucket)
         self.start_cache_monitor()
         # Test if 'axel' is available for parallel download and pull the key into cache
-        if which('axel'):
+        if which("axel"):
             self.use_axel = True
         else:
             self.use_axel = False
 
     def start_cache_monitor(self):
         # Clean cache only if value is set in galaxy.ini
         if self.cache_size != -1 and self.enable_cache_monitor:
@@ -240,26 +249,29 @@
                     file_tuple = last_access_time, filepath, file_size
                     file_list.append(file_tuple)
             # Sort the file list (based on access time)
             file_list.sort()
             # Initiate cleaning once within 10% of the defined cache size?
             cache_limit = self.cache_size * 0.9
             if total_size > cache_limit:
-                log.info("Initiating cache cleaning: current cache size: %s; clean until smaller than: %s",
-                         convert_bytes(total_size), convert_bytes(cache_limit))
+                log.info(
+                    "Initiating cache cleaning: current cache size: %s; clean until smaller than: %s",
+                    convert_bytes(total_size),
+                    convert_bytes(cache_limit),
+                )
                 # How much to delete? If simply deleting up to the cache-10% limit,
                 # is likely to be deleting frequently and may run the risk of hitting
                 # the limit - maybe delete additional #%?
                 # For now, delete enough to leave at least 10% of the total cache free
                 delete_this_much = total_size - cache_limit
                 self.__clean_cache(file_list, delete_this_much)
             self.sleeper.sleep(30)  # Test cache size every 30 seconds?
 
     def __clean_cache(self, file_list, delete_this_much):
-        """ Keep deleting files from the file_list until the size of the deleted
+        """Keep deleting files from the file_list until the size of the deleted
         files is greater than the value in delete_this_much parameter.
 
         :type file_list: list
         :param file_list: List of candidate files that can be deleted. This method
             will start deleting files from the beginning of the list so the list
             should be sorted accordingly. The list must contains 3-element tuples,
             positioned as follows: position 0 holds file last accessed timestamp
@@ -284,16 +296,16 @@
                 #     % (i, file_name, convert_bytes(f[2]), file_date, \
                 #     convert_bytes(deleted_amount), convert_bytes(delete_this_much)))
             else:
                 log.debug("Cache cleaning done. Total space freed: %s", convert_bytes(deleted_amount))
                 return
 
     def _get_bucket(self, bucket_name):
-        """ Sometimes a handle to a bucket is not established right away so try
-        it a few times. Raise error is connection is not established. """
+        """Sometimes a handle to a bucket is not established right away so try
+        it a few times. Raise error is connection is not established."""
         for i in range(5):
             try:
                 bucket = self.conn.get_bucket(bucket_name)
                 log.debug("Using cloud object store with bucket '%s'", bucket.name)
                 return bucket
             except S3ResponseError:
                 try:
@@ -303,35 +315,45 @@
                     log.exception("Could not get bucket '%s', attempt %s/5", bucket_name, i + 1)
                     time.sleep(2)
         # All the attempts have been exhausted and connection was not established,
         # raise error
         raise S3ResponseError
 
     def _fix_permissions(self, rel_path):
-        """ Set permissions on rel_path"""
+        """Set permissions on rel_path"""
         for basedir, _, files in os.walk(rel_path):
             umask_fix_perms(basedir, self.config.umask, 0o777, self.config.gid)
             for filename in files:
                 path = os.path.join(basedir, filename)
                 # Ignore symlinks
                 if os.path.islink(path):
                     continue
                 umask_fix_perms(path, self.config.umask, 0o666, self.config.gid)
 
-    def _construct_path(self, obj, base_dir=None, dir_only=None, extra_dir=None, extra_dir_at_root=False, alt_name=None, obj_dir=False, **kwargs):
+    def _construct_path(
+        self,
+        obj,
+        base_dir=None,
+        dir_only=None,
+        extra_dir=None,
+        extra_dir_at_root=False,
+        alt_name=None,
+        obj_dir=False,
+        **kwargs,
+    ):
         # extra_dir should never be constructed from provided data but just
         # make sure there are no shenannigans afoot
         if extra_dir and extra_dir != os.path.normpath(extra_dir):
-            log.warning('extra_dir is not normalized: %s', extra_dir)
+            log.warning("extra_dir is not normalized: %s", extra_dir)
             raise ObjectInvalid("The requested object is invalid")
         # ensure that any parent directory references in alt_name would not
         # result in a path not contained in the directory path constructed here
         if alt_name:
             if not safe_relpath(alt_name):
-                log.warning('alt_name would locate path outside dir: %s', alt_name)
+                log.warning("alt_name would locate path outside dir: %s", alt_name)
                 raise ObjectInvalid("The requested object is invalid")
             # alt_name can contain parent directory references, but S3 will not
             # follow them, so if they are valid we normalize them out
             alt_name = os.path.normpath(alt_name)
         rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
         if extra_dir is not None:
             if extra_dir_at_root:
@@ -343,15 +365,15 @@
         if obj_dir:
             rel_path = os.path.join(rel_path, str(self._get_object_id(obj)))
         if base_dir:
             base = self.extra_dirs.get(base_dir)
             return os.path.join(base, rel_path)
 
         # S3 folders are marked by having trailing '/' so add it now
-        rel_path = f'{rel_path}/'
+        rel_path = f"{rel_path}/"
 
         if not dir_only:
             rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
         return rel_path
 
     def _get_cache_path(self, rel_path):
         return os.path.abspath(os.path.join(self.staging_path, rel_path))
@@ -368,15 +390,15 @@
             log.exception("Could not get size of key '%s' from S3", rel_path)
             return -1
 
     def _key_exists(self, rel_path):
         exists = False
         try:
             # A hackish way of testing if the rel_path is a folder vs a file
-            is_dir = rel_path[-1] == '/'
+            is_dir = rel_path[-1] == "/"
             if is_dir:
                 keyresult = self._bucket.get_all_keys(prefix=rel_path)
                 if len(keyresult) > 0:
                     exists = True
                 else:
                     exists = False
             else:
@@ -384,15 +406,15 @@
                 exists = key.exists()
         except S3ResponseError:
             log.exception("Trouble checking existence of S3 key '%s'", rel_path)
             return False
         return exists
 
     def _in_cache(self, rel_path):
-        """ Check if the given dataset is in the local cache and return True if so. """
+        """Check if the given dataset is in the local cache and return True if so."""
         # log.debug("------ Checking cache for rel_path %s" % rel_path)
         cache_path = self._get_cache_path(rel_path)
         return os.path.exists(cache_path)
         # TODO: Part of checking if a file is in cache should be to ensure the
         # size of the cached file matches that on S3. Once the upload tool explicitly
         # creates, this check sould be implemented- in the mean time, it's not
         # looking likely to be implementable reliably.
@@ -429,24 +451,32 @@
     def _transfer_cb(self, complete, total):
         self.transfer_progress += 10
 
     def _download(self, rel_path):
         try:
             log.debug("Pulling key '%s' into cache to %s", rel_path, self._get_cache_path(rel_path))
             key = self._bucket.get_key(rel_path)
+            if key is None:
+                message = f"Attempting to download an invalid key for path {rel_path}."
+                log.critical(message)
+                raise Exception(message)
             # Test if cache is large enough to hold the new file
             if self.cache_size > 0 and key.size > self.cache_size:
-                log.critical("File %s is larger (%s) than the cache size (%s). Cannot download.",
-                             rel_path, key.size, self.cache_size)
+                log.critical(
+                    "File %s is larger (%s) than the cache size (%s). Cannot download.",
+                    rel_path,
+                    key.size,
+                    self.cache_size,
+                )
                 return False
             if self.use_axel:
                 log.debug("Parallel pulled key '%s' into cache to %s", rel_path, self._get_cache_path(rel_path))
                 ncores = multiprocessing.cpu_count()
                 url = key.generate_url(7200)
-                ret_code = subprocess.call(['axel', '-a', '-n', str(ncores), url])
+                ret_code = subprocess.call(["axel", "-a", "-n", str(ncores), url])
                 if ret_code == 0:
                     return True
             else:
                 log.debug("Pulled key '%s' into cache to %s", rel_path, self._get_cache_path(rel_path))
                 self.transfer_progress = 0  # Reset transfer progress counter
                 key.get_contents_to_filename(self._get_cache_path(rel_path), cb=self._transfer_cb, num_cb=10)
                 return True
@@ -463,38 +493,52 @@
         the string.
         """
         try:
             source_file = source_file if source_file else self._get_cache_path(rel_path)
             if os.path.exists(source_file):
                 key = Key(self._bucket, rel_path)
                 if os.path.getsize(source_file) == 0 and key.exists():
-                    log.debug("Wanted to push file '%s' to S3 key '%s' but its size is 0; skipping.", source_file, rel_path)
+                    log.debug(
+                        "Wanted to push file '%s' to S3 key '%s' but its size is 0; skipping.", source_file, rel_path
+                    )
                     return True
                 if from_string:
                     key.set_contents_from_string(from_string, reduced_redundancy=self.use_rr)
                     log.debug("Pushed data from string '%s' to key '%s'", from_string, rel_path)
                 else:
                     start_time = datetime.now()
-                    log.debug("Pushing cache file '%s' of size %s bytes to key '%s'", source_file, os.path.getsize(source_file), rel_path)
+                    log.debug(
+                        "Pushing cache file '%s' of size %s bytes to key '%s'",
+                        source_file,
+                        os.path.getsize(source_file),
+                        rel_path,
+                    )
                     mb_size = os.path.getsize(source_file) / 1e6
                     if mb_size < 10 or (not self.multipart):
                         self.transfer_progress = 0  # Reset transfer progress counter
-                        key.set_contents_from_filename(source_file,
-                                                       reduced_redundancy=self.use_rr,
-                                                       cb=self._transfer_cb,
-                                                       num_cb=10)
+                        key.set_contents_from_filename(
+                            source_file, reduced_redundancy=self.use_rr, cb=self._transfer_cb, num_cb=10
+                        )
                     else:
                         multipart_upload(self.s3server, self._bucket, key.name, source_file, mb_size)
                     end_time = datetime.now()
-                    log.debug("Pushed cache file '%s' to key '%s' (%s bytes transfered in %s sec)",
-                              source_file, rel_path, os.path.getsize(source_file), end_time - start_time)
+                    log.debug(
+                        "Pushed cache file '%s' to key '%s' (%s bytes transfered in %s sec)",
+                        source_file,
+                        rel_path,
+                        os.path.getsize(source_file),
+                        end_time - start_time,
+                    )
                 return True
             else:
-                log.error("Tried updating key '%s' from source file '%s', but source file does not exist.",
-                          rel_path, source_file)
+                log.error(
+                    "Tried updating key '%s' from source file '%s', but source file does not exist.",
+                    rel_path,
+                    source_file,
+                )
         except S3ResponseError:
             log.exception("Trouble pushing S3 key '%s' from file '%s'", rel_path, source_file)
             raise
         return False
 
     def file_ready(self, obj, **kwargs):
         """
@@ -502,31 +546,35 @@
         ready and available to be used. Return ``True`` if so, ``False`` otherwise.
         """
         rel_path = self._construct_path(obj, **kwargs)
         # Make sure the size in cache is available in its entirety
         if self._in_cache(rel_path):
             if os.path.getsize(self._get_cache_path(rel_path)) == self._get_size_in_s3(rel_path):
                 return True
-            log.debug("Waiting for dataset %s to transfer from OS: %s/%s", rel_path,
-                      os.path.getsize(self._get_cache_path(rel_path)), self._get_size_in_s3(rel_path))
+            log.debug(
+                "Waiting for dataset %s to transfer from OS: %s/%s",
+                rel_path,
+                os.path.getsize(self._get_cache_path(rel_path)),
+                self._get_size_in_s3(rel_path),
+            )
         return False
 
     def _exists(self, obj, **kwargs):
         in_cache = in_s3 = False
         rel_path = self._construct_path(obj, **kwargs)
 
         # Check cache
         if self._in_cache(rel_path):
             in_cache = True
         # Check S3
         in_s3 = self._key_exists(rel_path)
         # log.debug("~~~~~~ File '%s' exists in cache: %s; in s3: %s" % (rel_path, in_cache, in_s3))
         # dir_only does not get synced so shortcut the decision
-        dir_only = kwargs.get('dir_only', False)
-        base_dir = kwargs.get('base_dir', None)
+        dir_only = kwargs.get("dir_only", False)
+        base_dir = kwargs.get("base_dir", None)
         if dir_only:
             if in_cache or in_s3:
                 return True
             # for JOB_WORK directory
             elif base_dir:
                 if not os.path.exists(rel_path):
                     os.makedirs(rel_path, exist_ok=True)
@@ -541,20 +589,19 @@
         elif in_s3:
             return True
         else:
             return False
 
     def _create(self, obj, **kwargs):
         if not self._exists(obj, **kwargs):
-
             # Pull out locally used fields
-            extra_dir = kwargs.get('extra_dir', None)
-            extra_dir_at_root = kwargs.get('extra_dir_at_root', False)
-            dir_only = kwargs.get('dir_only', False)
-            alt_name = kwargs.get('alt_name', None)
+            extra_dir = kwargs.get("extra_dir", None)
+            extra_dir_at_root = kwargs.get("extra_dir_at_root", False)
+            dir_only = kwargs.get("dir_only", False)
+            alt_name = kwargs.get("alt_name", None)
 
             # Construct hashed path
             rel_path = os.path.join(*directory_hash_id(self._get_object_id(obj)))
 
             # Optionally append extra_dir
             if extra_dir is not None:
                 if extra_dir_at_root:
@@ -571,23 +618,22 @@
             # flat namespace), do so for consistency with the regular file system
             # S3 folders are marked by having trailing '/' so add it now
             # s3_dir = '%s/' % rel_path
             # self._push_to_os(s3_dir, from_string='')
             # If instructed, create the dataset in cache & in S3
             if not dir_only:
                 rel_path = os.path.join(rel_path, alt_name if alt_name else f"dataset_{self._get_object_id(obj)}.dat")
-                open(os.path.join(self.staging_path, rel_path), 'w').close()
-                self._push_to_os(rel_path, from_string='')
+                open(os.path.join(self.staging_path, rel_path), "w").close()
+                self._push_to_os(rel_path, from_string="")
 
     def _empty(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             return bool(self._size(obj, **kwargs) > 0)
         else:
-            raise ObjectNotFound('objectstore.empty, object does not exist: %s, kwargs: %s'
-                                 % (str(obj), str(kwargs)))
+            raise ObjectNotFound(f"objectstore.empty, object does not exist: {obj}, kwargs: {kwargs}")
 
     def _size(self, obj, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
         if self._in_cache(rel_path):
             try:
                 return os.path.getsize(self._get_cache_path(rel_path))
             except OSError as ex:
@@ -595,18 +641,18 @@
         elif self._exists(obj, **kwargs):
             return self._get_size_in_s3(rel_path)
         log.warning("Did not find dataset '%s', returning 0 for size", rel_path)
         return 0
 
     def _delete(self, obj, entire_dir=False, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
-        extra_dir = kwargs.get('extra_dir', None)
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        extra_dir = kwargs.get("extra_dir", None)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         try:
             # Remove temparory data in JOB_WORK directory
             if base_dir and dir_only and obj_dir:
                 shutil.rmtree(os.path.abspath(rel_path))
                 return True
 
             # For the case of extra_files, because we don't have a reference to
@@ -628,15 +674,15 @@
                     key = Key(self._bucket, rel_path)
                     log.debug("Deleting key %s", key.name)
                     key.delete()
                     return True
         except S3ResponseError:
             log.exception("Could not delete key '%s' from S3", rel_path)
         except OSError:
-            log.exception('%s delete error', self._get_filename(obj, **kwargs))
+            log.exception("%s delete error", self._get_filename(obj, **kwargs))
         return False
 
     def _get_data(self, obj, start=0, count=-1, **kwargs):
         rel_path = self._construct_path(obj, **kwargs)
         # Check cache first and get file if not there
         if not self._in_cache(rel_path):
             self._pull_into_cache(rel_path)
@@ -644,17 +690,17 @@
         data_file = open(self._get_cache_path(rel_path))
         data_file.seek(start)
         content = data_file.read(count)
         data_file.close()
         return content
 
     def _get_filename(self, obj, **kwargs):
-        base_dir = kwargs.get('base_dir', None)
-        dir_only = kwargs.get('dir_only', False)
-        obj_dir = kwargs.get('obj_dir', False)
+        base_dir = kwargs.get("base_dir", None)
+        dir_only = kwargs.get("dir_only", False)
+        obj_dir = kwargs.get("obj_dir", False)
         rel_path = self._construct_path(obj, **kwargs)
 
         # for JOB_WORK directory
         if base_dir and dir_only and obj_dir:
             return os.path.abspath(rel_path)
 
         cache_path = self._get_cache_path(rel_path)
@@ -676,16 +722,15 @@
             else:
                 if self._pull_into_cache(rel_path):
                     return cache_path
         # For the case of retrieving a directory only, return the expected path
         # even if it does not exist.
         # if dir_only:
         #     return cache_path
-        raise ObjectNotFound('objectstore.get_filename, no cache_path: %s, kwargs: %s'
-                             % (str(obj), str(kwargs)))
+        raise ObjectNotFound(f"objectstore.get_filename, no cache_path: {obj}, kwargs: {kwargs}")
         # return cache_path # Until the upload tool does not explicitly create the dataset, return expected path
 
     def _update_from_file(self, obj, file_name=None, create=False, **kwargs):
         if create:
             self._create(obj, **kwargs)
         if self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
@@ -702,16 +747,15 @@
                 except OSError:
                     log.exception("Trouble copying source file '%s' to cache '%s'", source_file, cache_file)
             else:
                 source_file = self._get_cache_path(rel_path)
             # Update the file on S3
             self._push_to_os(rel_path, source_file)
         else:
-            raise ObjectNotFound('objectstore.update_from_file, object does not exist: %s, kwargs: %s'
-                                 % (str(obj), str(kwargs)))
+            raise ObjectNotFound(f"objectstore.update_from_file, object does not exist: {obj}, kwargs: {kwargs}")
 
     def _get_object_url(self, obj, **kwargs):
         if self._exists(obj, **kwargs):
             rel_path = self._construct_path(obj, **kwargs)
             try:
                 key = Key(self._bucket, rel_path)
                 return key.generate_url(expires_in=86400)  # 24hrs
@@ -720,31 +764,34 @@
         return None
 
     def _get_store_usage_percent(self):
         return 0.0
 
     def shutdown(self):
         self.running = False
-        thread = getattr(self, 'cache_monitor_thread', None)
+        thread = getattr(self, "cache_monitor_thread", None)
         if thread:
             log.debug("Shutting down thread")
             self.sleeper.wake()
             thread.join(5)
 
 
 class SwiftObjectStore(S3ObjectStore):
     """
     Object store that stores objects as items in a Swift bucket. A local
     cache exists that is used as an intermediate location for files between
     Galaxy and Swift.
     """
-    store_type = 'swift'
+
+    store_type = "swift"
 
     def _configure_connection(self):
         log.debug("Configuring Swift Connection")
-        self.conn = boto.connect_s3(aws_access_key_id=self.access_key,
-                                    aws_secret_access_key=self.secret_key,
-                                    is_secure=self.is_secure,
-                                    host=self.host,
-                                    port=self.port,
-                                    calling_format=boto.s3.connection.OrdinaryCallingFormat(),
-                                    path=self.conn_path)
+        self.conn = boto.connect_s3(
+            aws_access_key_id=self.access_key,
+            aws_secret_access_key=self.secret_key,
+            is_secure=self.is_secure,
+            host=self.host,
+            port=self.port,
+            calling_format=boto.s3.connection.OrdinaryCallingFormat(),
+            path=self.conn_path,
+        )
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/s3_multipart_upload.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/s3_multipart_upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,62 +19,59 @@
 
 def mp_from_ids(s3server, mp_id, mp_keyname, mp_bucketname):
     """Get the multipart upload from the bucket and multipart IDs.
 
     This allows us to reconstitute a connection to the upload
     from within multiprocessing functions.
     """
-    if s3server['host']:
-        conn = boto.connect_s3(aws_access_key_id=s3server['access_key'],
-                               aws_secret_access_key=s3server['secret_key'],
-                               is_secure=s3server['is_secure'],
-                               host=s3server['host'],
-                               port=s3server['port'],
-                               calling_format=boto.s3.connection.OrdinaryCallingFormat(),
-                               path=s3server['conn_path'])
+    if s3server["host"]:
+        conn = boto.connect_s3(
+            aws_access_key_id=s3server["access_key"],
+            aws_secret_access_key=s3server["secret_key"],
+            is_secure=s3server["is_secure"],
+            host=s3server["host"],
+            port=s3server["port"],
+            calling_format=boto.s3.connection.OrdinaryCallingFormat(),
+            path=s3server["conn_path"],
+        )
     else:
-        if s3server['access_key']:
-            conn = S3Connection(s3server['access_key'], s3server['secret_key'])
+        if s3server["access_key"]:
+            conn = S3Connection(s3server["access_key"], s3server["secret_key"])
         else:
             conn = S3Connection()
 
     bucket = conn.lookup(mp_bucketname)
     mp = boto.s3.multipart.MultiPartUpload(bucket)
     mp.key_name = mp_keyname
     mp.id = mp_id
     return mp
 
 
 def transfer_part(s3server, mp_id, mp_keyname, mp_bucketname, i, part):
-    """Transfer a part of a multipart upload. Designed to be run in parallel.
-    """
+    """Transfer a part of a multipart upload. Designed to be run in parallel."""
     mp = mp_from_ids(s3server, mp_id, mp_keyname, mp_bucketname)
-    with open(part, 'rb') as t_handle:
+    with open(part, "rb") as t_handle:
         mp.upload_part_from_file(t_handle, i + 1)
     os.remove(part)
 
 
 def multipart_upload(s3server, bucket, s3_key_name, tarball, mb_size):
-    """Upload large files using Amazon's multipart upload functionality.
-    """
+    """Upload large files using Amazon's multipart upload functionality."""
+
     def split_file(in_file, mb_size, split_num=5):
-        prefix = os.path.join(os.path.dirname(in_file),
-                              f"{os.path.basename(s3_key_name)}S3PART")
-        max_chunk = s3server['max_chunk_size']
+        prefix = os.path.join(os.path.dirname(in_file), f"{os.path.basename(s3_key_name)}S3PART")
+        max_chunk = s3server["max_chunk_size"]
         # Split chunks so they are 5MB < chunk < 250MB(max_chunk_size)
         split_size = int(max(min(mb_size / (split_num * 2.0), max_chunk), 5))
         if not os.path.exists(f"{prefix}aa"):
             cl = ["split", f"-b{split_size}m", in_file, prefix]
             subprocess.check_call(cl)
         return sorted(glob.glob(f"{prefix}*"))
 
-    mp = bucket.initiate_multipart_upload(s3_key_name,
-                                          reduced_redundancy=s3server['use_rr'])
+    mp = bucket.initiate_multipart_upload(s3_key_name, reduced_redundancy=s3server["use_rr"])
 
-    for (i, part) in enumerate(split_file(tarball, mb_size)):
-        t = threading.Thread(
-            target=transfer_part,
-            args=(s3server, mp.id, mp.key_name, mp.bucket_name, i, part))
+    for i, part in enumerate(split_file(tarball, mb_size)):
+        t = threading.Thread(target=transfer_part, args=(s3server, mp.id, mp.key_name, mp.bucket_name, i, part))
         t.start()
         t.join()
 
     mp.complete_upload()
```

### Comparing `galaxy-objectstore-22.1.1/galaxy/objectstore/unittest_utils/__init__.py` & `galaxy-objectstore-23.0.1/galaxy/objectstore/unittest_utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     path: "${temp_directory}/tmp1"
   - type: job_work
     path: "${temp_directory}/job_working_directory1"
 """
 
 
 class Config:
-
     def __init__(self, config_str=DISK_TEST_CONFIG, clazz=None, store_by="id"):
         self.temp_directory = mkdtemp()
         if config_str.startswith("<"):
             config_file = "store.xml"
         else:
             config_file = "store.yaml"
         self.write(config_str, config_file)
@@ -61,26 +60,25 @@
         contents_template = Template(contents)
         expanded_contents = contents_template.safe_substitute(temp_directory=self.temp_directory)
         open(path, "w").write(expanded_contents)
         return path
 
 
 class MockConfig:
-
     def __init__(self, temp_directory, config_file, store_by="id"):
         self.file_path = temp_directory
         self.object_store_config_file = os.path.join(temp_directory, config_file)
         self.object_store_check_old_style = False
         self.object_store_cache_path = os.path.join(temp_directory, "staging")
         self.object_store_store_by = store_by
         self.jobs_directory = temp_directory
         self.new_file_path = temp_directory
         self.umask = 0000
         self.gid = 1000
 
 
 __all__ = [
-    'Config',
-    'MockConfig',
-    'DISK_TEST_CONFIG',
-    'DISK_TEST_CONFIG_YAML',
+    "Config",
+    "MockConfig",
+    "DISK_TEST_CONFIG",
+    "DISK_TEST_CONFIG_YAML",
 ]
```

### Comparing `galaxy-objectstore-22.1.1/galaxy_objectstore.egg-info/PKG-INFO` & `galaxy-objectstore-23.0.1/galaxy_objectstore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 Metadata-Version: 2.1
 Name: galaxy-objectstore
-Version: 22.1.1
-Summary: Galaxy Objectstore Framework and Plugins
+Version: 23.0.1
+Summary: Galaxy objectstore framework and plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-objectstore.svg
    :target: https://pypi.org/project/galaxy-objectstore/
 
 
 Overview
 --------
 
 The Galaxy_ object store framework and default implementations.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.2.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
-
----------------------
+-------------------
 20.9.1 (2021-03-01)
----------------------
-
+-------------------
 
+* Second release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
-
-
```

