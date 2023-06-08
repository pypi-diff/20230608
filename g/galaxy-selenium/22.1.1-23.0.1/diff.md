# Comparing `tmp/galaxy-selenium-22.1.1.tar.gz` & `tmp/galaxy-selenium-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-selenium-22.1.1.tar", last modified: Mon Aug 22 19:45:57 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/selenium/dist/.tmp-qu3m6_t1/galaxy-selenium-23.0.1.tar", last modified: Thu Jun  8 17:41:57 2023, max compression
```

## Comparing `galaxy-selenium-22.1.1.tar` & `galaxy-selenium-23.0.1.tar`

### file list

```diff
@@ -1,46 +1,36 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.113846 galaxy-selenium-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      332 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-selenium-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       57 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1670 2022-08-22 19:45:57.114060 galaxy-selenium-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      304 2022-03-24 19:47:11.000000 galaxy-selenium-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.107228 galaxy-selenium-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      434 2022-08-22 19:45:29.000000 galaxy-selenium-22.1.1/galaxy/project_galaxy_selenium.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.110465 galaxy-selenium-22.1.1/galaxy/selenium/
--rw-r--r--   0 mvandenb   (501) staff       (20)      269 2022-03-24 19:47:10.000000 galaxy-selenium-22.1.1/galaxy/selenium/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2737 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/cli.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6988 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/components.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2631 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/context.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      312 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/data.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5310 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/driver_factory.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8091 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/has_driver.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      355 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/jupyter_context.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    82353 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/navigates_galaxy.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    32063 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/navigation.yml
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.110901 galaxy-selenium-22.1.1/galaxy/selenium/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:10.000000 galaxy-selenium-22.1.1/galaxy/selenium/scripts/__init__.py
--rwxr-xr-x   0 mvandenb   (501) staff       (20)     1434 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/scripts/dump_tour.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3977 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/sizzle.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3420 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/smart_components.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.111332 galaxy-selenium-22.1.1/galaxy/selenium/toolbox/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:10.000000 galaxy-selenium-22.1.1/galaxy/selenium/toolbox/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      227 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/galaxy/selenium/toolbox/filters.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.112961 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1670 2022-08-22 19:45:56.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1047 2022-08-22 19:45:57.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:56.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       87 2022-08-22 19:45:56.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:56.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       21 2022-08-22 19:45:56.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:56.000000 galaxy-selenium-22.1.1/galaxy_selenium.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       21 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:57.113672 galaxy-selenium-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:57.119453 galaxy-selenium-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2879 2022-08-22 19:45:28.000000 galaxy-selenium-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-selenium-22.1.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-selenium-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/has_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/jupyter_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88548 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/navigates_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy/selenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/scripts/dump_tour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/sizzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/smart_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy/selenium/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/toolbox/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-selenium-22.1.1/LICENSE` & `galaxy-selenium-23.0.1/LICENSE`

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

### Comparing `galaxy-selenium-22.1.1/PKG-INFO` & `galaxy-selenium-23.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 22.1.1
-Summary: Galaxy Selenium Interaction Framework
+Version: 23.0.1
+Summary: Galaxy Selenium interaction framework
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
 
 
 .. image:: https://badge.fury.io/py/galaxy-selenium.svg
    :target: https://pypi.org/project/galaxy-selenium/
 
 
 
 Overview
 --------
 
 The Galaxy_ selenium framework.
 
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
-20.9.1.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
+
 
+============
+Enhancements
+============
 
+* Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
 
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
-
-
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/cli.py` & `galaxy-selenium-23.0.1/galaxy/selenium/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 from .navigates_galaxy import NavigatesGalaxy
 
 
 def add_selenium_arguments(parser):
     """Add common selenium arguments for argparse driver utility."""
 
     parser.add_argument(
-        '--selenium-browser',
+        "--selenium-browser",
         default="auto",
         help=BROWSER_DESCRIPTION,
     )
     parser.add_argument(
-        '--selenium-headless',
+        "--selenium-headless",
         default=False,
         action="store_true",
         help=HEADLESS_DESCRIPTION,
     )
     parser.add_argument(
-        '--selenium-remote',
+        "--selenium-remote",
         default=False,
         action="store_true",
         help=REMOTE_DESCRIPTION,
     )
     parser.add_argument(
-        '--selenium-remote-host',
+        "--selenium-remote-host",
         default="127.0.0.1",
         help=REMOTE_HOST_DESCRIPTION,
     )
     parser.add_argument(
-        '--selenium-remote-port',
+        "--selenium-remote-port",
         default="4444",
         help=REMOTE_PORT_DESCRIPTION,
     )
     parser.add_argument(
-        '--galaxy_url',
+        "--galaxy_url",
         default="http://127.0.0.1:8080/",
         help=GALAXY_URL_DESCRIPTION,
     )
 
     return parser
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/context.py` & `galaxy-selenium-23.0.1/galaxy/selenium/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from abc import abstractmethod
 from typing import Optional
+from urllib.parse import urljoin
 
 import yaml
-from six.moves.urllib.parse import urljoin
 
 from .driver_factory import ConfiguredDriver
 from .navigates_galaxy import NavigatesGalaxy
 
 
 class GalaxySeleniumContext(NavigatesGalaxy):
     url: str
     target_url_from_selenium: str
+    configured_driver: ConfiguredDriver
 
     def build_url(self, url: str, for_selenium: bool = True) -> str:
         if for_selenium:
             base = self.target_url_from_selenium
         else:
             base = self.url
         return urljoin(base, url)
@@ -35,14 +36,20 @@
         target = self._screenshot_path(label)
         if target is None:
             return
 
         self.driver.save_screenshot(target)
         return target
 
+    def screenshot_if(self, label: Optional[str]) -> Optional[str]:
+        target = None
+        if label:
+            target = self.screenshot(label)
+        return target
+
     @abstractmethod
     def _screenshot_path(self, label: str, extension=".png") -> str:
         """Path to store screenshots in."""
 
 
 class GalaxySeleniumContextImpl(GalaxySeleniumContext):
     """Minimal, simplified GalaxySeleniumContext useful outside the context of test cases.
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/driver_factory.py` & `galaxy-selenium-23.0.1/galaxy/selenium/driver_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     Display = None
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver.remote.webdriver import WebDriver
 
-logger = logging.getLogger('selenium.webdriver.remote.remote_connection')
+logger = logging.getLogger("selenium.webdriver.remote.remote_connection")
 logger.setLevel(logging.WARNING)
 
 DEFAULT_BROWSER = "auto"
-DEFAULT_DOWNLOAD_PATH = '/tmp/'
+DEFAULT_DOWNLOAD_PATH = "/tmp/"
 LOGGING_PREFS = {
     "browser": "ALL",
 }
 DEFAULT_SELENIUM_BROWSER = "auto"
 DEFAULT_SELENIUM_REMOTE = False
 DEFAULT_SELENIUM_REMOTE_PORT = "4444"
 DEFAULT_SELENIUM_REMOTE_HOST = "127.0.0.1"
 DEFAULT_WINDOW_WIDTH = 1280
 DEFAULT_WINDOW_HEIGHT = 1000
-VALID_LOCAL_BROWSERS = ["CHROME", "FIREFOX", "OPERA"]
+VALID_LOCAL_BROWSERS = ["CHROME", "FIREFOX"]
 
 
 class ConfiguredDriver:
     driver: WebDriver
 
     def __init__(
         self,
@@ -83,50 +83,44 @@
 def get_local_driver(browser=DEFAULT_BROWSER, headless=False) -> WebDriver:
     browser = get_local_browser(browser)
     if browser not in VALID_LOCAL_BROWSERS:
         raise AssertionError(f"{browser} not in VALID_LOCAL_BROWSERS ({VALID_LOCAL_BROWSERS})")
     driver_to_class = {
         "CHROME": webdriver.Chrome,
         "FIREFOX": webdriver.Firefox,
-        "OPERA": webdriver.Opera,
     }
     driver_class = driver_to_class[browser]
-    if browser == 'CHROME':
+    if browser == "CHROME":
         options = ChromeOptions()
         if headless:
-            options.add_argument('--headless')
-        prefs = {'download.default_directory': DEFAULT_DOWNLOAD_PATH}
-        options.add_experimental_option('prefs', prefs)
+            options.add_argument("--headless")
+        prefs = {"download.default_directory": DEFAULT_DOWNLOAD_PATH}
+        options.add_experimental_option("prefs", prefs)
         return driver_class(desired_capabilities={"loggingPrefs": LOGGING_PREFS}, chrome_options=options)
-    elif browser == 'FIREFOX':
+    elif browser == "FIREFOX":
         fp = webdriver.FirefoxProfile()
-        fp.set_preference('network.proxy.type', 2)
-        fp.set_preference('network.proxy.autoconfig_url',
-                          "http://127.0.0.1:9675")
-        fp.set_preference('browser.download.folderList', 2)
-        fp.set_preference('browser.download.dir', DEFAULT_DOWNLOAD_PATH)
-        fp.set_preference("browser.helperApps.neverAsk.saveToDisk", 'application/octet-stream')
+        fp.set_preference("network.proxy.type", 2)
+        fp.set_preference("network.proxy.autoconfig_url", "http://127.0.0.1:9675")
+        fp.set_preference("browser.download.folderList", 2)
+        fp.set_preference("browser.download.dir", DEFAULT_DOWNLOAD_PATH)
+        fp.set_preference("browser.helperApps.neverAsk.saveToDisk", "application/octet-stream")
         return driver_class(firefox_profile=fp)
 
     else:
         return driver_class(desired_capabilities={"loggingPrefs": LOGGING_PREFS})
 
 
-def get_remote_driver(
-    host,
-    port,
-    browser=DEFAULT_BROWSER
-) -> WebDriver:
+def get_remote_driver(host, port, browser=DEFAULT_BROWSER) -> WebDriver:
     # docker run -d -p 4444:4444 -v /dev/shm:/dev/shm selenium/standalone-chrome:3.0.1-aluminum
     if browser == "auto":
         browser = "CHROME"
-    assert browser in ["CHROME", "EDGE", "ANDROID", "FIREFOX", "INTERNETEXPLORER", "IPAD", "IPHONE", "OPERA", "SAFARI"]
+    assert browser in ["CHROME", "EDGE", "ANDROID", "FIREFOX", "INTERNETEXPLORER", "IPAD", "IPHONE", "SAFARI"]
     desired_capabilities = getattr(DesiredCapabilities, browser)
     desired_capabilities["loggingPrefs"] = LOGGING_PREFS
-    executor = f'http://{host}:{port}/wd/hub'
+    executor = f"http://{host}:{port}/wd/hub"
     driver = webdriver.Remote(
         command_executor=executor,
         desired_capabilities=desired_capabilities,
     )
     return driver
 
 
@@ -140,15 +134,14 @@
         display.start()
         return display
     else:
         return NoopDisplay()
 
 
 class NoopDisplay:
-
     def stop(self):
         """No-op stop for consistent use with pyvirtualdisplay Display class."""
 
 
 # Purposely copied from galaxy.util - just use galaxy.util if we decide
 # galaxy_selenium should definitely depend on Galaxy/galaxy-lib.
 def _which(file):
@@ -157,13 +150,13 @@
         if os.path.exists(f"{path}/{file}"):
             return f"{path}/{file}"
 
     return None
 
 
 __all__ = (
-    'ConfiguredDriver',
-    'get_local_driver',
-    'get_remote_driver',
-    'is_virtual_display_available',
-    'virtual_display_if_enabled',
+    "ConfiguredDriver",
+    "get_local_driver",
+    "get_remote_driver",
+    "is_virtual_display_available",
+    "virtual_display_if_enabled",
 )
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/navigates_galaxy.py` & `galaxy-selenium-23.0.1/galaxy/selenium/navigates_galaxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-"""A mixing that extends a HasDriver class with Galaxy-specific utilities.
+"""A mixin that extends a HasDriver class with Galaxy-specific utilities.
 
 Implementer must provide a self.build_url method to target Galaxy.
 """
 
 import collections
 import contextlib
 import random
 import string
 import time
 from abc import abstractmethod
-from functools import partial, wraps
-from typing import cast, Union
+from functools import (
+    partial,
+    wraps,
+)
+from typing import (
+    Any,
+    cast,
+    Dict,
+    Optional,
+    Union,
+)
 
 import requests
 import yaml
