# Comparing `tmp/calendar-view-2.2.0.tar.gz` & `tmp/calendar-view-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar-view-2.2.0.tar", last modified: Tue Apr  4 17:02:49 2023, max compression
+gzip compressed data, was "calendar-view-2.3.0.tar", last modified: Thu Jun  8 20:39:24 2023, max compression
```

## Comparing `calendar-view-2.2.0.tar` & `calendar-view-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-04-04 17:02:25.000000 calendar-view-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-04 17:02:25.000000 calendar-view-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-04 17:02:49.866993 calendar-view-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-04-04 17:02:25.000000 calendar-view-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.862993 calendar-view-2.2.0/calendar_view/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.862993 calendar-view-2.2.0/calendar_view/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/calendar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.862993 calendar-view-2.2.0/calendar_view/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.862993 calendar-view-2.2.0/calendar_view/config/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/config/__pycache__/style.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/config/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/config/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/calendar_view/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/calendar_view/core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/core/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/core/__pycache__/data.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/core/__pycache__/event.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/core/__pycache__/time_utils.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    18001 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/calendar_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/calendar_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/round_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/calendar_view/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/calendar_view/resources/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/resources/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/calendar_view/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/resources/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   168260 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/resources/fonts/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:25.000000 calendar-view-2.2.0/calendar_view/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/calendar_view/resources/fonts/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-04 17:02:42.000000 calendar-view-2.2.0/calendar_view/resources/fonts/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.862993 calendar-view-2.2.0/calendar_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-04-04 17:02:49.000000 calendar-view-2.2.0/calendar_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-04 17:02:49.000000 calendar-view-2.2.0/calendar_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 17:02:49.000000 calendar-view-2.2.0/calendar_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-04 17:02:49.000000 calendar-view-2.2.0/calendar_view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 17:02:49.000000 calendar-view-2.2.0/calendar_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 17:02:49.866993 calendar-view-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-04 17:02:25.000000 calendar-view-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:02:49.866993 calendar-view-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-04 17:02:25.000000 calendar-view-2.2.0/tests/test_calendar_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-04 17:02:25.000000 calendar-view-2.2.0/tests/test_time_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-08 20:38:59.000000 calendar-view-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 20:38:59.000000 calendar-view-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-08 20:39:24.209219 calendar-view-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-08 20:38:59.000000 calendar-view-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view/config/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/config/__pycache__/style.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/config/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/config/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/data.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/event.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/time_utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/calendar_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/calendar_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/round_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/resources/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   168260 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:38:59.000000 calendar-view-2.3.0/calendar_view/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/calendar_view/resources/fonts/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-08 20:39:17.000000 calendar-view-2.3.0/calendar_view/resources/fonts/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.205219 calendar-view-2.3.0/calendar_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 20:39:24.000000 calendar-view-2.3.0/calendar_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:39:24.209219 calendar-view-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-08 20:38:59.000000 calendar-view-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:39:24.209219 calendar-view-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-08 20:38:59.000000 calendar-view-2.3.0/tests/test_calendar_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-08 20:38:59.000000 calendar-view-2.3.0/tests/test_time_utils.py
```

### Comparing `calendar-view-2.2.0/LICENSE` & `calendar-view-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/PKG-INFO` & `calendar-view-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: calendar-view
-Version: 2.2.0
+Version: 2.3.0
 Summary: Library provides a graphical view of the calendar.
-Home-page: https://github.com/sakhnevych/CalendarView
+Home-page: https://github.com/sakhnevych/calendar-view
 Author: Oleksandr Sakhnevych, Daniil Limariev
 Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -17,15 +17,15 @@
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/calendar-view.svg
    :target: https://pypi.org/project/calendar-view/
    :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/dm/calendar-view
-   :target: https://pypi.org/project/calendar-view/
+   :target: https://pypistats.org/packages/calendar-view
    :alt: PyPi Package Monthly Download
 
 .. image:: https://img.shields.io/pypi/l/calendar-view.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT License
 
 
@@ -34,14 +34,32 @@
 =============
 
 Library provides a graphical view of the calendar. View, title and events can be easily configured.
 
 The output in ``*.png`` file.
 
 
+Installation
+============
+
+Install the package using PyPI:
+
+.. code-block:: bash
+
+    pip install calendar-view
+
+
+or directly from the repository:
+
+.. code-block:: bash
+
+    pip install git+https://github.com/sakhnevych/calendar-view.git
+
+
+
 Input parameters
 ================
 
 Configuration
 -------------
 
 Configuration for all views can be done using ``CalendarConfig`` class.
