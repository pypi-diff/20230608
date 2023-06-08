# Comparing `tmp/labbench-0.23.4.tar.gz` & `tmp/labbench-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labbench-0.23.4.tar", last modified: Thu Jan 26 21:04:43 2023, max compression
+gzip compressed data, was "labbench-0.25.0.tar", last modified: Thu Jun  8 18:04:23 2023, max compression
```

## Comparing `labbench-0.23.4.tar` & `labbench-0.25.0.tar`

### file list

```diff
@@ -1,66 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 21:04:43.183040 labbench-0.23.4/
--rw-rw-rw-   0        0        0     2858 2021-08-18 18:41:24.000000 labbench-0.23.4/LICENSE.md
--rw-rw-rw-   0        0        0     1118 2023-01-26 21:04:43.183040 labbench-0.23.4/PKG-INFO
--rw-rw-rw-   0        0        0    11272 2023-01-25 18:33:42.000000 labbench-0.23.4/README.md
-drwxrwxrwx   0        0        0        0 2023-01-26 21:04:42.833032 labbench-0.23.4/cli/
--rw-rw-rw-   0        0        0        0 2023-01-25 18:33:42.000000 labbench-0.23.4/cli/__init__.py
--rw-rw-rw-   0        0        0     9147 2023-01-25 18:33:42.000000 labbench-0.23.4/cli/__main__.py
-drwxrwxrwx   0        0        0        0 2023-01-26 21:04:43.022925 labbench-0.23.4/labbench/
--rw-rw-rw-   0        0        0     2959 2023-01-25 18:49:08.000000 labbench-0.23.4/labbench/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-01-25 20:32:51.000000 labbench-0.23.4/labbench/__init__.pyi
--rw-rw-rw-   0        0        0    46801 2023-01-25 18:54:08.000000 labbench-0.23.4/labbench/_backends.py
--rw-rw-rw-   0        0        0     6395 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/_backends.pyi
--rw-rw-rw-   0        0        0    74881 2023-01-25 18:52:44.000000 labbench-0.23.4/labbench/_data.py
--rw-rw-rw-   0        0        0     6687 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/_data.pyi
--rw-rw-rw-   0        0        0    16671 2023-01-25 18:52:53.000000 labbench-0.23.4/labbench/_device.py
--rw-rw-rw-   0        0        0     1272 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/_device.pyi
--rw-rw-rw-   0        0        0    12526 2023-01-25 18:53:11.000000 labbench-0.23.4/labbench/_host.py
--rw-rw-rw-   0        0        0     2116 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/_host.pyi
--rw-rw-rw-   0        0        0    55160 2023-01-25 18:52:17.000000 labbench-0.23.4/labbench/_rack.py
--rw-rw-rw-   0        0        0     6066 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/_rack.pyi
--rw-rw-rw-   0        0        0    11944 2023-01-25 18:42:27.000000 labbench-0.23.4/labbench/_serialize.py
--rw-rw-rw-   0        0        0      829 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/_serialize.pyi
--rw-rw-rw-   0        0        0    62482 2023-01-25 18:57:23.000000 labbench-0.23.4/labbench/_traits.py
--rw-rw-rw-   0        0        0    14582 2023-01-25 20:32:51.000000 labbench-0.23.4/labbench/_traits.pyi
--rw-rw-rw-   0        0        0     1744 2023-01-26 21:01:55.000000 labbench-0.23.4/labbench/_version.py
--rw-rw-rw-   0        0        0        0 2023-01-25 20:32:48.000000 labbench-0.23.4/labbench/_version.pyi
--rw-rw-rw-   0        0        0     2569 2023-01-25 18:58:08.000000 labbench-0.23.4/labbench/datareturn.py
--rw-rw-rw-   0        0        0     4109 2023-01-25 20:32:48.000000 labbench-0.23.4/labbench/datareturn.pyi
--rw-rw-rw-   0        0        0     7536 2023-01-25 18:33:42.000000 labbench-0.23.4/labbench/notebooks.py
--rw-rw-rw-   0        0        0      897 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/notebooks.pyi
--rw-rw-rw-   0        0        0     2568 2023-01-25 18:58:14.000000 labbench-0.23.4/labbench/property.py
--rw-rw-rw-   0        0        0     3933 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/property.pyi
--rw-rw-rw-   0        0        0        0 2021-08-18 18:41:24.000000 labbench-0.23.4/labbench/py.typed
--rw-rw-rw-   0        0        0    54361 2023-01-25 18:33:42.000000 labbench-0.23.4/labbench/util.py
--rw-rw-rw-   0        0        0     3048 2023-01-25 20:32:48.000000 labbench-0.23.4/labbench/util.pyi
--rw-rw-rw-   0        0        0     2600 2023-01-25 18:58:20.000000 labbench-0.23.4/labbench/value.py
--rw-rw-rw-   0        0        0     4353 2023-01-25 20:32:50.000000 labbench-0.23.4/labbench/value.pyi
-drwxrwxrwx   0        0        0        0 2023-01-26 21:04:43.055551 labbench-0.23.4/labbench.egg-info/
--rw-rw-rw-   0        0        0     1118 2023-01-26 21:04:42.000000 labbench-0.23.4/labbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-01-26 21:04:42.000000 labbench-0.23.4/labbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 21:04:42.000000 labbench-0.23.4/labbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-01-26 21:04:42.000000 labbench-0.23.4/labbench.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      293 2023-01-26 21:04:42.000000 labbench-0.23.4/labbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-01-26 21:04:42.000000 labbench-0.23.4/labbench.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-26 21:04:43.081687 labbench-0.23.4/scripts/
--rw-rw-rw-   0        0        0        0 2021-10-25 14:46:33.000000 labbench-0.23.4/scripts/__init__.py
--rw-rw-rw-   0        0        0     3679 2021-10-25 14:51:27.000000 labbench-0.23.4/scripts/cli.py
--rw-rw-rw-   0        0        0     5618 2023-01-25 20:32:13.000000 labbench-0.23.4/scripts/make_stubs.py
--rw-rw-rw-   0        0        0     2405 2023-01-25 18:33:42.000000 labbench-0.23.4/scripts/v21_to_v22.py
--rw-rw-rw-   0        0        0      114 2023-01-26 21:04:43.183040 labbench-0.23.4/setup.cfg
--rw-rw-rw-   0        0        0     5372 2023-01-25 18:33:42.000000 labbench-0.23.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-26 21:04:43.179037 labbench-0.23.4/tests/
--rw-rw-rw-   0        0        0        0 2021-05-11 16:34:25.000000 labbench-0.23.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2119 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/all.py
--rw-rw-rw-   0        0        0     1893 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/emulate.py
--rw-rw-rw-   0        0        0     3355 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/module_as_testbed.py
--rw-rw-rw-   0        0        0       57 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/profile_imports.py
--rw-rw-rw-   0        0        0     4754 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_data_logging.py
--rw-rw-rw-   0        0        0     2294 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_doc.py
--rw-rw-rw-   0        0        0     2211 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_email.py
--rw-rw-rw-   0        0        0     2211 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_notification.py
--rw-rw-rw-   0        0        0    10851 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_property.py
--rw-rw-rw-   0        0        0     8918 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_rack.py
--rw-rw-rw-   0        0        0    13357 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_sequencing.py
--rw-rw-rw-   0        0        0     4201 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_shell.py
--rw-rw-rw-   0        0        0     7727 2023-01-25 18:33:42.000000 labbench-0.23.4/tests/test_value.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:19:56.324416 labbench-0.25.0/cli/__init__.py
+-rw-r--r--   0        0        0     9144 2023-06-06 17:19:56.324416 labbench-0.25.0/cli/__main__.py
+-rw-r--r--   0        0        0     2946 2023-06-06 17:19:56.388415 labbench-0.25.0/labbench/__init__.py
+-rw-r--r--   0        0        0     1630 2023-06-06 17:19:56.392414 labbench-0.25.0/labbench/__init__.pyi
+-rw-r--r--   0        0        0    46636 2023-06-07 17:02:38.655815 labbench-0.25.0/labbench/_backends.py
+-rw-r--r--   0        0        0     5644 2023-06-06 17:19:56.396414 labbench-0.25.0/labbench/_backends.pyi
+-rw-r--r--   0        0        0    75388 2023-06-06 17:19:56.400415 labbench-0.25.0/labbench/_data.py
+-rw-r--r--   0        0        0     6201 2023-06-06 17:19:56.404415 labbench-0.25.0/labbench/_data.pyi
+-rw-r--r--   0        0        0    16241 2023-06-07 20:49:25.251548 labbench-0.25.0/labbench/_device.py
+-rw-r--r--   0        0        0     1056 2023-06-06 17:19:56.408414 labbench-0.25.0/labbench/_device.pyi
+-rw-r--r--   0        0        0    12576 2023-06-06 17:19:56.408414 labbench-0.25.0/labbench/_host.py
+-rw-r--r--   0        0        0     1765 2023-06-06 17:19:56.412414 labbench-0.25.0/labbench/_host.pyi
+-rw-r--r--   0        0        0    55225 2023-06-06 17:19:56.416415 labbench-0.25.0/labbench/_rack.py
+-rw-r--r--   0        0        0     5419 2023-06-06 17:19:56.420417 labbench-0.25.0/labbench/_rack.pyi
+-rw-r--r--   0        0        0    11878 2023-06-06 17:19:56.420417 labbench-0.25.0/labbench/_serialize.py
+-rw-r--r--   0        0        0      725 2023-06-06 17:19:56.424414 labbench-0.25.0/labbench/_serialize.pyi
+-rw-r--r--   0        0        0    62858 2023-06-07 20:49:14.039044 labbench-0.25.0/labbench/_traits.py
+-rw-r--r--   0        0        0    14105 2023-06-06 17:19:56.432415 labbench-0.25.0/labbench/_traits.pyi
+-rw-r--r--   0        0        0       60 2023-06-06 17:19:56.432415 labbench-0.25.0/labbench/_version.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:19:56.432415 labbench-0.25.0/labbench/_version.pyi
+-rw-r--r--   0        0        0     2569 2023-06-06 17:19:56.436416 labbench-0.25.0/labbench/datareturn.py
+-rw-r--r--   0        0        0     4144 2023-06-06 17:19:56.436416 labbench-0.25.0/labbench/datareturn.pyi
+-rw-r--r--   0        0        0     7451 2023-06-06 17:19:56.440414 labbench-0.25.0/labbench/notebooks.py
+-rw-r--r--   0        0        0      784 2023-06-06 17:19:56.440414 labbench-0.25.0/labbench/notebooks.pyi
+-rw-r--r--   0        0        0     2568 2023-06-06 17:19:56.444414 labbench-0.25.0/labbench/property.py
+-rw-r--r--   0        0        0     4001 2023-06-06 17:19:56.444414 labbench-0.25.0/labbench/property.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 17:19:56.444414 labbench-0.25.0/labbench/py.typed
+-rw-r--r--   0        0        0    51459 2023-06-06 17:19:56.448415 labbench-0.25.0/labbench/util.py
+-rw-r--r--   0        0        0     3285 2023-06-06 17:19:56.452415 labbench-0.25.0/labbench/util.pyi
+-rw-r--r--   0        0        0     2600 2023-06-06 17:19:56.452415 labbench-0.25.0/labbench/value.py
+-rw-r--r--   0        0        0     4447 2023-06-06 17:19:56.456416 labbench-0.25.0/labbench/value.pyi
+-rw-r--r--   0        0        0     2858 2023-06-06 17:19:56.320416 labbench-0.25.0/LICENSE.md
+-rw-r--r--   0        0        0     2481 2023-06-08 18:03:54.340433 labbench-0.25.0/pyproject.toml
+-rw-r--r--   0        0        0    11272 2023-06-06 17:19:56.320416 labbench-0.25.0/README.md
+-rw-r--r--   0        0        0     2119 2023-06-06 17:19:56.464416 labbench-0.25.0/tests/all.py
+-rw-r--r--   0        0        0     1880 2023-06-06 17:19:56.468415 labbench-0.25.0/tests/emulate.py
+-rw-r--r--   0        0        0     3332 2023-06-06 17:19:56.468415 labbench-0.25.0/tests/module_as_testbed.py
+-rw-r--r--   0        0        0       57 2023-06-06 17:19:56.472415 labbench-0.25.0/tests/profile_imports.py
+-rw-r--r--   0        0        0     4719 2023-06-06 17:19:56.472415 labbench-0.25.0/tests/test_data_logging.py
+-rw-r--r--   0        0        0     2287 2023-06-06 17:19:56.476415 labbench-0.25.0/tests/test_doc.py
+-rw-r--r--   0        0        0     2211 2023-06-06 17:19:56.480414 labbench-0.25.0/tests/test_email.py
+-rw-r--r--   0        0        0     2211 2023-06-06 17:19:56.480414 labbench-0.25.0/tests/test_notification.py
+-rw-r--r--   0        0        0    10850 2023-06-06 17:19:56.484414 labbench-0.25.0/tests/test_property.py
+-rw-r--r--   0        0        0     8889 2023-06-06 17:19:56.484414 labbench-0.25.0/tests/test_rack.py
+-rw-r--r--   0        0        0    13320 2023-06-06 17:19:56.488414 labbench-0.25.0/tests/test_sequencing.py
+-rw-r--r--   0        0        0     4192 2023-06-06 17:19:56.492414 labbench-0.25.0/tests/test_shell.py
+-rw-r--r--   0        0        0     7727 2023-06-06 17:19:56.492414 labbench-0.25.0/tests/test_value.py
+-rw-r--r--   0        0        0    27290 2023-02-06 21:28:33.062776 labbench-0.25.0/tests/testnb.ipynb
+-rw-r--r--   0        0        0    12103 1970-01-01 00:00:00.000000 labbench-0.25.0/PKG-INFO
```

### Comparing `labbench-0.23.4/LICENSE.md` & `labbench-0.25.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/README.md` & `labbench-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/cli/__main__.py` & `labbench-0.25.0/cli/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # skip the trace dump on ctrl+c
     sys.exit(1)
 
 EMPTY = inspect.Parameter.empty
 
 
 def empty_rack(cls):
-    """instantiate cls, filling in owned objects that have no default value """
+    """instantiate cls, filling in owned objects that have no default value"""
     init_params = inspect.signature(cls).parameters
     init_kws = {
         name: cls.__annotations__[name]() if param.default is EMPTY else param.default
         for name, param in init_params.items()
     }
     return cls(**init_kws)
 
@@ -33,15 +33,14 @@
     import labbench as lb
 
     if exc_info is None:
         exc_info = sys.exc_info()
     ex = exc_info[1]
 
     if isinstance(ex, lb.util.ConcurrentException) and len(ex.thread_exceptions) > 0:
-
         if isinstance(ex.thread_exceptions, (list, tuple)):
             ex.thread_exceptions = dict(enumerate(ex.thread_exceptions))
 
         for i, (name, thread_exc_info) in enumerate(ex.thread_exceptions.items()):
             progress_msg = (note or "") + "\n"
             progress_msg += f""
```

### Comparing `labbench-0.23.4/labbench/__init__.py` & `labbench-0.25.0/labbench/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,58 +23,55 @@
 .. PROVIDED HEREUNDER. Distributions of NIST software should also include
 .. copyright and licensing statements of any third-party software that are
 .. legally bundled with the code in compliance with the conditions of those
 .. licenses.
 """
 
 from .util import (
-    concurrently,
-    sequentially,
     Call,
-    stopwatch,
+    _force_full_traceback,
+    concurrently,
+    logger,
     retry,
-    until_timeout,
+    sequentially,
     show_messages,
     sleep,
-    logger,
+    stopwatch,
     timeout_iter,
-    _force_full_traceback,
+    until_timeout,
 )
 
 _force_full_traceback(True)
 
+from . import datareturn, property, util, value
 from ._backends import (
-    ShellBackend,
     DotNetDevice,
     LabviewSocketInterface,
     SerialDevice,
     SerialLoggingDevice,
+    ShellBackend,
     TelnetDevice,
     VISADevice,
     Win32ComDevice,
+    set_default_visa_backend,
 )
 from ._data import CSVLogger, HDFLogger, SQLiteLogger, read, read_relational
 from ._device import Device, list_devices, trait_info
 from ._host import Email
 from ._rack import (
     Rack,
     Sequence,
-    import_as_rack,
     find_owned_rack_by_type,
+    import_as_rack,
     rack_input_table,
     rack_kwargs_skip,
     rack_kwargs_template,
 )
-from ._traits import observe, unobserve, Undefined
-from ._serialize import load_rack, dump_rack
+from ._serialize import dump_rack, load_rack
+from ._traits import Undefined, observe, unobserve
 from ._version import __version__
 
-from . import value
-from . import property
-from . import datareturn
-from . import util
-
 # scrub __module__ for cleaner repr() and doc
 for _obj in dict(locals()).values():
     if getattr(_obj, "__module__", "").startswith("labbench."):
         _obj.__module__ = "labbench"
 del _obj
```

### Comparing `labbench-0.23.4/labbench/__init__.pyi` & `labbench-0.25.0/labbench/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,36 @@
-from . import datareturn as datareturn, property as property, util as util, value as value
+from . import (
+    datareturn as datareturn,
+    property as property,
+    util as util,
+    value as value,
+)
 from ._backends import (
     DotNetDevice as DotNetDevice,
     LabviewSocketInterface as LabviewSocketInterface,
     SerialDevice as SerialDevice,
     SerialLoggingDevice as SerialLoggingDevice,
     ShellBackend as ShellBackend,
     TelnetDevice as TelnetDevice,
     VISADevice as VISADevice,
     Win32ComDevice as Win32ComDevice,
+    set_default_visa_backend as set_default_visa_backend,
 )
 from ._data import (
     CSVLogger as CSVLogger,
     HDFLogger as HDFLogger,
     SQLiteLogger as SQLiteLogger,
     read as read,
     read_relational as read_relational,
 )
-from ._device import Device as Device, list_devices as list_devices, trait_info as trait_info
+from ._device import (
+    Device as Device,
+    list_devices as list_devices,
+    trait_info as trait_info,
+)
 from ._host import Email as Email
 from ._rack import (
     Rack as Rack,
     Sequence as Sequence,
     find_owned_rack_by_type as find_owned_rack_by_type,
     import_as_rack as import_as_rack,
     rack_input_table as rack_input_table,
```

### Comparing `labbench-0.23.4/labbench/_backends.py` & `labbench-0.25.0/labbench/_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,35 +20,33 @@
 # BY PERSONS OR PROPERTY OR OTHERWISE, AND WHETHER OR NOT LOSS WAS SUSTAINED
 # FROM, OR AROSE OUT OF THE RESULTS OF, OR USE OF, THE SOFTWARE OR SERVICES
 # PROVIDED HEREUNDER. Distributions of NIST software should also include
 # copyright and licensing statements of any third-party software that are
 # legally bundled with the code in compliance with the conditions of those
 # licenses.
 
-from ._device import Device
-from . import property as property_
-from . import value
-from ._traits import observe
-from . import util
-
-from collections import OrderedDict
 import contextlib
+import importlib
 import inspect
 import os
-import psutil
-import serial
-from queue import Queue, Empty
-import socket
 import select
+import socket
+import subprocess as sp
 import sys
-from threading import Thread, Event
+from collections import OrderedDict
+from pathlib import Path
+from queue import Empty, Queue
+from threading import Event, Thread
 
-# sentinel values unless they are imported later
-win32com = None
-pyvisa = None
+import psutil
+
+from . import property as property_
+from . import util, value
+from ._device import Device
+from ._traits import observe
 
 
 class ShellBackend(Device):
     """Virtual device controlled by a shell command in another process.
 
     Data can be captured from standard output, and standard error pipes, and
     optionally run as a background thread.