-from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 
+from galaxy.navigation.components import (
+    Component,
+    HasText,
+)
+from galaxy.navigation.data import load_root_component
 from galaxy.util import DEFAULT_SOCKET_TIMEOUT
 from . import sizzle
-from .components import Component, HasText
-from .data import (
-    load_root_component,
-)
 from .has_driver import (
+    exception_indicates_click_intercepted,
     exception_indicates_not_clickable,
     exception_indicates_stale_element,
     HasDriver,
     SeleniumTimeoutException,
 )
 from .smart_components import SmartComponent
 
 # Test case data
-DEFAULT_PASSWORD = '123456'
+DEFAULT_PASSWORD = "123456"
 
-RETRY_DURING_TRANSITIONS_SLEEP_DEFAULT = .1
+RETRY_DURING_TRANSITIONS_SLEEP_DEFAULT = 0.1
 RETRY_DURING_TRANSITIONS_ATTEMPTS_DEFAULT = 10
 
 GALAXY_MAIN_FRAME_ID = "galaxy_main"
 
 WaitType = collections.namedtuple("WaitType", ["name", "default_length"])
 
 
@@ -54,27 +65,26 @@
     # Creating a new history and loading it into the panel.
     DATABASE_OPERATION = WaitType("database_operation", 10)
     # Wait time for jobs to complete in default environment.
     JOB_COMPLETION = WaitType("job_completion", 30)
     # Wait time for a GIE to spawn.
     GIE_SPAWN = WaitType("gie_spawn", 30)
     # Wait time for toolshed search
-    SHED_SEARCH = WaitType('shed_search', 30)
+    SHED_SEARCH = WaitType("shed_search", 30)
     # Wait time for repository installation
-    REPO_INSTALL = WaitType('repo_install', 60)
-    # Beta history Polling Duration
+    REPO_INSTALL = WaitType("repo_install", 60)
+    # History Polling Duration
     HISTORY_POLL = WaitType("history_poll", 3)
 
 
 # Choose a moderate wait type for operations that don't specify a type.
 DEFAULT_WAIT_TYPE = WAIT_TYPES.DATABASE_OPERATION
 
 
 class NullTourCallback:
-
     def handle_step(self, step, step_index):
         pass
 
 
 def exception_seems_to_indicate_transition(e):
     """True if exception seems to indicate the page state is transitioning.
 
@@ -85,18 +95,27 @@
     cause of the exception. The methods that follow use it to allow retrying actions during
     transitions.
 
     Currently the two kinds of exceptions that we say may indicate a transition are
     StaleElement exceptions (a DOM element grabbed at one step is no longer available)
     and "not clickable" exceptions (so perhaps a popup modal is blocking a click).
     """
-    return exception_indicates_stale_element(e) or exception_indicates_not_clickable(e)
+    return (
+        exception_indicates_stale_element(e)
+        or exception_indicates_not_clickable(e)
+        or exception_indicates_click_intercepted(e)
+    )
 
 
-def retry_call_during_transitions(f, attempts=RETRY_DURING_TRANSITIONS_ATTEMPTS_DEFAULT, sleep=RETRY_DURING_TRANSITIONS_SLEEP_DEFAULT, exception_check=exception_seems_to_indicate_transition):
+def retry_call_during_transitions(
+    f,
+    attempts=RETRY_DURING_TRANSITIONS_ATTEMPTS_DEFAULT,
+    sleep=RETRY_DURING_TRANSITIONS_SLEEP_DEFAULT,
+    exception_check=exception_seems_to_indicate_transition,
+):
     previous_attempts = 0
     while True:
         try:
             return f()
         except Exception as e:
             if previous_attempts > attempts:
                 raise
@@ -104,37 +123,40 @@
             if not exception_check(e):
                 raise
 
             time.sleep(sleep)
             previous_attempts += 1
 
 
-def retry_during_transitions(f, attempts=RETRY_DURING_TRANSITIONS_ATTEMPTS_DEFAULT, sleep=RETRY_DURING_TRANSITIONS_SLEEP_DEFAULT, exception_check=exception_seems_to_indicate_transition):
-
+def retry_during_transitions(
+    f,
+    attempts=RETRY_DURING_TRANSITIONS_ATTEMPTS_DEFAULT,
+    sleep=RETRY_DURING_TRANSITIONS_SLEEP_DEFAULT,
+    exception_check=exception_seems_to_indicate_transition,
+):
     @wraps(f)
     def _retry(*args, **kwds):
-        return retry_call_during_transitions(partial(f, *args, **kwds), attempts=attempts, sleep=sleep, exception_check=exception_check)
+        return retry_call_during_transitions(
+            partial(f, *args, **kwds), attempts=attempts, sleep=sleep, exception_check=exception_check
+        )
 
     return _retry
 
 
-def edit_details(f, scope=".beta.history"):
+def edit_details(f, scope=".history-index"):
     """Open the editor, run the edits, hit the save button"""
 
     @wraps(f)
     def func_wrapper(self, *args, **kwds):
         # open editor
-        if self.is_beta_history():
-            self.open_history_editor(scope=scope)
+        self.open_history_editor(scope=scope)
         # run edits
         result = f(self, *args, **kwds)
         # save edits
-        if self.is_beta_history():
-            save_button = self.beta_history_element('editor save button')
-            save_button.wait_for_and_click()
+        self.history_click_editor_save()
         return result
 
     return func_wrapper
 
 
 class NavigatesGalaxy(HasDriver):
     """Class with helpers methods for driving components of the Galaxy interface.
@@ -148,14 +170,15 @@
     Some day this class will likely be split up into smaller mixins for particular
     components of Galaxy, but until that day the best practice is to prefix methods
     for driving or querying the interface with the name of the component or page
     the method operates on. These serve as pseudo-namespaces until we decompose this
     class. For instance, the method for clicking an option in the workflow editor is
     workflow_editor_click_option instead of click_workflow_editor_option.
     """
+
     timeout_multiplier: float
     driver: WebDriver
 
     @abstractmethod
     def build_url(self, url: str, for_selenium: bool = True) -> str:
         """Build URL to the target Galaxy."""
 
@@ -209,109 +232,134 @@
         return self.wait_length(wait_type)
 
     def home(self) -> None:
         """Return to root Galaxy page and wait for some basic widgets to appear."""
         self.get()
         self.components.masthead._.wait_for_visible()
 
-    def trs_search(self) -> None:
-        self.driver.get(self.build_url('workflows/trs_search'))
+    def go_to_trs_search(self) -> None:
+        self.driver.get(self.build_url("workflows/trs_search"))
         self.components.masthead._.wait_for_visible()
 
-    def trs_by_id(self) -> None:
-        self.driver.get(self.build_url('workflows/trs_import'))
+    def go_to_trs_by_id(self) -> None:
+        self.driver.get(self.build_url("workflows/trs_import"))
         self.components.masthead._.wait_for_visible()
 
+    def go_to_workflow_sharing(self, workflow_id: str) -> None:
+        self.driver.get(self.build_url(f"workflows/sharing?id={workflow_id}"))
+
+    def go_to_workflow_export(self, workflow_id: str) -> None:
+        self.driver.get(self.build_url(f"workflows/export?id={workflow_id}"))
+
+    def go_to_history_sharing(self, history_id: str) -> None:
+        self.driver.get(self.build_url(f"histories/sharing?id={history_id}"))
+
     def switch_to_main_panel(self):
         self.driver.switch_to.frame(GALAXY_MAIN_FRAME_ID)
 
     @contextlib.contextmanager
     def local_storage(self, key: str, value: Union[float, str]):
         """Method decorator to modify localStorage for the scope of the supplied context."""
-        self.driver.execute_script(f'''window.localStorage.setItem("{key}", {value});''')
+        self.driver.execute_script(f"""window.localStorage.setItem("{key}", {value});""")
         try:
             yield
         finally:
-            self.driver.execute_script(f'''window.localStorage.removeItem("{key}");''')
+            self.driver.execute_script(f"""window.localStorage.removeItem("{key}");""")
 
     @contextlib.contextmanager
     def main_panel(self):
         """Decorator to operate within the context of Galaxy's main frame."""
         try:
             self.switch_to_main_panel()
             yield
         finally:
             self.driver.switch_to.default_content()
 
     def api_get(self, endpoint, data=None, raw=False):
         data = data or {}
         full_url = self.build_url(f"api/{endpoint}", for_selenium=False)
-        response = requests.get(full_url, data=data, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT)
-        if raw:
-            return response
-        else:
-            return response.json()
+        response = requests.get(
+            full_url, data=data, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT
+        )
+        return self._handle_response(response, raw)
 
     def api_post(self, endpoint, data=None):
         data = data or {}
         full_url = self.build_url(f"api/{endpoint}", for_selenium=False)
-        response = requests.post(full_url, data=data, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT)
+        response = requests.post(
+            full_url, data=data, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT
+        )
         return response.json()
 
     def api_delete(self, endpoint, raw=False):
         full_url = self.build_url(f"api/{endpoint}", for_selenium=False)
-        response = requests.delete(full_url, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT)
+        response = requests.delete(
+            full_url, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT
+        )
+        return self._handle_response(response, raw)
+
+    def _handle_response(self, response: requests.Response, raw: bool = False):
         if raw:
             return response
         else:
-            return response.json()
+            return response.json() if response.content else None
 
     def get_galaxy_session(self):
         for cookie in self.driver.get_cookies():
             if cookie["name"] == "galaxysession":
                 return cookie["value"]
 
     def selenium_to_requests_cookies(self):
-        return {
-            'galaxysession': self.get_galaxy_session()
-        }
+        return {"galaxysession": self.get_galaxy_session()}
 
     def history_panel_name_element(self):
-        if self.is_beta_history():
-            component = self.beta_history_element("history name display")
-        else:
-            component = self.components.history_panel.name
+        component = self.history_element("name display")
         return component.wait_for_present()
 
     @retry_during_transitions
     def history_panel_name(self):
         return self.history_panel_name_element().text
 
+    def history_panel_collection_rename(self, hid: int, new_name: str, assert_old_name: Optional[str] = None):
+        toggle = self.history_element("editor toggle")
+        toggle.wait_for_and_click()
+        self.history_panel_rename(new_name)
+
+    def history_panel_expand_collection(self, collection_hid: int) -> SmartComponent:
+        self.history_panel_click_item_title(collection_hid)
+        collection_view = self.components.history_panel.collection_view
+        collection_view._.wait_for_present()
+        return collection_view
+
+    def history_panel_collection_name_element(self):
+        title_element = self.history_element("collection name display").wait_for_present()
+        return title_element
+
     def make_accessible_and_publishable(self):
         self.components.histories.sharing.make_accessible.wait_for_and_click()
         self.components.histories.sharing.make_publishable.wait_for_and_click()
 
-    def history_contents(self, history_id=None, view='summary', datasets_only=True):
+    def history_contents(self, history_id=None, view="summary", datasets_only=True):
         if history_id is None:
             history_id = self.current_history_id()
-        histories = self.api_get('histories?keys=id')
-        if history_id not in [h['id'] for h in histories]:
+        histories = self.api_get("histories?keys=id")
+        if history_id not in [h["id"] for h in histories]:
             return {}
         if datasets_only:
-            endpoint = f'histories/{history_id}/contents?view={view}'
+            endpoint = f"histories/{history_id}/contents?view={view}"
         else:
-            endpoint = f'histories/{history_id}?view={view}'
+            endpoint = f"histories/{history_id}?view={view}"
         return self.api_get(endpoint)
 
-    def current_history(self):
+    def current_history(self) -> Dict[str, Any]:
         full_url = self.build_url("history/current_history_json", for_selenium=False)
         response = requests.get(full_url, cookies=self.selenium_to_requests_cookies(), timeout=DEFAULT_SOCKET_TIMEOUT)
         return response.json()
 
-    def current_history_id(self):
+    def current_history_id(self) -> str:
         return self.current_history()["id"]
 
     def latest_history_item(self):
         history_contents = self.history_contents()
         assert len(history_contents) > 0
         return history_contents[-1]
 
@@ -336,33 +384,24 @@
 
     def history_panel_create_new(self):
         """Click create new and pause a bit for the history to begin to refresh."""
         self.history_click_create_new()
         self.sleep_for(WAIT_TYPES.UX_RENDER)
 
     def history_panel_wait_for_hid_ok(self, hid, allowed_force_refreshes=0):
