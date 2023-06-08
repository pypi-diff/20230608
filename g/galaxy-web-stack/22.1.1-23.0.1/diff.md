# Comparing `tmp/galaxy-web-stack-22.1.1.tar.gz` & `tmp/galaxy-web-stack-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-web-stack-22.1.1.tar", last modified: Mon Aug 22 19:46:11 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_stack/dist/.tmp-szsfagqx/galaxy-web-stack-23.0.1.tar", last modified: Thu Jun  8 17:44:05 2023, max compression
```

## Comparing `galaxy-web-stack-22.1.1.tar` & `galaxy-web-stack-23.0.1.tar`

### file list

```diff
@@ -1,38 +1,25 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.470676 galaxy-web-stack-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      217 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-web-stack-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       28 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1557 2022-08-22 19:46:11.470801 galaxy-web-stack-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      313 2022-03-24 19:47:11.000000 galaxy-web-stack-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.465908 galaxy-web-stack-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/galaxy/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      427 2022-08-22 19:45:30.000000 galaxy-web-stack-22.1.1/galaxy/project_galaxy_web_stack.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.467283 galaxy-web-stack-22.1.1/galaxy/web_stack/
--rw-r--r--   0 mvandenb   (501) staff       (20)    28897 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/galaxy/web_stack/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1949 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/galaxy/web_stack/gunicorn_config.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    23727 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/galaxy/web_stack/handlers.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5251 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/galaxy/web_stack/message.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6102 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/galaxy/web_stack/transport.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.468972 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1557 2022-08-22 19:46:10.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      805 2022-08-22 19:46:11.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:46:10.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:46:10.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:46:10.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       34 2022-08-22 19:46:10.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:46:10.000000 galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       34 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.469748 galaxy-web-stack-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:46:11.477421 galaxy-web-stack-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2764 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)       16 2022-08-18 15:49:03.000000 galaxy-web-stack-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.462886 galaxy-web-stack-22.1.1/tests/
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:11.470457 galaxy-web-stack-22.1.1/tests/web_stack/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:14.000000 galaxy-web-stack-22.1.1/tests/web_stack/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1639 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/tests/web_stack/test_application_stack.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      736 2022-08-22 19:45:28.000000 galaxy-web-stack-22.1.1/tests/web_stack/test_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-web-stack-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-web-stack-22.1.1/LICENSE` & `galaxy-web-stack-23.0.1/LICENSE`

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

### Comparing `galaxy-web-stack-22.1.1/PKG-INFO` & `galaxy-web-stack-23.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 22.1.1
-Summary: Galaxy Web Strack Abstraction
+Version: 23.0.1
+Summary: Galaxy web stack abstraction
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
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-stack.svg
    :target: https://pypi.python.org/pypi/galaxy-web-stack/
 
 
 Overview
 --------
 
 The Galaxy_ web strack abstraction.
 
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
-20.5.1.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-web-stack-22.1.1/galaxy/web_stack/gunicorn_config.py` & `galaxy-web-stack-23.0.1/galaxy/web_stack/gunicorn_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """
 Gunicorn config file based on https://gist.github.com/hynek/ba655c8756924a5febc5285c712a7946
 """
-import logging
 import os
 import sys
 
-log = logging.getLogger(__name__)
-
 
 def on_starting(server):
     """
     Attach a set of IDs that can be temporarily re-used.
 
     Used on reloads when each worker exists twice.
     """
@@ -31,15 +28,15 @@
 def _next_worker_id(server):
     """
     If there are IDs open for re-use, take one. Else look for a free one.
     """
     if server._worker_id_overload:
         return server._worker_id_overload.pop()
 
-    in_use = set(w._worker_id for w in tuple(server.WORKERS.values()) if w.alive)
+    in_use = {w._worker_id for w in tuple(server.WORKERS.values()) if w.alive}
     free = set(range(1, server._worker_id_current_workers + 1)) - in_use
 
     return free.pop()
 
 
 def on_reload(server):
     """
```

### Comparing `galaxy-web-stack-22.1.1/galaxy/web_stack/handlers.py` & `galaxy-web-stack-23.0.1/galaxy/web_stack/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,49 +4,46 @@
 for some activity such as queuing up jobs or scheduling workflows.
 """
 
 import logging
 import os
 import random
 from enum import Enum