@@ -82,19 +80,14 @@
     # )
     #
     # arguments_min = value.int(
     #     default=0, min=0,
     #     sets=False, help='minimum extra command line arguments needed to run'
     # )
 
-    @classmethod
-    def __imports__(cls):
-        global sp
-        import subprocess as sp
-
     def open(self):
         """The :meth:`open` method implements opening in the
         :class:`Device` object protocol. Call the
         :meth:`execute` method when open to
         execute the binary.
         """
 
@@ -136,28 +129,28 @@
                 check_return=check_return,
                 check_stderr=check_stderr,
                 timeout=timeout,
                 respawn=respawn,
             )
 
         if respawn:
-            raise ValueError(f"respawn argument requires pipe=True and background=True")
+            raise ValueError("respawn argument requires pipe=True and background=True")
 
         if pipe and not background:
             return self._run_piped(
                 *argv,
                 check_return=check_return,
                 check_stderr=check_stderr,
                 timeout=timeout,
             )
         else:
             if background:
-                raise ValueError(f"background argument requires pipe=True")
+                raise ValueError("background argument requires pipe=True")
             if check_stderr:
-                raise ValueError(f"check_stderr requires pipe=True")
+                raise ValueError("check_stderr requires pipe=True")
 
             return self._run_simple(*argv, check_return=check_return, timeout=timeout)
 
     def _run_simple(self, *argv, check_return=False, timeout=None):
         """Blocking execution of the binary at `self.binary_path`. If check=True, raise an exception
         on non-zero return code.
 
@@ -222,15 +215,15 @@
             remaining = max(0, len(lines) - show_count)
 
             logger_msgs = [f"► {line}" for line in lines[: show_count // 2]]
             if remaining > 0:
                 logger_msgs.append(f"…{remaining} more lines")
             for line in lines[-show_count // 2 :]:
                 logger_msgs.append(f"► {line}")
-            self._logger.debug('\n'.join(logger_msgs))
+            self._logger.debug("\n".join(logger_msgs))
         return ret
 
     def _background_piped(
         self, *argv, check_return=False, check_stderr=False, respawn=False, timeout=None
     ):
         """Run the executable in the background (returning immediately while
         the executable continues running).
@@ -311,15 +304,14 @@
             si = sp.STARTUPINFO()
             si.dwFlags |= sp.STARTF_USESHOWWINDOW
 
             proc = sp.Popen(
                 list(cmdl),
                 stdout=sp.PIPE,
                 startupinfo=si,
-                bufsize=1,
                 creationflags=sp.CREATE_NEW_PROCESS_GROUP,
                 stderr=sp.PIPE,
             )
 
             self.backend = proc
             Thread(target=lambda: stdout_to_queue(proc.stdout, cmdl)).start()
             if check_stderr:
@@ -358,15 +350,15 @@
                 continue
 
             elif trait.type is bool:
                 if flag_str is None:
                     # this would require a remap parameter in value traits, which are not supported (should they be?)
                     # (better to use string?)
                     raise ValueError(
-                        f"don't know how to map a Bool onto a string argument as specified by None mapping"
+                        "cannot map a Bool onto a string argument specified by None mapping"
                     )
 
                 elif trait_value:
                     # trait_value is truey
                     argv += [flag_str]
                     continue
 
@@ -428,15 +420,15 @@
 
             stdout
         """
         result = ""
 
         if not self.isopen:
             raise ConnectionError(
-                f"an open connection is necessary to read stdout from the background process"
+                "open the device to read stdout from the background process"
             )
 
         try:
             n = 0
             while True:
                 line = self._stdout.get(wait_for > 0, timeout=self.timeout)
                 if isinstance(line, Exception):
@@ -518,18 +510,14 @@
 
             for child in children:
                 ShellBackend._kill_proc_tree(child.pid)
         except psutil.NoSuchProcess:
             pass
 
 
-import importlib
-from pathlib import Path
-
-
 class DotNetDevice(Device):
     """Base class for .NET library wrappers based on pythonnet.
 
     To implement a DotNetDevice subclass::
 
         import labbench as lb
 
@@ -562,39 +550,36 @@
             raise ImportError("pythonnet module is required to use dotnet drivers")
 
         # base dotnet libraries needed to identify what we're working with
         clr.setPreload(False)
         clr.AddReference("System.Reflection")
 
         # more frustration for static linters
-        from System.Reflection import Assembly
         import System
+        from System.Reflection import Assembly
 
         try:
             contents = importlib.util.find_spec(library.__package__).loader.get_data(
                 str(dll_path)
             )
-        except:
+        except BaseException:
             with open(dll_path, "rb") as f:
                 contents = f.read()
 
         # binary file contents
         contents = importlib.util.find_spec(library.__package__).loader.get_data(
             str(dll_path)
         )
 
         # dump that into dotnet
         Assembly.Load(System.Array[System.Byte](contents))
 
         # do the actual import
         self.dll = importlib.import_module(dll_path.stem)
 
-    def open(self):
-        pass
-
 
 class LabviewSocketInterface(Device):
     """Base class demonstrating simple sockets-based control of a LabView VI.
 
     Keyed get/set with lb.property are implemented by simple ' command value'.
     Subclasses can therefore implement support for commands in
     specific labview VI similar to VISA commands by
@@ -703,14 +688,16 @@
     dsrdtr = value.bool(False, help="`True` to enable hardware (DSR/DTR) flow control.")
 
     # Overload methods as needed to implement the Device object protocol
     def open(self):
         """Connect to the serial device with the VISA resource string defined
         in self.resource
         """
+        import serial
+
         keys = "timeout", "parity", "stopbits", "xonxoff", "rtscts", "dsrdtr"
         params = dict([(k, getattr(self, k)) for k in keys])
         self.backend = serial.Serial(self.resource, self.baud_rate, **params)
         self._logger.debug(f"{repr(self)} connected")
 
     def close(self):
         """Disconnect the serial instrument"""
@@ -906,23 +893,20 @@
     the property trait set and get operations (as appropriate).
     """
 
     # Connection value traits
     resource = value.NetworkAddress("127.0.0.1:23", help="server host address")
     timeout = value.float(2, min=0, label="s", help="connection timeout")
 
-    @classmethod
-    def __imports__(cls):
-        global Telnet
-        from telnetlib import Telnet
-
     def open(self):
         """Open a telnet connection to the host defined
         by the string in self.resource
         """
+        from telnetlib import Telnet
+
         host, *port = self.resource.split(":")
 
         if len(port) > 0:
             port = int(port[0])
         else:
             port = 23
 
@@ -1004,21 +988,14 @@
             "message available": bool(code & 0b00010000),
             "event status flag": bool(code & 0b00100000),
             "service request": bool(code & 0b01000000),
             "top level status summary": bool(code & 0b01000000),
             "operating": bool(code & 0b10000000),
         }
 
-    @classmethod
-    def __imports__(cls):
-        global pyvisa
-        import pyvisa
-        import pyvisa.constants
-
-
     # Overload methods as needed to implement RemoteDevice
     def open(self):
         """opens the instrument.
 
         When managing device connection through a `with` context,
         this is called automatically and does not need
         to be invoked.
@@ -1034,14 +1011,16 @@
     def close(self):
         """closes the instrument.
 
         When managing device connection through a `with` context,
         this is called automatically and does not need
         to be invoked.
         """
+        import pyvisa
+
         if not self.isopen or self.backend is None:
             return
 
         try:
             with contextlib.suppress(pyvisa.errors.VisaIOError):
                 self._release_remote_control()
             with contextlib.suppress(pyvisa.Error):
@@ -1222,30 +1201,35 @@
 
             If the command 1 raises an exception, command 2 will not execute
             the context block is complete, and the exception from command 1
             is swallowed.
         """
 
         def __exit__(self, exctype, excinst, exctb):
+            import pyvisa
+
             EXC = pyvisa.errors.VisaIOError
             CODE = pyvisa.errors.StatusCode.error_timeout
 
             return exctype == EXC and excinst.error_code == CODE
 
     def _release_remote_control(self):
+        import pyvisa
+        import pyvisa.constants
+
         # From instrument and pyvisa docs
         self.backend.visalib.viGpibControlREN(
             self.backend.session, pyvisa.constants.VI_GPIB_REN_ADDRESS_GTL
         )
 
-    @classmethod
-    def _get_rm(cls):
-        cls.__imports__()
+    def _get_rm(self):
+        import pyvisa
+        import pyvisa.constants
 
-        backend_name = cls._rm.default
+        backend_name = self._rm
 
         if backend_name in ("@ivi", "@ni"):
             is_ivi = True
             # compatibility layer for changes in pyvisa 1.12
             if "ivi" in pyvisa.highlevel.list_backends():
                 backend_name = "@ivi"
             else:
@@ -1261,14 +1245,22 @@
                 msg = f"could not connect to NI VISA resource manager - see {url}"
                 e.args[0] += msg
             raise e
 
         return rm
 
 
+def set_default_visa_backend(name):
+    if name not in VISADevice._rm.only:
+        raise ValueError(
+            f"backend name '{name}' is not one of the allowed {VISADevice._rm.only}"
+        )
+    VISADevice._rm.default = name
+
+
 class SimulatedVISADevice(VISADevice, _rm="@sim"):
     """Base class for wrapping simulated VISA devices with pyvisa.
 
     See also:
         - _Backend information: https://pyvisa-sim.readthedocs.io/
     """
 
@@ -1278,22 +1270,22 @@
     )
 
     def _release_remote_control(self):
         pass
 
     @classmethod
     def _get_rm(cls):
-        cls.__imports__()
+        import pyvisa
 
         backend_name = f"{cls.yaml_source.default}@sim"
 
         try:
             rm = pyvisa.ResourceManager(backend_name)
         except OSError as e:
-            e.args[0] += f"is pyvisa-sim installed?"
+            e.args[0] += "is pyvisa-sim installed?"
             raise e
 
         return rm
 
 
 class Win32ComDevice(Device, concurrency=True):
     """Basic support for calling win32 COM APIs.
@@ -1309,22 +1301,18 @@
     # to the dispatched COM object block until the previous calls are completed
     # from within.
 
     com_object = value.str(
         default="", sets=False, help="the win32com object string"
     )  # Must be a module
 
-    @classmethod
-    def __imports__(cls):
-        global win32com
-        import win32com
-        import win32com.client
-
     def open(self):
         """Connect to the win32 com object"""
+        import win32com
+        import win32com.client
 
         def should_sandbox(obj):
             try:
                 name = win32com.__name__
                 return inspect.getmodule(obj).__name__.startswith(name)
             except AttributeError:
                 return False
```

### Comparing `labbench-0.23.4/labbench/_data.py` & `labbench-0.25.0/labbench/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 import io
 import json
 from numbers import Number
 import os
 from pathlib import Path
 import pickle
 import shutil
-import tarfile
 import warnings
 
 EMPTY = inspect._empty
 
 INSPECT_SKIP_FILES = _device.__file__, _traits.__file__, _rack.__file__, __file__
 
 
@@ -92,55 +91,52 @@
         path to the data saved on disk.
 
         Arguments:
             row: dictionary of {'entry_name': "entry_value"} pairs
         Returns:
             the row dictionary, replacing special entries with the relative path to the saved data file
         """
+        import pandas as pd
+        import numpy as np
 
         def is_path(v):
             if not isinstance(v, str):
                 return False
             try:
                 return os.path.exists(v)
             except ValueError:
                 return False
 
-        for name, value in row.items():
-            if is_path(value):
+        for name, v in row.items():
+            if is_path(v):
                 # Path to a datafile to move into the dataset
-                row[name] = self._from_external_file(name, value, index, row)
+                row[name] = self._from_external_file(name, v, index, row)
 
-            elif isinstance(value, (str, bytes)):
+            elif isinstance(v, (str, bytes)):
                 # A long string that should be written to a text file
                 if (
-                    len(value) > self.text_relational_min
+                    len(v) > self.text_relational_min
                     or name in self.force_relational
-                    or isinstance(value, bytes)
+                    or isinstance(v, bytes)
                 ):
-                    row[name] = self._from_text(name, value, index, row)
+                    row[name] = self._from_text(name, v, index, row)
 
-            elif isinstance(value, (np.ndarray, pd.Series, pd.DataFrame)):
+            elif isinstance(v, (np.ndarray, pd.Series, pd.DataFrame)):
                 # vector, table, matrix, etc.
-                row[name] = self._from_ndarraylike(name, value, index, row)
+                row[name] = self._from_ndarraylike(name, v, index, row)
 
-            elif hasattr(value, "__len__") or hasattr(value, "__iter__"):
+            elif hasattr(v, "__len__") or hasattr(v, "__iter__"):
                 # tuple, list, or other iterable
-                row[name] = self._from_sequence(name, value, index, row)
+                row[name] = self._from_sequence(name, v, index, row)
 
         return row
 
-    @classmethod
-    def __imports__(cls):
-        global np, pd
-
-        import numpy as np
+    def save_metadata(self, name, key_func, **extra):
         import pandas as pd
 
-    def save_metadata(self, name, key_func, **extra):
         def process_value(value, key_name):
             if isinstance(value, (str, bytes)):
                 if len(value) > self.text_relational_min:
                     self._from_text(key_name, value)
                 else:
                     return value
             elif hasattr(value, "__len__") or hasattr(value, "__iter__"):
@@ -149,15 +145,14 @@
                 else:
                     return ""
             else:
                 return value
 
         summary = dict(extra)
         for owner, owner_name in name.items():
-
             for trait_name, trait in owner._traits.items():
                 if trait.role == _traits.Trait.ROLE_VALUE or trait.cache:
                     summary[key_func(owner_name, trait_name)] = getattr(
                         owner, trait_name
                     )
         summary = {k: process_value(v, k) for k, v in summary.items()}
 
@@ -175,14 +170,15 @@
         Arguments:
             name: name of the entry to write, used as the filename
             value: the object containing array-like data
             row: row dictionary, or None (the default) to write to the metadata folder
         Returns:
             the path to the file, relative to the directory that contains the root database
         """
+        import pandas as pd
 
         def write(stream, ext, value):
             if ext == "csv":
                 value.to_csv(stream)
             elif ext == "json":
                 value.to_json(stream)
             elif ext in ("p", "pickle"):
@@ -301,14 +297,19 @@
         """
 
         raise NotImplementedError
 
     def _import_from_file(self, old_path, dest):
         raise NotImplementedError
 