@@ -132,15 +150,15 @@
 * 21/06
 
 
 Styles
 ------
 
 You can change styles by setting the required parameter. See the full list of parameters in the file:
-`style.py <https://github.com/sakhnevych/CalendarView/blob/master/calendar_view/config/style.py>`_
+`style.py <https://github.com/sakhnevych/calendar-view/blob/master/calendar_view/config/style.py>`_
 
 
 Example:
 
 .. code-block:: python
 
     from calendar_view.config import style
@@ -169,16 +187,16 @@
     calendar.add_event(day_of_week=5, start='09:00', end='12:00', style=EventStyles.RED)
     calendar.add_event(day_of_week=5, start='10:00', end='13:00', style=EventStyles.BLUE)
     calendar.add_event(day_of_week=6, start='15:00', end='18:00')
     calendar.save("simple_view.png")
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/simple_view.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/simple_view.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/simple_view.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/simple_view.png
     :width: 600 px
     :align: center
 
 2. Configuration and specific dates
 -----------------------------------
 
 View for one script. Configuration objects and events with specific dates are used.
@@ -211,16 +229,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("sprint_23.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/sprint_23.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/sprint_23.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/sprint_23.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/sprint_23.png
     :width: 600 px
     :align: center
 
 
 3. Legend view
 --------------
 
@@ -261,16 +279,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("yoga_class.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/yoga_class.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/yoga_class.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/yoga_class.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/yoga_class.png
     :width: 600 px
     :align: center
 
 
 4. Event notes and style
 ------------------------
 
@@ -318,16 +336,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("massage.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/massage.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/massage.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/massage.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/massage.png
     :width: 600 px
     :align: center
 
 License
 =======
 
-CalendarView is licensed under a MIT license. Please see the `LICENSE <LICENSE.rst>`_ file for details.
+calendar-view is licensed under a MIT license. Please see the `LICENSE <LICENSE.rst>`_ file for details.
```

### Comparing `calendar-view-2.2.0/README.rst` & `calendar-view-2.3.0/calendar_view.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,31 @@
+Metadata-Version: 2.1
+Name: calendar-view
+Version: 2.3.0
+Summary: Library provides a graphical view of the calendar.
+Home-page: https://github.com/sakhnevych/calendar-view
+Author: Oleksandr Sakhnevych, Daniil Limariev
+Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 .. image:: https://img.shields.io/pypi/v/calendar-view.svg
    :target: https://pypi.org/project/calendar-view/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/calendar-view.svg
    :target: https://pypi.org/project/calendar-view/
    :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/dm/calendar-view
-   :target: https://pypi.org/project/calendar-view/
+   :target: https://pypistats.org/packages/calendar-view
    :alt: PyPi Package Monthly Download
 
 .. image:: https://img.shields.io/pypi/l/calendar-view.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT License
 
 
@@ -20,14 +34,32 @@
 =============
 
 Library provides a graphical view of the calendar. View, title and events can be easily configured.
 
 The output in ``*.png`` file.
 
 
+Installation
+============
+
+Install the package using PyPI:
+
+.. code-block:: bash
+
+    pip install calendar-view
+
+
+or directly from the repository:
+
+.. code-block:: bash
+
+    pip install git+https://github.com/sakhnevych/calendar-view.git
+
+
+
 Input parameters
 ================
 
 Configuration
 -------------
 
 Configuration for all views can be done using ``CalendarConfig`` class.
@@ -118,15 +150,15 @@
 * 21/06
 
 
 Styles
 ------
 
 You can change styles by setting the required parameter. See the full list of parameters in the file:
-`style.py <https://github.com/sakhnevych/CalendarView/blob/master/calendar_view/config/style.py>`_
+`style.py <https://github.com/sakhnevych/calendar-view/blob/master/calendar_view/config/style.py>`_
 
 
 Example:
 
 .. code-block:: python
 
     from calendar_view.config import style
@@ -155,16 +187,16 @@
     calendar.add_event(day_of_week=5, start='09:00', end='12:00', style=EventStyles.RED)
     calendar.add_event(day_of_week=5, start='10:00', end='13:00', style=EventStyles.BLUE)
     calendar.add_event(day_of_week=6, start='15:00', end='18:00')
     calendar.save("simple_view.png")
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/simple_view.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/simple_view.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/simple_view.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/simple_view.png
     :width: 600 px
     :align: center
 
 2. Configuration and specific dates
 -----------------------------------
 
 View for one script. Configuration objects and events with specific dates are used.
@@ -197,16 +229,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("sprint_23.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/sprint_23.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/sprint_23.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/sprint_23.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/sprint_23.png
     :width: 600 px
     :align: center
 
 
 3. Legend view
 --------------
 
@@ -247,16 +279,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("yoga_class.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/yoga_class.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/yoga_class.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/yoga_class.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/yoga_class.png
     :width: 600 px
     :align: center
 
 
 4. Event notes and style
 ------------------------
 
@@ -304,16 +336,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("massage.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/massage.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/massage.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/massage.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/massage.png
     :width: 600 px
     :align: center
 
 License
 =======
 
-CalendarView is licensed under a MIT license. Please see the `LICENSE <LICENSE.rst>`_ file for details.
+calendar-view is licensed under a MIT license. Please see the `LICENSE <LICENSE.rst>`_ file for details.
```

### Comparing `calendar-view-2.2.0/calendar_view/calendar.py` & `calendar-view-2.3.0/calendar_view/calendar.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/config/__pycache__/style.cpython-311.pyc` & `calendar-view-2.3.0/calendar_view/config/__pycache__/style.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21582c64 (Tue Apr  4 17:02:25 2023 UTC)
+moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
 files sz: 1356
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `calendar-view-2.2.0/calendar_view/config/i18n.py` & `calendar-view-2.3.0/calendar_view/config/i18n.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/config/style.py` & `calendar-view-2.3.0/calendar_view/config/style.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/__pycache__/config.cpython-311.pyc` & `calendar-view-2.3.0/calendar_view/core/__pycache__/config.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21582c64 (Tue Apr  4 17:02:25 2023 UTC)
+moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
 files sz: 3558
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `calendar-view-2.2.0/calendar_view/core/__pycache__/data.cpython-311.pyc` & `calendar-view-2.3.0/calendar_view/core/__pycache__/data.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21582c64 (Tue Apr  4 17:02:25 2023 UTC)
+moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
 files sz: 1675
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `calendar-view-2.2.0/calendar_view/core/__pycache__/event.cpython-311.pyc` & `calendar-view-2.3.0/calendar_view/core/__pycache__/event.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21582c64 (Tue Apr  4 17:02:25 2023 UTC)
+moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
 files sz: 8898
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `calendar-view-2.2.0/calendar_view/core/__pycache__/time_utils.cpython-311.pyc` & `calendar-view-2.3.0/calendar_view/core/__pycache__/time_utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21582c64 (Tue Apr  4 17:02:25 2023 UTC)
+moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
 files sz: 5426
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `calendar-view-2.2.0/calendar_view/core/__pycache__/utils.cpython-311.pyc` & `calendar-view-2.3.0/calendar_view/core/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x21582c64 (Tue Apr  4 17:02:25 2023 UTC)
+moddate:  0x633c8264 (Thu Jun  8 20:38:59 2023 UTC)
 files sz: 1298
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `calendar-view-2.2.0/calendar_view/core/calendar_events.py` & `calendar-view-2.3.0/calendar_view/core/calendar_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                     to: datetime = datetime.combine(next_date, time(0, 0))
                 elif single_date == end_date:
                     fr: datetime = datetime.combine(single_date, time(0, 0))
                     to: datetime = datetime.combine(single_date, event.end_time)
                 else:
                     fr: datetime = datetime.combine(single_date, time(0, 0))
                     to: datetime = datetime.combine(next_date, time(0, 0))
-                self.__do_add_event(Event(title=event.title, style=event.style, start=fr, end=to))
+                self.__do_add_event(Event(title=event.title, style=event.style, start=fr, end=to, notes=event.notes))
 
     def __do_add_event(self, event: Event) -> None:
         data.validate_event(event, self.config)
         self.events.append(event)
         logging.debug(f'Added internal event: {event}')
 
         # if legend is needed
```

### Comparing `calendar-view-2.2.0/calendar_view/core/calendar_grid.py` & `calendar-view-2.3.0/calendar_view/core/calendar_grid.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/config.py` & `calendar-view-2.3.0/calendar_view/core/config.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/data.py` & `calendar-view-2.3.0/calendar_view/core/data.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/event.py` & `calendar-view-2.3.0/calendar_view/core/event.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/round_rectangle.py` & `calendar-view-2.3.0/calendar_view/core/round_rectangle.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/time_utils.py` & `calendar-view-2.3.0/calendar_view/core/time_utils.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/core/utils.py` & `calendar-view-2.3.0/calendar_view/core/utils.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/resources/fonts/LICENSE.txt` & `calendar-view-2.3.0/calendar_view/resources/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view/resources/fonts/Roboto-Regular.ttf` & `calendar-view-2.3.0/calendar_view/resources/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/calendar_view.egg-info/PKG-INFO` & `calendar-view-2.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,17 @@
-Metadata-Version: 2.1
-Name: calendar-view
-Version: 2.2.0
-Summary: Library provides a graphical view of the calendar.
-Home-page: https://github.com/sakhnevych/CalendarView
-Author: Oleksandr Sakhnevych, Daniil Limariev
-Author-email: o.sakhnevych@gmail.com, danillim02102003@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. image:: https://img.shields.io/pypi/v/calendar-view.svg
    :target: https://pypi.org/project/calendar-view/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/calendar-view.svg
    :target: https://pypi.org/project/calendar-view/
    :alt: Supported Python versions
 
 .. image:: https://img.shields.io/pypi/dm/calendar-view
-   :target: https://pypi.org/project/calendar-view/
+   :target: https://pypistats.org/packages/calendar-view
    :alt: PyPi Package Monthly Download
 
 .. image:: https://img.shields.io/pypi/l/calendar-view.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT License
 
 
@@ -34,14 +20,32 @@
 =============
 
 Library provides a graphical view of the calendar. View, title and events can be easily configured.
 
 The output in ``*.png`` file.
 
 
+Installation
+============
+
+Install the package using PyPI:
+
+.. code-block:: bash
+
+    pip install calendar-view
+
+
+or directly from the repository:
+
+.. code-block:: bash
+
+    pip install git+https://github.com/sakhnevych/calendar-view.git
+
+
+
 Input parameters
 ================
 
 Configuration
 -------------
 
 Configuration for all views can be done using ``CalendarConfig`` class.
@@ -132,15 +136,15 @@
 * 21/06
 
 
 Styles
 ------
 
 You can change styles by setting the required parameter. See the full list of parameters in the file:
-`style.py <https://github.com/sakhnevych/CalendarView/blob/master/calendar_view/config/style.py>`_
+`style.py <https://github.com/sakhnevych/calendar-view/blob/master/calendar_view/config/style.py>`_
 
 
 Example:
 
 .. code-block:: python
 
     from calendar_view.config import style
@@ -169,16 +173,16 @@
     calendar.add_event(day_of_week=5, start='09:00', end='12:00', style=EventStyles.RED)
     calendar.add_event(day_of_week=5, start='10:00', end='13:00', style=EventStyles.BLUE)
     calendar.add_event(day_of_week=6, start='15:00', end='18:00')
     calendar.save("simple_view.png")
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/simple_view.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/simple_view.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/simple_view.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/simple_view.png
     :width: 600 px
     :align: center
 
 2. Configuration and specific dates
 -----------------------------------
 
 View for one script. Configuration objects and events with specific dates are used.
@@ -211,16 +215,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("sprint_23.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/sprint_23.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/sprint_23.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/sprint_23.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/sprint_23.png
     :width: 600 px
     :align: center
 
 
 3. Legend view
 --------------
 
@@ -261,16 +265,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("yoga_class.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/yoga_class.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/yoga_class.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/yoga_class.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/yoga_class.png
     :width: 600 px
     :align: center
 
 
 4. Event notes and style
 ------------------------
 
@@ -318,16 +322,16 @@
     calendar = Calendar.build(config)
     calendar.add_events(events)
     calendar.save("massage.png")
 
 
 Output:
 
-.. image:: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/massage.png
-    :target: https://raw.githubusercontent.com/sakhnevych/CalendarView/master/docs/massage.png
+.. image:: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/massage.png
+    :target: https://raw.githubusercontent.com/sakhnevych/calendar-view/master/docs/massage.png
     :width: 600 px
     :align: center
 
 License
 =======
 
-CalendarView is licensed under a MIT license. Please see the `LICENSE <LICENSE.rst>`_ file for details.
+calendar-view is licensed under a MIT license. Please see the `LICENSE <LICENSE.rst>`_ file for details.
```

### Comparing `calendar-view-2.2.0/calendar_view.egg-info/SOURCES.txt` & `calendar-view-2.3.0/calendar_view.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/setup.py` & `calendar-view-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.rst", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="calendar-view",
-    version="2.2.0",
+    version="2.3.0",
     author="Oleksandr Sakhnevych, Daniil Limariev",
     author_email="o.sakhnevych@gmail.com, danillim02102003@gmail.com",
     description="Library provides a graphical view of the calendar.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    url="https://github.com/sakhnevych/CalendarView",
+    url="https://github.com/sakhnevych/calendar-view",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `calendar-view-2.2.0/tests/test_calendar_config.py` & `calendar-view-2.3.0/tests/test_calendar_config.py`

 * *Files identical despite different names*

### Comparing `calendar-view-2.2.0/tests/test_time_utils.py` & `calendar-view-2.3.0/tests/test_time_utils.py`

 * *Files identical despite different names*