-from typing import Set, Tuple
+from typing import Tuple
 
 from sqlalchemy.orm import object_session
 
 from galaxy.exceptions import HandlerAssignmentError
 from galaxy.util import (
     ExecutionTimer,
-    listify
+    listify,
 )
 
 log = logging.getLogger(__name__)
 
 
 class HANDLER_ASSIGNMENT_METHODS(str, Enum):
-    MEM_SELF = 'mem-self'
-    DB_SELF = 'db-self'
-    DB_PREASSIGN = 'db-preassign'
-    DB_TRANSACTION_ISOLATION = 'db-transaction-isolation'
-    DB_SKIP_LOCKED = 'db-skip-locked'
-    UWSGI_MULE_MESSAGE = 'uwsgi-mule-message'
+    MEM_SELF = "mem-self"
+    DB_SELF = "db-self"
+    DB_PREASSIGN = "db-preassign"
+    DB_TRANSACTION_ISOLATION = "db-transaction-isolation"
+    DB_SKIP_LOCKED = "db-skip-locked"
 
     @classmethod
     def has_value(cls, value):
         return value in cls._value2member_map_
 
 
 class HandlerAssignmentSkip(Exception):
-    """Exception for handler assignment methods to raise if the next method should be tried.
-    """
+    """Exception for handler assignment methods to raise if the next method should be tried."""
 
 
 class ConfiguresHandlers:
-    DEFAULT_HANDLER_TAG = '_default_'
+    DEFAULT_HANDLER_TAG = "_default_"
     DEFAULT_BASE_HANDLER_POOLS: Tuple[str, ...] = ()
-    UNSUPPORTED_HANDLER_ASSIGNMENT_METHODS: Set[str] = set()
 
     def add_handler(self, handler_id, tags):
         if handler_id not in self.handlers:
             self.handlers[handler_id] = (handler_id,)
         for tag in tags:
             if tag in self.handlers and handler_id not in self.handlers[tag]:
                 self.handlers[tag].append(handler_id)
@@ -58,36 +55,36 @@
         handling_config_dict = {}
 
         processes = {}
         handling_config_dict["processes"] = processes
 
         # Parse handlers
         if config_element is not None:
-            for handler in ConfiguresHandlers._findall_with_required(config_element, 'handler'):
-                handler_id = handler.get('id')
+            for handler in ConfiguresHandlers._findall_with_required(config_element, "handler"):
+                handler_id = handler.get("id")
                 if handler_id in processes:
                     log.error("Handler '%s' overlaps handler with the same name, ignoring", handler_id)
                 else:
                     log.debug("Read definition for handler '%s'", handler_id)
                     plugins = []
-                    for plugin in ConfiguresHandlers._findall_with_required(handler, 'plugin', ['id']):
+                    for plugin in ConfiguresHandlers._findall_with_required(handler, "plugin", ["id"]):
                         plugins.append(plugin.get("id"))
-                    tags = [x.strip() for x in handler.get('tags', ConfiguresHandlers.DEFAULT_HANDLER_TAG).split(',')]
+                    tags = [x.strip() for x in handler.get("tags", ConfiguresHandlers.DEFAULT_HANDLER_TAG).split(",")]
                     handler_def = {"tags": tags}
                     if plugins:
                         handler_def["plugins"] = plugins
                     processes[handler_id] = handler_def
             default_handler = ConfiguresHandlers.get_xml_default(config, config_element)
             if default_handler:
                 handling_config_dict["default"] = default_handler
 
-            assign = listify(config_element.attrib.get('assign_with', []), do_strip=True)
+            assign = listify(config_element.attrib.get("assign_with", []), do_strip=True)
             if len(assign) > 0:
                 handling_config_dict["assign"] = assign