+    def open(self):
+        # make sure these are fresh in the module cache
+        import pandas as pd
+        import numpy as np
+
 
 class MungeToDirectory(MungerBase):
     """Implement data munging into subdirectories."""
 
     def _open_relational(self, name, index, row, mode):
         if "host_time" not in row:
             self._logger.error(
@@ -360,14 +361,16 @@
 
         # TODO: Find a more generic way to force valid path name
         relpath = relpath.replace(":", "")
         relpath = os.path.join(self.resource, relpath)
         return relpath
 
     def _write_metadata(self, metadata):
+        import pandas as pd
+
         def recursive_dict_fix(d):
             d = dict(d)
             for name, obj in dict(d).items():
                 if isinstance(obj, Path):
                     d[name] = str(obj)
                 elif isinstance(obj, bytes):
                     d[name] = obj.decode()
@@ -416,14 +419,16 @@
     #
 
     def close(self):
         # First: dump the data into the tar file
         #        tarpath = os.path.join(self.tarbase, self.tarname)
         #        f = tarfile.open(tarpath, 'a')
 
+        import tarfile
+
         try:
             if not self.overwrite and self.name in self.tarfile.getnames():
                 raise IOError(f"{self.name} already exists in {self.tarfile.name}")
 
             tarinfo = tarfile.TarInfo(self.name)
             tarinfo.size = self.tell()
 
@@ -454,14 +459,15 @@
         return TarFileIO(self.tarfile, relpath, mode=mode)
 
     def _open_metadata(self, name, mode):
         dirpath = os.path.join(self.metadata_dirname, name)
         return TarFileIO(self.tarfile, dirpath, mode=mode)
 
     def open(self):
+        import tarfile
 
         if not os.path.exists(self.resource):
             with suppress(FileExistsError):
                 os.makedirs(self.resource)
         self.tarfile = tarfile.open(os.path.join(self.resource, self.tarname), "a")
 
     def close(self):
@@ -493,14 +499,16 @@
         try:
             remove()
             self._logger.debug(f"moved {old_path} to into tar file as {dest}")
         except PermissionError:
             self._logger.warning(f"could not remove old file or directory {old_path}")
 
     def _write_metadata(self, metadata):
+        import pandas as pd
+
         for k, v in metadata.items():
             stream = self._open_metadata(k + ".json", "w")
             if hasattr(stream, "overwrite"):
                 stream.overwrite = True
 
             if isinstance(v, pd.DataFrame):
                 v = v.to_dict()["Value"]
@@ -659,24 +667,24 @@
 
     def _receive_rack_input(self, msg: dict):
         """called by an owning Rack notifying that managed procedural steps have returned data"""
         # trait data or previous returned data may cause problems here. perhaps this should be an exception?
 
         if self._rack_toplevel_caller is None:
             # take the first call as the top-level caller
-            self._rack_toplevel_caller = msg['owner']
+            self._rack_toplevel_caller = msg["owner"]
 
-        elif self._rack_toplevel_caller != msg['owner']:
+        elif self._rack_toplevel_caller != msg["owner"]:
             # only track calls to the top-level caller
             return
 
         else:
             self._rack_input_index += 1
 
-        iter_info = msg["new"]
+        # iter_info = msg["new"]
         row_data = dict(index=self._rack_input_index)
 
         # if len(self._iter_index_names) > 0:
         #     self._iter_index_names.setdefault(
         #         msg["owner"], "index_" + msg["owner"]._owned_name
         #     )
         # else:
@@ -689,15 +697,15 @@
         # TODO: should there be some kind of conflict check for this?
         # key_conflicts = set(row_data).intersection(self._pending_traits_persistent)
         # if len(key_conflicts) > 0:
         #     self._logger.warning(
         #         f"Rack call overwrites prior data with existing keys {key_conflicts}"
         #     )
 
-        self._pending_rack_input = dict(row_data, **msg['new'])
+        self._pending_rack_input = dict(row_data, **msg["new"])
 
     def _receive_trait_update(self, msg: dict):
         """called by trait owners on changes observed
 
         Arguments:
             msg (dict): callback info dictionary generated by traitlets
         Returns:
@@ -791,26 +799,22 @@
             raise ValueError("devices argument must be a device or iterable of devices")
 
         if isinstance(always, str):
             always = (always,)
         elif hasattr(always, "__iter__"):
             always = tuple(always)
         else:
-            raise ValueError(
-                "argument 'always' must be a str or iterable of str"
-            )
+            raise ValueError("argument 'always' must be a str or iterable of str")
 
         if isinstance(never, str):
             never = (never,)
         elif hasattr(never, "__iter__"):
             never = tuple(never)
         else:
-            raise ValueError(
-                "argument 'never' must be a str or iterable of str"
-            )
+            raise ValueError("argument 'never' must be a str or iterable of str")
 
         # if isinstance(role, (str,bytes)):
         #     role = [role]
         # TODO: remove this for good?
         # if role not in VALID_TRAIT_ROLES:
         #     raise ValueError(f"the 'role' argument must be one of {str(VALID_TRAIT_ROLES)}, not {role}")
 
@@ -920,15 +924,14 @@
         dirname_fmt="{id} {host_time}",
         nonscalar_file_type="csv",
         metadata_dirname="metadata",
         tar=False,
         git_commit_in=None,
         # **metadata
     ):
-
         self.aggregator = Aggregator()
 
         super().__init__()
 
         # log host introspection
         # TODO: smarter
         self.host = _host.Host(git_commit_in=git_commit_in)
@@ -1068,40 +1071,39 @@
         with the relative path to the data file.
 
         Returns:
 
             None
         """
         if len(self.pending_output) != len(self.pending_input):
-            util.logger.warning('the input and output have mismatched length')
+            util.logger.warning("the input and output have mismatched length")
 
         count = max(len(self.pending_output), len(self.pending_input))
 
         if count > 0:
             proc = self._row_preprocessor
 
             self.pending_output = [
                 self.munge(self.output_index + i, proc(row))
                 for i, row in enumerate(self.pending_output)
             ]
 
-
             self.pending_input = [
                 self.munge(self.output_index + i, proc(row))
                 for i, row in enumerate(self.pending_input)
             ]
 
             self.output_index += len(self.pending_output) - 1
             self._write_root()
             self.clear()
 
     @contextmanager
     @util.hide_in_traceback
     def context(self, *args, **kws):
-        """ calls `self.new_row(*args, **kws); self.write()` on context exit.
+        """calls `self.new_row(*args, **kws); self.write()` on context exit.
 
         This is meant as a convenience for defining execution behavior in
         table inputs for Racks.
         """
 
         try:
             yield self
@@ -1169,15 +1171,15 @@
         This is an abstract base method (to be overridden by inheriting classes)
 
         Returns:
             None
         """
 
         if self.path is None:
-            raise TypeError(f"cannot open dB while path is None")
+            raise TypeError("cannot open dB while path is None")
 
         self.observe(self.munge, never=self.munge._traits)
         self.observe(self.host, always=["time", "log"])
 
         # Do some checks on the relative data directory before we consider overwriting
         # the root db.
         self.aggregator.enable()
@@ -1239,14 +1241,16 @@
                 pass
 
         would instantiate a `CSVLogger` instance, and also guarantee
         a final attempt to write unwritten data is written, and that
         the file is closed when exiting the `with` block, even if there
         is an exception.
         """
+        import pandas as pd
+
         self.tables = {}
 
         self.path.mkdir(parents=True, exist_ok=self._append)
 
         for file_name in self.OUTPUT_FILE_NAME, self.INPUT_FILE_NAME:
             file_path = self.path / file_name
             try:
@@ -1272,27 +1276,32 @@
     def _write_root(self):
         """Write queued rows of data to csv. This is called automatically on :func:`close`, or when
         exiting a `with` block.
 
         If the class was created with overwrite=True, then the first call to _write_root() will overwrite
         the preexisting file; subsequent calls append.
         """
+        import pandas as pd
 
         def append_csv(path_to_csv, df):
             if len(df) == 0:
                 return
-            isfirst = self.tables.get(path_to_csv.name,None) is None
+            isfirst = self.tables.get(path_to_csv.name, None) is None
             pending = pd.DataFrame(df)
             pending.index.name = self.index_label
             pending.index = pending.index + self.output_index
 
             if isfirst:
                 self.tables[path_to_csv.name] = pending
             else:
-                self.tables[path_to_csv.name] = self.tables[path_to_csv.name].append(pending).loc[self.output_index :]
+                self.tables[path_to_csv.name] = (
+                    self.tables[path_to_csv.name]
+                    .append(pending)
+                    .loc[self.output_index :]
+                )
             self.tables[path_to_csv.name].sort_index(inplace=True)
             self.output_index = self.tables[path_to_csv.name].index[-1]
 
             self.path.mkdir(exist_ok=True, parents=True)
 
             with open(path_to_csv, "a") as f:
                 self.tables[path_to_csv.name].to_csv(f, header=isfirst, index=False)
@@ -1324,15 +1333,15 @@
         "{id} {host_time}",
         help="format for linked data in the root database (keyed on column)",
     )
 
     def open(self):
         import h5py
 
-        self.backend = h5 = h5py.File(self.resource, "a")
+        self.backend = h5py.File(self.resource, "a")
 
     def close(self):
         self.backend.close()
 
     def __call__(self, index, row):
         """
         Break special cases of row items that need to be stored in
@@ -1349,37 +1358,39 @@
             if not isinstance(v, str):
                 return False
             try:
                 return os.path.exists(v)
             except ValueError:
                 return False
 
-        for name, value in row.items():
+        for name, v in row.items():
             # A path outside the relational database tree
-            if is_path(value):
+            if is_path(v):
                 # A file or directory that should be moved in
-                row[name] = self._from_external_file(name, value, index, row)
+                row[name] = self._from_external_file(name, v, index, row)
 
             # A long string that should be written to a text file
-            elif isinstance(value, (str, bytes, Number)):
-                row[name] = value
+            elif isinstance(v, (str, bytes, Number)):
+                row[name] = v
 
-            elif hasattr(value, "__len__") or hasattr(value, "__iter__"):
+            elif hasattr(v, "__len__") or hasattr(v, "__iter__"):
                 # vector, table, matrix, etc.
-                row[name] = self._from_nonscalar(name, value, index, row)
+                row[name] = self._from_nonscalar(name, v, index, row)
 
             else:
                 self._logger.warning(
-                    fr"unrecognized type for row entry '{name}' with type {repr(value)}"
+                    rf"unrecognized type for row entry '{name}' with type {repr(v)}"
                 )
-                row[name] = value
+                row[name] = v
 
         return row
 
     def save_metadata(self, name, key_func, **extra):
+        import pandas as pd
+
         def process_value(value, key_name):
             if isinstance(value, (str, bytes)):
                 return value
             elif hasattr(value, "__len__") or hasattr(value, "__iter__"):
                 if not hasattr(value, "__len__") or len(value) > 0:
                     self._from_nonscalar(key_name, value)
                 else:
@@ -1406,14 +1417,15 @@
         Arguments:
             name: name of the entry to write, used as the filename
             value: the object containing array-like data
             row: row dictionary, or None (the default) to write to the metadata folder
         Returns:
             the path to the file, relative to the directory that contains the root database
         """
+        import pandas as pd
 
         key = self._get_key(name, index, row)
 
         try:
             df = pd.DataFrame(value)
             if df.shape[0] == 0:
                 df = pd.DataFrame([df])
@@ -1426,15 +1438,14 @@
 
         else:
             df.to_hdf(self.resource, key=key)
 
         return key
 
     def _from_external_file(self, name, old_path, index=0, row=None, ntries=10):
-
         with open(old_path, "rb") as f:
             return f.read()
 
     def _get_key(self, name, index, row):
         if row is None:
             return f"/metadata {name}"
         else:
@@ -1454,16 +1465,16 @@
     Arguments:
         path (str): Base path to use for the root database
         append (bool): Whether to append to the root database if it already exists (otherwise, raise IOError)
         key_fmt (str): format to use for keys in the h5
 
     """
 
-    KEY_OUTPUT = 'output'
-    KEY_INPUT = 'input'
+    KEY_OUTPUT = "output"
+    KEY_INPUT = "input"
 
     nonscalar_file_type = "csv"
 
     def __init__(
         self,
         path,
         *,
@@ -1474,15 +1485,17 @@
     ):
         if str(path).endswith(".h5"):
             path = Path(path)
         else:
             path = Path(str(path) + ".h5")
 
         super().__init__(
-            path=path, append=append, git_commit_in=git_commit_in,
+            path=path,
+            append=append,
+            git_commit_in=git_commit_in,
         )
 
         # Switch to the HDF munger
         self.munge = MungeToHDF(path, key_fmt=key_fmt)
 
     def open(self):
         """Instead of calling `open` directly, consider using
@@ -1507,25 +1520,26 @@
     def _write_root(self):
         """Write queued rows of data to csv. This is called automatically on :func:`close`, or when
         exiting a `with` block.
 
         If the class was created with overwrite=True, then the first call to _write_root() will overwrite
         the preexisting file; subsequent calls append.
         """
+        import pandas as pd
 
         def write_table(key, data):
-            print('write table! ', key, data)
+            print("write table! ", key, data)
             if len(data) == 0:
                 return
             isfirst = self.df is None
             pending = pd.DataFrame(data)
             pending.index.name = self.index_label
             pending.index += self.output_index
             if isfirst:
-                print('first!')
+                print("first!")
                 self.df = pending
             else:
                 print(self.df.columns, pending.columns)
                 self.df = self.df.append(pending).loc[self.output_index :]
             self.df.sort_index(inplace=True)
             self.output_index = self.df.index[-1]
 
@@ -1574,14 +1588,16 @@
                 pass
 
         would instantiate a `SQLiteLogger` instance, and also guarantee
         a final attempt to write unwritten data is written, and that
         the file is closed when exiting the `with` block, even if there
         is an exception.
         """
+        from sqlalchemy import create_engine  # database connection
+        import pandas as pd
 
         if self.path.exists():
             root = str(self.path.absolute())
             if not self.path.is_dir():
                 raise IOError(
                     f"the root data directory path '{root}' already exists, and is not a directory."
                 )
@@ -1599,16 +1615,14 @@
 
         #        if not self.path.lower().endswith('.db'):
         #            self.path += '.db'
         os.makedirs(self.path, exist_ok=True)
         path = os.path.join(self.path, self.ROOT_FILE_NAME)
 
         # Create an engine via sqlalchemy
-        from sqlalchemy import create_engine  # database connection
-
         self._engine = create_engine("sqlite:///{}".format(path))
 
         if os.path.exists(path):
             if self._append:
                 # read the last row to 1) list the columns and 2) get index
                 query = f"select * from {self.OUTPUT_TABLE_NAME} order by {self.index_label} desc limit 1"
 
@@ -1633,14 +1647,15 @@
     def _write_root(self):
         """Write queued rows of data to the database. This also is called automatically on :func:`close`, or when
         exiting a `with` block.
 
         If the class was created with overwrite=True, then the first call to _write_root() will overwrite
         the preexisting file; subsequent calls append.
         """
+        import pandas as pd
 
         if len(self.pending_output) == 0:
             return
 
         # Put together a DataFrame from self.pending that is guaranteed
         # to include the columns defined in self._columns
         traits = pd.DataFrame(self.pending_output)
@@ -1720,14 +1735,15 @@
 
     def _get_notnull_col_dtype(self, col):
         """
         Infer datatype of the Series col.  In case the dtype of col is 'object'
         and it contains NA values, this infers the datatype of the not-NA
         values.  Needed for inserting typed data containing NULLs, GH8778.
         """
+        import pandas as pd
 
         col_for_inference = col
         if col.dtype == "object":
             notnulldata = col[~pd.isnull(col)]
             if len(notnulldata):
                 col_for_inference = notnulldata
 
@@ -1747,14 +1763,15 @@
         None
 
     """
     import numpy as np
 
     iname, data.index.name = data.index.name, None
     cname, data.columns.name = data.columns.name, None
+
     try:
         if not (
             data.index.is_monotonic
             and data.index[0] == 0
             and data.index[-1] == data.shape[0] - 1
         ):
             data = data.reset_index()
@@ -1779,15 +1796,15 @@
         table_name: name of table in the sqlite database
         columns: columns to query and return, or None (default) to return all columns
         nrows: number of rows of data to read, or None (default) to return all rows
         index_col: the name of the column to use as the index
     Returns:
         pandas.DataFrame instance containing data loaded from `path`
     """
-
+    import pandas as pd
     from sqlalchemy import create_engine
 
     engine = create_engine(f"sqlite:///{path}")
     df = pd.read_sql_table(table_name, engine, index_col=index_col, columns=columns)
     engine.dispose()
     if nrows is not None:
         df = df.iloc[:nrows]
@@ -1804,14 +1821,15 @@
         nrows: number of rows to read at the beginning of the table, or None (the default) to read all rows
         format (str): data file format, one of ['pickle','feather','csv','json','csv'], or 'auto' (the default) to guess from the file extension
         kws: additional keyword arguments to pass to the pandas read_<ext> function matching the file extension
     Returns:
         pandas.DataFrame instance containing data read from file
     """
 
+    import pandas as pd
     from pyarrow.feather import read_feather
 
     reader_guess = {
         "p": pd.read_pickle,
         "pickle": pd.read_pickle,
         "db": read_sqlite,
         "sqlite": read_sqlite,
@@ -1838,15 +1856,17 @@
             raise ValueError(
                 "can only guess format for string path - specify extension"
             )
 
     try:
         reader = reader_guess[format]
     except KeyError as e:
-        raise Exception(f"couldn't guess a reader from extension of file {path_or_buf}")
+        raise Exception(
+            f"couldn't guess a reader from extension of file {path_or_buf}"
+        ) from e
 
     if reader == read_sqlite:
         return reader(path_or_buf, columns=columns, nrows=nrows, **kws)
     elif reader == pd.read_csv:
         return reader(path_or_buf, usecols=columns, nrows=nrows, **kws)
     else:
         if columns is None:
@@ -1863,15 +1883,14 @@
         self.tarfile = tarfile.open(os.path.join(path, tarname), "r")
 
     def __call__(self, key, *args, **kws):
         key = key.replace("\\\\", "\\")
 
         for k in key, key.replace("\\", "/").replace("//", "/"):
             try:
-
                 ext = os.path.splitext(key)[1][1:]
                 return read(self.tarfile.extractfile(k), format=ext, *args, **kws)
             except KeyError as e:
                 ex = e
                 continue
             else:
                 break
@@ -1933,14 +1952,15 @@
         target_cols: a column (or array-like iterable of multiple columns) listing the root columns to include in the expanded dataframe, or None (the default) to pass all columns loaded from each root[expand_col]
         root_path: a string containing the full path to the root database (to help find the relational files)
         prepend_column_name (bool): whether to prepend the name of the expanded column from the root database
     Returns:
         the expanded dataframe
 
     """
+    import pandas as pd
 
     # if not isinstance(root, (pd.DataFrame,pd.Series)):
     #     raise ValueError('expected root to be a DataFrame instance, but it is {} instead'\
     #                      .format(repr(type(root))))
     if not isinstance(expand_col, str):
         raise ValueError(f"expand_col must a str, not {type(expand_col)}")
```

### Comparing `labbench-0.23.4/labbench/_data.pyi` & `labbench-0.25.0/labbench/_data.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,323 +1,219 @@
 import io
 from . import _device as core, util as util, value as value
 from ._device import Device as Device
 from ._rack import Owner as Owner, Rack as Rack
 from ._traits import observe as observe
 from _typeshed import Incomplete
 from collections.abc import Generator
+
 EMPTY: Incomplete
 INSPECT_SKIP_FILES: Incomplete
 
-
 class MungerBase(core.Device):
-
     def __init__(
         self,
-        resource: str='WindowsPath',
-        text_relational_min: str='int',
-        force_relational: str='list',
-        dirname_fmt: str='str',
-        nonscalar_file_type: str='str',
-        metadata_dirname: str='str'
-    ):
-        ...
+        resource: str = "WindowsPath",
+        text_relational_min: str = "int",
+        force_relational: str = "list",
+        dirname_fmt: str = "str",
+        nonscalar_file_type: str = "str",
+        metadata_dirname: str = "str",
+    ): ...
     resource: Incomplete
     text_relational_min: Incomplete
     force_relational: Incomplete
     dirname_fmt: Incomplete
     nonscalar_file_type: Incomplete
     metadata_dirname: Incomplete
 
-    def __call__(self, index, row):
-        ...
-
-    @classmethod
-    def __imports__(cls) -> None:
-        ...
-
-    def save_metadata(self, name, key_func, **extra):
-        ...
-
+    def __call__(self, index, row): ...
+    def save_metadata(self, name, key_func, **extra): ...
+    def open(self) -> None: ...
 
 class MungeToDirectory(MungerBase):
-
     def __init__(
         self,
-        resource: str='WindowsPath',
-        text_relational_min: str='int',
-        force_relational: str='list',
-        dirname_fmt: str='str',
-        nonscalar_file_type: str='str',
-        metadata_dirname: str='str'
-    ):
-        ...
+        resource: str = "WindowsPath",
+        text_relational_min: str = "int",
+        force_relational: str = "list",
+        dirname_fmt: str = "str",
+        nonscalar_file_type: str = "str",
+        metadata_dirname: str = "str",
+    ): ...
     ...
 
-
 class TarFileIO(io.BytesIO):
     tarfile: Incomplete
     overwrite: bool
     name: Incomplete
     mode: Incomplete
 
-    def __init__(self, open_tarfile, relname, mode: str=..., overwrite: bool=...) -> None:
-        ...
-
-    def __del__(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
+    def __init__(
+        self, open_tarfile, relname, mode: str = ..., overwrite: bool = ...
+    ) -> None: ...
+    def __del__(self) -> None: ...
+    def close(self) -> None: ...
 
 class MungeToTar(MungerBase):
-
     def __init__(
         self,
-        resource: str='WindowsPath',
-        text_relational_min: str='int',
-        force_relational: str='list',
-        dirname_fmt: str='str',
-        nonscalar_file_type: str='str',
-        metadata_dirname: str='str'
-    ):
-        ...
+        resource: str = "WindowsPath",
+        text_relational_min: str = "int",
+        force_relational: str = "list",
+        dirname_fmt: str = "str",
+        nonscalar_file_type: str = "str",
+        metadata_dirname: str = "str",
+    ): ...
     tarname: str
     tarfile: Incomplete
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
+    def open(self) -> None: ...
+    def close(self) -> None: ...
 
 class Aggregator(util.Ownable):
     PERSISTENT_TRAIT_ROLES: Incomplete
     name_map: Incomplete
     trait_rules: Incomplete
     metadata: Incomplete
 