-        return self.history_panel_wait_for_hid_state(hid, 'ok', allowed_force_refreshes=allowed_force_refreshes)
+        return self.history_panel_wait_for_hid_state(hid, "ok", allowed_force_refreshes=allowed_force_refreshes)
+
+    def history_panel_wait_for_hid_deferred(self, hid, allowed_force_refreshes=0):
+        return self.history_panel_wait_for_hid_state(hid, "deferred", allowed_force_refreshes=allowed_force_refreshes)
 
     def history_panel_item_component(self, history_item=None, hid=None, multi_history_panel=False):
-        if self.is_beta_history():
-            assert hid
-            return self.content_item_by_attributes(hid=hid)
-        if history_item is None:
-            assert hid
-            history_item = self.hid_to_history_item(hid)
-        item = self.components.history_panel.item.selector
-        if multi_history_panel:
-            item = self.components.multi_history_view.item
-        return item(
-            history_content_type=history_item["history_content_type"],
-            id=history_item["id"]
-        )
+        assert hid
+        return self.content_item_by_attributes(hid=hid, multi_history_panel=multi_history_panel)
 
     def wait_for_history_to_have_hid(self, history_id, hid):
-
         def get_hids():
             contents = self.api_get(f"histories/{history_id}/contents")
             return [d["hid"] for d in contents]
 
         def history_has_hid(driver):
             hids = get_hids()
             return any(h == hid for h in hids)
@@ -378,19 +417,22 @@
     def history_panel_wait_for_hid_visible(self, hid, allowed_force_refreshes=0, multi_history_panel=False):
         current_history_id = self.current_history_id()
         self.wait_for_history_to_have_hid(current_history_id, hid)
         # TODO: just use HID and stop resolving history_item -or- place history item in DOM.
         # I think Mason thought the first was cleaner based on recent changes, but I think duplicated
         # HIDs due to conversions and such make using the actual history item ID more robust.
         history_item = self.hid_to_history_item(hid, current_history_id=current_history_id)
-        history_item_selector = self.history_panel_item_component(history_item, hid=hid, multi_history_panel=multi_history_panel)
+        history_item_selector = self.history_panel_item_component(
+            history_item, hid=hid, multi_history_panel=multi_history_panel
+        )
         try:
             self.history_item_wait_for(history_item_selector, allowed_force_refreshes)
         except SeleniumTimeoutException as e:
-            contents_elements = self.find_elements(self.navigation.history_panel.selectors.contents)
+            selector = self.navigation.history_panel.selectors.contents
+            contents_elements = self.find_elements(selector)
             div_ids = [f"#{d.get_attribute('id')}" for d in contents_elements]
             template = "Failed waiting on history item %d to become visible, visible datasets include [%s]."
             message = template % (hid, ",".join(div_ids))
             raise self.prepend_timeout_message(e, message)
         return history_item_selector
 
     def hid_to_history_item(self, hid, current_history_id=None):
@@ -411,160 +453,162 @@
                     raise
 
             attempt += 1
             self.history_panel_refresh_click()
         return rval
 
     def history_panel_wait_for_history_loaded(self):
-        # Use the search box showing up as a proxy that the history display
-        # has left the "loading" state and is showing a valid set of history contents
-        # (even if empty).
-        self.wait_for_visible(self.navigation.history_panel.selectors.search, wait_type=WAIT_TYPES.DATABASE_OPERATION)
+        # Verify that the history has been loaded and is empty.
+        self.wait_for_visible(
+            self.navigation.history_panel.selectors.empty_message, wait_type=WAIT_TYPES.DATABASE_OPERATION
+        )
 
     def history_panel_wait_for_hid_hidden(self, hid, multi_history_panel=False):
-        history_item = self.hid_to_history_item(hid)
-        history_item_selector = self.history_panel_item_component(history_item, multi_history_panel=multi_history_panel)
+        history_item_selector = self.history_panel_item_component(hid=hid, multi_history_panel=multi_history_panel)
         self.wait_for_absent_or_hidden(history_item_selector, wait_type=WAIT_TYPES.JOB_COMPLETION)
         return history_item_selector
 
     def history_panel_wait_for_hid_state(self, hid, state, allowed_force_refreshes=0, multi_history_panel=False):
-        history_item_selector = self.history_panel_wait_for_hid_visible(hid, allowed_force_refreshes=allowed_force_refreshes, multi_history_panel=multi_history_panel)
-        if self.is_beta_history():
-            history_item_selector_state = self.content_item_by_attributes(hid=hid, state=state)
-        else:
-            # history_item_selector_state = history_item_selector.with_class(f"state-{state}")
-            history_item_selector_state = history_item_selector.with_data("state", state)
+        history_item_selector = self.history_panel_wait_for_hid_visible(
+            hid, allowed_force_refreshes=allowed_force_refreshes, multi_history_panel=multi_history_panel
+        )
+        history_item_selector_state = self.content_item_by_attributes(
+            hid=hid, state=state, multi_history_panel=multi_history_panel
+        )
         try:
             self.history_item_wait_for(history_item_selector_state, allowed_force_refreshes)
         except SeleniumTimeoutException as e:
             history_item = self.wait_for_visible(history_item_selector)
             current_state = "UNKNOWN"
             classes = history_item.get_attribute("class").split(" ")
             for clazz in classes:
                 if clazz.startswith("state-"):
-                    current_state = clazz[len("state-"):]
+                    current_state = clazz[len("state-") :]
             template = "Failed waiting on history item %d state to change to [%s] current state [%s]. "
             message = template % (hid, state, current_state)
             raise self.prepend_timeout_message(e, message)
         return history_item_selector_state
 
     def click_grid_popup_option(self, item_name, option_label):
         item_button = None
         grid = self.components.grids.body.wait_for_visible()
-        for row in grid.find_elements_by_tag_name('tr'):
-            name_cell = row.find_elements_by_tag_name('td')[1]
+        for row in grid.find_elements(By.TAG_NAME, "tr"):
+            name_cell = row.find_elements(By.TAG_NAME, "td")[1]
             if name_cell.text == item_name:
                 item_button = name_cell
                 break
 
         if item_button is None:
-            raise AssertionError(f'Failed to find item with name [{item_name}]')
+            raise AssertionError(f"Failed to find item with name [{item_name}]")
 
-        popup_menu_button = item_button.find_element_by_css_selector('.dropdown-toggle')
+        popup_menu_button = item_button.find_element(By.CSS_SELECTOR, ".dropdown-toggle")
         popup_menu_button.click()
-        popup_option = self.driver.find_element_by_link_text(option_label)
+        popup_option = self.driver.find_element(By.LINK_TEXT, option_label)
         popup_option.click()
 
     def published_grid_search_for(self, search_term=None):
         return self._inline_search_for(
             self.navigation.grids.free_text_search,
             search_term,
         )
 
     def get_logged_in_user(self):
         return self.api_get("users/current")
 
     def get_api_key(self, force=False):
-        # If force is false, use the form inputs API and allow the key to be absent.
         if not force:
-            return self.api_get(f"users/{self.get_user_id()}/api_key/inputs")["inputs"][0]["value"]
+            response = self.api_get(f"users/{self.get_user_id()}/api_key/detailed")
+            return response["key"] if response else None
         else:
             return self.api_post(f"users/{self.get_user_id()}/api_key")
 
     def get_user_id(self):
         user = self.get_logged_in_user()
         return user["id"]
 
     def is_logged_in(self):
         return "email" in self.get_logged_in_user()
 
     @retry_during_transitions
-    def _inline_search_for(self, selector, search_term=None):
+    def _inline_search_for(self, selector, search_term=None, escape_to_clear=False):
         # Clear tooltip resulting from clicking on the masthead to get here.
         self.clear_tooltips()
         search_box = self.wait_for_and_click(selector)
+        if escape_to_clear:
+            # The combination of DebouncedInput+b-input doesn't seem to uniformly respect
+            # .clear() below. We use escape handling a lot - and that does cauase to the input
+            # to reset correctly and fire the required re-active events/handlers.
+            self.send_escape(search_box)
         search_box.clear()
         if search_term is not None:
             search_box.send_keys(search_term)
         self.send_enter(search_box)
         return search_box
 
     def _get_random_name(self, prefix=None, suffix=None, len=10):