-            max_grab_str = config_element.attrib.get('max_grab', None)
+            max_grab_str = config_element.attrib.get("max_grab", None)
             if max_grab_str:
                 handling_config_dict["max_grab"] = int(max_grab_str)
             ready_window_size_str = config_element.attrib.get("ready_window_size", None)
             if ready_window_size_str:
                 handling_config_dict["ready_window_size"] = int(ready_window_size_str)
 
         return handling_config_dict
@@ -99,75 +96,82 @@
             if handler_id in self.handlers:
                 log.error("Handler '%s' overlaps handler with the same name, ignoring", handler_id)
             else:
                 log.debug("Read definition for handler '%s'", handler_id)
                 self._parse_handler(handler_id, process)
                 self.add_handler(handler_id, process.get("tags") or [self.DEFAULT_HANDLER_TAG])
 
-        self.default_handler_id = self._ensure_default_set(handling_config_dict.get("default"), list(self.handlers.keys()), required=False)
+        self.default_handler_id = self._ensure_default_set(
+            handling_config_dict.get("default"), list(self.handlers.keys()), required=False
+        )
 
     def _init_handler_assignment_methods(self, handling_config_dict=None):
         handling_config_dict = handling_config_dict or {}
 
         self.__is_handler = None
         # This is set by the stack job handler init code
         self.pool_for_tag = {}
         self._handler_assignment_method_methods = {
             HANDLER_ASSIGNMENT_METHODS.MEM_SELF: self._assign_mem_self_handler,
             HANDLER_ASSIGNMENT_METHODS.DB_SELF: self._assign_db_self_handler,
             HANDLER_ASSIGNMENT_METHODS.DB_PREASSIGN: self._assign_db_preassign_handler,
             HANDLER_ASSIGNMENT_METHODS.DB_TRANSACTION_ISOLATION: self._assign_db_tag,
             HANDLER_ASSIGNMENT_METHODS.DB_SKIP_LOCKED: self._assign_db_tag,
-            HANDLER_ASSIGNMENT_METHODS.UWSGI_MULE_MESSAGE: self._assign_uwsgi_mule_message_handler,
         }
         if handling_config_dict:
             for method in handling_config_dict.get("assign", []):
                 method = method.lower()
-                assert HANDLER_ASSIGNMENT_METHODS.has_value(method), \
-                    "Invalid job handler assignment method '{}', must be one of: {}".format(
-                        method, ', '.join(h.value for h in HANDLER_ASSIGNMENT_METHODS))
+                assert HANDLER_ASSIGNMENT_METHODS.has_value(
+                    method
+                ), "Invalid job handler assignment method '{}', must be one of: {}".format(
+                    method, ", ".join(h.value for h in HANDLER_ASSIGNMENT_METHODS)
+                )
                 try:
                     self.handler_assignment_methods.append(method)
                 except AttributeError:
                     self.handler_assignment_methods_configured = True
                     self.handler_assignment_methods = [method]
             if self.handler_assignment_methods == [HANDLER_ASSIGNMENT_METHODS.MEM_SELF]:
                 self.app.config.track_jobs_in_database = False
-            self.handler_max_grab = handling_config_dict.get('max_grab', self.handler_max_grab)
+            self.handler_max_grab = handling_config_dict.get("max_grab", self.handler_max_grab)
             if self.handler_max_grab is not None:
                 self.handler_max_grab = int(self.handler_max_grab)
 
     def _set_default_handler_assignment_methods(self):
         if not self.handler_assignment_methods_configured:
-            if not self.app.config.track_jobs_in_database and \
-                    HANDLER_ASSIGNMENT_METHODS.MEM_SELF not in self.UNSUPPORTED_HANDLER_ASSIGNMENT_METHODS:
+            if not self.app.config.track_jobs_in_database:
                 # DEPRECATED: You should just set mem_self as the only method if you want this