-    def __init__(self) -> None:
-        ...
-
-    def enable(self) -> None:
-        ...
-
-    def disable(self) -> None:
-        ...
-
-    def is_persistent_trait(self, device, attr):
-        ...
-
-    def get(self) -> None:
-        ...
-
-    def key(self, device_name, state_name):
-        ...
-
-    def set_device_labels(self, **mapping) -> None:
-        ...
-
-    def observe(self, devices, changes: bool=..., always=..., never=...) -> None:
-        ...
-
+    def __init__(self) -> None: ...
+    def enable(self) -> None: ...
+    def disable(self) -> None: ...
+    def is_persistent_trait(self, device, attr): ...
+    def get(self) -> None: ...
+    def key(self, device_name, state_name): ...
+    def set_device_labels(self, **mapping) -> None: ...
+    def observe(self, devices, changes: bool = ..., always=..., never=...) -> None: ...
 
 class RelationalTableLogger(Owner, util.Ownable):
     index_label: str
     aggregator: Incomplete
     host: Incomplete
     munge: Incomplete
     last_row: int
     pending_output: Incomplete
     pending_input: Incomplete
     path: Incomplete
 
     def __init__(
         self,
-        path: Incomplete | None=...,
+        path: Incomplete | None = ...,
         *,
-        append: bool=...,
-        text_relational_min: int=...,
+        append: bool = ...,
+        text_relational_min: int = ...,
         force_relational=...,
-        dirname_fmt: str=...,
-        nonscalar_file_type: str=...,
-        metadata_dirname: str=...,
-        tar: bool=...,
-        git_commit_in: Incomplete | None=...
-    ) -> None:
-        ...
-
-    def __copy__(self):
-        ...
-
-    def __owner_init__(self, owner) -> None:
-        ...
-
-    def observe(self, devices, changes: bool=..., always=..., never=...) -> None:
-        ...
-
-    def set_row_preprocessor(self, func):
-        ...
-
-    def new_row(self, *args, **kwargs) -> None:
-        ...
-
-    def write(self) -> None:
-        ...
-
-    def context(self, *args, **kws) -> Generator[Incomplete, None, None]:
-        ...
-
-    def clear(self) -> None:
-        ...
-
-    def set_relational_file_format(self, format) -> None:
-        ...
-
-    def set_path_format(self, format) -> None:
-        ...
+        dirname_fmt: str = ...,
+        nonscalar_file_type: str = ...,
+        metadata_dirname: str = ...,
+        tar: bool = ...,
+        git_commit_in: Incomplete | None = ...,
+    ) -> None: ...
+    def __copy__(self): ...
+    def __owner_init__(self, owner) -> None: ...
+    def observe(self, devices, changes: bool = ..., always=..., never=...) -> None: ...
+    def set_row_preprocessor(self, func): ...
+    def new_row(self, *args, **kwargs) -> None: ...
+    def write(self) -> None: ...
+    def context(self, *args, **kws) -> Generator[Incomplete, None, None]: ...
+    def clear(self) -> None: ...
+    def set_relational_file_format(self, format) -> None: ...
+    def set_path_format(self, format) -> None: ...
     output_index: int
 
-    def open(self):
-        ...
-
-    def close(self) -> None:
-        ...
-
+    def open(self): ...
+    def close(self) -> None: ...
 
 class CSVLogger(RelationalTableLogger):
     ROOT_FILE_NAME: str
     OUTPUT_FILE_NAME: str
     INPUT_FILE_NAME: str
     output_index: int
     tables: Incomplete
     nonscalar_file_type: str
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
+    def open(self) -> None: ...
+    def close(self) -> None: ...
 
 class MungeToHDF(Device):
-
-    def __init__(self, resource: str='WindowsPath', key_fmt: str='str'):
-        ...
+    def __init__(self, resource: str = "WindowsPath", key_fmt: str = "str"): ...
     resource: Incomplete
     key_fmt: Incomplete
     backend: Incomplete
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    def __call__(self, index, row):
-        ...
-
-    def save_metadata(self, name, key_func, **extra):
-        ...
-
+    def open(self) -> None: ...
+    def close(self) -> None: ...
+    def __call__(self, index, row): ...
+    def save_metadata(self, name, key_func, **extra): ...
 
 class HDFLogger(RelationalTableLogger):
     KEY_OUTPUT: str
     KEY_INPUT: str
     nonscalar_file_type: str
     munge: Incomplete
 
     def __init__(
         self,
         path,
         *,
-        append: bool=...,
-        key_fmt: str=...,
-        git_commit_in: Incomplete | None=...
-    ) -> None:
-        ...
+        append: bool = ...,
+        key_fmt: str = ...,
+        git_commit_in: Incomplete | None = ...,
+    ) -> None: ...
     df: Incomplete
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
+    def open(self) -> None: ...
+    def close(self) -> None: ...
 
 class SQLiteLogger(RelationalTableLogger):
     index_label: str
     ROOT_FILE_NAME: str
     OUTPUT_TABLE_NAME: str
     inprogress: Incomplete
     committed: Incomplete
     output_index: int
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    def key(self, name, attr):
-        ...
-
-def to_feather(data, path) -> None:
-    ...
+    def open(self) -> None: ...
+    def close(self) -> None: ...
+    def key(self, name, attr): ...
 
+def to_feather(data, path) -> None: ...
 def read_sqlite(
     path,
     table_name=...,
-    columns: Incomplete | None=...,
-    nrows: Incomplete | None=...,
-    index_col=...
-):
-    ...
-
+    columns: Incomplete | None = ...,
+    nrows: Incomplete | None = ...,
+    index_col=...,
+): ...
 def read(
     path_or_buf,
-    columns: Incomplete | None=...,
-    nrows: Incomplete | None=...,
-    format: str=...,
-    **kws
-):
-    ...
+    columns: Incomplete | None = ...,
+    nrows: Incomplete | None = ...,
+    format: str = ...,
+    **kws,
+): ...
 
-
-class MungeTarReader():
+class MungeTarReader:
     tarnames: Incomplete
     tarfile: Incomplete
 
-    def __init__(self, path, tarname: str=...) -> None:
-        ...
-
-    def __call__(self, key, *args, **kws):
-        ...
+    def __init__(self, path, tarname: str = ...) -> None: ...
+    def __call__(self, key, *args, **kws): ...
 
-
-class MungeDirectoryReader():
+class MungeDirectoryReader:
     path: Incomplete
 
-    def __init__(self, path) -> None:
-        ...
-
-    def __call__(self, key, *args, **kws):
-        ...
+    def __init__(self, path) -> None: ...
+    def __call__(self, key, *args, **kws): ...
 
-
-class MungeReader():
-
-    def __new__(cls, path):
-        ...
+class MungeReader:
+    def __new__(cls, path): ...
 
 def read_relational(
     path,
     expand_col,
-    root_cols: Incomplete | None=...,
-    target_cols: Incomplete | None=...,
-    root_nrows: Incomplete | None=...,
-    root_format: str=...,
-    prepend_column_name: bool=...
-):
-    ...
+    root_cols: Incomplete | None = ...,
+    target_cols: Incomplete | None = ...,
+    root_nrows: Incomplete | None = ...,
+    root_format: str = ...,
+    prepend_column_name: bool = ...,
+): ...
```

### Comparing `labbench-0.23.4/labbench/_device.py` & `labbench-0.25.0/labbench/_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 """
 This implementation is deeply intertwined obscure details of the python object
 model. Consider starting with a close read of the documentation and exploring
 the objects in an interpreter instead of reverse-engineering this code.
 """
 
 from functools import wraps
-from copy import deepcopy
 import inspect
 import sys
 import traceback
+from warnings import warn
 
 from . import util
 from . import property as property_
 from . import value
 
 from ._traits import (
     HasTraits,
@@ -45,15 +45,15 @@
     Undefined,
     BoundedNumber,
     observe,
     unobserve,
     hold_trait_notifications,
 )
 
-__all__ = ["Device", "list_devices", "property", "value", "datareturn", "trait_info"]
+__all__ = ["Device", "list_devices", "property", "value", "trait_info"]
 
 
 def trace_methods(cls, name, until_cls=None):
     """Look for a method called `name` in cls and all of its parent classes."""
     methods = []
     last_method = None
 
@@ -75,15 +75,15 @@
     """Look for Device instances, and their names, in the calling
     code context (depth == 1) or its callers (if depth in (2,3,...)).
     Checks locals() in that context first.
     If no Device instances are found there, search the first
     argument of the first function argument, in case this is
     a method in a class.
     """
-    from inspect import getouterframes, currentframe
+    from inspect import currentframe
 
     f = frame = currentframe()
     for i in range(depth):
         f = f.f_back
     try:
         ret = {k: v for k, v in list(f.frame.f_locals.items()) if isinstance(v, Device)}
 
@@ -130,30 +130,30 @@
 
 
 def log_trait_activity(msg):
     """emit debug messages for trait values"""
 
     # print('logger debug!', msg)
 
-    if msg['name'] == 'isopen':
+    if msg["name"] == "isopen":
         return
 
     owner = msg["owner"]
     trait_name = msg["name"]
 
     if msg["type"] == "set":
         label = owner._traits[trait_name].label or " "
         if label:
             label = f" {label} "
         value = repr(msg["new"])
         if len(value) > 180:
             value = f'<data of type {type(msg["new"]).__qualname__}>'
         owner._logger.debug(f'set trait "{trait_name}" → {value}{label}')
     elif msg["type"] == "get":
-        if msg['new'] != msg['old']:
+        if msg["new"] != msg["old"]:
             label = owner._traits[trait_name].label
             if label:
                 label = f" {label} "
 
             value = repr(msg["new"])
             if len(value) > 180:
                 value = f'<data of type {type(msg["new"]).__qualname__}>'
@@ -230,15 +230,19 @@
 
     __children__ = {}
 
     @util.hide_in_traceback
     def __init__(self, resource=Undefined, **values):
         """Update default values with these arguments on instantiation."""
 
-        self.__imports__()        
+        if hasattr(self, "__imports__"):
+            warn(
+                "the use of __imports__ has been deprecated. switch to importing each backend-specific module in each method that uses it."
+            )
+            self.__imports__()
 
         # validate presence of required arguments
         inspect.signature(self.__init__).bind(resource, **values)
 
         if resource is not Undefined:
             values["resource"] = resource
 
@@ -260,15 +264,14 @@
 
     @classmethod
     @util.hide_in_traceback
     def __init_subclass__(cls, **value_defaults):
         super().__init_subclass__()
 
         for trait_name, new_default in value_defaults.items():
-
             trait = getattr(cls, trait_name, None)
 
             if trait is None or trait.role != Trait.ROLE_VALUE:
                 parent_name = cls.__mro__[1].__qualname__
                 raise AttributeError(
                     f"there is no value trait {parent_name}.{trait_name}, cannot update its default"
                 )
@@ -312,31 +315,14 @@
         cls.__init__ = util.copy_func(cls.__init__)
         cls.__init__.__signature__ = inspect.Signature(params)
 
         # generate the __init__ docstring
         value_docs = "".join((f"    {t.doc()}\n" for t in settable_values.values()))
         cls.__init__.__doc__ = f"\nArguments:\n{value_docs}"
 
-        # update the class docstring
-        property_docs = "".join(
-            (f"    {getattr(cls, name).doc()}\n" for name in cls._property_attrs)
-        )
-
-        if cls.__doc__ is None:
-            # use the static doc written for the parent
-            cls.__baredoc__ = cls.__baredoc__
-        else:
-            cls.__baredoc__ = cls.__doc__
-
-        cls.__doc__ = str(cls.__baredoc__)  # <- copy so we can +=
-        cls.__doc__ += "\nValue Attributes:\n" + value_docs
-        cls.__doc__ += "\nProperty Attributes:\n" + property_docs
-
-        # cls.__imports__()
-
     @util.hide_in_traceback
     @wraps(open)
     def __open_wrapper__(self):
         """A wrapper for the connect() method. It steps through the
         method resolution order of self.__class__ and invokes each open()
         method, starting with labbench.Device and working down
         """
@@ -345,19 +331,19 @@
             return
 
         self.backend = None
 
         try:
             for opener in trace_methods(self.__class__, "open", Device)[::-1]:
                 opener(self)
-        except:
+        except BaseException:
             self.backend = DisconnectedBackend(self)
             raise
 
-        self._logger.debug(f"opened")
+        self._logger.debug("opened")
 
         # Force an update to self.isopen
         self.isopen
 
     @util.hide_in_traceback
     @wraps(close)
     def __close_wrapper__(self):
@@ -397,18 +383,14 @@
             if len(all_ex) > 0:
                 ex = util.ConcurrentException(
                     f"multiple exceptions while closing {self}"
                 )
                 ex.thread_exceptions = all_ex
                 raise ex
 
-    @classmethod
-    def __imports__(cls):
-        pass
-
     @util.hide_in_traceback
     def __enter__(self):
         try:
             self.open()
             return self
         except BaseException as e:
             args = list(e.args)
@@ -423,15 +405,15 @@
             self.close()
         except BaseException as e:
             args = list(e.args)
             args[0] = "{}: {}".format(repr(self), str(args[0]))
             e.args = tuple(args)
             raise e
 
-    ### Object boilerplate
+    # Object boilerplate
     def __del__(self):
         try:
             isopen = self.isopen
         except AttributeError:
             # the object failed to instantiate properly
             isopen = False
 
@@ -447,29 +429,30 @@
             return f"{name}()"
 
     @property_.bool()
     def isopen(self):
         """is the backend ready?"""
         try:
             return DisconnectedBackend not in self.backend.__class__.__mro__
-        except:
+        except BaseException:
             # Run into this sometimes on reloading a module or ipython shell:
             # the namespace is gone. we just assume disconnected
             return False
 
 
 Device.__init_subclass__()
 
 
 def trait_info(device: Device, name: str) -> dict:
-    """ returns the keywords used to define the trait attribute named `name` in `device`
-    """
+    """returns the keywords used to define the trait attribute named `name` in `device`"""
 
     trait = device._traits[name]
     info = dict(trait.kws)
 
     if isinstance(trait, BoundedNumber):
         info.update(
-            min=trait._min(device), max=trait._max(device), step=trait.step,
+            min=trait._min(device),
+            max=trait._max(device),
+            step=trait.step,
         )
 
     return info
```

### Comparing `labbench-0.23.4/labbench/_host.py` & `labbench-0.25.0/labbench/_host.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,18 @@
         help="git commit on open() if run inside a git repo with this branch name",
     )
 
     time_format = "%Y-%m-%d %H:%M:%S"
 
     def open(self):
         """The host setup method tries to commit current changes to the tree"""
+        import git
+        import pandas as pd
+        import pip
+
         log_formatter = JSONFormatter()
         stream = LogStreamBuffer()
         sh = logging.StreamHandler(stream)
         sh.setFormatter(log_formatter)
         sh.setLevel(logging.DEBUG)
 
         # Add to the labbench logger handler
@@ -252,40 +256,37 @@
         logger.setLevel(logging.DEBUG)
         logger.addHandler(sh)
 
         # git repository information
         try:
             repo = git.Repo(".", search_parent_directories=True)
             self._logger.debug("running in git repository")
-            if self.git_commit_in is not None and repo.active_branch == self.git_commit_in:
+            if (
+                self.git_commit_in is not None
+                and repo.active_branch == self.git_commit_in
+            ):
                 repo.index.commit("start of measurement")
                 self._logger.debug("git commit finished")
         except git.NoSuchPathError:
             repo = None
-            self._logger.info(f"not running in a git repository")
+            self._logger.info("not running in a git repository")
 
         self.backend = {
             "logger": logger,
             "log_stream": stream,
             "log_handler": sh,
             "log_formatter": log_formatter,
             "repo": repo,
         }
 
         # Preload the git repo parameters
         for name in self._traits:
             if name.startswith("git"):
                 getattr(self, name)
 
-    @classmethod
-    def __imports__(self):
-        global git, pip
-        import git
-        import pip
-
     def close(self):
         try:
             self.backend["logger"].removeHandler(self.backend["log_handler"])
         except (AttributeError, TypeError):
             pass
         try:
             self.backend["log_stream"].close()
@@ -297,14 +298,15 @@
         ret = super().metadata()
         ret["python_modules"] = self.__python_module_versions()
         return ret
 
     def __python_module_versions(self):
         """Enumerate the versions of installed python modules"""
         import pandas as pd
