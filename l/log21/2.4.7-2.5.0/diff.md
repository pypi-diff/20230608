# Comparing `tmp/log21-2.4.7.tar.gz` & `tmp/log21-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.4.7.tar", last modified: Tue May  9 19:44:45 2023, max compression
+gzip compressed data, was "log21-2.5.0.tar", last modified: Thu Jun  8 13:27:36 2023, max compression
```

## Comparing `log21-2.4.7.tar` & `log21-2.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-09 19:44:39.000000 log21-2.4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-09 19:44:45.972288 log21-2.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-09 19:44:39.000000 log21-2.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-09 19:44:39.000000 log21-2.4.7/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-05-09 19:44:39.000000 log21-2.4.7/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 19:44:39.000000 log21-2.4.7/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-09 19:44:39.000000 log21-2.4.7/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-05-09 19:44:39.000000 log21-2.4.7/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 19:44:39.000000 log21-2.4.7/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-05-09 19:44:39.000000 log21-2.4.7/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-09 19:44:39.000000 log21-2.4.7/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-09 19:44:39.000000 log21-2.4.7/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-09 19:44:39.000000 log21-2.4.7/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-05-09 19:44:39.000000 log21-2.4.7/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:44:45.972288 log21-2.4.7/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 19:44:45.000000 log21-2.4.7/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:44:45.972288 log21-2.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 19:44:39.000000 log21-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:27:36.656492 log21-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-08 13:27:32.000000 log21-2.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-08 13:27:36.656492 log21-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-06-08 13:27:32.000000 log21-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:27:36.656492 log21-2.5.0/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-06-08 13:27:32.000000 log21-2.5.0/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-08 13:27:32.000000 log21-2.5.0/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:27:36.656492 log21-2.5.0/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-08 13:27:32.000000 log21-2.5.0/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-08 13:27:32.000000 log21-2.5.0/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 13:27:32.000000 log21-2.5.0/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 13:27:32.000000 log21-2.5.0/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-06-08 13:27:32.000000 log21-2.5.0/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-08 13:27:32.000000 log21-2.5.0/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-08 13:27:32.000000 log21-2.5.0/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-06-08 13:27:32.000000 log21-2.5.0/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-08 13:27:32.000000 log21-2.5.0/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25549 2023-06-08 13:27:32.000000 log21-2.5.0/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-06-08 13:27:32.000000 log21-2.5.0/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-08 13:27:32.000000 log21-2.5.0/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-08 13:27:32.000000 log21-2.5.0/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21423 2023-06-08 13:27:32.000000 log21-2.5.0/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:27:36.656492 log21-2.5.0/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-08 13:27:36.000000 log21-2.5.0/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 13:27:36.000000 log21-2.5.0/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:27:36.000000 log21-2.5.0/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 13:27:36.000000 log21-2.5.0/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 13:27:36.000000 log21-2.5.0/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:27:36.656492 log21-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-08 13:27:32.000000 log21-2.5.0/setup.py
```

### Comparing `log21-2.4.7/LICENSE.txt` & `log21-2.5.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [2021-2022] [CodeWriter21]
+   Copyright [2021-2023] [CodeWriter21]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `log21-2.4.7/PKG-INFO` & `log21-2.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.7
+Version: 2.5.0
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -69,22 +69,20 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.7
+### 2.5.0
 
-Added `extra_values` argument to `CrashReporter.Formatter` which will let you pass extra static or dynamic values to the
-report formatter.
-They can be used in the format string. For dynamic values you can pass a function that takes no
-arguments as the value.
+Added `level_colors` argument to `log21.get_logger` function with will be passed to the formatter and allows
+user to set custom level colors while making a new logger.
 
-[Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
+[Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
 ```python3
 import log21
```

### Comparing `log21-2.4.7/README.md` & `log21-2.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,20 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.7
+### 2.5.0
 
-Added `extra_values` argument to `CrashReporter.Formatter` which will let you pass extra static or dynamic values to the
-report formatter.
-They can be used in the format string. For dynamic values you can pass a function that takes no
-arguments as the value.
+Added `level_colors` argument to `log21.get_logger` function with will be passed to the formatter and allows
+user to set custom level colors while making a new logger.
 