-                log.warning("The `track_jobs_in_database` option is deprecated, please set `%s` as the job"
-                            " handler assignment method in the job handler configuration",
-                            HANDLER_ASSIGNMENT_METHODS.MEM_SELF)
+                log.warning(
+                    "The `track_jobs_in_database` option is deprecated, please set `%s` as the job"
+                    " handler assignment method in the job handler configuration",
+                    HANDLER_ASSIGNMENT_METHODS.MEM_SELF,
+                )
                 self.handler_assignment_methods = [HANDLER_ASSIGNMENT_METHODS.MEM_SELF]
             else:
                 self.handler_assignment_methods = [self.app.application_stack.get_preferred_handler_assignment_method()]
             # If the stack has handler pools it can override these defaults
             self.app.application_stack.init_job_handling(self)
-            log.info("%s: No job handler assignment method is set, defaulting to '%s', set the `assign_with` attribute"
-                     " on <handlers> to override the default", self.__class__.__name__,
-                     self.handler_assignment_methods[0])
+            log.info(
+                "%s: No job handler assignment method is set, defaulting to '%s', set the `assign_with` attribute"
+                " on <handlers> to override the default",
+                self.__class__.__name__,
+                self.handler_assignment_methods[0],
+            )
 
     def _parse_handler(self, handler_id, handler_def):
         pass
 
     @staticmethod
     def get_xml_default(config, parent):
-        rval = parent.get('default')
-        if 'default_from_environ' in parent.attrib:
-            environ_var = parent.attrib['default_from_environ']
+        rval = parent.get("default")
+        if "default_from_environ" in parent.attrib:
+            environ_var = parent.attrib["default_from_environ"]
             rval = os.environ.get(environ_var, rval)
-        elif 'default_from_config' in parent.attrib:
-            config_val = parent.attrib['default_from_config']
+        elif "default_from_config" in parent.attrib:
+            config_val = parent.attrib["default_from_config"]
             rval = config.config_dict.get(config_val, rval)
         return rval
 
     def _get_default(self, config, parent, names, auto=False, required=True):
         """
         Returns the default attribute set in a parent tag like <handlers> or
         <destinations>, or return the ID of the child, if there is no explicit
@@ -211,83 +215,82 @@
         :param attribs: List of required attributes in children elements.
         :type attribs: list of str
 
         :returns: list of ``lxml.etree._Element``
         """
         rval = []
         if attribs is None:
-            attribs = ('id',)
+            attribs = ("id",)
         for elem in parent.findall(match):
             for attrib in attribs:
                 if attrib not in elem.attrib:
                     log.warning(f"required '{attrib}' attribute is missing from <{match}> element")
                     break
             else:
                 rval.append(elem)
         return rval
 
     @property
-    def use_messaging(self):
-        # The job manager uses this to determine whether the messaging job queue should be used
-        return HANDLER_ASSIGNMENT_METHODS.UWSGI_MULE_MESSAGE in self.handler_assignment_methods
-
-    @property
     def deterministic_handler_assignment(self):
         return self.handler_assignment_methods and any(
-            filter(lambda x: x in (
-                HANDLER_ASSIGNMENT_METHODS.UWSGI_MULE_MESSAGE,
-                HANDLER_ASSIGNMENT_METHODS.DB_PREASSIGN,
-            ), self.handler_assignment_methods))
+            filter(lambda x: x == HANDLER_ASSIGNMENT_METHODS.DB_PREASSIGN), self.handler_assignment_methods
+        )
 
     def _get_is_handler(self):
         """Indicate whether the current server is configured as a handler.
 
         :return: bool
         """
         if self.__is_handler is not None:
             return self.__is_handler
-        if (HANDLER_ASSIGNMENT_METHODS.DB_SELF in self.handler_assignment_methods
-                or HANDLER_ASSIGNMENT_METHODS.MEM_SELF in self.handler_assignment_methods):
+        if (
+            HANDLER_ASSIGNMENT_METHODS.DB_SELF in self.handler_assignment_methods
+            or HANDLER_ASSIGNMENT_METHODS.MEM_SELF in self.handler_assignment_methods
+        ):
             return True
         for collection in self.handlers.values():
             if self.app.config.server_name in collection:
                 return True