+        import pip
 
         versions = dict(
             [str(d).lower().split(" ") for d in pip.get_installed_distributions()]
         )
         running = dict(
             sorted(
                 [(k, versions[k.lower()]) for k in sys.modules.keys() if k in versions]
@@ -332,14 +334,16 @@
             return self._ret
         else:
             return {}
 
     @property_.str(cache=True)
     def git_commit_id(self):
         """Try to determine the current commit hash of the current git repo"""
+        import git
+
         try:
             commit = self.backend["repo"].commit()
             return commit.hexsha
         except git.NoSuchPathError:
             return ""
 
     @property_.str(cache=True)
```

### Comparing `labbench-0.23.4/labbench/_host.pyi` & `labbench-0.25.0/labbench/_host.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,65 @@
 import logging
 from . import _device as core
 from _typeshed import Incomplete
 
-
-class LogStreamBuffer():
-
-    def __init__(self) -> None:
-        ...
-
-    def write(self, msg):
-        ...
-
-    def read(self):
-        ...
-
-    def flush(self) -> None:
-        ...
-
+class LogStreamBuffer:
+    def __init__(self) -> None: ...
+    def write(self, msg): ...
+    def read(self): ...
+    def flush(self) -> None: ...
 
 class LogStderr(core.Device):
-
-    def __init__(self, resource: str='str'):
-        ...
+    def __init__(self, resource: str = "str"): ...
     log: str
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    def write(self, what) -> None:
-        ...
-
-    def flush(self) -> None:
-        ...
-
+    def open(self) -> None: ...
+    def close(self) -> None: ...
+    def write(self, what) -> None: ...
+    def flush(self) -> None: ...
 
 class Email(core.Device):
-
     def __init__(
         self,
-        resource: str='str',
-        port: str='int',
-        sender: str='str',
-        recipients: str='list',
-        success_message: str='str',
-        failure_message: str='str'
-    ):
-        ...
+        resource: str = "str",
+        port: str = "int",
+        sender: str = "str",
+        recipients: str = "list",
+        success_message: str = "str",
+        failure_message: str = "str",
+    ): ...
     resource: Incomplete
     port: Incomplete
     sender: Incomplete
     recipients: Incomplete
     success_message: Incomplete
     failure_message: Incomplete
     backend: Incomplete
 
-    def open(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    def send_summary(self):
-        ...
-
+    def open(self) -> None: ...
+    def close(self) -> None: ...
+    def send_summary(self): ...
 
 class JSONFormatter(logging.Formatter):
     t0: Incomplete
 
-    def __init__(self, *args, **kws) -> None:
-        ...
-
+    def __init__(self, *args, **kws) -> None: ...
     @staticmethod
-    def json_serialize_dates(obj):
-        ...
-
-    def format(self, rec):
-        ...
-
+    def json_serialize_dates(obj): ...
+    def format(self, rec): ...
 
 class Host(core.Device):
-
-    def __init__(self, resource: str='str', git_commit_in: str='NoneType'):
-        ...
+    def __init__(self, resource: str = "str", git_commit_in: str = "NoneType"): ...
     git_commit_in: Incomplete
     time_format: str
     backend: Incomplete
 
-    def open(self) -> None:
-        ...
-
-    @classmethod
-    def __imports__(self) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    def metadata(self):
-        ...
-
-    def time(self):
-        ...
-
-    def log(self):
-        ...
-
-    def git_commit_id(self):
-        ...
-
-    def git_remote_url(self):
-        ...
-
-    def hostname(self):
-        ...
-
-    def git_browse_url(self):
-        ...
-
-    def git_pending_changes(self):
-        ...
+    def open(self) -> None: ...
+    def close(self) -> None: ...
+    def metadata(self): ...
+    def time(self): ...
+    def log(self): ...
+    def git_commit_id(self): ...
+    def git_remote_url(self): ...
+    def hostname(self): ...
+    def git_browse_url(self): ...
+    def git_pending_changes(self): ...
```

### Comparing `labbench-0.23.4/labbench/_rack.py` & `labbench-0.25.0/labbench/_rack.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,25 +90,25 @@
             except KeyError:
                 pass
 
     @classmethod
     def return_event(cls, owner, returned: dict):
         if owner in cls._owner_hold_list:
             return
-            
+
         if not isinstance(returned, dict):
             raise TypeError(f"returned data was {repr(returned)}, which is not a dict")
         for handler in cls._handlers["returns"]:
             handler(dict(name=owner._owned_name, owner=owner, old=None, new=returned))
 
     @classmethod
     def call_event(cls, owner, parameters: dict):
         if owner in cls._owner_hold_list:
             return
-            
+
         if not isinstance(parameters, dict):
             raise TypeError(
                 f"parameters data was {repr(parameters)}, which is not a dict"
             )
         for handler in cls._handlers["calls"]:
             handler(dict(name=owner._owned_name, owner=owner, old=None, new=parameters))
 
@@ -195,59 +195,59 @@
             name: p
             for name, p in template_sig.parameters.items()
             if name not in skip_names and p.kind in (p.KEYWORD_ONLY,)
         }
 
 
 class MethodTaggerDataclass:
-    """ subclasses decorated with @dataclass will operate as decorators that stash annotated keywords here into the pending attribute dict """
+    """subclasses decorated with @dataclass will operate as decorators that stash annotated keywords here into the pending attribute dict"""
 
     pending = {}
 
     def __call__(self, func):
         self.pending.setdefault(func, {}).update(
             {n: getattr(self, n) for n in self.__annotations__}
         )
 
         return func
 
 
 @dataclass
 class rack_input_table(MethodTaggerDataclass):
     """tag a method defined in a Rack to support execution from a flat table.
-    
-    In practice, this often means a very long argument list. 
-    
+
+    In practice, this often means a very long argument list.
+
     Arguments:
         table_path: location of the input table
     """
 
     table_path: str
 
 
 @dataclass
 class rack_kwargs_template(MethodTaggerDataclass):
     """tag a method defined in a Rack to replace a **kwargs argument using the signature of the specified callable.
-    
-    In practice, this often means a very long argument list. 
-    
+
+    In practice, this often means a very long argument list.
+
     Arguments:
         callable_template: replace variable keyword arguments (**kwargs) with the keyword arguments defined in this callable
 
         skip: list of column names to omit
     """
 
     template: callable = None
 
 
 class rack_kwargs_skip(MethodTaggerDataclass):
     """tag a method defined in a Rack to replace a **kwargs argument using the signature of the specified callable.
-    
-    In practice, this often means a very long argument list. 
-    
+
+    In practice, this often means a very long argument list.
+
     Arguments:
         callable_template: replace variable keyword arguments (**kwargs) with the keyword arguments defined in this callable
 
         skip: list of column names to omit
     """
 
     skip: list = None
@@ -296,14 +296,15 @@
     def iterate_from_csv(self, path):
         """call the BoundSequence for each row in a csv table.
         keyword argument names are taken from the column header
         (0th row). keyword values are taken from corresponding column in
         each row.
         """
         import pandas as pd
+
         table = pd.read_csv(path, index_col=0)
         for i, row in enumerate(table.index):
             util.logger.info(
                 f"{self._owned_name} from '{str(path)}' "
                 f"- '{row}' ({i+1}/{len(table.index)})"
             )
             notify.call_iteration_event(self, i, row, len(table.index))
@@ -325,15 +326,15 @@
     def __owner_subclass__(self, owner_cls):
         # allow the owner class a chance to set up self.
         super().__owner_subclass__(owner_cls)
         self._apply_signature()
 
     def _apply_signature(self):
         """updates self.__signature__
-        
+
         __owner_subclass__ must have been called first to do introspection on self._callable_template.
         """
         self.__call__ = util.copy_func(self.__call__)
 
         # note the devices needed to execute this function
         if isinstance(self._owner, Rack):
             annotations = getattr(self._owner, "__annotations__", {})
@@ -438,15 +439,15 @@
         return sig.replace(
             parameters=[
                 param.replace(name=k) for k, param in zip(ext_names, param_list)
             ]
         )
 
     def extended_arguments(self, name_map={}):
-        """ returns a list of argument names from in the owned context.
+        """returns a list of argument names from in the owned context.
 
         Arguments:
             name_map (dict): name remapping, overriding self.tags
         """
         # TODO: should these all have 'owner' as a name, to specify the context?
         sig = self.__call__.__signature__
         if hasattr(self._owner, "__name__"):
@@ -580,14 +581,15 @@
     def iterate_from_csv(self, path):
         """call the BoundSequence for each row in a csv table.
         keyword argument names are taken from the column header
         (0th row). keyword values are taken from corresponding column in
         each row.
         """
         import pandas as pd
+
         table = pd.read_csv(path, index_col=0)
         for i, row in enumerate(table.index):
             util.logger.info(
                 f"{self._owned_name} from '{str(path)}' "
                 f"- '{row}' ({i+1}/{len(table.index)})"
             )
             notify.call_iteration_event(self, i, row, len(table.index))
@@ -631,34 +633,37 @@
     each will be called
 
     """
 
     def __init__(self, owner):
         self._owner = owner
         self._owned_name = getattr(owner, "_owned_name", repr(owner))
-
-        display_name = getattr(self, "_owned_name", type(self).__name__)
+        # display_name = getattr(self, "_owned_name", type(self).__name__)
 
     def __enter__(self):
         try:
-            hold = [o for o in self._owner._ownables.values() if isinstance(o, RackMethod)]
+            hold = [
+                o for o in self._owner._ownables.values() if isinstance(o, RackMethod)
+            ]
             notify.hold_owner_notifications(*hold)
             cls = type(self._owner)
             for opener in core.trace_methods(cls, "open", Owner)[::-1]:
                 opener(self._owner)
 
             # self._owner.open()
             getattr(self._owner, "_logger", util.logger).debug("opened")
 
         finally:
             notify.allow_owner_notifications(*hold)
 
     def __exit__(self, *exc_info):
         try:
-            holds = [o for o in self._owner._ownables.values() if isinstance(o, RackMethod)]
+            holds = [
+                o for o in self._owner._ownables.values() if isinstance(o, RackMethod)
+            ]
             notify.hold_owner_notifications(*holds)
             cls = type(self._owner)
             methods = core.trace_methods(cls, "close", Owner)
 
             all_ex = []
             for closer in methods:
                 try:
@@ -674,18 +679,20 @@
                     depth = len(tuple(traceback.walk_tb(ex[2])))
                     traceback.print_exception(*ex, limit=-(depth - 1))
                     # sys.stderr.write("(Exception suppressed to continue close)\n\n")
 
             getattr(self._owner, "_logger", util.logger).debug("closed")
 
         finally:
-            notify.allow_owner_notifications(*holds)            
+            notify.allow_owner_notifications(*holds)
 
             if len(all_ex) > 0:
-                ex = util.ConcurrentException(f"multiple exceptions while closing {self}")
+                ex = util.ConcurrentException(
+                    f"multiple exceptions while closing {self}"
+                )
                 ex.thread_exceptions = all_ex
                 raise ex
 
     def __repr__(self):
         return repr(self._owner)
 
     def __str__(self):
@@ -1078,28 +1085,31 @@
 
     return sequence
 
 
 class Sequence(util.Ownable):
     """An experimental procedure defined with methods in Rack instances. The input is a specification for sequencing these
     steps, including support for threading.
-    
+
     Sequence are meant to be defined as attributes of Rack subclasses in instances of the Rack subclasses.
     """
 
     access_spec = None
     cleanup_func = None
     exception_allowlist = NeverRaisedException
 
     def __init__(self, *specification, shared_names=[], input_table=None):
         self.spec = [standardize_spec_step(spec) for spec in specification]
-        self.tags = dict(table_path=input_table, shared_names=shared_names,)
+        self.tags = dict(
+            table_path=input_table,
+            shared_names=shared_names,
+        )
 
     def return_on_exceptions(self, exception_or_exceptions, cleanup_func=None):
-        """ Configures calls to the bound Sequence to swallow the specified exceptions raised by
+        """Configures calls to the bound Sequence to swallow the specified exceptions raised by
         constitent steps. If an exception is swallowed, subsequent steps
         Sequence are not executed. The dictionary of return values from each Step is returned with
         an additional 'exception' key indicating the type of the exception that occurred.
         """
         self.exception_allowlist = exception_or_exceptions
         self.cleanup_func = cleanup_func
 
@@ -1519,15 +1529,15 @@
     # subclass into a new Rack
     return type(cls_name, (base_cls,), dict(base_cls.__dict__, **namespace))
 
 
 def find_owned_rack_by_type(
     parent_rack: Rack, target_type: Rack, include_parent: bool = True
 ):
-    """ return a rack instance of `target_type` owned by `parent_rack`. if there is
+    """return a rack instance of `target_type` owned by `parent_rack`. if there is
     not exactly 1 for `target_type`, TypeError is raised.
     """
     # TODO: add this to labbench
     if include_parent and isinstance(parent_rack, target_type):
         target_rack = parent_rack
     else:
         type_matches = {
```

### Comparing `labbench-0.23.4/labbench/_rack.pyi` & `labbench-0.25.0/labbench/_rack.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,306 +1,172 @@
 import inspect
 from . import util as util
 from _typeshed import Incomplete
 from collections.abc import Generator
-EMPTY: Incomplete
-
-def null_context(owner) -> Generator[Incomplete, None, None]:
-    ...
-
 
-class NeverRaisedException(BaseException):
-    ...
+EMPTY: Incomplete
 
+def null_context(owner) -> Generator[Incomplete, None, None]: ...
 
-class notify():
+class NeverRaisedException(BaseException): ...
 
+class notify:
     @classmethod
-    def clear(cls) -> None:
-        ...
-
+    def clear(cls) -> None: ...
     @classmethod
-    def hold_owner_notifications(cls, *owners) -> None:
-        ...
-
+    def hold_owner_notifications(cls, *owners) -> None: ...
     @classmethod
-    def allow_owner_notifications(cls, *owners) -> None:
-        ...
-
+    def allow_owner_notifications(cls, *owners) -> None: ...
     @classmethod
-    def return_event(cls, owner, returned: dict):
-        ...
-
+    def return_event(cls, owner, returned: dict): ...
     @classmethod
-    def call_event(cls, owner, parameters: dict):
-        ...
-
+    def call_event(cls, owner, parameters: dict): ...
     @classmethod
-    def call_iteration_event(cls, owner, index: int, step_name: str=..., total_count: int=...):
-        ...
-
+    def call_iteration_event(
+        cls, owner, index: int, step_name: str = ..., total_count: int = ...
+    ): ...
     @classmethod
-    def observe_returns(cls, handler) -> None:
-        ...
-
+    def observe_returns(cls, handler) -> None: ...
     @classmethod
-    def observe_calls(cls, handler) -> None:
-        ...
-
+    def observe_calls(cls, handler) -> None: ...
     @classmethod
-    def observe_call_iteration(cls, handler) -> None:
-        ...
-
+    def observe_call_iteration(cls, handler) -> None: ...
     @classmethod
-    def unobserve_returns(cls, handler) -> None:
-        ...
-
+    def unobserve_returns(cls, handler) -> None: ...
     @classmethod
-    def unobserve_calls(cls, handler) -> None:
-        ...
-
+    def unobserve_calls(cls, handler) -> None: ...
     @classmethod
-    def unobserve_call_iteration(cls, handler) -> None:
-        ...
+    def unobserve_call_iteration(cls, handler) -> None: ...
 
-
-class CallSignatureTemplate():
+class CallSignatureTemplate:
     target: Incomplete
 
-    def __init__(self, target) -> None:
-        ...
-
-    def get_target(self, owner):
-        ...
-
-    def get_keyword_parameters(self, owner, skip_names):
-        ...
-
+    def __init__(self, target) -> None: ...
+    def get_target(self, owner): ...
+    def get_keyword_parameters(self, owner, skip_names): ...
 
-class MethodTaggerDataclass():
+class MethodTaggerDataclass:
     pending: Incomplete
 
-    def __call__(self, func):
-        ...
-
+    def __call__(self, func): ...
 
 class rack_input_table(MethodTaggerDataclass):
     table_path: str
 
-    def __init__(self, table_path) -> None:
-        ...
-
+    def __init__(self, table_path) -> None: ...
 
 class rack_kwargs_template(MethodTaggerDataclass):
     template: callable
 
-    def __init__(self, template) -> None:
-        ...
-
+    def __init__(self, template) -> None: ...
 
 class rack_kwargs_skip(MethodTaggerDataclass):
     skip: list
 
-    def __init__(self, *arg_names) -> None:
-        ...
-
+    def __init__(self, *arg_names) -> None: ...
 
 class RackMethod(util.Ownable):
     tags: Incomplete
     __doc__: Incomplete
     __name__: Incomplete
     __qualname__: Incomplete
 
-    def __init__(self, owner, name: str, kwdefaults: dict=...) -> None:
-        ...
-
-    def iterate_from_csv(self, path) -> Generator[Incomplete, None, None]:
-        ...
+    def __init__(self, owner, name: str, kwdefaults: dict = ...) -> None: ...
+    def iterate_from_csv(self, path) -> Generator[Incomplete, None, None]: ...
     debug: Incomplete
 
     @classmethod
-    def from_method(self, method):
-        ...
-
-    def __copy__(self):
-        ...
-
-    def __deepcopy__(self, memo: Incomplete | None=...):
-        ...
-
-    def __owner_subclass__(self, owner_cls) -> None:
-        ...
-
-    def set_kwdefault(self, name, new_default) -> None:
-        ...
-
-    def extended_signature(self, name_map=...):
-        ...
-
-    def extended_arguments(self, name_map=...):
-        ...
-
-    def call_by_extended_argnames(self, *args, **kws):
-        ...
-
-    def __call__(self, *args, **kws):
-        ...
-
+    def from_method(self, method): ...
+    def __copy__(self): ...
+    def __deepcopy__(self, memo: Incomplete | None = ...): ...
+    def __owner_subclass__(self, owner_cls) -> None: ...
+    def set_kwdefault(self, name, new_default) -> None: ...
+    def extended_signature(self, name_map=...): ...
+    def extended_arguments(self, name_map=...): ...
+    def call_by_extended_argnames(self, *args, **kws): ...
+    def __call__(self, *args, **kws): ...
 
 class BoundSequence(util.Ownable):
     cleanup_func: Incomplete
-    exception_allowlist: Incomplete
-
-    def __call__(self, **kwargs):
-        ...
+    exception_allowlist = NeverRaisedException
 
+    def __call__(self, **kwargs): ...
     @classmethod
-    def to_template(cls, path) -> None:
-        ...
-
-    def iterate_from_csv(self, path) -> Generator[Incomplete, None, None]:
-        ...
-
-
-class OwnerContextAdapter():
-
-    def __init__(self, owner) -> None:
-        ...
-
-    def __enter__(self) -> None:
-        ...
-
-    def __exit__(self, *exc_info) -> None:
-        ...
-
-def recursive_devices(top):
-    ...
-
-def flatten_nested_owner_contexts(top) -> dict:
-    ...
-
-def package_owned_contexts(top):
-    ...
-
-def owner_getattr_chains(owner):
-    ...
-
-
-class Owner():
-
-    def __init_subclass__(cls, entry_order: list=...):
-        ...
-
-    def __init__(self, **update_ownables) -> None:
-        ...
-
-    def __setattr__(self, key, obj) -> None:
-        ...
-
-    def close(self) -> None:
-        ...
-
-    def open(self) -> None:
-        ...
+    def to_template(cls, path) -> None: ...
+    def iterate_from_csv(self, path) -> Generator[Incomplete, None, None]: ...
 
+class OwnerContextAdapter:
+    def __init__(self, owner) -> None: ...
+    def __enter__(self) -> None: ...
+    def __exit__(self, *exc_info) -> None: ...
+
+def recursive_devices(top): ...
+def flatten_nested_owner_contexts(top) -> dict: ...
+def package_owned_contexts(top): ...
+def owner_getattr_chains(owner): ...
+
+class Owner:
+    def __init_subclass__(cls, entry_order: list = ...): ...
+    def __init__(self, **update_ownables) -> None: ...
+    def __setattr__(self, key, obj) -> None: ...
+    def close(self) -> None: ...
+    def open(self) -> None: ...
     @property
-    def __enter__(self):
-        ...
-
+    def __enter__(self): ...
     @property
-    def __exit__(self):
-        ...
-
-def override_empty(a, b, param_name, field):
-    ...
-
-def update_parameter_dict(dest: dict, signature: inspect.Signature):
-    ...
-
-def attr_chain_to_method(root_obj, chain):
-    ...
-
-def standardize_spec_step(sequence):
-    ...
+    def __exit__(self): ...
 
+def override_empty(a, b, param_name, field): ...
+def update_parameter_dict(dest: dict, signature: inspect.Signature): ...
+def attr_chain_to_method(root_obj, chain): ...
+def standardize_spec_step(sequence): ...
 
 class Sequence(util.Ownable):
     access_spec: Incomplete
     cleanup_func: Incomplete
-    exception_allowlist: Incomplete
+    exception_allowlist = NeverRaisedException
     spec: Incomplete
     tags: Incomplete
 
-    def __init__(self, *specification, shared_names=..., input_table: Incomplete | None=...) -> None:
-        ...
-
-    def return_on_exceptions(self, exception_or_exceptions, cleanup_func: Incomplete | None=...) -> None:
-        ...
-
-    def __owner_subclass__(self, owner_cls):
-        ...
+    def __init__(
+        self, *specification, shared_names=..., input_table: Incomplete | None = ...
+    ) -> None: ...
+    def return_on_exceptions(
+        self, exception_or_exceptions, cleanup_func: Incomplete | None = ...
+    ) -> None: ...
+    def __owner_subclass__(self, owner_cls): ...
     last_spec: Incomplete
 
-    def __owner_init__(self, owner) -> None:
-        ...
-
+    def __owner_init__(self, owner) -> None: ...
 
 class RackMeta(type):
-
-    def __enter__(cls) -> None:
-        ...
-
-    def __exit__(cls, *exc_info) -> None:
-        ...
-
+    def __enter__(cls) -> None: ...
+    def __exit__(cls, *exc_info) -> None: ...
 
 class Rack(Owner, util.Ownable, metaclass=RackMeta):
+    def __init__(): ...
+    def __init_subclass__(cls, entry_order=...) -> None: ...
+    def __deepcopy__(self, memo: Incomplete | None = ...): ...
+    def __owner_init__(self, owner) -> None: ...
+    def __getattribute__(self, item): ...
+    def __getitem__(self, item): ...
+    def __len__(self) -> int: ...
+    def __iter__(self): ...
 
-    def __init__():
-        ...
-
-    def __init_subclass__(cls, entry_order=...) -> None:
-        ...
-
-    def __deepcopy__(self, memo: Incomplete | None=...):
-        ...
-
-    def __owner_init__(self, owner) -> None:
-        ...
-
-    def __getattribute__(self, item):
-        ...
-
-    def __getitem__(self, item):
-        ...
-
-    def __len__(self) -> int:
-        ...
-
-    def __iter__(self):
-        ...
-
-
-class _use_module_path():
+class _use_module_path:
     path: Incomplete
 
-    def __init__(self, path) -> None:
-        ...
-
-    def __enter__(self) -> None:
-        ...
-
-    def __exit__(self, exc_type, exc_value, traceback) -> None:
-        ...
+    def __init__(self, path) -> None: ...
+    def __enter__(self) -> None: ...
+    def __exit__(self, exc_type, exc_value, traceback) -> None: ...
 
 def import_as_rack(
     import_string: str,
     *,
-    cls_name: str=...,
-    append_path: list=...,
-    base_cls: type=...,
-    replace_attrs: list=...
-):
-    ...
-
-def find_owned_rack_by_type(parent_rack: Rack, target_type: Rack, include_parent: bool=...):
-    ...
+    cls_name: str = ...,
+    append_path: list = ...,
+    base_cls: type = ...,
+    replace_attrs: list = ...,
+): ...
+def find_owned_rack_by_type(
+    parent_rack: Rack, target_type: Rack, include_parent: bool = ...
+): ...
```

### Comparing `labbench-0.23.4/labbench/_serialize.py` & `labbench-0.25.0/labbench/_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 """functions and CLI tools for mapping labbench objects onto config directories"""
 
-import importlib
 import inspect
 import os
-from pathlib import Path
 from numbers import Number
+from pathlib import Path
 
-from ._rack import (
-    Rack,
-    RackMethod,
-    Sequence,
-    BoundSequence,
-    import_as_rack,
-    update_parameter_dict,
-)
 from . import util
+from ._rack import Rack, import_as_rack, update_parameter_dict
 
 # some packages install ruamel_yaml, others ruamel.yaml. fall back to ruamel_yaml in case ruamel.yaml fails
 # using ruamel yaml instead of pyyaml because it allows us to place comments for human readability
 try:
     import ruamel.yaml as ruamel_yaml
     from ruamel.yaml.comments import CommentedMap
 except ModuleNotFoundError:
@@ -112,17 +104,17 @@
 
 def _adjust_sequence_defaults(rack_cls: type, defaults_in: dict, **override_defaults):
     """adjusts the method argument parameters in the Rack subclass `cls` according to config file"""
     params, methods = _search_method_parameters(rack_cls)
 
     defaults_in = dict(defaults_in, **override_defaults)
 
-    sequences = [
-        obj for obj in rack_cls._ownables.values() if isinstance(obj, Sequence)
-    ]
+    # sequences = [
+    #     obj for obj in rack_cls._ownables.values() if isinstance(obj, Sequence)
+    # ]
 
     for name, default in dict(defaults_in).items():
         if default == params[name].default:
             del defaults_in[name]
             continue
 
         annot = params[name].annotation
@@ -148,15 +140,14 @@
             method.set_kwdefault(short_name, default)
 
     if len(defaults_in) > 0:
         util.logger.debug(f"applied defaults {defaults_in}")
 
 
 def write_table_stub(rack: Rack, name: str, path: Path, with_defaults: bool = False):
-
     """forms an empty DataFrame containing the headers needed for Sequence
     csv files.
 
     Arguments:
         rack: the Rack instance containing the sequence
         path: base directory where the csv should be saved
         with_defaults: whether to include columns when method parameters have defaults
@@ -221,15 +212,16 @@
 
 def _map_devices(cls):
     cm = CommentedMap()
 
     for dev_name, dev in cls._devices.items():
         cm[dev_name] = CommentedMap()
         cm.yaml_set_comment_before_after_key(
-            dev_name, before="\n",
+            dev_name,
+            before="\n",
         )
 
         for value_name in dev._value_attrs:
             if not dev._traits[value_name].sets:
                 # only show settable traits
                 continue
 
@@ -261,15 +253,15 @@
     sourcepath: Path,
     pythonpath: Path = None,
     exist_ok: bool = False,
     with_defaults: bool = False,
     skip_tables: bool = False,
 ):
     if not isinstance(rack, Rack):
-        raise TypeError(f"'rack' argument must be an instance of labbench.Rack")
+        raise TypeError("'rack' argument must be an instance of labbench.Rack")
 
     cls = type(rack)
 
     output_path = Path(output_path)
     output_path.mkdir(exist_ok=exist_ok, parents=True)
 
     with open(output_path / RACK_CONFIG_FILENAME, "w") as stream:
@@ -282,15 +274,16 @@
                 ),
                 _FIELD_KEYWORD_DEFAULTS: _map_method_defaults(rack),
                 _FIELD_DEVICES: _map_devices(cls),
             }
         )
 
         cm.yaml_set_comment_before_after_key(
-            _FIELD_SOURCE, before="orient the python interpreter to the source",
+            _FIELD_SOURCE,
+            before="orient the python interpreter to the source",
         )
 
         cm.yaml_set_comment_before_after_key(
             _FIELD_KEYWORD_DEFAULTS,
             before="\nparameter defaults for sequences in rack:"
             "\nthese parameters can be omitted from sequence table columns",
         )
@@ -326,15 +319,15 @@
         config = _yaml.load(f)
         util.logger.debug(f'loaded configuration from "{str(config_path)}"')
     return config
 
 
 def load_rack(output_path: str, defaults: dict = {}, apply: bool = True) -> Rack:
     """instantiates a Rack object from a config directory created by dump_rack.
-    
+
     After instantiation, the current working directory is changed to output_path.
     """
 
     config_path = Path(output_path) / RACK_CONFIG_FILENAME
     config = read_yaml_config(config_path)
 
     if "import_string" not in config[_FIELD_SOURCE]:
```

### Comparing `labbench-0.23.4/labbench/_serialize.pyi` & `labbench-0.25.0/labbench/_serialize.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 from . import util as util
 from ._rack import (
-    BoundSequence as BoundSequence,
     Rack as Rack,
-    RackMethod as RackMethod,
-    Sequence as Sequence,
     import_as_rack as import_as_rack,
     update_parameter_dict as update_parameter_dict,
 )
 from _typeshed import Incomplete
 from pathlib import Path
+
 RACK_CONFIG_FILENAME: str
 EMPTY: Incomplete
 INDEX_COLUMN_NAME: str
 
-def write_table_stub(rack: Rack, name: str, path: Path, with_defaults: bool=...):
-    ...
-
+def write_table_stub(rack: Rack, name: str, path: Path, with_defaults: bool = ...): ...
 def dump_rack(
     rack: Rack,
     output_path: Path,
     sourcepath: Path,
-    pythonpath: Path=...,
-    exist_ok: bool=...,
-    with_defaults: bool=...,
-    skip_tables: bool=...
-):
-    ...
-
-def read_yaml_config(config_path: str):
-    ...
-
-def load_rack(output_path: str, defaults: dict=..., apply: bool=...) -> Rack:
-    ...
+    pythonpath: Path = ...,
+    exist_ok: bool = ...,
+    with_defaults: bool = ...,
+    skip_tables: bool = ...,
+): ...
+def read_yaml_config(config_path: str): ...
+def load_rack(output_path: str, defaults: dict = ..., apply: bool = ...) -> Rack: ...
```

### Comparing `labbench-0.23.4/labbench/_traits.py` & `labbench-0.25.0/labbench/_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from functools import wraps
 import validators as _val
 from contextlib import contextmanager
 
 from inspect import isclass
 import inspect
 import numbers
-import re
 
 # for common types
 from pathlib import Path
 
 Undefined = inspect.Parameter.empty
 
 T = typing.TypeVar("T")
@@ -150,15 +149,15 @@
                     raise ValueError(f"duplicate 'default' argument in {self}")
                 kws["default"] = args[0]
             elif len(args) == 1 and self.role == self.ROLE_DATARETURN:
                 if "func" in kws:
                     raise ValueError("duplicate 'func' argument")
                 kws["func"] = args[0]
             else:
-                raise ValueError(f"no positional arguments supported")
+                raise ValueError("no positional arguments supported")
 
         self.kws = dict(kws)
         self.metadata = {}
         self._decorated_funcs = []
 
         cls_defaults = {k: getattr(self, k) for k in self.__annotations__.keys()}
 
@@ -205,15 +204,15 @@
                 self.remap_inbound = {v: k for k, v in kws["remap"].items()}
             else:
                 self.remap_inbound = {}
         except KeyError:
             raise
 
         if len(kws["remap"]) != len(self.remap_inbound):
-            raise ValueError(f"'remap' has duplicate values")
+            raise ValueError("'remap' has duplicate values")
 
         # set value traits
         for k, v in kws.items():
             setattr(self, k, v)
 
     @classmethod
     def __init_subclass__(cls, type=Undefined):
@@ -244,30 +243,30 @@
         # if 'default' in cls._arg_defaults:
         #     cls._arg_defaults['default'] = Undefined
 
         # TODO: remove this
         # util.wrap_attribute(cls, '__init__', __init__, tuple(annots.keys()), cls._arg_defaults, 1, annots)
 
         # Help to reduce memory use by __slots__ definition (instead of __dict__)
-        cls.__slots__ = [n for n in dir(cls) if not n.startswith("_")] + [
+        cls.__slots__ = [n for n in dir(cls) if not callable(getattr(cls, n))] + [
             "metadata",
             "kind",
             "name",
         ]
 
     def copy(self, new_type=None, **update_kws):
         if new_type is None:
             new_type = type(self)
         obj = new_type(**dict(self.kws, **update_kws))
         obj._getter = self._getter
         obj._setter = self._setter
         obj._returner = self._returner
         return obj
 
-    ### Descriptor methods (called automatically by the owning class or instance)
+    # Descriptor methods (called automatically by the owning class or instance)
     def __set_name__(self, owner_cls, name):
         """Immediately after an owner class is instantiated, it calls this
         method for each of its attributes that implements this method.
 
         Trait takes advantage of this to remember the owning class for debug
         messages and to register with the owner class.
         """
@@ -293,15 +292,15 @@
         """
 
         if self.role == self.ROLE_VALUE and len(self._decorated_funcs) > 0:
             raise AttributeError(
                 f"tried to combine a default value and a decorator implementation in {self}"
             )
         elif self.role == self.ROLE_DATARETURN and len(self._decorated_funcs) == 0:
-            raise AttributeError(f"decorate a method to tag its return data")
+            raise AttributeError("decorate a method to tag its return data")
         elif len(self._decorated_funcs) == 0:
             return
 
         positional_argcounts = [
             f.__code__.co_argcount - len(f.__defaults__ or tuple())
             for f in self._decorated_funcs
         ]
@@ -385,15 +384,15 @@
                 objname = owner.__class__.__qualname__ + "." + self.name
                 raise AttributeError(
                     f"cannot set {objname}: no @{self.__repr__(owner_inst=owner)}."
                     f"setter and no key argument"
                 )
 
         else:
-            raise AttributeError(f"data return traits cannot be set")
+            raise AttributeError("data return traits cannot be set")
 
         owner.__notify__(self.name, value, "set", cache=self.cache)
 
     @util.hide_in_traceback
     def __get__(self, owner, owner_cls=None):
         """Called by the class instance that owns this attribute to
         retreive its value. This, in turn, decides whether to call a wrapped
@@ -440,15 +439,15 @@
             value = self._getter(owner)
 
         else:
             # otherwise, get with owner.get_key, if available
             if self.key is None:
                 # otherwise, 'get'
                 objname = owner.__class__.__qualname__
-                ownername = self.__repr__(owner_inst=owner)
+                # ownername = self.__repr__(owner_inst=owner)
                 raise AttributeError(
                     f"to set the property {self.name}, decorate a method in {objname} or use the function key argument"
                 )
             value = owner.get_key(self.key, self.name)
 
         # apply remapping as appropriate for the trait
         if len(self.remap_inbound) > 0:
@@ -533,15 +532,15 @@
                 f"{repr(self)} type must be '{typename}', not '{valuetypename}'"
             )
         return value
 
     def contains(self, iterable, value):
         return value in iterable
 
-    ### Decorator methods
+    # Decorator methods
     @util.hide_in_traceback
     def __call__(self, func):
         """use the Trait as a decorator, which ties this Trait instance to evaluate a property or method in the
         owning class. you can specify
         """
         # only decorate functions.
         if not callable(func):
@@ -557,24 +556,35 @@
             self.name = func.__name__
         if len(HasTraitsMeta.__cls_namespace__) > 0:
             HasTraitsMeta.__cls_namespace__[-1][func.__name__] = self
 
         # return self to ensure `self` is the value assigned in the class definition
         return self
 
+    # introspection
     ### introspection
     ###
-    def doc(self):
-        params = self.doc_params(omit=["help", "default"])
+    def doc(self, as_argument=False):
         typename = "Any" if self.type is None else self.type.__qualname__
 
-        doc = f"{self.name} ({typename}): {self.help}"
-        if len(params) > 0:
-            doc += f" ({params})"
+        if self.label:
+            typename += f" ({self.label})"
 
+        params = self.doc_params(omit=["help", "default", "label"])
+        if as_argument:
+            doc = f"{self.name} ({typename}): {self.help}"
+            if len(params) > 0:
+                doc += f" where ({params})"
+
+        else:
+            # as property
+            doc = f"{typename}: {self.help}"
+
+            if len(params) > 0:
+                doc += f"\n\nConstraints:\n    {params}"
         return doc
 
     def doc_params(self, omit=["help"]):
         pairs = []
 
         for name in self.__annotations__.keys():
             default = getattr(type(self), name)
@@ -606,15 +616,15 @@
     def _owned_name(self, owner):
         if owner._owned_name is None:
             return type(owner).__qualname__ + "." + self.name
         else:
             return owner._owned_name + "." + self.name
 
     def update(self, obj=None, **attrs):
-        """ returns `self` or (if `obj` is None) or `other`, after updating its keyword
+        """returns `self` or (if `obj` is None) or `other`, after updating its keyword
         parameters with `attrs`
         """
         if obj is None:
             obj = self
         invalid_params = set(attrs).difference(obj.__dict__)
         if len(invalid_params) > 0:
             raise AttributeError(
@@ -627,17 +637,16 @@
 
 Trait.__init_subclass__()
 
 
 @contextmanager
 def hold_trait_notifications(owner):
     def skip_notify(name, value, type, cache):
-        old = owner.__cache__.setdefault(name, Undefined)
-
-        msg = dict(new=value, old=old, owner=owner, name=name, type=type, cache=cache)
+        # old = owner.__cache__.setdefault(name, Undefined)
+        # msg = dict(new=value, old=old, owner=owner, name=name, type=type, cache=cache)
 
         owner.__cache__[name] = value
 
     original, owner.__notify__ = owner.__notify__, skip_notify
     yield
     owner.__notify__ = original
 
@@ -662,15 +671,15 @@
 
     @util.hide_in_traceback
     def __init_subclass__(cls):
         cls._traits = dict(getattr(cls, "_traits", {}))
         cls._property_attrs = []
         cls._value_attrs = []
         cls._datareturn_attrs = []
-        parent_traits = getattr(cls.__mro__[1], "_traits", {})
+        # parent_traits = getattr(cls.__mro__[1], "_traits", {})
 
         # annotations = getattr(cls, '__annotations__', {})
 
         for name, trait in dict(cls._traits).items():
             # Apply the trait decorator to the object if it is "part 2" of a decorator
             obj = getattr(cls, name)
 
@@ -832,15 +841,15 @@
     def wrapped(msg):
         # filter according to name and type
         if name is not Any and msg["name"] not in name:
             return
         elif msg["type"] not in type_:
             return
         elif isinstance(msg["new"], Trait):
-            raise TypeError(f"Trait instance returned as a callback value")
+            raise TypeError("Trait instance returned as a callback value")
         handler(msg)
 
     if isinstance(obj, HasTraits):
         obj.__notify_list__[handler] = wrapped
     else:
         raise TypeError("object to observe must be an instance of Device")
 
@@ -996,15 +1005,15 @@
     def set_mapping(self, series_or_uncal, cal=None, owner=None):
         """set the lookup mapping as `set_mapping(series)`, where `series` is a pandas Series (uncalibrated
         values in the index), or `set_mapping(cal_vector, uncal_vector)`, where both vectors have 1
         dimension of the same length.
         """
 
         if owner is None:
-            raise ValueError(f"must pass owner to set_mapping")
+            raise ValueError("must pass owner to set_mapping")
 
         import pandas as pd
 
         if isinstance(series_or_uncal, pd.Series):
             by_uncal = pd.Series(series_or_uncal).copy()
         elif cal is not None:
             by_uncal = pd.Series(cal, index=series_or_uncal)
@@ -1052,15 +1061,15 @@
                 cache=self.cache or (self.role == self.ROLE_VALUE),
             )
 
         return ret
 
     @util.hide_in_traceback
     def __set__(self, owner, cal):
-        owner_cal = owner._calibrations.get(self.name, self.EMPTY_STORE)
+        # owner_cal = owner._calibrations.get(self.name, self.EMPTY_STORE)
         self._validate_trait_dependencies(owner, False, "set")
 
         # start with type conversion and validation on the requested calibrated value
         cal = self._trait_dependencies["base"].to_pythonic(cal)
 
         # lookup the uncalibrated value that results in the nearest calibrated result
         uncal = self.find_uncal(cal, owner)
@@ -1137,18 +1146,16 @@
 
         else:
             raise KeyError(f"unsupported trait name {msg['name']}")
 
         # return self._update_index_value(msg["owner"], msg["new"])
 
     def _load_calibration_table(self, owner, path):
-        """ stash the calibration table from disk
-        """
+        """stash the calibration table from disk"""
         import pandas as pd
-        from pathlib import Path
 
         def read(path):
             # quick read
             cal = pd.read_csv(str(path), index_col=self.table_index_column, dtype=float)
 
             cal.columns = cal.columns.astype(float)
             if self.index_lookup_trait.max in cal.index:
@@ -1184,23 +1191,24 @@
                 setattr(owner, self.index_lookup_trait.name, index)
 
     def _update_index_value(self, owner, index_value):
         """update the calibration on change of index_value"""
         cal = owner._calibrations.get(self.name, {}).get(self._CAL_TABLE_KEY, None)
 
         if cal is None:
-            txt = f"index_value change has no effect because calibration_data has not been set"
+            txt = "index_value change has no effect because calibration_data has not been set"
         elif index_value is None:
             cal = None
-            txt = f"set {owner}.{self.index_lookup_trait.name} to enable calibration"
+            txt = "set {owner}.{self.index_lookup_trait.name} to enable calibration"
         else:
             # pull in the calibration mapping specific to this index_value
             i_freq = cal.index.get_loc(index_value, "nearest")
             cal = cal.iloc[i_freq]
-            txt = f"calibrated at {index_value/1e6:0.3f} MHz"
+            txt = f"calibrated to {index_value} {self.label}"
+        owner._logger.debug(txt)
 
         self.set_mapping(cal, owner=owner)
 
     @util.hide_in_traceback
     def __get__(self, owner, owner_cls=None):
         if owner is None or owner_cls is not self.__objclass__:
             return self
@@ -1211,15 +1219,14 @@
 
     @util.hide_in_traceback
     def __set__(self, owner, cal):
         self._touch_table(owner)
         super().__set__(owner, cal)
 
 
-
 class TransformMixIn(DependentTrait):
     """act as an arbitrarily-defined (but reversible) transformation of another BoundedNumber trait"""
 
     _forward: Any = lambda x, y: x
     _reverse: Any = lambda x, y: x
 
     def __init_owner_instance__(self, owner):
@@ -1374,15 +1381,17 @@
 
     def _min(self, owner):
         """overload this to dynamically compute max"""
         return self.min
 
     path_trait: Any = None  # TODO: should be a Unicode string trait
 
-    index_lookup_trait: Any = None  # TODO: this is a trait that should almost certainly be a BoundedNumber
+    index_lookup_trait: Any = (
+        None  # TODO: this is a trait that should almost certainly be a BoundedNumber
+    )
 
     table_index_column: str = None
 
     def calibrate_from_table(
         self,
         path_trait,
         index_lookup_trait,
@@ -1401,15 +1410,18 @@
         """
 
         if label is Undefined:
             label = self.label
 
         ret = TableCorrectionMixIn.derive(
             self,
-            dict(path_trait=path_trait, index_lookup_trait=index_lookup_trait,),
+            dict(
+                path_trait=path_trait,
+                index_lookup_trait=index_lookup_trait,
+            ),
             help=help,
             label=self.label if label is Undefined else label,
             sets=self.sets,
             gets=self.gets,
             allow_none=allow_none,
             table_index_column=table_index_column,
         )
@@ -1429,15 +1441,15 @@
             obj = trait_expression
             while isinstance(obj, DependentTrait):
                 obj = obj._trait_dependencies["base"]
                 if obj == self:
                     break
             else:
                 raise TypeError(
-                    f"the trait being calibrated must also be the first trait in the calibration expression"
+                    "calibration target trait must the first trait in the calibration expression"
                 )
 
         return self.update(
             trait_expression, help=help, label=label, allow_none=allow_none
         )
 
     # def calibrate(
@@ -1592,17 +1604,17 @@
 
 class NonScalar(Any):
     """generically non-scalar data, such as a list, array, but not including a string or bytes"""
 
     @util.hide_in_traceback
     def validate(self, value, owner=None):
         if isinstance(value, (bytes, str)):
-            raise ValueError(f"given text data but expected a non-scalar data")
+            raise ValueError("given text data but expected a non-scalar data")
         if not hasattr(value, "__iter__") and not hasattr(value, "__len__"):
-            raise ValueError(f"expected non-scalar data but given a non-iterable")
+            raise ValueError("expected non-scalar data but given a non-iterable")
         return value
 
 
 class Int(BoundedNumber, type=int):
     """accepts numerical, str, or bytes values, following normal python casting procedures (with bounds checking)"""
```

### Comparing `labbench-0.23.4/labbench/_version.py` & `labbench-0.25.0/tests/test_email.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,26 @@
 # BY PERSONS OR PROPERTY OR OTHERWISE, AND WHETHER OR NOT LOSS WAS SUSTAINED
 # FROM, OR AROSE OUT OF THE RESULTS OF, OR USE OF, THE SOFTWARE OR SERVICES
 # PROVIDED HEREUNDER. Distributions of NIST software should also include
 # copyright and licensing statements of any third-party software that are
 # legally bundled with the code in compliance with the conditions of those
 # licenses.
 
-__version__ = "0.23.4"
+import sys
+
+if ".." not in sys.path:
+    sys.path.insert(0, "..")
+import labbench as lb
+
+if __name__ == "__main__":
+    lb.show_messages("info")
+
+    try:
+        with lb.Email(
+            sender="AggregateLTETestTeam@nistgov.onmicrosoft.com",
+            recipients=["dkuester@nist.gov"],
+        ) as email:
+            lb.logger.warning("test warning message")
+            sys.stderr.write("error info\n")
+            1 // 0
+    except ZeroDivisionError:
+        pass
```

### Comparing `labbench-0.23.4/labbench/datareturn.py` & `labbench-0.25.0/labbench/datareturn.py`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/labbench/datareturn.pyi` & `labbench-0.25.0/labbench/value.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,204 +1,185 @@
 from . import _traits
 
+class any(_traits.Any):
+    def __init__(
+        default=None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
+    ...
 
 class bool(_traits.Bool):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        default: bool = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class float(_traits.Float):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=True,
-        remap: dict={},
-        min: float=None,
-        max: float=None,
+        default: float = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = True,
+        remap: dict = {},
+        min: float = None,
+        max: float = None,
         path_trait=None,
         index_lookup_trait=None,
-        table_index_column: str=None,
-        step: float=None
-    ):
-        ...
+        table_index_column: str = None,
+        step: float = None,
+    ): ...
     ...
 
-
 class int(_traits.Int):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=True,
-        remap: dict={},
-        min: int=None,
-        max: int=None,
+        default: int = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = True,
+        remap: dict = {},
+        min: int = None,
+        max: int = None,
         path_trait=None,
         index_lookup_trait=None,
-        table_index_column: str=None
-    ):
-        ...
+        table_index_column: str = None,
+    ): ...
     ...
 
-
 class complex(_traits.Complex):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        default: complex = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class str(_traits.Unicode):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        case: bool=True
-    ):
-        ...
+        default: str = "",
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        case: bool = True,
+    ): ...
     ...
 
-
 class bytes(_traits.Bytes):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        case: bool=True
-    ):
-        ...
+        default: bytes = b"",
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        case: bool = True,
+    ): ...
     ...
 
-
 class list(_traits.List):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        default: list = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class tuple(_traits.Tuple):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=False,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        default: tuple = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = False,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class dict(_traits.Dict):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        default: dict = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class Path(_traits.Path):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        must_exist: bool=False
-    ):
-        ...
+        default: Path = None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        must_exist: bool = False,
+    ): ...
     ...
 
-
 class NetworkAddress(_traits.NetworkAddress):
-
     def __init__(
-        func: _CallableType=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        case: bool=True,
-        accept_port: bool=True
-    ):
-        ...
+        default: str = "",
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        case: bool = True,
+        accept_port: bool = True,
+    ): ...
     ...
```

### Comparing `labbench-0.23.4/labbench/notebooks.py` & `labbench-0.25.0/labbench/notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,18 @@
 from ._rack import Rack
 from ._traits import observe
 
 import logging
 import time
 from io import StringIO
 import numbers
-import builtins
 
 import pandas as pd
-import numpy as np
 
 import ipywidgets as widgets
-from ipywidgets import IntProgress, HTML, VBox
 from IPython.display import display
 
 skip_traits = {VISADevice: ["identity"], Host: ["log"], core.Device: ["isopen"]}
 
 
 def trait_table(device):
     """Generate a formatted html table widget which updates with recently-observed properties
```

### Comparing `labbench-0.23.4/labbench/notebooks.pyi` & `labbench-0.25.0/labbench/notebooks.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 import logging
 from ._backends import VISADevice as VISADevice
 from ._host import Host as Host
 from ._rack import Rack as Rack
 from ._traits import observe as observe
 from .util import show_messages as show_messages
 from _typeshed import Incomplete
-from ipywidgets import HTML as HTML, IntProgress as IntProgress, VBox as VBox
-skip_traits: Incomplete
 
-def trait_table(device):
-    ...
+skip_traits: Incomplete
 
+def trait_table(device): ...
 
 class TextareaLogHandler(logging.StreamHandler):
     log_format: str
     time_format: str
     max_buffer: int
     min_delay: float
     stream: Incomplete
     widget: Incomplete
     last_time: Incomplete
 
-    def __init__(self, level=...) -> None:
-        ...
-
-    def emit(self, record):
-        ...
-
+    def __init__(self, level=...) -> None: ...
+    def emit(self, record): ...
 
-class panel():
+class panel:
     widget: Incomplete
     ncols: int
     devices: Incomplete
     children: Incomplete
 
-    def __new__(cls, source: int=..., ncols: int=...):
-        ...
+    def __new__(cls, source: int = ..., ncols: int = ...): ...
```

### Comparing `labbench-0.23.4/labbench/property.py` & `labbench-0.25.0/labbench/property.py`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/labbench/property.pyi` & `labbench-0.25.0/labbench/property.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,204 +1,171 @@
 from . import _traits
 
-
 class bool(_traits.Bool):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class float(_traits.Float):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=True,
-        remap: dict={},
-        min: float=None,
-        max: float=None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = True,
+        remap: dict = {},
+        min: float = None,
+        max: float = None,
         path_trait=None,
         index_lookup_trait=None,
-        table_index_column: str=None,
-        step: float=None
-    ):
-        ...
+        table_index_column: str = None,
+        step: float = None,
+    ): ...
     ...
 
-
 class int(_traits.Int):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=True,
-        remap: dict={},
-        min: int=None,
-        max: int=None,
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = True,
+        remap: dict = {},
+        min: int = None,
+        max: int = None,
         path_trait=None,
         index_lookup_trait=None,
-        table_index_column: str=None
-    ):
-        ...
+        table_index_column: str = None,
+    ): ...
     ...
 
-
 class complex(_traits.Complex):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class str(_traits.Unicode):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        case: bool=True
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        case: bool = True,
+    ): ...
     ...
 
-
 class bytes(_traits.Bytes):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        case: bool=True
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        case: bool = True,
+    ): ...
     ...
 
-
 class list(_traits.List):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class tuple(_traits.Tuple):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=False,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = False,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class dict(_traits.Dict):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={}
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+    ): ...
     ...
 
-
 class Path(_traits.Path):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        must_exist: bool=False
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        must_exist: bool = False,
+    ): ...
     ...
 
-
 class NetworkAddress(_traits.NetworkAddress):
-
     def __init__(
         key=None,
-        help: str='',
-        label: str='',
-        sets: bool=True,
-        gets: bool=True,
-        cache: bool=False,
-        only: tuple=(),
-        allow_none: bool=False,
-        remap: dict={},
-        case: bool=True,
-        accept_port: bool=True
-    ):
-        ...
+        help: str = "",
+        label: str = "",
+        sets: bool = True,
+        gets: bool = True,
+        cache: bool = False,
+        only: tuple = (),
+        allow_none: bool = False,
+        remap: dict = {},
+        case: bool = True,
+        accept_port: bool = True,
+    ): ...
     ...
```

### Comparing `labbench-0.23.4/labbench/util.py` & `labbench-0.25.0/labbench/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,80 +41,84 @@
     "ThreadSandbox",
     "ThreadEndedByMaster",
     # timing and flow management
     "retry",
     "until_timeout",
     "sleep",
     "stopwatch",
-    "timeout_iter"
+    "timeout_iter",
     # wrapper helpers
     "copy_func",
     # traceback scrubbing
     "hide_in_traceback",
     "_force_full_traceback",
     # helper objects
     "Ownable",
 ]
 
-from contextlib import contextmanager, _GeneratorContextManager
-from functools import wraps
-from queue import Queue, Empty
-from threading import Thread, ThreadError, Event
-from typing import Callable
-
-import builtins
+import ast
 import hashlib
 import inspect
 import logging
-import psutil
+import re
 import sys
+import textwrap
 import time
+import types
 import traceback
+from contextlib import _GeneratorContextManager, contextmanager
+from functools import wraps
+from queue import Empty, Queue
+from threading import Event, Thread, ThreadError
+from typing import Callable
 from warnings import simplefilter
 
+import psutil
+
 import_t0 = time.perf_counter()
 
 logger = logging.LoggerAdapter(
     logging.getLogger("labbench"),
     dict(
         label="labbench"
     ),  # description of origin within labbench (for screen logs only)
 )
 
+
 # show deprecation warnings only once
 class LabbenchDeprecationWarning(DeprecationWarning):
     pass
 
 
 simplefilter("once", LabbenchDeprecationWarning)
-import weakref
 
 
 def show_messages(minimum_level, colors=True):
-    """Configure screen debug message output for any messages as least as important as indicated by `level`.
+    """filters logging messages displayed to the console by importance
 
     Arguments:
-        minimum_level: One of 'debug', 'warning', 'error', or None. If None, there will be no output.
+        minimum_level: 'debug', 'warning', 'error', or None (to disable all output)
     Returns:
         None
     """
 
     import logging
 
     err_map = {
         "debug": logging.DEBUG,
         "warning": logging.WARNING,
         "error": logging.ERROR,
         "info": logging.INFO,
         None: None,
+        False: None,
     }
 
     if minimum_level not in err_map and not isinstance(minimum_level, int):
         raise ValueError(
-            f"message level must be a flag {tuple(err_map.keys())} or an integer, not {repr(minimum_level)}"
+            f"message level must be a flag {tuple(err_map)} or an integer, not {repr(minimum_level)}"
         )
 
     level = (
         err_map[minimum_level.lower()]
         if isinstance(minimum_level, str)
         else minimum_level
     )
@@ -129,34 +133,39 @@
         return
 
     logger._screen_handler = logging.StreamHandler()
     logger._screen_handler.setLevel(level)
     # - %(pathname)s:%(lineno)d'
 
     if colors:
-        from coloredlogs import ColoredFormatter, DEFAULT_FIELD_STYLES
+        from coloredlogs import DEFAULT_FIELD_STYLES, ColoredFormatter
 
         log_fmt = "{levelname:^7s} {asctime}.{msecs:03.0f} • {label}: {message}"
-        styles = dict(DEFAULT_FIELD_STYLES, label=dict(color="blue"),)
+        styles = dict(
+            DEFAULT_FIELD_STYLES,
+            label=dict(color="blue"),
+        )
         formatter = ColoredFormatter(log_fmt, style="{", field_styles=styles)
     else:
         log_fmt = "{levelname:^7s} {asctime}.{msecs:03.0f} • {label}: {message}"
         formatter = logging.Formatter(log_fmt, style="{")
 
     logger._screen_handler.setFormatter(formatter)
     logger.logger.addHandler(logger._screen_handler)
 
 
 show_messages("info")
 
 
 def _inject_logger_metadata(obj):
     d = dict(
-        object=repr(obj), origin=type(obj).__qualname__, owned_name=obj._owned_name,
-    )  
+        object=repr(obj),
+        origin=type(obj).__qualname__,
+        owned_name=obj._owned_name,
+    )
 
     if d["owned_name"] is not None:
         d["label"] = d["owned_name"]
     elif repr(obj) == object.__repr__(obj):
         d["label"] = type(obj).__qualname__ + "(...)"
     else:
         txt = repr(obj)
@@ -179,15 +188,16 @@
 
     __objclass__ = None
     _owned_name = None
     _logger = logger
 
     def __init__(self):
         self._logger = logging.LoggerAdapter(
-            logger.logger, extra=_inject_logger_metadata(self),
+            logger.logger,
+            extra=_inject_logger_metadata(self),
         )
 
     def __set_name__(self, owner_cls, name):
         self.__objclass__ = owner_cls
         self.__name__ = name
 
     def __get__(self, owner, owner_cls=None):
@@ -241,16 +251,14 @@
 
 
 concurrency_count = 0
 stop_request_event = Event()
 
 sys._debug_tb = False
 
-import types
-
 TRACEBACK_HIDE_TAG = "🦙 hide from traceback 🦙"
 
 
 def hide_in_traceback(func):
     def adjust(f):
         code = f.__code__
 
@@ -318,15 +326,15 @@
                         prev_tb.tb_next = tb.tb_next
 
                 # on to the next traceback
                 prev_tb, tb = tb, tb.tb_next
 
             return etype, evalue, start_tb
 
-        except BaseException as e:
+        except BaseException:
             raise
 
 
 def copy_func(
     func,
     assigned=("__module__", "__name__", "__qualname__", "__doc__", "__annotations__"),
     updated=("__dict__",),
@@ -352,92 +360,14 @@
 
     for attr in updated:
         getattr(new, attr).update(getattr(func, attr))
 
     return new
 
 
-# TODO: remove this
-def withsignature(
-    cls,
-    name: str,
-    fields: list,
-    defaults: dict,
-    positional: int = None,
-    annotations: dict = {},
-):
-    """Replace cls.__init__ with a wrapper function with an explicit
-    call signature, replacing the actual call signature that can be
-    dynamic __init__(self, *args, **kws) call signature.
-
-    :fields: iterable of names of each call signature argument
-    :
-    """
-    # Is the existing cls.__init__ already a __init__ wrapper?
-    wrapped = getattr(cls, name)
-    orig_doc = getattr(wrapped, "__origdoc__", cls.__init__.__doc__)
-    reuse = hasattr(wrapped, "__dynamic__")
-
-    defaults = tuple(defaults.items())
-
-    if positional is None:
-        positional = len(fields)
-
-    # Generate a code object with the adjusted signature
-    code = wrapper.__code__
-
-    if tuple(sys.version_info)[:2] >= (3, 8):
-        # there is a new co_posonlyargs argument since 3.8 - use the new .replace
-        # to be less brittle to future signature changes
-        code = code.replace(
-            co_argcount=1 + positional,  # to include self
-            co_posonlyargcount=0,
-            co_kwonlyargcount=len(fields) - positional,
-            co_nlocals=len(fields) + 1,  # to include self
-            co_varnames=("self",) + tuple(fields),
-        )
-    else:
-        code = types.CodeType(
-            1 + positional,  # co_argcount
-            len(fields) - positional,  # co_kwonlyargcount
-            len(fields) + 1,  # co_nlocals
-            code.co_stacksize,
-            code.co_flags,
-            code.co_code,
-            code.co_consts,
-            code.co_names,
-            ("self",) + tuple(fields),  # co_varnames
-            code.co_filename,
-            code.co_name,
-            code.co_firstlineno,
-            code.co_lnotab,
-            code.co_freevars,
-            code.co_cellvars,
-        )
-
-    # Generate the new wrapper function and its signature
-    __globals__ = getattr(wrapped, "__globals__", builtins.__dict__)
-    import functools
-
-    wrapper = types.FunctionType(code, __globals__, wrapped.__name__)
-
-    wrapper.__doc__ = wrapped.__doc__
-    wrapper.__qualname__ = wrapped.__qualname__
-    wrapper.__defaults__ = tuple((v for k, v in defaults[:positional]))
-    wrapper.__kwdefaults__ = {k: v for k, v in defaults[positional:]}
-    wrapper.__annotations__ = annotations
-    wrapper.__dynamic__ = True
-
-    if not reuse:
-        setattr(cls, name + "_wrapped", wrapped)
-    setattr(cls, name, wrapper)
-
-    wrapper.__doc__ = wrapper.__origdoc__ = orig_doc
-
-
 if not hasattr(sys.exc_info, "lb_wrapped"):
     # monkeypatch sys.exc_info if it needs
     sys.exc_info, exc_info = _filtered_exc_info(sys.exc_info), sys.exc_info
 
 
 def sleep(seconds, tick=1.0):
     """Drop-in replacement for time.sleep that raises ConcurrentException
@@ -787,15 +717,15 @@
                     msg = (
                         f"another callable is already named {repr(name)} - "
                         "pass as a keyword argument to specify a different name"
                     )
                     raise KeyError(msg)
 
                 ret[name] = func
-            except:
+            except BaseException:
                 raise
 
         return ret
 
 
 class MultipleContexts:
     """Handle opening multiple contexts in a single `with` block. This is
@@ -851,15 +781,15 @@
         """
         enter!
         """
         if not self.abort:
             # proceed only if there have been no exceptions
             try:
                 context.__enter__()  # start of a context entry thread
-            except:
+            except BaseException:
                 self.abort = True
                 self.exc[name] = sys.exc_info()
                 raise
             else:
                 self._entered[name] = context
 
     @hide_in_traceback
@@ -882,15 +812,15 @@
                 context = self._entered[name]
 
                 if name in self.exc:
                     continue
 
                 try:
                     context.__exit__(None, None, None)
-                except:
+                except BaseException:
                     exc = sys.exc_info()
                     traceback.print_exc()
 
                     # don't overwrite the original exception, if there was one
                     self.exc.setdefault(name, exc)
 
             contexts = dict(self.objs)
@@ -1008,15 +938,14 @@
 
     dicts = []
 
     # Make sure candidates are either (1) all context managers
     # or (2) all callables. Decide what type of operation to proceed with.
     runner = None
     for i, (k, obj) in enumerate(candidates):
-
         # pass through dictionary objects from nested calls
         if isdictducktype(obj.__class__):
             dicts.append(candidates.pop(i))
             continue
 
         thisone = RUNNERS[
             (
@@ -1024,29 +953,27 @@
             ),  # Is it callable?
             (
                 hasattr(obj, "__enter__") or isinstance(obj, _GeneratorContextManager)
             ),  # Is it a context manager?
         ]
 
         if thisone is None:
-            msg = f"each argument must be a callable and/or a context manager, "
+            msg = "each argument must be a callable and/or a context manager, "
 
             if k is None:
                 msg += f"but given {repr(obj)}"
             else:
                 msg += f"but given {k}={repr(obj)}"
 
             raise TypeError(msg)
         elif runner in (None, "both"):
             runner = thisone
         else:
             if thisone not in (runner, "both"):
-                raise TypeError(
-                    f"cannot run a mixture of context managers and callables"
-                )
+                raise TypeError("cannot mix context managers and callables")
 
     # Enforce uniqueness in the (callable or context manager) object
     candidate_objs = [c[1] for c in candidates]
     if len(set(candidate_objs)) != len(candidate_objs):
         raise ValueError("each callable and context manager must be unique")
 
     if runner is None:
@@ -1147,15 +1074,14 @@
             logger.error(
                 f"raising {parent_exception.__class__.__name__} in main thread after child threads {names} return"
             )
 
         # if there was an exception that wasn't us ending the thread,
         # show messages
         if called.traceback is not None:
-
             tb = traceback_skip(called.traceback, 1)
 
             if called.traceback[0] is not ThreadEndedByMaster:
                 #                exception_count += 1
                 tracebacks.append(tb)
                 last_exception = called.traceback[1]
 
@@ -1302,18 +1228,18 @@
      This is the sequential implementation of the `concurrently` function,
      with a compatible convention of returning dictionaries.
 
     Multiple references to the same function in `objs` only result in one call. The `nones`
     argument may be callables in  case they are executed (and each flag value is treated as defaults).
 
     Arguments:
-        objs:  each argument may be a callable (function, or class that defines a __call__ method), or context manager (such as a Device instance)
-        kws: dictionary of further callables or context managers, with names set by the dictionary key
-        nones: if True, include dictionary entries for calls that return None (default is False); left as another entry in `kws` if callable or a context manager
-        flatten: if `True`, results of callables that returns a dictionary are merged into the return dictionary with update (instead of passed through as dictionaries)
+        objs:  callables or context managers or Device instances for connections
+        kws: dictionary of additional callables or Device instances for connections
+        nones: `True` to include dictionary entries for calls that return None (default: False)
+        flatten: `True` to flatten any `dict` return values into the return dictionary
     Returns:
         a dictionary keyed on the object name containing the return value of each function
     :rtype: dictionary of keyed by function
 
     Here are some examples:
 
     :Example: Call each function `myfunc1` and `myfunc2`, each with no arguments:
@@ -1575,19 +1501,14 @@
 
         df = pd.DataFrame([cls.all()]).T
         df.columns.name = "Value"
         df.index.name = "Parameter"
         return df
 
 
-import ast
-import textwrap
-import re
-
-
 def accessed_attributes(method):
     """enumerate the attributes of the parent class accessed by `method`
 
     :method: callable that is a method or defined in a class
     Returns:
         tuple of attribute names
     """
@@ -1598,15 +1519,15 @@
     elif not inspect.ismethod(method) and "." not in method.__qualname__:
         raise ValueError(f"{method} is not defined in a class")
 
     # parse into a code tree
     source = inspect.getsource(method)
 
     # filter out lines that start with comments, which have no tokens and confuse textwrap.dedent
-    source = "\n".join(re.findall("^[\ \t\r\n]*[^\#].*", source, re.MULTILINE))
+    source = "\n".join(re.findall("^[ \t\r\n]*[^#].*", source, re.MULTILINE))
 
     parsed = ast.parse(textwrap.dedent(source))
     if len(parsed.body) > 1:
         # this should not be possible
         raise Exception("ast parsing gave unexpected extra nodes")
 
     # pull out the function node and the name for the class instance
```

### Comparing `labbench-0.23.4/labbench/util.pyi` & `labbench-0.25.0/labbench/util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from _typeshed import Incomplete
+from collections.abc import Generator
 from threading import ThreadError
 from typing import Callable
 
 import_t0: Incomplete
 logger: Incomplete
 
 class LabbenchDeprecationWarning(DeprecationWarning): ...
@@ -27,18 +28,32 @@
 def hide_in_traceback(func): ...
 
 class _filtered_exc_info:
     lb_wrapped: Incomplete
     def __init__(self, wrapped) -> None: ...
     def __call__(self): ...
 
+def copy_func(func, assigned=..., updated=...) -> callable: ...
 def sleep(seconds, tick: float = ...) -> None: ...
 def check_hanging_thread() -> None: ...
-def retry(exception_or_exceptions, tries: int = ..., delay: int = ..., backoff: int = ..., exception_func=...): ...
-def until_timeout(exception_or_exceptions, timeout, delay: int = ..., backoff: int = ..., exception_func=...): ...
+def retry(
+    exception_or_exceptions,
+    tries: int = ...,
+    delay: int = ...,
+    backoff: int = ...,
+    exception_func=...,
+): ...
+def until_timeout(
+    exception_or_exceptions,
+    timeout,
+    delay: int = ...,
+    backoff: int = ...,
+    exception_func=...,
+): ...
+def timeout_iter(duration) -> Generator[Incomplete, None, None]: ...
 def kill_by_name(*names) -> None: ...
 def hash_caller(call_depth: int = ...): ...
 def stopwatch(desc: str = ..., threshold: float = ...): ...
 
 class Call:
     func: Incomplete
     name: Incomplete
@@ -56,15 +71,17 @@
 class MultipleContexts:
     abort: bool
     __name__: str
     objs: Incomplete
     params: Incomplete
     call_handler: Incomplete
     exc: Incomplete
-    def __init__(self, call_handler: Callable[[dict, list, dict], dict], params: dict, objs: list) -> None: ...
+    def __init__(
+        self, call_handler: Callable[[dict, list, dict], dict], params: dict, objs: list
+    ) -> None: ...
     def enter(self, name, context) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(self, *exc) -> None: ...
 
 def concurrently(*objs, **kws): ...
 def sequentially(*objs, **kws): ...
 
@@ -74,22 +91,23 @@
     def __getattribute__(self, name): ...
     def __dir__(self): ...
     def __setattr__(self, name, value): ...
 
 class ThreadSandbox:
     __repr_root__: str
     __dir_root__: Incomplete
-    def __init__(self, factory, should_sandbox_func: Incomplete | None = ...) -> None: ...
+    def __init__(
+        self, factory, should_sandbox_func: Incomplete | None = ...
+    ) -> None: ...
     def __getattr__(self, name): ...
     def __setattr__(self, name, value): ...
     def __del__(self) -> None: ...
     def __dir__(self): ...
 
 class ConfigStore:
     @classmethod
     def all(cls): ...
     @classmethod
     def frame(cls): ...
 
 # Names in __all__ with no definition:
 #   _force_full_traceback
-#   timeout_itercopy_func
```

### Comparing `labbench-0.23.4/labbench/value.py` & `labbench-0.25.0/labbench/value.py`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/tests/all.py` & `labbench-0.25.0/tests/all.py`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/tests/emulate.py` & `labbench-0.25.0/tests/emulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import labbench as lb
 
 
 class EmulatedVISADevice(lb.Device):
-    """ Act as a VISA device without dispatching any visa keys
-    """
+    """Act as a VISA device without dispatching any visa keys"""
 
     # Settings
     read_termination = lb.value.str("\n", help="end-of-receive termination character")
     write_termination = lb.value.str("\n", help="end-of-transmit termination character")
 
     # States
     @lb.property.str(key="*IDN", sets=False, cache=True)
     def identity(self):
-        """ identity string reported by the instrument """
+        """identity string reported by the instrument"""
         return self.__class__.__qualname__
 
     @lb.property.str(key="*OPT", sets=False, cache=True)
     def options(self):
-        """ options reported by the instrument """
+        """options reported by the instrument"""
 
         param_strs = (f"{s}={getattr(self,s)}" for s in self._value_attrs)
         return ",".join(param_strs)
 
     @lb.property.dict(key="*STB", sets=False)
     def status_byte(self):
-        """ VISA status byte reported by the instrument """
+        """VISA status byte reported by the instrument"""
         return {
             "error queue not empty": False,
             "questionable state": False,
             "message available": False,
             "event status flag": False,
             "service request": False,
             "master status summary": False,
```

### Comparing `labbench-0.23.4/tests/module_as_testbed.py` & `labbench-0.25.0/tests/module_as_testbed.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 lb = importlib.reload(lb)
 
 from emulate import EmulatedVISADevice
 
 
 class LaggyInstrument(EmulatedVISADevice):
-    """ A mock "instrument"
+    """A mock "instrument"
     with value and property traits to
     demonstrate the process of value trait
     up a measurement.
     """
 
     # Connection and driver value traits
     delay = lb.value.float(default=0, min=0, help="connection time (s)")
@@ -28,28 +28,26 @@
     def open(self):
         self.perf = {}
         t0 = time.perf_counter()
         lb.sleep(self.delay)
         self.perf["open"] = time.perf_counter() - t0
 
     def fetch(self):
-        """ Return the argument after a 1s delay
-        """
+        """Return the argument after a 1s delay"""
         lb.logger.info(f"{self}.fetch start")
         t0 = time.perf_counter()
         lb.sleep(self.fetch_time)
         self.perf["fetch"] = time.perf_counter() - t0
         return self.fetch_time
 
     def dict(self):
         return {self.resource: self.resource}
 
     def none(self):
-        """ Return None
-        """
+        """Return None"""
         return None
 
     def close(self):
         if self.fail_disconnect:
             1 / 0
```

### Comparing `labbench-0.23.4/tests/test_data_logging.py` & `labbench-0.25.0/tests/test_data_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 lb._force_full_traceback(True)
 
 FREQUENCIES = 10e6, 100e6, 1e9, 10e9
 METADATA = dict(power=1.21e9, potato=7)
 
 
 class EmulatedInstrument(EmulatedVISADevice):
-    """ This "instrument" makes mock data and instrument property traits to
-        demonstrate we can show the process of value trait
-        up a measurement.
+    """This "instrument" makes mock data and instrument property traits to
+    demonstrate we can show the process of value trait
+    up a measurement.
     """
 
     # values
     trace_index = lb.value.int(0)
 
     # properties
     initiate_continuous = lb.property.bool(key="INIT:CONT")
@@ -58,25 +58,23 @@
     )
     frequency = lb.property.float(
         key="SENS:FREQ", min=10e6, max=18e9, help="center frequency (in Hz)"
     )
     atten = lb.property.float(key="POW", min=0, max=100, step=0.5)
 
     def trigger(self):
-        """ This would tell the instrument to start a measurement
-        """
+        """This would tell the instrument to start a measurement"""
         pass
 
     def method(self):
         print("method!")
 
     @lb.datareturn.DataFrame
     def fetch_trace(self, N=101):
-        """ Generate N points of junk data as a pandas series.
-        """
+        """Generate N points of junk data as a pandas series."""
         self.trace_index = self.trace_index + 1
 
         series = pd.Series(
             self.trace_index * np.ones(N),
             index=self.sweep_aperture * np.arange(N),
             name="Voltage (V)",
         )
@@ -84,27 +82,25 @@
         series.index.name = "Time (s)"
         return series
 
 
 class TestDB(unittest.TestCase):
     def test_state_wrapper_type(self):
         with EmulatedInstrument() as m, lb.SQLiteLogger(path) as db:
-
             self.assertEqual(m.param, int_start)
             m.param = int_stop
             self.assertEqual(m.param, int_stop)
 
 
 if __name__ == "__main__":
     lb.show_messages("debug")
 
     path = f"test db/{np.random.bytes(8).hex()}"
 
     with EmulatedInstrument() as inst, lb.SQLiteLogger(path, tar=False) as db:
-
         db.observe(inst, changes=True, always="sweep_aperture")
 
         inst.fetch_trace()
 
         for inst.frequency in FREQUENCIES:
             inst.index = inst.frequency
             inst.fetch_trace()
```

### Comparing `labbench-0.23.4/tests/test_doc.py` & `labbench-0.25.0/tests/test_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,15 @@
         print("connect child")
 
     def close(self):
         print("disconnect child")
 
 
 class Mock(lb.Device):
-    """ Helpful driver wrapper
-    """
+    """Helpful driver wrapper"""
 
     child0 = Child("addr0")
     child1 = Child("addr1")
 
 
 if __name__ == "__main__":
     with Mock() as m:
```

### Comparing `labbench-0.23.4/tests/test_email.py` & `labbench-0.25.0/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `labbench-0.23.4/tests/test_property.py` & `labbench-0.25.0/tests/test_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
                         m.PYTHONIC_VALUE_DEFAULT[trait_name],
                         msg=msg,
                     )
                     self.assertEqual(m.get_get_count(trait_name), 1, msg=msg)
 
     def test_get_default(self):
         """
-        Ensure that values are returned, typing is correct, and 
+        Ensure that values are returned, typing is correct, and
         """
         with self.TestDevice() as m:
             m.clear_counts()
 
             # remapped bool "get"
             for trait_name, value in m.PYTHONIC_VALUE_DEFAULT.items():
                 msg = f'testing property "{trait_name}"'
```

### Comparing `labbench-0.23.4/tests/test_rack.py` & `labbench-0.25.0/tests/test_rack.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     from emulate import EmulatedVISADevice
 from contextlib import contextmanager
 import labbench as lb
 import numpy as np
 
 
 class LaggyInstrument(EmulatedVISADevice):
-    """ A fake "instrument" with traits and fetch methods
-    """
+    """A fake "instrument" with traits and fetch methods"""
 
     # Connection and driver value traits
     delay = lb.value.float(0, min=0, help="connection time")
     fetch_time = lb.value.float(0, min=0, help="fetch time")
     fail_disconnect = lb.value.bool(
         False, help="True to raise DivideByZero on disconnect"
     )
@@ -62,30 +61,28 @@
     def open(self):
         self.perf = {}
         t0 = time.perf_counter()
         lb.sleep(self.delay)
         self.perf["open"] = time.perf_counter() - t0
 
     def fetch(self):
-        """ Return the argument after a 1s delay
-        """
+        """Return the argument after a 1s delay"""
         import pandas as pd
 
         lb.logger.info(f"{self}.fetch start")
         t0 = time.perf_counter()
         lb.sleep(self.fetch_time)
         self.perf["fetch"] = time.perf_counter() - t0
         return pd.Series([1, 2, 3, 4, 5, 6])
 
     def dict(self):
         return {self.resource: self.resource}
 
     def none(self):
-        """ Return None
-        """
+        """Return None"""
         return None
 
     def close(self):
         if self.fail_disconnect:
             1 // 0
```

### Comparing `labbench-0.23.4/tests/test_sequencing.py` & `labbench-0.25.0/tests/test_sequencing.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
 lb.util.show_messages("debug")
 
 lb._force_full_traceback(True)
 
 
 class LaggyInstrument(EmulatedVISADevice):
-    """A mock "instrument" to measure time response in (a)sync operations
-    """
+    """A mock "instrument" to measure time response in (a)sync operations"""
 
     delay = lb.value.float(0, min=0, help="connection time")
     fetch_time = lb.value.float(0, min=0, help="fetch time")
     fail_disconnect = lb.value.bool(
         False, help="whether to raise DivideByZero on disconnect"
     )
 
@@ -58,29 +57,27 @@
         self._logger.info(f"{self} connect start")
         t0 = time.perf_counter()
         lb.sleep(self.delay)
         self.perf["open"] = time.perf_counter() - t0
         self._logger.info(f"{self} connected")
 
     def fetch(self):
-        """ Return the argument after a 1s delay
-        """
+        """Return the argument after a 1s delay"""
         lb.logger.info(f"{self}.fetch start")
         t0 = time.perf_counter()
         lb.sleep(self.fetch_time)
         lb.logger.info(f"{self}.fetch done")
         self.perf["fetch"] = time.perf_counter() - t0
         return self.fetch_time
 
     def dict(self):
         return {self.resource: self.resource}
 
     def none(self):
-        """ Return None
-        """
+        """Return None"""
         return None
 
     def close(self):
         self._logger.info(f"{self} disconnected")
         if self.fail_disconnect:
             1 / 0
 
@@ -98,20 +95,20 @@
 
 class TestConcurrency(unittest.TestCase):
     # Acceptable error in delay time meaurement
     delay_tol = 0.08
 
     @contextmanager
     def assert_delay(self, expected_delay):
-        """ Time a block of code using a with statement like this:
-    
+        """Time a block of code using a with statement like this:
+
         >>> with stopwatch('sleep statement'):
         >>>     time.sleep(2)
         sleep statement time elapsed 1.999s.
-    
+
         :param desc: text for display that describes the event being timed
         :type desc = str
         :return: context manager
         """
         t0 = time.perf_counter()
         try:
             yield
```

### Comparing `labbench-0.23.4/tests/test_shell.py` & `labbench-0.25.0/tests/test_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,18 @@
         return (
             name
             for name, trait in self._traits.items()
             if trait.key is not lb.Undefined
         )
 
     def _commandline(self, **flags):
-        """ Form a list of commandline argument strings for foreground
-            or background calls.
+        """Form a list of commandline argument strings for foreground
+        or background calls.
 
-            :returns: tuple of string
+        :returns: tuple of string
         """
 
         # validate the set of flags
         unsupported = set(flags).difference(self._flag_names())
         if len(unsupported) > 1:
             raise KeyError(f"flags {unsupported} are unsupported")
```

### Comparing `labbench-0.23.4/tests/test_value.py` & `labbench-0.25.0/tests/test_value.py`

 * *Files identical despite different names*