-[Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
+[Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
 ```python3
 import log21
```

### Comparing `log21-2.4.7/log21/Argparse.py` & `log21-2.5.0/log21/Argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # log21.Argparse.py
 # CodeWriter21
 
 import re as _re
 import sys as _sys
 import log21 as _log21
 import argparse as _argparse
-from typing import Dict as _Dict
+from typing import Mapping as _Mapping
 from gettext import gettext as _gettext
 from textwrap import TextWrapper as _TextWrapper
 from log21.Colors import get_colors as _gc
 from log21.Formatters import DecolorizingFormatter as _Formatter
 
 __all__ = ['ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper']
 
@@ -23,15 +23,15 @@
         'colons': 'LightRed',
         'commas': 'LightRed',
         'section headers': 'LightGreen',
         'help': 'LightWhite',
         'choices': 'LightGreen'
     }
 
-    def __init__(self, prog, indent_increment=2, max_help_position=24, width=None, colors: _Dict[str, str] = None):
+    def __init__(self, prog, indent_increment=2, max_help_position=24, width=None, colors: _Mapping[str, str] = None):
         super().__init__(prog, indent_increment, max_help_position, width)
         if colors:
             for key, value in colors.items():
                 if key in self.colors:
                     self.colors[key] = value
 
     class _Section(object):
@@ -473,15 +473,15 @@
                         lines.append(indent + self.placeholder.lstrip())
                     break
 
         return lines
 
 
 class ColorizingArgumentParser(_argparse.ArgumentParser):
-    def __init__(self, formatter_class=ColorizingHelpFormatter, colors: _Dict[str, str] = None, **kwargs):
+    def __init__(self, formatter_class=ColorizingHelpFormatter, colors: _Mapping[str, str] = None, **kwargs):
         self.logger = _log21.Logger('ArgumentParser')
         self.colors = colors
         super().__init__(formatter_class=formatter_class, **kwargs)
 
     def _print_message(self, message, file=None):
         if message:
             self.logger.handlers.clear()
```

### Comparing `log21-2.4.7/log21/Colors.py` & `log21-2.5.0/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/CrashReporter/Formatters.py` & `log21-2.5.0/log21/CrashReporter/Formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # log21.CrashReporter.Formatters.py
 # CodeWriter21
 
 import traceback
 
 from datetime import datetime as _datetime
-from typing import Dict as _Dict, Union as _Union, Callable as _Callable, Any as _Any
+from typing import Mapping as _Mapping, Union as _Union, Callable as _Callable, Any as _Any
 
 __all__ = ['Formatter', 'CONSOLE_REPORTER_FORMAT', 'FILE_REPORTER_FORMAT', 'EMAIL_REPORTER_FORMAT']
 
 RESERVED_KEYS = (
     '__name__',
     'type',
     'message',
@@ -19,15 +19,15 @@
     'function',
     'asctime'
 )
 
 
 class Formatter:
     def __init__(self, format_: str, style: str = '%', datefmt: str = '%Y-%m-%d %H:%M:%S',
-                 extra_values: _Dict[str, _Union[str, _Callable, _Any]] = None):
+                 extra_values: _Mapping[str, _Union[str, _Callable, _Any]] = None):
         self._format = format_
 
         if style in ['%', '{']:
             self.__style = style
         else:
             raise ValueError('Invalid style: "' + str(style) + '" Valid styles: %, {')
```

### Comparing `log21-2.4.7/log21/CrashReporter/Reporters.py` & `log21-2.5.0/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/FileHandler.py` & `log21-2.5.0/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/Formatters.py` & `log21-2.5.0/log21/Formatters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # log21.Formatters.py
 # CodeWriter21
 
 import time as _time
 from logging import Formatter as __Formatter