-        if not self.handlers and not self.handler_assignment_methods_configured \
-                and (HANDLER_ASSIGNMENT_METHODS.DB_TRANSACTION_ISOLATION in self.handler_assignment_methods
-                or HANDLER_ASSIGNMENT_METHODS.DB_SKIP_LOCKED in self.handler_assignment_methods):
+        if (
+            not self.handlers
+            and not self.handler_assignment_methods_configured
+            and (
+                HANDLER_ASSIGNMENT_METHODS.DB_TRANSACTION_ISOLATION in self.handler_assignment_methods
+                or HANDLER_ASSIGNMENT_METHODS.DB_SKIP_LOCKED in self.handler_assignment_methods
+            )
+        ):
             return True
         return False
 
     def _set_is_handler(self, value):
         self.__is_handler = value
 
     is_handler = property(_get_is_handler, _set_is_handler)
 
     def _get_single_item(self, collection, index=None):
-        """Given a collection of handlers or destinations, return one item from the collection at random.
-        """
+        """Given a collection of handlers or destinations, return one item from the collection at random."""
         # Done like this to avoid random under the assumption it's faster to avoid it
         if len(collection) == 1:
             return collection[0]
         elif index is None:
             return random.choice(collection)
         else:
             return collection[index % len(collection)]
 
     @property
     def handler_tags(self):
-        """Get an iterable of all configured handler tags.
-        """
+        """Get an iterable of all configured handler tags."""
         return filter(lambda k: isinstance(self.handlers[k], list), self.handlers.keys())
 
     @property
     def self_handler_tags(self):
-        """Get an iterable of the current process's configured handler tags.
-        """
-        return [k for k in self.handler_tags if self.app.config.server_name in self.handlers[k]] or [self.DEFAULT_HANDLER_TAG]
+        """Get an iterable of the current process's configured handler tags."""
+        return [k for k in self.handler_tags if self.app.config.server_name in self.handlers[k]] or [
+            self.DEFAULT_HANDLER_TAG
+        ]
 
     # If these get to be any more complex we should probably modularize them, or at least move to a separate class
 
     def _assign_handler_direct(self, obj, configured, flush=True):
         """Directly assign a handler if the object has been preconfigured to a known single static handler.
 
         :param obj:             Same as :method:`ConfiguresHandlers.assign_handler()`.
@@ -317,20 +320,25 @@
         :param configured:      Ignored.
         :param queue_callback:  Callback to be executed when the job should be queued (i.e. a callback to the handler's
                                 ``put()`` method). No arguments are passed.
         :type queue_callback:   callable
 
         :returns: str -- This process's server name (handler ID).
         """
-        assert queue_callback is not None, \
-            f"Cannot perform '{HANDLER_ASSIGNMENT_METHODS.MEM_SELF}' handler assignment: `queue_callback` is None"
+        assert (
+            queue_callback is not None
+        ), f"Cannot perform '{HANDLER_ASSIGNMENT_METHODS.MEM_SELF}' handler assignment: `queue_callback` is None"
         if configured:
-            log.warning("(%s) Ignoring handler assignment to '%s' because configured handler assignment method"
-                        " '' overrides per-tool handler assignment", obj.log_str(),
-                        HANDLER_ASSIGNMENT_METHODS.MEM_SELF, configured)
+            log.warning(
+                "(%s) Ignoring handler assignment to '%s' because configured handler assignment method"
+                " '' overrides per-tool handler assignment",
+                obj.log_str(),
+                HANDLER_ASSIGNMENT_METHODS.MEM_SELF,
+                configured,
+            )
         if flush():
             _timed_flush_obj(obj)
         queue_callback()
         return self.app.config.server_name
 
     def _assign_db_self_handler(self, obj, method, configured, flush=True, **kwargs):
         """Assign object to this process by setting its ``handler`` column in the database to this process.
@@ -375,16 +383,17 @@
             handler = self.default_handler_id or self.DEFAULT_HANDLER_TAG
         # Get a random handler ID from the possible handlers. If the admin has configured a tool with a handler tag that
         # does not exist, or if there are no default handlers and configured is None, this will raise KeyError to
         # assign_handler, which should log it, try the next method (if any), and if no other methods succeed, raise
         # HandlerAssigmentError.
         handler_id = self._get_single_item(self.handlers[handler], index=index)
         if handler != handler_id:
-            log.debug("(%s) Selected handler '%s' by random choice from handler tag '%s'", obj.log_str(),
-                      handler_id, handler)
+            log.debug(
+                "(%s) Selected handler '%s' by random choice from handler tag '%s'", obj.log_str(), handler_id, handler
+            )
         obj.set_handler(handler_id)
         if flush:
             _timed_flush_obj(obj)
         return handler_id
 
     def _assign_db_tag(self, obj, method, configured, flush=True, **kwargs):
         """Assign object to a handler by setting its ``handler`` column in the database to either the configured handler