-        return '{}{}{}'.format(
-            prefix or '',
-            ''.join(random.choice(string.ascii_lowercase + string.digits) for _ in range(len)),
-            suffix or '',
+        return "{}{}{}".format(
+            prefix or "",
+            "".join(random.choice(string.ascii_lowercase + string.digits) for _ in range(len)),
+            suffix or "",
         )
 
     def _get_random_email(self, username=None, domain=None):
-        username = username or 'test'
-        domain = domain or 'test.test'
+        username = username or "test"
+        domain = domain or "test.test"
         return self._get_random_name(prefix=username, suffix=f"@{domain}")
 
     # Creates a random password of length len by creating an array with all ASCII letters and the numbers 0 to 9,
     # then using the random number generator to pick one elemenent to concatinate it to the end of the password string until
     # we have a password of length len.
     def _get_random_password(self, len=6):
-        return ''.join(random.SystemRandom().choice(string.ascii_letters + string.digits) for _ in range(len))
+        return "".join(random.SystemRandom().choice(string.ascii_letters + string.digits) for _ in range(len))
 
     def submit_login(self, email, password=None, assert_valid=True, retries=0):
-        if password is None:
-            password = self.default_password
-        login_info = {
-            'login': email,
-            'password': password,
-        }
         self.components.masthead.register_or_login.wait_for_and_click()
         self.sleep_for(WAIT_TYPES.UX_RENDER)
-        form = self.wait_for_visible(self.navigation.login.selectors.form)
-        self.fill(form, login_info)
-        self.snapshot("logging-in")
-        self.wait_for_and_click(self.navigation.login.selectors.submit)
-        self.snapshot("login-submitted")
+        self.fill_login_and_submit(email, password=password)
         if assert_valid:
             try:
                 self.wait_for_logged_in()
             except NotLoggedInException:
                 self.snapshot("login-failed")
                 if retries > 0:
                     self.submit_login(email, password, assert_valid, retries - 1)
                 else:
                     raise
             self.snapshot("logged-in")
 
+    def fill_login_and_submit(self, email, password=None):
+        if password is None:
+            password = self.default_password
+        login_info = {
+            "login": email,
+            "password": password,
+        }
+        form = self.wait_for_visible(self.navigation.login.selectors.form)
+        self.fill(form, login_info)
+        self.snapshot("logging-in")
+        self.wait_for_and_click(self.navigation.login.selectors.submit)
+        self.snapshot("login-submitted")
+
     def register(self, email=None, password=None, username=None, confirm=None, assert_valid=True):
         if email is None:
             email = self._get_random_email()
         if password is None:
             password = self.default_password
         if confirm is None:
             confirm = password
         if username is None:
             username = email.split("@")[0]
 
         self.home()
         self.components.masthead.register_or_login.wait_for_and_click()
         self.wait_for_and_click(self.navigation.registration.selectors.toggle)
         form = self.wait_for_visible(self.navigation.registration.selectors.form)
-        self.fill(form, dict(
-            email=email,
-            password=password,
-            username=username,
-            confirm=confirm
-        ))
+        self.fill(form, dict(email=email, password=password, username=username, confirm=confirm))
         self.wait_for_and_click(self.navigation.registration.selectors.submit)
         if assert_valid is False:
             self.assert_error_message()
         elif assert_valid:
             self.wait_for_logged_in()
 
             # Code below previously was needed because there was a bug that would prevent the masthead from changing,
@@ -574,15 +618,15 @@
             self.wait_for_logged_in()
             self.click_masthead_user()
             # Make sure the user menu was dropped down
             user_menu = self.components.masthead.user_menu.wait_for_visible()
             try:
                 username_element = self.components.masthead.username.wait_for_visible()
             except SeleniumTimeoutException as e:
-                menu_items = user_menu.find_elements_by_css_selector("li a")
+                menu_items = user_menu.find_elements(By.CSS_SELECTOR, "li a")
                 menu_text = [mi.text for mi in menu_items]
                 message = f"Failed to find logged in message in menu items {', '.join(menu_text)}"
                 raise self.prepend_timeout_message(e, message)
 
             text = username_element.text
             assert username in text
             assert self.get_logged_in_user()["email"] == email
@@ -592,61 +636,101 @@
 
     def wait_for_logged_in(self):
         try:
             self.components.masthead.logged_in_only.wait_for_visible()
         except SeleniumTimeoutException as e:
             ui_logged_out = self.components.masthead.logged_out_only.is_displayed
             if ui_logged_out:
-                dom_message = "Element a.loggedout-only is present in DOM, indicating Login or Register button still in masthead."
+                dom_message = (
+                    "Element a.loggedout-only is present in DOM, indicating Login or Register button still in masthead."
+                )
             else:
                 dom_message = "Element a.loggedout-only is *not* present in DOM."
             user_info = self.api_get("users/current")
             if "username" in user_info:
                 template = "Failed waiting for masthead to update for login, but user API response indicates [%s] is logged in. This seems to be a bug in Galaxy. %s logged API response was [%s]. "
                 message = template % (user_info["username"], dom_message, user_info)
                 raise self.prepend_timeout_message(e, message)
             else:
                 raise NotLoggedInException(e, user_info, dom_message)
 
     def click_center(self):
         action_chains = self.action_chains()
-        center_element = self.driver.find_element_by_css_selector("#center")
+        center_element = self.driver.find_element(By.CSS_SELECTOR, "#center")
         action_chains.move_to_element(center_element).click().perform()
 
+    def hover_over(self, target):
+        action_chains = self.action_chains()
+        action_chains.move_to_element(target).perform()
+
     def perform_upload(self, test_path, **kwd):
         self._perform_upload(test_path=test_path, **kwd)
 
     def perform_upload_of_pasted_content(self, paste_data, **kwd):
         self._perform_upload(paste_data=paste_data, **kwd)
 
-    def _perform_upload(self, test_path=None, paste_data=None, ext=None, genome=None, ext_all=None, genome_all=None):
+    def _perform_upload(
+        self, test_path=None, paste_data=None, ext=None, genome=None, ext_all=None, genome_all=None, deferred=None
+    ):
         self.home()
         self.upload_start_click()
 
         self.upload_set_footer_extension(ext_all)
         self.upload_set_footer_genome(genome_all)
 
         if test_path:
             self.upload_queue_local_file(test_path)
         else:
             assert paste_data is not None
             self.upload_paste_data(paste_data)
 
         if ext is not None:
-            self.wait_for_selector_visible('.upload-extension')
+            self.wait_for_selector_visible(".upload-extension")
             self.select2_set_value(".upload-extension", ext)
 
         if genome is not None:
-            self.wait_for_selector_visible('.upload-genome')
+            self.wait_for_selector_visible(".upload-genome")
             self.select2_set_value(".upload-genome", genome)
 
+        if deferred is not None:
+            upload = self.components.upload
+            upload.settings_button(n=0).wait_for_and_click()
+            upload.settings.wait_for_visible()
+            setting = upload.setting_deferred.wait_for_visible()
+            classes = setting.get_attribute("class").split(" ")
+            if deferred is True and "fa-check-square-o" not in classes:
+                setting.click()
+            elif deferred is False and "fa-check-square-o" in classes:
+                setting.click()
+
         self.upload_start()
 
         self.wait_for_and_click_selector("button#btn-close")
 
+    def perform_upload_of_composite_dataset_pasted_data(self, ext, paste_content):
+        self.home()
+        self.upload_start_click()
+        self.components.upload.tab(tab="composite").wait_for_and_click()
+        self.upload_set_footer_extension(ext, tab_id="composite")
+
+        table = self.components.upload.composite.table().wait_for_visible()
+        source_select_buttons = table.find_elements(self.by.CSS_SELECTOR, "div.dropdown button.btn")
+        paste_buttons = table.find_elements(
+            self.by.CSS_SELECTOR, ".upload-source .dropdown-menu .dropdown-item .fa-edit"
+        )
+        textareas = table.find_elements(self.by.CSS_SELECTOR, "div.upload-text-column textarea.upload-text-content")
+
+        for i in range(len(paste_content)):
+            source_select_buttons[i].click()
+            paste_buttons[i].click()
+            textareas[i].send_keys(paste_content[i])
+
+        self.upload_start(tab_id="composite")
+        self.components.upload.composite.close.wait_for_and_click()
+
     def upload_list(self, test_paths, name="test", ext=None, genome=None, hide_source_items=True):
         self._collection_upload_start(test_paths, ext, genome, "List")
         if not hide_source_items:
             self.collection_builder_hide_originals()
 
         self.collection_builder_set_name(name)
         self.collection_builder_create()
@@ -695,22 +779,22 @@
 
     def upload_start_click(self):
         self.components.upload.start.wait_for_and_click()
 
     @retry_during_transitions
     def upload_set_footer_extension(self, ext, tab_id="regular"):
         if ext is not None:
-            selector = f'div#{tab_id} .upload-footer-extension'
+            selector = f"div#{tab_id} .upload-footer-extension"
             self.wait_for_selector_visible(selector)
             self.select2_set_value(selector, ext)
 
     @retry_during_transitions
     def upload_set_footer_genome(self, genome, tab_id="regular"):
         if genome is not None:
-            selector = f'div#{tab_id} .upload-footer-genome'
+            selector = f"div#{tab_id} .upload-footer-genome"
             self.wait_for_selector_visible(selector)
             self.select2_set_value(selector, genome)
 
     @retry_during_transitions
     def upload_set_collection_type(self, collection_type):
         self.wait_for_selector_visible(".upload-footer-collection-type")
         self.select2_set_value(".upload-footer-collection-type", collection_type)
@@ -718,15 +802,15 @@
     def upload_start(self, tab_id="regular"):
         self.wait_for_and_click_selector(f"div#{tab_id} button#btn-start")
 
     @retry_during_transitions
     def upload_build(self, tab="collection"):
         build_selector = f"div#{tab} button#btn-build"
         # Pause a bit to let the callback on the build button be registered.
-        time.sleep(.5)
+        time.sleep(0.5)
         # Click the Build button and make sure it disappears.
         self.wait_for_and_click_selector(build_selector)
         try:
             self.wait_for_selector_absent_or_hidden(build_selector)
         except SeleniumTimeoutException:
             # Sometimes the callback in the JS hasn't be registered by the
             # time that the build button is clicked. By the time the timeout
@@ -778,132 +862,122 @@
     def rule_builder_set_extension(self, extension):
         self.select2_set_value(self.navigation.rule_builder.selectors.extension_select, extension)
 
     def rule_builder_filter_count(self, count=1):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_filter.wait_for_and_click()
         with self.rule_builder_rule_editor("add-filter-count") as editor_element:
-            filter_input = editor_element.find_element_by_css_selector("input[type='number']")
+            filter_input = editor_element.find_element(By.CSS_SELECTOR, "input[type='number']")
             filter_input.clear()
             filter_input.send_keys(f"{count}")
 
     def rule_builder_sort(self, column_label, screenshot_name=None):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_rules.wait_for_and_click()
         with self.rule_builder_rule_editor("sort") as editor_element:
-            column_elem = editor_element.find_element_by_css_selector(".rule-column-selector")
+            column_elem = editor_element.find_element(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elem, column_label)
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_add_regex_groups(self, column_label, group_count, regex, screenshot_name):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_column.wait_for_and_click()
         with self.rule_builder_rule_editor("add-column-regex") as editor_element:
-
-            column_elem = editor_element.find_element_by_css_selector(".rule-column-selector")
+            column_elem = editor_element.find_element(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elem, column_label)
 
-            groups_elem = editor_element.find_element_by_css_selector("input[type='radio'][value='groups']")
+            groups_elem = editor_element.find_element(By.CSS_SELECTOR, "input[type='radio'][value='groups']")
             groups_elem.click()
 
-            regex_elem = editor_element.find_element_by_css_selector("input.rule-regular-expression")
+            regex_elem = editor_element.find_element(By.CSS_SELECTOR, "input.rule-regular-expression")
             regex_elem.clear()
             regex_elem.send_keys(regex)
 
-            filter_input = editor_element.find_element_by_css_selector("input[type='number']")
+            filter_input = editor_element.find_element(By.CSS_SELECTOR, "input[type='number']")
             filter_input.clear()
             filter_input.send_keys(f"{group_count}")
 
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_add_regex_replacement(self, column_label, regex, replacement, screenshot_name=None):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_column.wait_for_and_click()
         with self.rule_builder_rule_editor("add-column-regex") as editor_element:
-
-            column_elem = editor_element.find_element_by_css_selector(".rule-column-selector")
+            column_elem = editor_element.find_element(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elem, column_label)
 
-            groups_elem = editor_element.find_element_by_css_selector("input[type='radio'][value='replacement']")
+            groups_elem = editor_element.find_element(By.CSS_SELECTOR, "input[type='radio'][value='replacement']")
             groups_elem.click()
 
-            regex_elem = editor_element.find_element_by_css_selector("input.rule-regular-expression")
+            regex_elem = editor_element.find_element(By.CSS_SELECTOR, "input.rule-regular-expression")
             regex_elem.clear()
             regex_elem.send_keys(regex)
 
-            filter_input = editor_element.find_element_by_css_selector("input.rule-replacement")
+            filter_input = editor_element.find_element(By.CSS_SELECTOR, "input.rule-replacement")
             filter_input.clear()
             filter_input.send_keys(f"{replacement}")
 
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_add_value(self, value, screenshot_name=None):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_column.wait_for_and_click()
         with self.rule_builder_rule_editor("add-column-value") as editor_element:
-            filter_input = editor_element.find_element_by_css_selector("input[type='text']")
+            filter_input = editor_element.find_element(By.CSS_SELECTOR, "input[type='text']")
             filter_input.clear()
             filter_input.send_keys(value)
 
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_remove_columns(self, column_labels, screenshot_name=None):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_rules.wait_for_and_click()
         with self.rule_builder_rule_editor("remove-columns") as filter_editor_element:
-            column_elem = filter_editor_element.find_element_by_css_selector(".rule-column-selector")
+            column_elem = filter_editor_element.find_element(By.CSS_SELECTOR, ".rule-column-selector")
             for column_label in column_labels:
                 self.select2_set_value(column_elem, column_label)
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_concatenate_columns(self, column_label_1, column_label_2, screenshot_name=None):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_column.wait_for_and_click()
         with self.rule_builder_rule_editor("add-column-concatenate") as filter_editor_element:
-            column_elems = filter_editor_element.find_elements_by_css_selector(".rule-column-selector")
+            column_elems = filter_editor_element.find_elements(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elems[0], column_label_1)
-            column_elems = filter_editor_element.find_elements_by_css_selector(".rule-column-selector")
+            column_elems = filter_editor_element.find_elements(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elems[1], column_label_2)
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_split_columns(self, column_labels_1, column_labels_2, screenshot_name=None):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_rules.wait_for_and_click()
         with self.rule_builder_rule_editor("split-columns") as filter_editor_element:
-            column_elems = filter_editor_element.find_elements_by_css_selector(".rule-column-selector")
+            column_elems = filter_editor_element.find_elements(By.CSS_SELECTOR, ".rule-column-selector")
             clear = True
             for column_label_1 in column_labels_1:
                 self.select2_set_value(column_elems[0], column_label_1, clear_value=clear)
                 clear = False
 
-            column_elems = filter_editor_element.find_elements_by_css_selector(".rule-column-selector")
+            column_elems = filter_editor_element.find_elements(By.CSS_SELECTOR, ".rule-column-selector")
             clear = True
             for column_label_2 in column_labels_2:
                 self.select2_set_value(column_elems[1], column_label_2, clear_value=clear)
                 clear = False
 
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     def rule_builder_swap_columns(self, column_label_1, column_label_2, screenshot_name):
         rule_builder = self.components.rule_builder
         rule_builder.menu_button_rules.wait_for_and_click()
         with self.rule_builder_rule_editor("swap-columns") as filter_editor_element:
-            column_elems = filter_editor_element.find_elements_by_css_selector(".rule-column-selector")
+            column_elems = filter_editor_element.find_elements(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elems[0], column_label_1)
-            column_elems = filter_editor_element.find_elements_by_css_selector(".rule-column-selector")
+            column_elems = filter_editor_element.find_elements(By.CSS_SELECTOR, ".rule-column-selector")
             self.select2_set_value(column_elems[1], column_label_2)
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
 
     @contextlib.contextmanager
     def rule_builder_rule_editor(self, rule_type):
         rule_builder = self.components.rule_builder
         rule_builder.menu_item_rule_type(rule_type=rule_type).wait_for_and_click()
         filter_editor = rule_builder.rule_editor(rule_type=rule_type)
         filter_editor_element = filter_editor.wait_for_visible()
@@ -915,26 +989,24 @@
         rule_builder.menu_button_rules.wait_for_and_click()
         rule_builder.menu_item_rule_type(rule_type="mapping").wait_for_and_click()
         rule_builder.add_mapping_menu.wait_for_and_click()
         rule_builder.add_mapping_button(mapping_type=mapping_type).wait_for_and_click()
         if mapping_type != "list-identifiers" or not isinstance(column_label, list):
             mapping_elem = rule_builder.mapping_edit(mapping_type=mapping_type).wait_for_visible()
             self.select2_set_value(mapping_elem, column_label)
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
         else:
             assert len(column_label) > 0
             column_labels = column_label
             for i, column_label in enumerate(column_labels):
                 if i > 0:
                     rule_builder.mapping_add_column(mapping_type=mapping_type).wait_for_and_click()
                 mapping_elem = rule_builder.mapping_edit(mapping_type=mapping_type).wait_for_visible()
                 self.select2_set_value(mapping_elem, column_label)
-            if screenshot_name:
-                self.screenshot(screenshot_name)
+            self.screenshot_if(screenshot_name)
         rule_builder.mapping_ok.wait_for_and_click()
 
     def rule_builder_set_source(self, json):
         rule_builder = self.components.rule_builder
         rule_builder.view_source.wait_for_and_click()
         self.rule_builder_enter_source_text(json)
         rule_builder.main_button_ok.wait_for_and_click()
@@ -945,15 +1017,15 @@
         text_area_elem = rule_builder.source.wait_for_visible()
         text_area_elem.clear()
         text_area_elem.send_keys(json)
 
     def workflow_editor_click_option(self, option_label):
         self.workflow_editor_click_options()
         menu_element = self.workflow_editor_options_menu_element()
-        option_elements = menu_element.find_elements_by_css_selector("a")
+        option_elements = menu_element.find_elements(By.CSS_SELECTOR, "a")
         assert len(option_elements) > 0, "Failed to find workflow editor options"
         self.sleep_for(WAIT_TYPES.UX_RENDER)
         found_option = False
         for option_element in option_elements:
             if option_label in option_element.text:
                 action_chains = self.action_chains()
                 action_chains.move_to_element(option_element)
@@ -989,14 +1061,19 @@
         self.components.masthead.preferences.wait_for_and_click()
 
     def navigate_to_invocations(self):
         self.home()
         self.click_masthead_user()
         self.components.masthead.invocations.wait_for_and_click()
 
+    def navigate_to_pages(self):
+        self.home()
+        self.click_masthead_user()
+        self.components.masthead.pages.wait_for_and_click()
+
     def admin_open(self):
         self.components.masthead.admin.wait_for_and_click()
 
     def select_dataset_from_lib_import_modal(self, filenames):
         for name in filenames:
             self.components.libraries.folder.select_import_dir_item(name=name).wait_for_and_click()
         self.components.libraries.folder.import_dir_btn.wait_for_and_click()
@@ -1013,27 +1090,27 @@
         self.click_masthead_shared_data()
         self.components.masthead.libraries.wait_for_and_click()
         self.components.libraries.selector.wait_for_visible()
 
     def libraries_open_with_name(self, name):
         self.libraries_open()
         self.libraries_index_search_for(name)
-        self.libraries_index_table_elements()[0].find_element_by_css_selector("td a").click()
+        self.libraries_index_table_elements()[0].find_element(By.CSS_SELECTOR, "td a").click()
 
     @retry_during_transitions
     def libraries_index_table_elements(self):
         container = self.components.libraries._.wait_for_visible()
 
-        elements = container.find_elements_by_css_selector("tbody")
+        elements = container.find_elements(By.CSS_SELECTOR, "tbody")
         if not elements:
             return []
         else:
             assert len(elements) == 1
             element = elements[0]
-            return element.find_elements_by_css_selector("tr")  # [style='display: table-row']
+            return element.find_elements(By.CSS_SELECTOR, "tr")  # [style='display: table-row']
 
     def libraries_index_create(self, name):
         self.components.libraries.create_new_library_btn.wait_for_and_click()
         name_input_field = self.components.libraries.new_library_name_input.wait_for_visible()
         input_field = self.components.libraries.new_library_description_input.wait_for_visible()
 
         name_input_field.send_keys(name)
@@ -1078,30 +1155,30 @@
     def libraries_dataset_import_from_history_select(self, to_select_items):
         self.wait_for_visible(self.navigation.libraries.folder.selectors.import_history_content)
         history_elements = self.find_elements(self.navigation.libraries.folder.selectors.import_history_contents_items)
         for to_select_item in to_select_items:
             found = False
             for history_element in history_elements:
                 if to_select_item in history_element.text:
-                    history_element.find_element_by_css_selector("input").click()
+                    history_element.find_element(By.CSS_SELECTOR, "input").click()
                     found = True
                     break
 
             if not found:
                 raise Exception(f"Failed to find history item [{to_select_item}] to select")
 
     def libraries_dataset_import_from_history_click_ok(self, wait=True):
         self.wait_for_and_click(self.navigation.libraries.folder.selectors.import_datasets_ok_button)
         if wait:
             # Let the progress bar disappear...
             self.wait_for_absent_or_hidden(self.navigation.libraries.folder.selectors.import_progress_bar)
 
     def libraries_table_elements(self):
         tbody_element = self.wait_for_selector_visible("#folder_list_body > tbody")
-        return tbody_element.find_elements_by_css_selector("tr:not(.b-table-empty-row)")
+        return tbody_element.find_elements(By.CSS_SELECTOR, "tr:not(.b-table-empty-row)")
 
     def populate_library_folder_from_import_dir(self, library_name, filenames):
         self.libraries_open_with_name(library_name)
         self.libraries_dataset_import(self.navigation.libraries.folder.labels.from_import_dir)
         self.select_dataset_from_lib_import_modal(filenames)
 
     def navigate_to_new_library(self, login=True):
@@ -1111,134 +1188,178 @@
     def wait_for_overlays_cleared(self):
         """Wait for modals and Toast notifications to disappear."""
         self.wait_for_selector_absent_or_hidden(".ui-modal", wait_type=WAIT_TYPES.UX_POPUP)
         self.wait_for_selector_absent_or_hidden(".toast", wait_type=WAIT_TYPES.UX_POPUP)
 
     def clear_tooltips(self):
         action_chains = self.action_chains()
-        center_element = self.driver.find_element_by_css_selector("#center")
+        center_element = self.driver.find_element(By.CSS_SELECTOR, "#center")
         action_chains.move_to_element(center_element).perform()
         self.wait_for_selector_absent_or_hidden(".b-tooltip", wait_type=WAIT_TYPES.UX_POPUP)
 
     def workflow_index_open(self):
         self.home()
         self.click_masthead_workflow()
 
     def workflow_index_table_elements(self):
-        self.wait_for_selector_visible("#workflow-table")
-        table_elements = self.driver.find_elements_by_css_selector("#workflow-table > tbody > tr:not([style*='display: none'])")
-        return table_elements
+        workflows = self.components.workflows
+        workflows.workflow_table.wait_for_visible()
+        return workflows.workflow_rows.all()
 
     def workflow_index_table_row(self, workflow_index=0):
+        self.components.workflows.workflow_rows.wait_for_element_count_of_at_least(workflow_index + 1)
         return self.workflow_index_table_elements()[workflow_index]
 
     @retry_during_transitions
     def workflow_index_column_text(self, column_index, workflow_index=0):
-        row_element = self.workflow_index_table_row()
-        columns = row_element.find_elements_by_css_selector("td")
+        row_element = self.workflow_index_table_row(workflow_index=workflow_index)
+        columns = row_element.find_elements(By.CSS_SELECTOR, "td")
         return columns[column_index].text
 
     def workflow_index_click_search(self):
         return self.wait_for_and_click_selector("#workflow-search")
 
     def workflow_index_search_for(self, search_term=None):
         return self._inline_search_for(
             self.navigation.workflows.search_box,
             search_term,
+            escape_to_clear=True,
         )
 
     def workflow_index_click_import(self):
         return self.components.workflows.import_button.wait_for_and_click()
 
     def workflow_index_rename(self, new_name, workflow_index=0):
         self.workflow_index_click_option("Rename", workflow_index=workflow_index)
         alert = self.driver.switch_to.alert
         alert.send_keys(new_name)
         alert.accept()
+        self.components.workflows.workflow_with_name(workflow_name=new_name).wait_for_visible()
 
     @retry_during_transitions
     def workflow_index_name(self, workflow_index=0):
         """Get workflow name for workflow_index'th row."""
         row_element = self.workflow_index_table_row(workflow_index=workflow_index)
-        workflow_button = row_element.find_element_by_css_selector(".workflow-dropdown")
+        workflow_button = row_element.find_element(By.CSS_SELECTOR, ".workflow-dropdown")
         return workflow_button.text
 
     @retry_during_transitions
     def workflow_click_option(self, workflow_selector, workflow_index=0):
         workflow_row = self.workflow_index_table_row(workflow_index=workflow_index)
-        workflow_button = workflow_row.find_element_by_css_selector(workflow_selector)
+        workflow_button = workflow_row.find_element(By.CSS_SELECTOR, workflow_selector)
         workflow_button.click()
 
     def select_dropdown_item(self, option_title):
         menu_element = self.wait_for_selector_visible(".dropdown-menu.show")
-        menu_options = menu_element.find_elements_by_css_selector("a.dropdown-item")
+        menu_options = menu_element.find_elements(By.CSS_SELECTOR, "a.dropdown-item")
         for menu_option in menu_options:
             if option_title in menu_option.text:
                 menu_option.click()
                 return True
 
     def workflow_index_click_option(self, option_title, workflow_index=0):
         self.workflow_click_option(".workflow-dropdown", workflow_index)
         if not self.select_dropdown_item(option_title):
             raise AssertionError(f"Failed to find workflow action option with title [{option_title}]")
 
     def workflow_index_click_tag_display(self, workflow_index=0):
         workflow_row_element = self.workflow_index_table_row(workflow_index)
-        tag_display = workflow_row_element.find_element_by_css_selector(".tags-display")
+        tag_display = workflow_row_element.find_element(By.CSS_SELECTOR, ".tags-display")
         tag_display.click()
 
+    def workflow_index_add_tag(self, tag: str, workflow_index: int = 0):
+        self.workflow_index_click_tag_display(workflow_index=workflow_index)
+        self.tagging_add([tag])
+
     @retry_during_transitions
     def workflow_index_tags(self, workflow_index=0):
-        workflow_row_element = self.workflow_index_table_row(workflow_index)
-        tag_display = workflow_row_element.find_element_by_css_selector(".tags-display")
-        tag_spans = tag_display.find_elements_by_css_selector(".tag-name")
+        tag_spans = self.workflow_index_tag_elements(workflow_index=workflow_index)
         tags = []
         for tag_span in tag_spans:
             tags.append(tag_span.text)
         return tags
 
+    @retry_during_transitions
+    def workflow_index_tag_elements(self, workflow_index=0):
+        workflow_row_element = self.workflow_index_table_row(workflow_index)
+        tag_display = workflow_row_element.find_element(By.CSS_SELECTOR, ".tags-display")
+        tag_spans = tag_display.find_elements(By.CSS_SELECTOR, ".tag-name")
+        return tag_spans
+
+    @retry_during_transitions
+    def workflow_index_click_tag(self, tag, workflow_index=0):
+        tag_spans = self.workflow_index_tag_elements(workflow_index=workflow_index)
+        clicked = False
+        for tag_span in tag_spans:
+            if tag_span.text == tag:
+                tag_span.click()
+                clicked = True
+                break
+        if not clicked:
+            raise KeyError(f"Failed to find tag {tag} on workflow with index {workflow_index}")
+
     def workflow_import_submit_url(self, url):
         form_button = self.wait_for_selector_visible("#workflow-import-button")
         url_element = self.wait_for_selector_visible("#workflow-import-url-input")
         url_element.send_keys(url)
         form_button.click()
 
     def workflow_sharing_click_publish(self):
         self.wait_for_and_click_selector("input[name='make_accessible_and_publish']")
 
     def tagging_add(self, tags, auto_closes=True, parent_selector=""):
-
         for i, tag in enumerate(tags):
             if auto_closes or i == 0:
                 tag_area = f"{parent_selector}.tags-input input[type='text']"
                 tag_area = self.wait_for_selector_clickable(tag_area)
                 tag_area.click()
 
             tag_area.send_keys(tag)
             self.send_enter(tag_area)
 
+    def workflow_run_with_name(self, name: str):
+        self.workflow_index_open()
+        self.workflow_index_search_for(name)
+        self.workflow_click_option(".workflow-run")
+
+    def workflow_run_specify_inputs(self, inputs: Dict[str, Any]):
+        workflow_run = self.components.workflow_run
+        for label, value in inputs.items():
+            input_div_element = workflow_run.input_data_div(label=label).wait_for_visible()
+            self.select2_set_value(input_div_element, "%d: " % value["hid"])
+
     def workflow_run_submit(self):
-        self.wait_for_and_click_selector("button.btn-primary")
+        self.components.workflow_run.run_workflow.wait_for_and_click()
+
+    def workflow_run_ensure_expanded(self):
+        workflow_run = self.components.workflow_run
+        if workflow_run.expanded_form.is_absent:
+            workflow_run.expand_form_link.wait_for_and_click()
+            workflow_run.expanded_form.wait_for_visible()
 
     def workflow_create_new(self, annotation=None, clear_placeholder=False):
         self.workflow_index_open()
         self.sleep_for(self.wait_types.UX_RENDER)
         self.click_button_new_workflow()
         self.sleep_for(self.wait_types.UX_RENDER)
-        form_element = self.driver.find_element_by_id("submit")
         name = self._get_random_name()
-        annotation = annotation or self._get_random_name()
-        inputs = self.driver.find_elements_by_class_name("ui-input")
+        name_component = self.components.workflows.create.name
         if clear_placeholder:
-            inputs[0].clear()
-        inputs[0].send_keys(name)
-        inputs[1].send_keys(annotation)
-        form_element.click()
+            name_component.wait_for_visible().clear()
+        name_component.wait_for_and_send_keys(name)
+        annotation = annotation or self._get_random_name()
+        self.components.workflows.create.annotation.wait_for_and_send_keys(annotation)
+        self.components.workflows.create.submit.wait_for_and_click()
         return name
 
+    def invocation_index_table_elements(self):
+        invocations = self.components.invocations
+        invocations.invocations_table.wait_for_visible()
+        return invocations.invocations_table_rows.all()
+
     def tool_open(self, tool_id, outer=False):
         if outer:
             tool_link = self.components.tool_panel.outer_tool_link(tool_id=tool_id)
         else:
             tool_link = self.components.tool_panel.tool_link(tool_id=tool_id)
         tool_element = tool_link.wait_for_present()
         self.driver.execute_script("arguments[0].scrollIntoView(true);", tool_element)
@@ -1246,30 +1367,48 @@
 
     def datasource_tool_open(self, tool_id):
         tool_link = self.components.tool_panel.data_source_tool_link(tool_id=tool_id)
         tool_element = tool_link.wait_for_present()
         self.driver.execute_script("arguments[0].scrollIntoView(true);", tool_element)
         tool_link.wait_for_and_click()
 
+    def create_page_and_edit(self, name=None, slug=None, screenshot_name=None):
+        name = self.create_page(name=name, slug=slug, screenshot_name=screenshot_name)
+        self.click_grid_popup_option(name, "Edit content")
+        self.components.pages.editor.markdown_editor.wait_for_visible()
+        return name
+
+    def create_page(self, name=None, slug=None, screenshot_name=None):
+        self.components.pages.create.wait_for_and_click()
+        name = name or self._get_random_name(prefix="page")
+        slug = slug = self._get_random_name(prefix="pageslug")
+        self.tool_set_value("title", name)
+        self.tool_set_value("slug", slug)
+        self.screenshot_if(screenshot_name)
+        # Sometimes 'submit' button not yet hooked up?
+        self.sleep_for(self.wait_types.UX_RENDER)
+        self.components.pages.submit.wait_for_and_click()
+        return name
+
     def tool_parameter_div(self, expanded_parameter_id):
         return self.components.tool_form.parameter_div(parameter=expanded_parameter_id).wait_for_clickable()
 
     def tool_parameter_edit_rules(self):
         rules_div_element = self.tool_parameter_div("rules")
-        edit_button_element = rules_div_element.find_element_by_css_selector("i.fa-edit")
+        edit_button_element = rules_div_element.find_element(By.CSS_SELECTOR, ".form-rules-edit button")
         edit_button_element.click()
 
     def tool_set_value(self, expanded_parameter_id, value, expected_type=None):
         div_element = self.tool_parameter_div(expanded_parameter_id)
         assert div_element
         if expected_type in ["select", "data", "data_collection"]:
             div_selector = f"div.ui-form-element[id$='form-element-{expanded_parameter_id}']"
             self.select2_set_value(div_selector, value)
         else:
-            input_element = div_element.find_element_by_css_selector("input")
+            input_element = div_element.find_element(By.CSS_SELECTOR, "input")
             # Clear default value
             input_element.clear()
             input_element.send_keys(value)
 
     def tool_form_generate_tour(self):
         self.components.tool_form.options.wait_for_and_click()
         self.components.tool_form.generate_tour.wait_for_and_click()
@@ -1297,118 +1436,110 @@
         return element
 
     @retry_during_transitions
     def click_history_options(self):
         component = self.components.history_panel.options_button_icon
         component.wait_for_and_click()
 
+    def click_history_option_export_to_file(self):
+        self.use_bootstrap_dropdown(option="export to file", menu="history options")
+
+    def click_history_option_sharing(self):
+        self.use_bootstrap_dropdown(option="share or publish", menu="history options")
+
     def click_history_option(self, option_label_or_component):
         # Open menu
         self.click_history_options()
 
         if isinstance(option_label_or_component, str):
             option_label = option_label_or_component
-            # Click labelled option
+            # Click labeled option
             self.wait_for_visible(self.navigation.history_panel.options_menu)
-            menu_item_sizzle_selector = self.navigation.history_panel.options_menu_item(option_label=option_label).selector
+            menu_item_sizzle_selector = self.navigation.history_panel.options_menu_item(
+                option_label=option_label
+            ).selector
             menu_selection_element = self.wait_for_sizzle_selector_clickable(menu_item_sizzle_selector)
             menu_selection_element.click()
         else:
             option_component = option_label_or_component
             option_component.wait_for_and_click()
 
-    def use_beta_history(self):
-        if not self.is_beta_history():
-            self.click_history_option(self.components.history_panel.options_use_beta_history)
-            self.components.history_panel.beta.wait_for_present()
-
-    def is_beta_history(self):
-        return not self.components.history_panel.beta.is_absent
-
     # avoids problematic ID and classes on markup
-    def beta_history_element(self, attribute_value, attribute_name="data-description", scope=".beta.history"):
+    def history_element(self, attribute_value, attribute_name="data-description", scope=".history-index"):
         return self.components._.by_attribute(name=attribute_name, value=attribute_value, scope=scope)
 
-    # join list of attrs into css attribute selectors and append to base beta_item selector
-    def content_item_by_attributes(self, **attrs):
-        suffix_list = [f'[data-{k}="{v}"]' for (k, v) in attrs.items()]
+    # join list of attrs into css attribute selectors and append to base item selector
+    def content_item_by_attributes(self, multi_history_panel=False, **attrs):
+        suffix_list = [f'[data-{k}="{v}"]' for (k, v) in attrs.items() if v is not None]
         suffix = "".join(suffix_list)
-        return self.components.history_panel.content_item.selector(suffix=suffix)
+        selector = self.components.history_panel.content_item.selector
+        if multi_history_panel:
+            selector = self.components.multi_history_panel.selector(suffix=suffix)
+        return selector(suffix=suffix)
 
     def history_click_create_new(self):
-        if not self.is_beta_history():
-            self.components.history_panel.new_history_button.wait_for_and_click()
-        else:
-            dropdown = self.beta_history_element("histories operation menu")
-            dropdown.wait_for_and_click()
-            option = self.beta_history_element("create new history")
-            option.wait_for_and_click()
+        self.components.history_panel.new_history_button.wait_for_and_click()
+
+    def history_click_editor_save(self):
+        option = self.history_element("editor save button")
+        option.wait_for_and_click()
+        self.sleep_for(self.wait_types.UX_RENDER)
 
     def history_panel_click_copy_elements(self):
-        if self.is_beta_history():
-            self.use_bootstrap_dropdown(option="copy datasets", menu="history action menu")
-        else:
-            self.click_history_option("Copy Datasets")
+        self.use_bootstrap_dropdown(option="copy datasets", menu="history action menu")
 
     def use_bootstrap_dropdown(self, option=None, menu=None):
         """uses bootstrap dropdown by data-description attributes"""
         if option is None:
             raise TypeError
         if menu is None:
             raise TypeError
-        toggle = self.beta_history_element(menu).descendant("button")
+        toggle = self.history_element(menu).descendant("button")
         self.wait_for_and_click(toggle)
-        return self.beta_history_element(option).wait_for_and_click()
+        return self.history_element(option).wait_for_and_click()
 
     @retry_during_transitions
     def histories_click_advanced_search(self):
-        search_selector = '#standard-search .advanced-search-toggle'
+        search_selector = "#standard-search .advanced-search-toggle"
         self.wait_for_and_click_selector(search_selector)
 
     @retry_during_transitions
     def histories_get_history_names(self):
         self.sleep_for(self.wait_types.UX_RENDER)
         names = []
-        grid = self.wait_for_selector('#grid-table-body')
-        for row in grid.find_elements_by_tag_name('tr'):
-            td = row.find_elements_by_tag_name('td')
-            name = td[1].text if td[0].text == '' else td[0].text
+        grid = self.wait_for_selector("#grid-table-body")
+        for row in grid.find_elements(By.TAG_NAME, "tr"):
+            td = row.find_elements(By.TAG_NAME, "td")
+            name = td[1].text if td[0].text == "" else td[0].text
             if name != "No items" and not name.startswith("No matching entries found"):
                 names.append(name)
         return names
 
     @edit_details
     def history_panel_add_tags(self, tags):
-        tag_icon = self.components.history_panel.tag_icon
-        tag_area = self.components.history_panel.tag_area
-        tag_area_input = self.components.history_panel.tag_area_input
-
-        # if the tag editor is not present but the tag_icon is, then click it
-        if not tag_icon.is_absent and (tag_area.is_absent or not tag_area.is_displayed):
-            tag_icon.wait_for_and_click()
+        tag_area_button = self.components.history_panel.tag_area_button
 
-        input_element = tag_area_input.wait_for_and_click()
+        tag_area_button.wait_for_and_click()
+        input_element = self.components.history_panel.tag_area_input.wait_for_visible()
 
         for tag in tags:
             input_element.send_keys(tag)
             self.send_enter(input_element)
             self.sleep_for(self.wait_types.UX_RENDER)
 
+        self.send_escape(input_element)
+
     @edit_details
     def history_panel_rename(self, new_name):
         editable_text_input_element = self.history_panel_name_input()
-        if self.is_beta_history():
-            editable_text_input_element.clear()
+        editable_text_input_element.clear()
         editable_text_input_element.send_keys(new_name)
-        self.send_enter(editable_text_input_element)
         return editable_text_input_element
 
     def history_panel_name_input(self):
-        if not self.is_beta_history():
-            editable_text_input_element = self.history_panel_click_to_rename()
         history_panel = self.components.history_panel
         edit = history_panel.name_edit_input
         editable_text_input_element = edit.wait_for_visible()
         return editable_text_input_element
 
     def history_panel_click_to_rename(self):
         history_panel = self.components.history_panel
@@ -1432,69 +1563,55 @@
         # Maybe isn't needed?
         # self.sleep_for(WAIT_TYPES.UX_RENDER)
         self.wait_for_and_click(self.navigation.history_panel.multi_operations.selectors.action_button)
 
         @retry_during_transitions
         def _click_action_in_menu():
             menu_element = self.wait_for_visible(self.navigation.history_panel.multi_operations.selectors.action_menu)
-            menu_element.find_element_by_link_text(action.text).click()
+            menu_element.find_element(By.LINK_TEXT, action.text).click()
 
         _click_action_in_menu()
 
     def open_history_multi_view(self):
-        if self.is_beta_history():
-            self.components.history_panel.histories_operation_menu.wait_for_and_click()
-            self.components.history_panel.multi_view_button_beta.wait_for_and_click()
-        else:
-            self.components.history_panel.multi_view_button.wait_for_and_click()
-
-    def history_panel_show_structure(self):
-        if self.is_beta_history():
-            self.use_bootstrap_dropdown(option="show structure", menu="history menu")
-        else:
-            self.click_history_option(self.components.history_panel.options_show_history_structure)
+        self.components.history_panel.histories_operation_menu.wait_for_and_click()
+        self.components.history_panel.multi_view_button.wait_for_and_click()
 
     def history_multi_view_display_collection_contents(self, collection_hid, collection_type="list"):
         self.open_history_multi_view()
 
         selector = self.history_panel_wait_for_hid_state(collection_hid, "ok", multi_history_panel=True)
         self.click(selector)
-        next_level_element_selector = selector
         for _ in range(len(collection_type.split(":")) - 1):
-            next_level_element_selector = next_level_element_selector.descendant(".dataset-collection-element")
-            self.wait_for_and_click(next_level_element_selector)
+            selector = self.history_panel_wait_for_hid_state(1, "ok", multi_history_panel=True)
+            self.click(selector)
 
-        dataset_selector = next_level_element_selector.descendant(".dataset")
+        dataset_selector = self.history_panel_wait_for_hid_state(1, "ok", multi_history_panel=True)
         self.wait_for_and_click(dataset_selector)
+        self.history_panel_wait_for_hid_state(1, "ok", multi_history_panel=True)
 
     def history_panel_item_view_dataset_details(self, hid):
-        if not self.is_beta_history():
-            self.history_panel_ensure_showing_item_details(hid)
-            self.hda_click_details(hid)
-            self.components.dataset_details._.wait_for_visible()
-        else:
-            item = self.history_panel_item_component(hid=hid)
-            item.dataset_operations_dropdown.wait_for_and_click()
-            item.info_button.wait_for_and_click()
-            self.components.dataset_details._.wait_for_visible()
+        item = self.history_panel_item_component(hid=hid)
+        item.dataset_operations_dropdown.wait_for_and_click()
+        item.info_button.wait_for_and_click()
+        self.components.dataset_details._.wait_for_visible()
 
     def history_panel_item_click_visualization_menu(self, hid):
         viz_button_selector = f"{self.history_panel_item_selector(hid)} .visualizations-dropdown"
         self.wait_for_and_click_selector(viz_button_selector)
         self.wait_for_selector_visible(f"{viz_button_selector} .dropdown-menu")
 
     def history_panel_item_available_visualizations_elements(self, hid):
         # Precondition: viz menu has been opened with history_panel_item_click_visualization_menu
         viz_menu_selectors = f"{self.history_panel_item_selector(hid)} a.visualization-link"
-        return self.driver.find_elements_by_css_selector(viz_menu_selectors)
+        return self.driver.find_elements(By.CSS_SELECTOR, viz_menu_selectors)
 
-    def history_panel_item_get_nametags(self, hid):
+    def history_panel_item_get_tags(self, hid):
         item_component = self.history_panel_item_component(hid=hid)
         item_component.wait_for_visible()
-        return [e.text for e in item_component.nametags.all()]
+        return [e.text for e in item_component.alltags.all()]
 
     def history_panel_item_available_visualizations(self, hid):
         # Precondition: viz menu has been opened with history_panel_item_click_visualization_menu
         return [e.text for e in self.history_panel_item_available_visualizations_elements(hid)]
 
     def history_panel_item_click_visualization(self, hid, visualization_name):
         # Precondition: viz menu has been opened with history_panel_item_click_visualization_menu
@@ -1572,15 +1689,15 @@
 
     def collection_builder_clear_filters(self):
         self.wait_for_and_click_selector("a.clear-filters-link")
 
     def collection_builder_click_paired_item(self, forward_or_reverse, item):
         assert forward_or_reverse in ["forward", "reverse"]
         forward_column = self.wait_for_selector_visible(f".{forward_or_reverse}-column .column-datasets")
-        first_datset_forward = forward_column.find_elements_by_css_selector("li")[item]
+        first_datset_forward = forward_column.find_elements(By.CSS_SELECTOR, "li")[item]
         first_datset_forward.click()
 
     def logout_if_needed(self):
         if self.is_logged_in():
             self.home()
             self.logout()
 
@@ -1589,24 +1706,24 @@
         self.click_masthead_user()
         self.components.masthead.logout.wait_for_and_click()
         try:
             self.components.masthead.logged_out_only.wait_for_visible()
         except SeleniumTimeoutException as e:
             message = "Clicked logout button but waiting for 'Login or Registration' button failed, perhaps the logout button was clicked before the handler was setup?"
             raise self.prepend_timeout_message(e, message)
-        assert not self.is_logged_in(), "Clicked to logged out and UI reflects a logout, but API still thinks a user is logged in."
+        assert (
+            not self.is_logged_in()
+        ), "Clicked to logged out and UI reflects a logout, but API still thinks a user is logged in."
 
     def run_tour(self, path, skip_steps=None, sleep_on_steps=None, tour_callback=None):
         skip_steps = skip_steps or []
         sleep_on_steps = sleep_on_steps or {}
         if tour_callback is None:
             tour_callback = NullTourCallback()
-
         self.home()
-
         with open(path) as f:
             tour_dict = yaml.safe_load(f)
         steps = tour_dict["steps"]
         for i, step in enumerate(steps):
             title = step.get("title", None)
             skip = False
             if skip_steps:
@@ -1681,15 +1798,17 @@
 
     def assert_tooltip_text(self, element, expected: Union[str, HasText], sleep: int = 0, click_away: bool = True):
         if hasattr(expected, "text"):
             expected = cast(HasText, expected).text
         text = self.get_tooltip_text(element, sleep=sleep, click_away=click_away)
         assert text == expected, f"Tooltip text [{text}] was not expected text [{expected}]."
 
-    def assert_tooltip_text_contains(self, element, expected: Union[str, HasText], sleep: int = 0, click_away: bool = True):
+    def assert_tooltip_text_contains(
+        self, element, expected: Union[str, HasText], sleep: int = 0, click_away: bool = True
+    ):
         if hasattr(expected, "text"):
             expected = cast(HasText, expected).text
         text = self.get_tooltip_text(element, sleep=sleep, click_away=click_away)
         assert expected in text, f"Tooltip text [{text}] was not expected text [{expected}]."
 
     def assert_error_message(self, contains=None):
         self.components._.messages.error.wait_for_visible()
@@ -1698,48 +1817,58 @@
 
     def assert_warning_message(self, contains=None):
         element = self.components._.messages["warning"]
         return self.assert_message(element, contains=contains)
 
     def assert_message(self, element, contains=None):
         if contains is not None:
-
             if type(element) == list:
-                assert any(contains in el.text for el in element), \
-                    f"{contains} was not found in {[el.text for el in element]}"
+                assert any(
+                    contains in el.text for el in element
+                ), f"{contains} was not found in {[el.text for el in element]}"
                 return
 
             element = element.wait_for_visible()
             text = element.text
             if contains not in text:
                 message = f"Text [{contains}] expected inside of [{text}] but not found."
                 raise AssertionError(message)
 
     def assert_no_error_message(self):
         self.components._.messages.error.assert_absent_or_hidden()
 
     def run_tour_step(self, step, step_index, tour_callback):
+        element_str = step.get("element", None)
+        if element_str is None:
+            component = step.get("component", None)
+            if component is not None:
+                element_str = self.components.resolve_component_locator(component).locator
+
         preclick = step.get("preclick", [])
+        if preclick is True:
+            preclick = [element_str]
+
         for preclick_selector in preclick:
             print(f"(Pre)Clicking {preclick_selector}")
             self._tour_wait_for_and_click_element(preclick_selector)
 
-        element_str = step.get("element", None)
         if element_str is not None:
             print(f"Waiting for element {element_str}")
             element = self.tour_wait_for_element_present(element_str)
             assert element is not None
 
         textinsert = step.get("textinsert", None)
         if textinsert is not None:
             element.send_keys(textinsert)
 
         tour_callback.handle_step(step, step_index)
 
         postclick = step.get("postclick", [])
+        if postclick is True:
+            postclick = [element_str]
         for postclick_selector in postclick:
             print(f"(Post)Clicking {postclick_selector}")
             self._tour_wait_for_and_click_element(postclick_selector)
 
     @retry_during_transitions
     def _tour_wait_for_and_click_element(self, selector):
         element = self.tour_wait_for_clickable_element(selector)
@@ -1754,42 +1883,21 @@
     @retry_during_transitions
     def wait_for_and_click(self, selector_template):
         element = self.wait_for_clickable(selector_template)
         element.click()
         return element
 
     def set_history_annotation(self, annotation, clear_text=False):
-        history_panel = self.components.history_panel
-
-        if self.is_beta_history():
-            toggle = self.beta_history_element("editor toggle")
-            toggle.wait_for_and_click()
-            annotation_input = self.beta_history_element("annotation input").wait_for_visible()
-            if clear_text:
-                annotation_input.clear()
-            annotation_input.send_keys(annotation)
-            save_button = self.beta_history_element("editor save button")
-            save_button.wait_for_and_click()
-        else:
-            self.ensure_history_annotation_area_displayed()
-            editable = history_panel.annotation_editable_text
-            edit = history_panel.annotation_edit
-
-            editable.wait_for_and_click()
-            edit_el = edit.wait_for_and_click()
-            if clear_text:
-                # previously this was just edit_el.clear() but
-                # .clear() doesn't work with beta history panel
-                action_chains = self.action_chains()
-                for _ in range(40):
-                    action_chains.send_keys(Keys.BACKSPACE)
-                action_chains.perform()
-            edit_el.send_keys(annotation)
-
-            history_panel.annotation_done.wait_for_and_click()
+        toggle = self.history_element("editor toggle")
+        toggle.wait_for_and_click()
+        annotation_input = self.history_element("annotation input").wait_for_visible()
+        if clear_text:
+            annotation_input.clear()
+        annotation_input.send_keys(annotation)
+        self.history_click_editor_save()
 
     def ensure_history_annotation_area_displayed(self):
         annotation_area = self.components.history_panel.annotation_area
         annotation_icon = self.components.history_panel.annotation_icon
 
         if annotation_area.is_absent or not annotation_area.is_displayed:
             annotation_icon.wait_for_and_click()
@@ -1800,59 +1908,104 @@
         #                    only the selected value.
         #   with_click=False: This presses enter on the selection. Not sure
         #                     why.
         # with_click seems to work in all situtations - the enter methods
         # doesn't seem to work with the tool form for some reason.
         if hasattr(container_selector_or_elem, "selector"):
             container_selector_or_elem = container_selector_or_elem.selector
-        if not hasattr(container_selector_or_elem, "find_element_by_css_selector"):
+        if not hasattr(container_selector_or_elem, "find_element"):
             container_elem = self.wait_for_selector(container_selector_or_elem)
         else:
             container_elem = container_selector_or_elem
 
-        text_element = container_elem.find_element_by_css_selector("input[type='text']")
+        text_element = container_elem.find_element(By.CSS_SELECTOR, "input[type='text']")
         if clear_value:
             self.send_backspace(text_element)
             self.send_backspace(text_element)
         text_element.send_keys(value)
         # Wait for select2 options to load and then click to add this one.
         drop_elem = self.wait_for_selector_visible("#select2-drop")
         # Sleep seems to be needed - at least for send_enter.
-        time.sleep(.5)
+        time.sleep(0.5)
         if not with_click:
             # Wait for select2 options to load and then click to add this one.
             self.send_enter(text_element)
         else:
-            select_elem = drop_elem.find_elements_by_css_selector(".select2-result-label")[0]
+            candidate_elements = drop_elem.find_elements(By.CSS_SELECTOR, ".select2-result-label")
+            # try to find exact match
+            for elem in candidate_elements:
+                if elem.text == value:
+                    select_elem = elem
+                    break
+            else:
+                # Pick first match. We're replacing select2 anyway ...
+                select_elem = candidate_elements[0]
             action_chains = self.action_chains()
             action_chains.move_to_element(select_elem).click().perform()
         self.wait_for_selector_absent_or_hidden("#select2-drop")
 
     def snapshot(self, description):
         """Test case subclass overrides this to provide detailed logging."""
 
-    def open_history_editor(self, scope=".beta.history"):
-        if self.is_beta_history():
-            panel = self.components.history_panel.editor.selector(scope=scope)
+    def open_history_editor(self, scope=".history-index"):
+        panel = self.components.history_panel.editor.selector(scope=scope)
+        if panel.name_input.is_absent:
             toggle = panel.toggle
             toggle.wait_for_and_click()
             editor = panel.form
             editor.wait_for_present()
 
-    def close_history_editor(self, scope=".beta.history"):
-        if self.is_beta_history():
-            toggle = self.components.history_panel.edit_toggle
-            toggle.wait_for_and_click()
-            editor = self.components.history_panel.editor.selector(scope=scope)
-            self.assert_absent_or_hidden(editor)
+    def close_history_editor(self, scope=".history-index"):
+        toggle = self.components.history_panel.edit_toggle
+        toggle.wait_for_and_click()
+        editor = self.components.history_panel.editor.selector(scope=scope)
+        self.assert_absent_or_hidden(editor)
+
+    def share_ensure_by_user_available(self, sharing_component):
+        collapse = sharing_component.share_with_collapse
+        collapse.wait_for_visible()
+        if collapse.has_class("collapsed"):
+            collapse.wait_for_and_click()
+        sharing_component.share_with_multiselect.wait_for_visible()
+
+    def share_unshare_with_user(self, sharing_component, email):
+        self.share_ensure_by_user_available(sharing_component)
+        unshare_user_button = self.components.histories.sharing.unshare_with_user_button(email=email)
+        unshare_user_button.wait_for_and_click()
+        self.components.histories.sharing.submit_sharing_with.wait_for_and_click()
+        unshare_user_button.wait_for_absent_or_hidden()
+
+    def share_with_user(
+        self,
+        sharing_component,
+        user_id=None,
+        user_email=None,
+        screenshot_before_submit=None,
+        screenshot_after_submit=None,
+        assert_valid=False,
+    ):
+        self.share_ensure_by_user_available(sharing_component)
+        multiselect = sharing_component.share_with_multiselect.wait_for_and_click()
+        sharing_component.share_with_input.wait_for_and_send_keys(user_id or user_email)
+        self.send_enter(multiselect)
 
+        self.screenshot_if(screenshot_before_submit)
+        sharing_component.submit_sharing_with.wait_for_and_click()
 
-class NotLoggedInException(SeleniumTimeoutException):
+        if assert_valid:
+            self.assert_no_error_message()
+
+            xpath = f'//span[contains(text(), "{user_email}")]'
+            self.wait_for_xpath_visible(xpath)
+        self.screenshot_if(screenshot_after_submit)
+
+    def tutorial_mode_activate(self):
+        search_selector = "#gtn a"
+        self.wait_for_and_click_selector(search_selector)
+        self.wait_for_selector_visible("#gtn-screen")
 
+
+class NotLoggedInException(SeleniumTimeoutException):
     def __init__(self, timeout_exception, user_info, dom_message):
         template = "Waiting for UI to reflect user logged in but it did not occur. API indicates no user is currently logged in. %s API response was [%s]. %s"
         msg = template % (dom_message, user_info, timeout_exception.msg)
-        super().__init__(
-            msg=msg,
-            screen=timeout_exception.screen,
-            stacktrace=timeout_exception.stacktrace
-        )
+        super().__init__(msg=msg, screen=timeout_exception.screen, stacktrace=timeout_exception.stacktrace)
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/scripts/dump_tour.py` & `galaxy-selenium-23.0.1/galaxy/selenium/scripts/dump_tour.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,28 +24,27 @@
     else:
         os.makedirs(output)
     callback = DumpTourCallback(driver_wrapper, output)
     driver_wrapper.run_tour(args.tour, tour_callback=callback)
 
 
 class DumpTourCallback:
-
     def __init__(self, driver_wrapper, output):
         self.driver_wrapper = driver_wrapper
         self.output = output
 
     def handle_step(self, step, step_index):
-        time.sleep(.5)
+        time.sleep(0.5)
         self.driver_wrapper.driver.save_screenshot("%s/%i.png" % (self.output, step_index))
-        time.sleep(.5)
+        time.sleep(0.5)
 
 
 def _arg_parser():
     parser = argparse.ArgumentParser(description=DESCRIPTION)
-    parser.add_argument('tour', metavar='TOUR', help='tour to walk')
-    parser.add_argument('-o', '--output', default="tour_dump_TIMESTAMP", help='directory to dump tour to')
+    parser.add_argument("tour", metavar="TOUR", help="tour to walk")
+    parser.add_argument("-o", "--output", default="tour_dump_TIMESTAMP", help="directory to dump tour to")
     parser = cli.add_selenium_arguments(parser)
     return parser
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/sizzle.py` & `galaxy-selenium-23.0.1/galaxy/selenium/sizzle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for using sizzle (jQuery-style) selectors with Selenium."""
 
 import json
 
 from selenium.common.exceptions import NoSuchElementException
-from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support.wait import WebDriverWait
 
 from .has_driver import exception_indicates_stale_element
 
 SIZZLE_LOAD_TIMEOUT = 5
 SIZZLE_URL = "//cdnjs.cloudflare.com/ajax/libs/sizzle/1.10.18/sizzle.js"
 
 
@@ -68,17 +68,15 @@
 
     :param sizzle_selector: The sizzle selector to use when finding element.
     """
     elements = driver.find_elements_by_sizzle(sizzle_selector)
     if elements:
         return elements[0]
     else:
-        raise NoSuchElementException(
-            f"Unable to locate element by Sizzle: {sizzle_selector}"
-        )
+        raise NoSuchElementException(f"Unable to locate element by Sizzle: {sizzle_selector}")
 
 
 def find_elements_by_sizzle(driver, sizzle_selector: str):
     """
     Finds elements by sizzle selector.
 
     :param sizzle_selector: The sizzle selector to use when finding elements.
@@ -86,35 +84,37 @@
     if not _is_sizzle_loaded(driver):
         _inject_sizzle(driver, SIZZLE_URL, SIZZLE_LOAD_TIMEOUT)
     elements = driver.execute_script(_make_sizzle_string(sizzle_selector))
     return elements
 
 
 def _inject_sizzle(driver, sizzle_url, timeout):
-    script = """
+    script = (
+        """
         if(typeof(window.$) != "undefined") {
             // Just reuse jQuery if it is available, avoids potential amd problems
             // that have cropped up with Galaxy for instance.
             window.Sizzle = window.$;
         } else {
             var _s = document.createElement("script");
             _s.type = "text/javascript";
             _s.src = "%s";
             var _h = document.getElementsByTagName("head")[0];
             _h.appendChild(_s);
         }
-    """ % sizzle_url
+    """
+        % sizzle_url
+    )
     driver.execute_script(script)
     wait = WebDriverWait(driver, timeout)
-    wait.until(lambda d: _is_sizzle_loaded(d),
-               f"Can't inject Sizzle in {timeout} seconds")
+    wait.until(lambda d: _is_sizzle_loaded(d), f"Can't inject Sizzle in {timeout} seconds")
 
 
 def _is_sizzle_loaded(driver):
-    script = "return typeof(Sizzle) != \"undefined\";"
+    script = 'return typeof(Sizzle) != "undefined";'
     return driver.execute_script(script)
 
 
 def _make_sizzle_string(sizzle_selector):
     # Use json.dumps to escape quotes
     selector = json.dumps(sizzle_selector)
     return f"return Sizzle({selector});"
```

### Comparing `galaxy-selenium-22.1.1/galaxy/selenium/smart_components.py` & `galaxy-selenium-23.0.1/galaxy/selenium/smart_components.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from .components import (
+from selenium.webdriver.support.select import Select
+
+from galaxy.navigation.components import (
     Component,
     Target,
 )
 
 
 class SmartComponent:
     """Wrap a Component with driver aware methods.
 
-    Allows smarter selectors that know how to wait for themselves, test themselves,
+    Adapts Galaxy's component locators more tightly to Selenium - including a Selenium
+    runtime. Allows smarter selectors that know how to wait for themselves, test themselves,
     click themselves, etc.... More "magic", but much cleaner usage.
     """
 
     def __init__(self, component, has_driver):
         self._component = component
         self._has_driver = has_driver
 
@@ -27,16 +30,15 @@
         elif isinstance(simple_object, Target):
             return SmartTarget(simple_object, self._has_driver)
         else:
             return simple_object
 
 
 class SmartTarget:
-    """Wrap a Target with driver aware methods.
-    """
+    """Wrap a Target with driver aware methods."""
 
     def __init__(self, target, has_driver):
         self._target = target
         self._has_driver = has_driver
 
     def __call__(self, *args, **kwds):
         return self._wrap(self._target(*args[:], **kwds.copy()))
@@ -52,20 +54,26 @@
             return SmartTarget(simple_object, self._has_driver)
         else:
             return simple_object
 
     def all(self):
         return self._has_driver.driver.find_elements(*self._target.element_locator)
 
+    def wait_for_element_count_of_at_least(self, n: int, **kwds):
+        self._has_driver.wait_for_element_count_of_at_least(self._target, n, **kwds)
+
     def wait_for_and_click(self, **kwds):
         return self._has_driver.wait_for_and_click(self._target, **kwds)
 
     def wait_for_visible(self, **kwds):
         return self._has_driver.wait_for_visible(self._target, **kwds)
 
+    def wait_for_select(self, **kwds):
+        return Select(self.wait_for_visible(**kwds))
+
     def wait_for_clickable(self, **kwds):
         return self._has_driver.wait_for_clickable(self._target, **kwds)
 
     def wait_for_text(self, **kwds):
         return self._has_driver.wait_for_visible(self._target, **kwds).text
 
     def wait_for_value(self, **kwds):
@@ -93,12 +101,16 @@
 
     def assert_absent_or_hidden(self, **kwds):
         self._has_driver.assert_absent_or_hidden(self._target, **kwds)
 
     def assert_absent_or_hidden_after_transitions(self, **kwds):
         self._has_driver.assert_absent_or_hidden_after_transitions(self._target, **kwds)
 
+    def assert_disabled(self, **kwds):
+        self._has_driver.assert_disabled(self._target, **kwds)
+
     def has_class(self, class_name):
-        return class_name in self._has_driver.driver.find_element(*self._target.element_locator).get_attribute("class")
+        classes_str = self._has_driver.driver.find_element(*self._target.element_locator).get_attribute("class") or ""
+        return class_name in classes_str.split(" ")
 
     def wait_for_and_send_keys(self, *text):
         self.wait_for_visible().send_keys(*text)
```

### Comparing `galaxy-selenium-22.1.1/galaxy_selenium.egg-info/PKG-INFO` & `galaxy-selenium-23.0.1/galaxy_selenium.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 22.1.1
-Summary: Galaxy Selenium Interaction Framework
+Version: 23.0.1
+Summary: Galaxy Selenium interaction framework
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
 
 
 .. image:: https://badge.fury.io/py/galaxy-selenium.svg
    :target: https://pypi.org/project/galaxy-selenium/
 
 
 
 Overview
 --------
 
 The Galaxy_ selenium framework.
 
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
-20.9.1.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
+
 
+============
+Enhancements
+============
 
+* Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
 
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
-
-
```

### Comparing `galaxy-selenium-22.1.1/galaxy_selenium.egg-info/SOURCES.txt` & `galaxy-selenium-23.0.1/galaxy_selenium.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
 dev-requirements.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 test-requirements.txt
 galaxy/__init__.py
-galaxy/project_galaxy_selenium.py
+galaxy/py.typed
 galaxy/selenium/__init__.py
 galaxy/selenium/cli.py
-galaxy/selenium/components.py
 galaxy/selenium/context.py
-galaxy/selenium/data.py
 galaxy/selenium/driver_factory.py
 galaxy/selenium/has_driver.py
 galaxy/selenium/jupyter_context.py
 galaxy/selenium/navigates_galaxy.py
-galaxy/selenium/navigation.yml
 galaxy/selenium/sizzle.py
 galaxy/selenium/smart_components.py
 galaxy/selenium/scripts/__init__.py
 galaxy/selenium/scripts/dump_tour.py
 galaxy/selenium/toolbox/__init__.py
 galaxy/selenium/toolbox/filters.py
 galaxy_selenium.egg-info/PKG-INFO
 galaxy_selenium.egg-info/SOURCES.txt
 galaxy_selenium.egg-info/dependency_links.txt
 galaxy_selenium.egg-info/entry_points.txt
-galaxy_selenium.egg-info/not-zip-safe
 galaxy_selenium.egg-info/requires.txt
-galaxy_selenium.egg-info/top_level.txt
-scripts/commit_version.py
-scripts/new_version.py
-scripts/print_version_for_release.py
+galaxy_selenium.egg-info/top_level.txt
```