-from typing import Dict as _Dict, Tuple as _Tuple
+from typing import Mapping as _Mapping, Tuple as _Tuple
 from log21.Colors import get_colors as _gc, ansi_escape
 from log21.Levels import INPUT, CRITICAL, ERROR, WARNING, INFO, DEBUG, PRINT
 
 __all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
 
 
 class _Formatter(__Formatter):
-    _level_names: _Dict[int, str] = {
+    _level_names: _Mapping[int, str] = {
         DEBUG: 'DEBUG',
         INFO: 'INFO',
         WARNING: 'WARNING',
         ERROR: 'ERROR',
         CRITICAL: 'CRITICAL',
         PRINT: 'PRINT',
         INPUT: 'INPUT'
     }
 
-    def __init__(self, fmt: str = None, datefmt: str = None, style: str = '%', level_names: _Dict[int, str] = None):
+    def __init__(self, fmt: str = None, datefmt: str = None, style: str = '%', level_names: _Mapping[int, str] = None):
         """
         `level_names` usage:
         >>> import log21
         >>> logger = log21.Logger('MyLogger', log21.DEBUG)
         >>> stream_handler = log21.ColorizingStreamHandler()
         >>> formatter = log21.ColorizingFormatter(fmt='[%(levelname)s] %(message)s',
         ...             level_names={log21.DEBUG: ' ', log21.INFO: '+', log21.WARNING: '-', log21.ERROR: '!',
@@ -55,16 +55,16 @@
     @property
     def level_names(self):
         return self._level_names
 
     @level_names.setter
     def level_names(self, level_names):
         if level_names:
-            if not isinstance(level_names, _Dict):
-                raise TypeError('`level_names` must be a dictionary!')
+            if not isinstance(level_names, _Mapping):
+                raise TypeError('`level_names` must be a Mapping, a dictionary like object!')
             self._level_names = level_names
         else:
             self._level_names = dict()
 
     def format(self, record) -> str:
         record.message = record.getMessage()
         if self.usesTime():
@@ -85,70 +85,70 @@
                 s = s + "\n"
             s = s + self.formatStack(record.stack_info)
         return s
 
 
 class ColorizingFormatter(_Formatter):
     # Default color values
-    level_colors: _Dict[int, _Tuple[str, ...]] = {
+    level_colors: _Mapping[int, _Tuple[str, ...]] = {
         DEBUG: ('lightblue',),
         INFO: ('green',),
         WARNING: ('lightyellow',),
         ERROR: ('light red',),
         CRITICAL: ('background red', 'white'),
         PRINT: ('Cyan',),
         INPUT: ('Magenta',)
     }
     time_color: _Tuple[str, ...] = ('lightblue',)
     name_color = pathname_color = filename_color = module_color = func_name_color = thread_name_color = \
         message_color = tuple()
 
-    def __init__(self, fmt: str = None, datefmt: str = None, style: str = '%', level_names: _Dict[int, str] = None,
-                 level_colors: _Dict[int, _Tuple[str]] = None,
+    def __init__(self, fmt: str = None, datefmt: str = None, style: str = '%', level_names: _Mapping[int, str] = None,
+                 level_colors: _Mapping[int, _Tuple[str]] = None,
                  time_color: _Tuple[str, ...] = None, name_color: _Tuple[str, ...] = None,
                  pathname_color: _Tuple[str, ...] = None, filename_color: _Tuple[str, ...] = None,
                  module_color: _Tuple[str, ...] = None, func_name_color: _Tuple[str, ...] = None,
                  thread_name_color: _Tuple[str, ...] = None, message_color: _Tuple[str, ...] = None):
         super().__init__(fmt=fmt, datefmt=datefmt, style=style, level_names=level_names)
         # Checks and sets colors
         if level_colors:
-            if type(level_colors) is not dict:
-                raise TypeError('`level_colors` must be a dictionary!')
+            if not isinstance(level_colors, _Mapping):
+                raise TypeError('`level_colors` must be a dictionary like object!')
             for level, color in level_colors.items():
                 self.level_colors[level] = (_gc(*color),)
         if time_color:
-            if type(time_color) is not tuple:
+            if not isinstance(time_color, tuple):
                 raise TypeError('`time_color` must be a tuple!')
             self.time_color = time_color
         if name_color:
-            if type(name_color) is not tuple:
+            if not isinstance(name_color, tuple):
                 raise TypeError('`name_color` must be a tuple!')
             self.name_color = name_color
         if pathname_color:
-            if type(pathname_color) is not tuple:
+            if not isinstance(pathname_color, tuple):
                 raise TypeError('`pathname_color` must be a tuple!')
             self.pathname_color = pathname_color
         if filename_color:
-            if type(filename_color) is not tuple:
+            if not isinstance(filename_color, tuple):
                 raise TypeError('`filename_color` must be a tuple!')
             self.filename_color = filename_color
         if module_color:
-            if type(module_color) is not tuple:
+            if not isinstance(module_color, tuple):
                 raise TypeError('`module_color` must be a tuple!')
             self.module_color = module_color
         if func_name_color:
-            if type(func_name_color) is not tuple:
+            if not isinstance(func_name_color, tuple):
                 raise TypeError('`func_name_color` must be a tuple!')
             self.func_name_color = func_name_color
         if thread_name_color:
-            if type(thread_name_color) is not tuple:
+            if not isinstance(thread_name_color, tuple):
                 raise TypeError('`thread_name_color` must be a tuple!')
             self.thread_name_color = thread_name_color
         if message_color:
-            if type(message_color) is not tuple:
+            if not isinstance(message_color, tuple):
                 raise TypeError('`message_color` must be a tuple!')
             self.message_color = message_color
 
     def format(self, record) -> str:
         """
         Colorizes the record and returns the formatted message.
```

### Comparing `log21-2.4.7/log21/Logger.py` & `log21-2.5.0/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/LoggingWindow.py` & `log21-2.5.0/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/Manager.py` & `log21-2.5.0/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/PPrint.py` & `log21-2.5.0/log21/PPrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import re as _re
 import sys as _sys
 import types as _types
 import collections as _collections
 import dataclasses as _dataclasses
 
-from typing import Dict as _Dict, Union as _Union
+from typing import Mapping as _Mapping, Union as _Union
 from pprint import PrettyPrinter as _PrettyPrinter
 
 from log21.Colors import get_colors as _gc
 
 _builtin_scalars = frozenset({str, bytes, bytearray, float, complex, bool, type(None)})
 
 
@@ -61,25 +61,25 @@
         try:
             return self.obj < other.obj
         except TypeError:
             return (str(type(self.obj)), id(self.obj)) < (str(type(other.obj)), id(other.obj))
 
 
 class PrettyPrinter(_PrettyPrinter):
-    signs_colors: _Dict[str, str] = {
+    signs_colors: _Mapping[str, str] = {
         'square-brackets': _gc('LightCyan'),
         'curly-braces': _gc('LightBlue'),
         'parenthesis': _gc('LightGreen'),
         'comma': _gc('LightRed'),
         'colon': _gc('LightRed'),
         '...': _gc('LightMagenta'),
         'data': _gc('Green')
     }
 
-    def __init__(self, indent=1, width=80, depth=None, stream=None, signs_colors: _Dict[str, str] = None, *,
+    def __init__(self, indent=1, width=80, depth=None, stream=None, signs_colors: _Mapping[str, str] = None, *,
                  compact=False, sort_dicts=True, underscore_numbers=False, **kwargs):
         super().__init__(indent=indent, width=width, depth=depth, stream=stream, compact=compact, **kwargs)
         self._depth = depth
         self._indent_per_level = indent
         self._width = width
         if stream is not None:
             self._stream = stream
@@ -558,12 +558,12 @@
 
     def _pprint_user_string(self, obj, stream, indent, allowance, context, level):
         self._format(obj.data, stream, indent, allowance, context, level - 1)
 
     _dispatch[_collections.UserString.__repr__] = _pprint_user_string
 
 
-def pformat(obj, indent=1, width=80, depth=None, signs_colors: _Dict[str, str] = None, *, compact=False,
+def pformat(obj, indent=1, width=80, depth=None, signs_colors: _Mapping[str, str] = None, *, compact=False,
             sort_dicts=True, underscore_numbers=False, **kwargs):
     """Format a Python object into a pretty-printed representation."""
     return PrettyPrinter(indent=indent, width=width, depth=depth, compact=compact, signs_colors=signs_colors,
                          sort_dicts=True, underscore_numbers=False, **kwargs).pformat(obj)
```

### Comparing `log21-2.4.7/log21/ProgressBar.py` & `log21-2.5.0/log21/ProgressBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # log21.ProgressBar.py
 # CodeWriter21
 
 import shutil as _shutil
 
-from typing import Dict as _Dict, Any as _Any
+from typing import Mapping as _Mapping, Any as _Any
 
 import log21 as _log21
 from log21.Logger import Logger as _Logger
 from log21.StreamHandler import ColorizingStreamHandler as _ColorizingStreamHandler
 from log21.Colors import get_colors as _gc
 
 _logger = _Logger('ProgressBar')
@@ -38,15 +38,15 @@
         >>> # Of course, You should try it yourself to see the progress! XD
         >>>
     """
 
     def __init__(self, *args, width: int = None, show_percentage: bool = True, prefix: str = '|', suffix: str = '|',
                  fill: str = '█', empty: str = ' ', format_: str = None, style: str = '%',
                  new_line_when_complete: bool = True, colors: dict = None, no_color: bool = False,
-                 logger: '_log21.Logger' = _logger, additional_variables: _Dict[str, _Any] = None):
+                 logger: '_log21.Logger' = _logger, additional_variables: _Mapping[str, _Any] = None):
         """
         :param args: Prevents the use of positional arguments
         :param width: The width of the progress bar
         :param show_percentage: Whether to show the percentage of the progress
         :param prefix: The prefix of the progress bar
         :param suffix: The suffix of the progress bar
         :param fill: The fill character of the progress bar
@@ -83,16 +83,16 @@
         if len(empty) != 1:
             raise ValueError('`empty` must be a single character')
         if style not in ['%', '{']:
             raise ValueError('`style` must be either `%` or `{`')
         if colors and no_color:
             raise PermissionError('You cannot use `no_color` and `colors` parameters together!')
         if additional_variables:
-            if not isinstance(additional_variables, dict):
-                raise TypeError('`additional_variables` must be a dictionary')
+            if not isinstance(additional_variables, _Mapping):
+                raise TypeError('`additional_variables` must be a dictionary like object.')
             for key, value in additional_variables.items():
                 if not isinstance(key, str):
                     raise TypeError('`additional_variables` keys must be strings')
                 if not isinstance(value, str):
                     additional_variables[key] = str(value)
         else:
             additional_variables = dict()
```

### Comparing `log21-2.4.7/log21/StreamHandler.py` & `log21-2.5.0/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/log21/TreePrint.py` & `log21-2.5.0/log21/TreePrint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # log21.TreePrint.py
 # CodeWriter21
 
-from typing import Union as _Union
+from typing import Union as _Union, Mapping as _Mapping, Sequence as _Sequence
 
 from log21.Colors import get_colors as _gc
 
 
 class TreePrint:
     class Node:
         colors = {
             'branches': _gc('Green'),
             'fruit': _gc('LightMagenta'),
         }
 
-        def __init__(self, value: _Union[str, int], children: list = None, indent: int = 4, colors: dict = None,
-                     mode='-'):
+        def __init__(self, value: _Union[str, int], children: list = None, indent: int = 4,
+                     colors: _Mapping[str, str] = None, mode='-'):
             self.value = str(value)
             if children:
                 self._children = children
             else:
                 self._children = []
             self.indent = indent
             self.colors = self.colors.copy()
@@ -102,64 +102,66 @@
                 for child in self._children:
                     if child.value == value:
                         return child
             if index:
                 return self._children[index]
 
         @staticmethod
-        def add_to(node: 'TreePrint.Node', data: _Union[dict, list, str, int], indent: int = 4, colors: dict = None,
-                   mode='-'):
-            if isinstance(data, dict):
+        def add_to(node: 'TreePrint.Node', data: _Union[_Mapping, _Sequence, str, int], indent: int = 4,
+                   colors: _Mapping[str, str] = None, mode='-'):
+            if isinstance(data, _Mapping):
                 if len(data) == 1:
                     child = TreePrint.Node(list(data.keys())[0], indent=indent, colors=colors, mode=mode)
                     TreePrint.Node.add_to(child, list(data.values())[0], indent=indent, colors=colors, mode=mode)
                     node.add_child(child)
                 else:
                     for key, value in data.items():
                         child = TreePrint.Node(key, indent=indent, colors=colors, mode=mode)
                         TreePrint.Node.add_to(child, value, indent=indent, colors=colors, mode=mode)
                         node.add_child(child)
-            elif isinstance(data, list):
+            elif isinstance(data, _Sequence):
                 for value in data:
-                    if isinstance(value, dict):
+                    if isinstance(value, _Mapping):
                         for key, dict_value in value.items():
                             child = TreePrint.Node(key, indent=indent, colors=colors, mode=mode)
                             TreePrint.Node.add_to(child, dict_value, indent=indent, colors=colors, mode=mode)
                             node.add_child(child)
-                    elif isinstance(value, list):
+                    elif isinstance(value, _Sequence):
                         child = TreePrint.Node('>', indent=indent, colors=colors, mode=mode)
                         TreePrint.Node.add_to(child, value, indent=indent, colors=colors, mode=mode)
                         node.add_child(child)
                     else:
                         child = TreePrint.Node(str(value), indent=indent, colors=colors, mode=mode)
                         node.add_child(child)
             else:
                 child = TreePrint.Node(str(data), indent=indent, colors=colors, mode=mode)
                 node.add_child(child)
 
-    def __init__(self, data: _Union[dict, list, str, int], indent: int = 4, colors: dict = None, mode='-'):
+    def __init__(self, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, 
+                 colors: _Mapping[str, str] = None, mode='-'):
         self.indent = indent
         self.mode = mode
-        if isinstance(data, dict):
+        if isinstance(data, _Mapping):
             if len(data) == 1:
                 self.root = self.Node(list(data.keys())[0], indent=indent, colors=colors)
                 self.add_to_root(list(data.values()), colors=colors)
             else:
                 self.root = self.Node('root', indent=indent, colors=colors)
                 self.add_to_root(data, colors=colors)
-        elif isinstance(data, list):
+        elif isinstance(data, _Sequence):
             self.root = self.Node('root', indent=indent, colors=colors)
             self.add_to_root(data, colors=colors)
         else:
             self.root = self.Node(str(data), indent=indent, colors=colors)
 
-    def add_to_root(self, data: _Union[dict, list, str, int], colors: dict = None):
+    def add_to_root(self, data: _Union[_Mapping, _Sequence, str, int], colors: _Mapping[str, str] = None):
         self.Node.add_to(self.root, data, indent=self.indent, colors=colors, mode=self.mode)
 
     def __str__(self, mode=None):
         if not mode:
             mode = self.mode
         return self.root.__str__(mode=mode)
 
 
-def tree_format(data: _Union[dict, list, str, int], indent: int = 4, mode='-', colors: dict = None):
+def tree_format(data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, mode='-',
+                colors: _Mapping[str, str] = None):
     return str(TreePrint(data, indent=indent, colors=colors, mode=mode))
```

### Comparing `log21-2.4.7/log21/__init__.py` & `log21-2.5.0/log21/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # log21.__init__.py
 # CodeWriter21
 
 import io as _io
 import os as _os
 import logging as _logging
 
-from typing import Union as _Union, Dict as _Dict, Type as _Type
+from typing import Union as _Union, Mapping as _Mapping, Type as _Type, Tuple as _Tuple
 
 import log21.CrashReporter as CrashReporter
 
 from log21.Levels import INPUT, CRITICAL, FATAL, ERROR, WARNING, WARN, INFO, DEBUG, NOTSET
 from log21.Logger import Logger
 from log21.Manager import Manager
 from log21.ProgressBar import ProgressBar
@@ -18,15 +18,15 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.4.7"
+__version__ = "2.5.0"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
@@ -36,41 +36,52 @@
 
 _manager = Manager()
 _logging.setLoggerClass(Logger)
 
 
 def _prepare_formatter(fmt: str = None, style: str = '%', datefmt: str = "%H:%M:%S", show_level: bool = True,
                        show_time: bool = True, colorize_time_and_level: bool = True,
-                       level_names: _Dict[int, str] = None,
+                       level_names: _Mapping[int, str] = None, 
+                       level_colors: _Mapping[int, _Tuple[str, ...]] = None,
                        formatter_class: _Type[_logging.Formatter] = ColorizingFormatter):
     # Prepares a formatting if the fmt was None
     if not fmt:
         style = '%'
         fmt = "%(message)s"
         if show_level:
             fmt = "[%(levelname)s] " + fmt
         if show_time:
             fmt = "[%(asctime)s] " + fmt
         fmt = '\r' + fmt
+
+    if level_colors and not issubclass(formatter_class, ColorizingFormatter):
+        warning('`formatter_class` should be a subclass of ColorizingFormatter when used with level_colors.')
+        warning(f'Using `{formatter_class.__class__.__name__}` might lead to unexpected behaviour!')
+
     # Defines the formatter
-    formatter = formatter_class(fmt, datefmt, style=style)
+    if level_colors:
+        formatter = formatter_class(fmt, datefmt, style=style, level_colors=level_colors)
+    else:
+        formatter = formatter_class(fmt, datefmt, style=style)
+    
     if isinstance(formatter, Formatters._Formatter) and level_names:
         formatter.level_names = level_names
     if not colorize_time_and_level and isinstance(formatter, ColorizingFormatter):
         for key in formatter.level_colors:
             formatter.level_colors[key] = tuple()
         formatter.time_color = tuple()
 
     return formatter
 
 
 def get_logger(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
                show_level: bool = True, colorize_time_and_level: bool = True, fmt: str = None,
                datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-               handle_new_line: bool = True, override=False, level_names: _Dict[int, str] = None,
+               handle_new_line: bool = True, override=False, level_names: _Mapping[int, str] = None,
+               level_colors: _Mapping[int, _Tuple[str, ...]] = None,
                file: _Union[_os.PathLike, str] = None) -> Logger:
     """
     Returns a logging.Logger with colorizing support.
     >>>
     >>> import log21
     >>>
     >>> l = log21.get_logger()
@@ -121,26 +132,28 @@
         %-formatting, :meth:`str.format` (``{}``) formatting or :class:`string.Template` formatting in your format
         string.
     :param colorize_time_and_level: bool = True: Colorizes the time and level using the default colors
     :param handle_carriage_return: bool = True: Adds a line of space characters to remove any text before the CR
     :param handle_new_line: bool = True: Places the NewLine characters at the beginning of the text before everything
         else
     :param override: bool = True: Overrides the logger attributes even if it already exists
-    :param level_names: Dict[int, str] = None: You can specify custom level names.
+    :param level_names: Mapping[int, str] = None: You can specify custom level names.
+    :param level_colors: Mapping[int, Tuple[str, ...]] = None: You can specify custom level colors.
     :param file: Union[os.PathLike, str] = None: The file to log to
     :return: log21.Logger
     """
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
     logger = None
     if name:
         logger = _manager.getLogger(name)
     if (not logger) or override:
         logger = Logger(name, level)
-        formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, colorize_time_and_level, level_names)
+        formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+                                       level_names, level_colors)
 
         # Defines the handler
         handler = ColorizingStreamHandler(handle_carriage_return=handle_carriage_return,
                                           handle_new_line=handle_new_line)
         handler.setFormatter(formatter)
         logger.addHandler(handler)
         _manager.addLogger(name, logger)
@@ -154,15 +167,15 @@
 
     return logger
 
 
 def get_logging_window(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
                        show_level: bool = True, colorize_time_and_level: bool = True, fmt: str = None,
                        datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-                       handle_new_line: bool = True, override=False, level_names: _Dict[int, str] = None,
+                       handle_new_line: bool = True, override=False, level_names: _Mapping[int, str] = None,
                        width: int = 80, height: int = 20, allow_shell: bool = False) -> LoggingWindow:
     """
     Returns a logging window.
 
     >>> # Let's see how it works
     >>> # Imports log21 and time modules
     >>> import log21, time
@@ -203,15 +216,15 @@
         %-formatting, :meth:`str.format` (``{}``) formatting or :class:`string.Template` formatting in your format
         string.
     :param colorize_time_and_level: bool = True: Colorizes the time and level using the default colors
     :param handle_carriage_return: bool = True: Adds a line of space characters to remove any text before the CR
     :param handle_new_line: bool = True: Places the NewLine characters at the beginning of the text before everything
         else
     :param override: bool = True: Overrides the logger attributes even if it already exists
-    :param level_names: Dict[int, str] = None: You can specify custom level names.
+    :param level_names: Mapping[int, str] = None: You can specify custom level names.
     :param width: int = 80: The width of the window
     :param height: int = 20: The height of the window
     :param allow_shell: bool = False: Allow the user to use the shell
     :return: log21.LoggingWindow
     """
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
@@ -245,25 +258,25 @@
 
 
 def getpass(*msg, args: tuple = (), end='', **kwargs):
     logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
     return logger.getpass(*msg, args=args, end=end, **kwargs)
 
 
-def pprint(obj, indent=1, width=80, depth=None, signs_colors: _Dict[str, str] = None, *, sort_dicts=True,
+def pprint(obj, indent=1, width=80, depth=None, signs_colors: _Mapping[str, str] = None, *, sort_dicts=True,
            underscore_numbers=False, compact=False, end='\033[0m\n', **kwargs):
     logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
     logger.print(pformat(obj=obj, indent=indent, width=width, depth=depth, signs_colors=signs_colors, compact=compact,
                          sort_dicts=sort_dicts, underscore_numbers=underscore_numbers), end=end, **kwargs)
 
 
 pretty_print = pprint
 
 
-def tree_print(obj, indent: int = 4, mode='-', colors: _Dict[str, str] = None, end='\033[0m\n', **kwargs):
+def tree_print(obj, indent: int = 4, mode='-', colors: _Mapping[str, str] = None, end='\033[0m\n', **kwargs):
     logger = get_logger('log21.tree_print', level=DEBUG, show_time=False, show_level=False)
     logger.print(tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs)
 
 
 tprint = tree_print
 
 root = Logger('root-logger', INFO)
```

### Comparing `log21-2.4.7/log21.egg-info/PKG-INFO` & `log21-2.5.0/log21.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.7
+Version: 2.5.0
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
@@ -69,22 +69,20 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.7
+### 2.5.0
 
-Added `extra_values` argument to `CrashReporter.Formatter` which will let you pass extra static or dynamic values to the
-report formatter.
-They can be used in the format string. For dynamic values you can pass a function that takes no
-arguments as the value.
+Added `level_colors` argument to `log21.get_logger` function with will be passed to the formatter and allows
+user to set custom level colors while making a new logger.
 
-[Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
+[Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
 
 ```python3
 import log21
```

### Comparing `log21-2.4.7/log21.egg-info/SOURCES.txt` & `log21-2.5.0/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.7/setup.py` & `log21-2.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 DESCRIPTION = 'A simple logging package that helps you log colorized messages in Windows console.'
-VERSION = '2.4.7'
+VERSION = '2.5.0'
 
 setup(
     name='log21',
     version=VERSION,
     url='https://github.com/MPCodeWriter21/log21',
     author='CodeWriter21(Mehrad Pooryoussof)',
     author_email='<CodeWriter21@gmail.com>',
```