@@ -400,43 +409,14 @@
         if handler is None:
             handler = self.default_handler_id or self.DEFAULT_HANDLER_TAG
         obj.set_handler(handler)
         if flush:
             _timed_flush_obj(obj)
         return handler
 
-    def _assign_uwsgi_mule_message_handler(self, obj, method, configured, message_callback=None, flush=True, **kwargs):
-        """Assign object to a handler by sending a setup message to the appropriate handler pool (farm), where a handler
-        (mule) will receive the message and assign itself.
-
-        :param obj:             Same as :method:`ConfiguresHandlers.assign_handler()`.
-        :param method:          Same as :method:`ConfiguresHandlers._assign_db_preassign_handler()`.
-        :param configured:      Same as :method:`ConfiguresHandlers.assign_handler()`.
-        :param queue_callback:  Callback returning a setup message to be sent via the stack messaging interface's
-                                ``send_message()`` method. No arguments are passed.
-        :type queue_callback:   callable
-
-        :raises HandlerAssignmentSkip: if the configured or default handler is not a known handler pool (farm)
-        :returns: str -- The assigned handler pool.
-        """
-        assert message_callback is not None, \
-            "Cannot perform '%s' handler assignment: `message_callback` is None" \
-            % HANDLER_ASSIGNMENT_METHODS.UWSGI_MULE_MESSAGE
-        tag = configured or self.DEFAULT_HANDLER_TAG
-        pool = self.pool_for_tag.get(tag)
-        if pool is None:
-            log.debug("(%s) No handler pool (uWSGI farm) for '%s' found", obj.log_str(), tag)
-            raise HandlerAssignmentSkip()
-        else:
-            if flush or not obj.id:
-                _timed_flush_obj(obj)
-            message = message_callback()
-            self.app.application_stack.send_message(pool, message)
-        return pool
-
     def assign_handler(self, obj, configured=None, **kwargs):
         """Set a job handler, flush obj
 
         Called assignment methods should raise py:class:`HandlerAssignmentSkip` to indicate that the next method
         should be tried.
 
         :param obj:         Object to assign a handler to (must be a model object with ``handler`` attribute and
@@ -447,27 +427,32 @@
 
         :returns: bool -- True on successful assignment, False otherwise.
         """
         # It's a bit awkward that the method that actually hands off job execution is in the JobConfiguration, but
         # that's currently the best place for it. It's worth noting that this method is also part of the
         # WorkflowSchedulingManager, which acts like a combined JobConfiguration and JobManager. Combining those two
         # classes would probably be reasonable (and would remove the need for the queue callback).
-        if self._assign_handler_direct(obj, configured, flush=kwargs.get('flush', True)):
-            log.info("(%s) Skipped handler assignment logic due to explicit configuration` to a single handler: %s",
-                     obj.log_str(), configured)
+        if self._assign_handler_direct(obj, configured, flush=kwargs.get("flush", True)):
+            log.info(
+                "(%s) Skipped handler assignment logic due to explicit configuration` to a single handler: %s",
+                obj.log_str(),
+                configured,
+            )
             return True
         for method in self.handler_assignment_methods:
             try:
-                handler = self._handler_assignment_method_methods[method](
-                    obj, method, configured=configured, **kwargs)
+                handler = self._handler_assignment_method_methods[method](obj, method, configured=configured, **kwargs)
                 log.info("(%s) Handler '%s' assigned using '%s' assignment method", obj.log_str(), handler, method)
                 return handler
             except HandlerAssignmentSkip:
-                log.debug("(%s) Handler assignment method '%s' did not assign a handler, trying next method",
-                          obj.log_str(), method)
+                log.debug(
+                    "(%s) Handler assignment method '%s' did not assign a handler, trying next method",
+                    obj.log_str(),
+                    method,
+                )
             except Exception:
                 log.exception("Caught exception in handler assignment method: %s", method)
         else:
             # Ideally we could just expunge the object from the SA session here, but in most cases, some of its related
             # objects have already been created, so instead we'll just have to fail it.
             log.error("(%s) Failed to select handler", obj.log_str())
             raise HandlerAssignmentError("Job handler assignment failed.", obj=obj)
```

### Comparing `galaxy-web-stack-22.1.1/galaxy/web_stack/message.py` & `galaxy-web-stack-23.0.1/galaxy/web_stack/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Web Application Stack worker messaging."""
 
 import json
 import logging
 import types
-from typing import Optional, Tuple
+from typing import (
+    Optional,
+    Tuple,
+)
 
 log = logging.getLogger(__name__)
 
 
 class ApplicationStackMessageDispatcher:
     def __init__(self):
         self.__funcs = {}
@@ -33,133 +36,140 @@
         return len(self.__funcs)
 
     def dispatch(self, msg_str):
         msg = decode(msg_str)
         try:
             msg.validate()
         except AssertionError as exc:
-            log.error('Invalid message received: %s, error: %s', msg_str, exc)
+            log.error("Invalid message received: %s, error: %s", msg_str, exc)
             return
         if msg.target not in self.__funcs:
-            log.error("Received message with target '%s' but no functions were registered with that name. Params were: %s", msg.target, msg.params)
+            log.error(
+                "Received message with target '%s' but no functions were registered with that name. Params were: %s",
+                msg.target,
+                msg.params,
+            )
         else:
             self.__funcs[msg.target](msg)
 
 
 class ApplicationStackMessage(dict):
     default_handler = None
-    _validate_kwargs = ('target',)
+    _validate_kwargs = ("target",)
 
     def __init__(self, target=None, **kwargs):
-        self['target'] = target
+        self["target"] = target
         self._merge_class_tuples()
 
     def _merge_class_tuples(self):
         """Locates any class-level tuples beginning with a single (but not double) underscore in the MRO and creates a
         property on the instance with the same name (without the leading underscore) that will return the union of
         those tuples.
         """
         names = set()
         for cls in reversed(self.__class__.mro()):
-            names.update([x for x in dir(cls) if x.startswith('_') and not x.startswith('__') and type(getattr(cls, x)) == tuple])
+            names.update(
+                [x for x in dir(cls) if x.startswith("_") and not x.startswith("__") and type(getattr(cls, x)) == tuple]
+            )
         for name in names:
-            setattr(self.__class__, name.lstrip('_'), property(lambda self, name=name: self._get_list_from_mro(name)))
+            setattr(self.__class__, name.lstrip("_"), property(lambda self, name=name: self._get_list_from_mro(name)))
 
     def _get_list_from_mro(self, name):
-        """Locate all class-level tuples with the given `name` in the MRO and return their union.
-        """
+        """Locate all class-level tuples with the given `name` in the MRO and return their union."""
         r = set()
         for cls in reversed(self.__class__.mro()):
             r.update(getattr(cls, name, []))
         return r
 
     def _validate_items(self, obj, items, name):
         for item in items:
             assert item in obj, f"Missing '{item}' message {name}"
 
     def validate(self):
-        self._validate_items(self, self.validate_kwargs, 'argument')
+        self._validate_items(self, self.validate_kwargs, "argument")
 
     def encode(self):
-        self['__classname__'] = self.__class__.__name__
+        self["__classname__"] = self.__class__.__name__
         return json.dumps(self)
 
     def bind_default_handler(self, obj, name):
         """Bind the default handler method to `obj` as attribute `name`.
 
         This could also be implemented as a mixin class.
         """
-        assert self.default_handler is not None, f'{self.__class__.__name__} has no default handler method, cannot bind'
+        assert self.default_handler is not None, f"{self.__class__.__name__} has no default handler method, cannot bind"
         setattr(obj, name, types.MethodType(self.default_handler, obj))
-        log.debug("Bound default message handler '%s.%s' to %s", self.__class__.__name__, self.default_handler.__name__,
-                  getattr(obj, name))
+        log.debug(
+            "Bound default message handler '%s.%s' to %s",
+            self.__class__.__name__,
+            self.default_handler.__name__,
+            getattr(obj, name),
+        )
 
     @property
     def target(self) -> Optional[str]:
-        return self['target']
+        return self["target"]
 
     @target.setter  # type: ignore[attr-defined]
     def set_target(self, target):
-        self['target'] = target
+        self["target"] = target
 
 
 class ParamMessage(ApplicationStackMessage):
-    _validate_kwargs = ('params',)
+    _validate_kwargs = ("params",)
     _validate_params: Tuple[str, ...] = ()
     _exclude_params: Tuple[str, ...] = ()
 
     def __init__(self, target=None, params=None, **kwargs):
         super().__init__(target=target)
-        self['params'] = params or {}
+        self["params"] = params or {}
         for k, v in kwargs.items():
-            self['params'][k] = v
+            self["params"][k] = v
 
     def validate(self):
         super().validate()
-        self._validate_items(self['params'], self.validate_params, 'parameters')
+        self._validate_items(self["params"], self.validate_params, "parameters")
 
     @property
     def params(self):
-        d = self['params'].copy()
+        d = self["params"].copy()
         for key in self.exclude_params:
             d.pop(key, None)
         return d
 
     @params.setter
     def params(self, params):
-        self['params'] = params
+        self["params"] = params
 
 
 class TaskMessage(ParamMessage):
-    _validate_params = ('task',)
-    _exclude_params = ('task',)
+    _validate_params = ("task",)
+    _exclude_params = ("task",)
 
     @staticmethod
     def default_handler(self, msg):
-        """Can be bound to an instance of any class that has message handling methods named like `_handle_{task}_method`
-        """
-        name = f'_handle_{msg.task}_msg'
+        """Can be bound to an instance of any class that has message handling methods named like `_handle_{task}_method`"""
+        name = f"_handle_{msg.task}_msg"
         assert name in dir(self), "{cls} has no method _handle_{task}_msg, cannot handle message: {msg}".format(
-            cls=self.__class__.__name__,
-            task=msg.task,
-            msg=msg)
-        getattr(self, f'_handle_{msg.task}_msg')(**msg.params)
+            cls=self.__class__.__name__, task=msg.task, msg=msg
+        )
+        getattr(self, f"_handle_{msg.task}_msg")(**msg.params)
 
     @property
     def task(self):
-        return self['params']['task']
+        return self["params"]["task"]
 
 
 class JobHandlerMessage(TaskMessage):
-    target = 'job_handler'
-    _validate_params = ('job_id',)
+    target = "job_handler"
+    _validate_params = ("job_id",)
 
 
 class WorkflowSchedulingMessage(TaskMessage):
-    target = 'workflow_scheduling'
-    _validate_params = ('workflow_invocation_id',)
+    target = "workflow_scheduling"
+    _validate_params = ("workflow_invocation_id",)
 
 
 def decode(msg_str):
     d = json.loads(msg_str)
-    cls = d.pop('__classname__')
+    cls = d.pop("__classname__")
     return globals()[cls](**d)
```

### Comparing `galaxy-web-stack-22.1.1/galaxy_web_stack.egg-info/PKG-INFO` & `galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 22.1.1
-Summary: Galaxy Web Strack Abstraction
+Version: 23.0.1
+Summary: Galaxy web stack abstraction
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
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-stack.svg
    :target: https://pypi.python.org/pypi/galaxy-web-stack/
 
 
 Overview
 --------
 
 The Galaxy_ web strack abstraction.
 
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
-20.5.1.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

