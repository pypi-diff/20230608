# Comparing `tmp/mighty_logger-0.5.0.tar.gz` & `tmp/mighty_logger-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.5.0.tar", last modified: Thu Apr 13 16:58:05 2023, max compression
+gzip compressed data, was "mighty_logger-0.5.1.tar", last modified: Thu Jun  8 16:17:12 2023, max compression
```

## Comparing `mighty_logger-0.5.0.tar` & `mighty_logger-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:58:05.973991 mighty_logger-0.5.0/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     9583 2023-04-13 16:58:05.973991 mighty_logger-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     8638 2023-04-13 16:21:44.000000 mighty_logger-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:58:05.928671 mighty_logger-0.5.0/mighty_logger/
--rw-rw-rw-   0        0        0      819 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:58:05.962485 mighty_logger-0.5.0/mighty_logger/basic/
--rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.5.0/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     5175 2023-04-12 11:20:05.000000 mighty_logger-0.5.0/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.5.0/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.5.0/mighty_logger/basic/patterns.py
--rw-rw-rw-   0        0        0     3108 2023-04-12 10:25:59.000000 mighty_logger-0.5.0/mighty_logger/basic/text_buffer_type.py
--rw-rw-rw-   0        0        0    46277 2023-04-12 09:02:23.000000 mighty_logger-0.5.0/mighty_logger/powerful_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:58:05.968015 mighty_logger-0.5.0/mighty_logger/src/
--rw-rw-rw-   0        0        0      883 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     4570 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8657 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/src/color_picker.py
--rw-rw-rw-   0        0        0      728 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/src/log_environment.py
--rw-rw-rw-   0        0        0      171 2023-04-11 12:29:17.000000 mighty_logger-0.5.0/mighty_logger/src/~status_variables.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:58:05.971991 mighty_logger-0.5.0/mighty_logger/text/
--rw-rw-rw-   0        0        0      701 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/text/__init__.py
--rw-rw-rw-   0        0        0     4863 2023-04-12 10:50:05.000000 mighty_logger-0.5.0/mighty_logger/text/text_buffer.py
--rw-rw-rw-   0        0        0     4822 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/text/~animation.py
--rw-rw-rw-   0        0        0     1704 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/mighty_logger/text/~icon_set.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:58:05.942013 mighty_logger-0.5.0/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0     9583 2023-04-13 16:58:05.000000 mighty_logger-0.5.0/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-04-13 16:58:05.000000 mighty_logger-0.5.0/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:58:05.000000 mighty_logger-0.5.0/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 16:58:05.000000 mighty_logger-0.5.0/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:58:05.974992 mighty_logger-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2800 2023-04-10 16:24:05.000000 mighty_logger-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.349214 mighty_logger-0.5.1/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    10255 2023-06-08 16:17:12.350214 mighty_logger-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9290 2023-06-08 12:57:30.000000 mighty_logger-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.268080 mighty_logger-0.5.1/mighty_logger/
+-rw-rw-rw-   0        0        0      823 2023-06-08 16:11:27.000000 mighty_logger-0.5.1/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.304869 mighty_logger-0.5.1/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.5.1/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     5454 2023-06-06 13:48:02.000000 mighty_logger-0.5.1/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.5.1/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.5.1/mighty_logger/basic/patterns.py
+-rw-rw-rw-   0        0        0     3125 2023-06-08 10:41:07.000000 mighty_logger-0.5.1/mighty_logger/basic/text_buffer_type.py
+-rw-rw-rw-   0        0        0    47848 2023-06-08 10:41:07.000000 mighty_logger-0.5.1/mighty_logger/powerful_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.320295 mighty_logger-0.5.1/mighty_logger/src/
+-rw-rw-rw-   0        0        0      935 2023-06-07 17:37:14.000000 mighty_logger-0.5.1/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     4570 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8657 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0      728 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/src/log_environment.py
+-rw-rw-rw-   0        0        0     5640 2023-06-08 10:15:33.000000 mighty_logger-0.5.1/mighty_logger/src/status_variables.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.325296 mighty_logger-0.5.1/mighty_logger/text/
+-rw-rw-rw-   0        0        0      789 2023-06-08 15:16:03.000000 mighty_logger-0.5.1/mighty_logger/text/__init__.py
+-rw-rw-rw-   0        0        0     2373 2023-06-08 15:16:03.000000 mighty_logger-0.5.1/mighty_logger/text/icon_set.py
+-rw-rw-rw-   0        0        0     4993 2023-06-08 14:51:35.000000 mighty_logger-0.5.1/mighty_logger/text/text_buffer.py
+-rw-rw-rw-   0        0        0     4822 2023-04-10 16:24:05.000000 mighty_logger-0.5.1/mighty_logger/text/~animation.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.272078 mighty_logger-0.5.1/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10255 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-08 16:17:12.000000 mighty_logger-0.5.1/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:17:12.351217 mighty_logger-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2796 2023-06-08 16:11:27.000000 mighty_logger-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:17:12.348215 mighty_logger-0.5.1/test/
+-rw-rw-rw-   0        0        0     1239 2023-06-08 14:24:28.000000 mighty_logger-0.5.1/test/test_console.py
+-rw-rw-rw-   0        0        0     1184 2023-06-08 15:16:03.000000 mighty_logger-0.5.1/test/test_html.py
```

### Comparing `mighty_logger-0.5.0/LICENSE` & `mighty_logger-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/PKG-INFO` & `mighty_logger-0.5.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,180 @@
-Metadata-Version: 2.1
-Name: mighty_logger
-Version: 0.5.0
-Summary: Powerful functional logger with support for qt programming
-Home-page: https://github.com/Nakama3942/qt_colored_logger
-Author: Kalynovsky 'Nakama3942' Valentin
-Author-email: nakama3942@gmail.com
-License: Apache License, Version 2.0, see LICENSE file
-Project-URL: Releases, https://github.com/Nakama3942/qt_colored_logger/releases
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Logging
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-[![template](https://img.shields.io/badge/Repository-template-darkred)](https://github.com/Nakama3942/template_rep)
-[![GitHub license](https://img.shields.io/github/license/Nakama3942/qt_colored_logger?color=gold&style=flat-square)](https://github.com/Nakama3942/qt_colored_logger/blob/master/LICENSE)
-
-![PyPI](https://img.shields.io/pypi/v/qt-colored-logger?color=yellow&logo=pypi&logoColor=white&style=flat-square)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/qt_colored_logger?label=latest%20release&logo=github&style=flat-square)
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/qt_colored_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=flat-square)
-![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/qt_colored_logger/v0.3.0?include_prereleases&style=flat-square)
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qt_colored_logger?style=flat-square)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/qt_colored_logger?style=flat-square)
-![PyPI - Format](https://img.shields.io/pypi/format/qt_colored_logger?label=PyPI%20format&style=flat-square)
-![PyPI - Status](https://img.shields.io/pypi/status/qt_colored_logger?label=PyPI%20status&style=flat-square)
-
-![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/qt_colored_logger?style=flat-square)
-![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/qt_colored_logger?style=flat-square)
-![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/qt_colored_logger?label=%28pre-%29release%20date&style=flat-square)
-
-![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/qt_colored_logger?color=darkgreen&style=flat-square)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/qt_colored_logger?color=darkgreen&style=flat-square)
-
-[![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CHANGELOG.md)
-[![CONTRIBUTING](https://img.shields.io/badge/here-CONTRIBUTING-indigo)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CONTRIBUTING.md)
-[![CODE_OF_CONDUCT](https://img.shields.io/badge/here-CODE_OF_CONDUCT-darkgreen)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CODE_OF_CONDUCT.md)
-[![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange)](https://github.com/Nakama3942/qt_colored_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
-
-</div>
-
-# Mighty Logger
-### Content
-- [Qt_Сolored-logger](#mighty-logger)
-	- [Content](#content)
-	- [Preamble](#preamble)
-	- [Overview](#overview)
-    - [Important releases](#important-releases)
-	- [LICENSE](#license)
-	- [Installation](#installation)
-	- [Usage](#usage)
-	- [Additional functionality](#additional-functionality)
-	- [Data](#data)
-	- [Troubleshooting](#troubleshooting)
-	- [Authors](#authors)
-
-## Preamble
-I often came across the opinion that it is better to use not standard output to the console, but full-fledged logging... However, the standard libraries do not provide exactly what I need... Therefore, I decided to make my own library! Which will implement the functionality I need.
-
-I was inspired by the [colored-logs](https://pypi.org/project/colored-logs/) library.
-
-- [Content](#content)
-
-## Overview
-The library implements the formation of a beautifully formatted colored text, similar to a log, which has all the necessary information:
-- Device name and registered profile, system name, etc. (this data is displayed only once at the beginning of the logging)
-- Log entry time
-- Log entry status
-- Description of the log entry status
-- Log entry type
-- Entry message
-
-Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background.
-
-- [Content](#content)
-
-## Important releases
-<details><summary>See the important releases (possible spoilers)</summary>
-
-- [x] v0.1.0 - First official release (complete basic HTML logger)
-- [x] v0.2.0 - Structural update (added basic console logger with HTML base)
-- [x] v0.3.0 - Background update (added background for log entries)
-- [x] v0.4.0 - Buffer update (added text buffer)
-- [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
-- [ ] v0.5.1 - Symbols update (added hint symbols near log entries types)
-- [ ] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [ ] v0.7.0 - Animation update (added animations in processes)
-- [ ] v0.8.0 - Search update (added search by log entry types)
-- [ ] v0.8.1 - Extension update (made wheel format and instruction of toml)
-- [ ] v1.0.0 - Completion of logger development (logger development completed)
-- [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
-
-</details>
-
-- [Content](#content)
-
-## LICENSE
-The full text of the license can be found at the following [link](https://github.com/Nakama3942/qt_colored_logger/blob/master/LICENSE).
-
-> Copyright © 2023 Kalynovsky Valentin. All rights reserved.
->
-> Licensed under the Apache License, Version 2.0 (the "License");
-> you may not use this file except in compliance with the License.
-> You may obtain a copy of the License at
->
->     http://www.apache.org/licenses/LICENSE-2.0
->
-> Unless required by applicable law or agreed to in writing, software
-> distributed under the License is distributed on an "AS IS" BASIS,
-> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-> See the License for the specific language governing permissions and
-
-- [Content](#content)
-
-## Installation
-Despite the fact that the library was originally developed for use in PyQt, it does not require PyQt to be installed, since this framework for outputting to Text fields, which support not only Plain Text, uses HTML and this library simply simplifies the logging process, since the creation process already formatted strings is registered in this library.
-
-To install the library, enter the command:
-```sh
-pip install mighty_logger
-```
-
-## Usage
-This is the simplest example of using the library:
-```python
-from mighty_logger import Logger
-
-if __name__ == "__main__":
-	logger = Logger(program_name="Test", console_width=115)
-	logger.message(status_message_text="Hooray", message_text="Hello world!")
-```
-
-The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
-> <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
-> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-04-09 12:37:07.198496 </span><span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
-
-See the APPLYING.md file for more details.
-
-- [Content](#content)
-
-## *Additional functionality*
-*Additional functionality is also planned. Let's keep it a secret for now. Let it be a surprise.*
-
-- [Content](#content)
-
-## Data
-See the DATA.md file.
-
-- [Content](#content)
-
-## Troubleshooting
-All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/qt_colored_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/qt_colored_logger/blob/master/CODE_OF_CONDUCT.md).
-
-- [Content](#content)
-
-## Authors
-<table align="center" style="border-width: 10; border-style: ridge">
-	<tr>
-		<td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
-		<!--<td></td>-->
-	</tr>
-<!--
-	<tr>
-		<td></td>
-		<td></td>
-	</tr>
--->
-</table>
+<div align="center">
+
+[![template](https://img.shields.io/badge/Repository-template-darkred?style=for-the-badge)](https://github.com/Nakama3942/template_rep)
+[![GitHub license](https://img.shields.io/github/license/Nakama3942/mighty_logger?color=gold&style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE)
+[![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/CHANGELOG.md)
+[![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
+
+![PyPI](https://img.shields.io/pypi/v/mighty-logger?color=yellow&logo=pypi&logoColor=white&style=for-the-badge)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?label=latest%20release&logo=github&style=for-the-badge)
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=for-the-badge)
+![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/mighty_logger/v0.5.0?include_prereleases&style=for-the-badge)
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mighty-logger?style=for-the-badge)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/mighty-logger?style=for-the-badge)
+![PyPI - Format](https://img.shields.io/pypi/format/mighty-logger?label=PyPI%20format&style=for-the-badge)
+![PyPI - Status](https://img.shields.io/pypi/status/mighty-logger?label=PyPI%20status&style=for-the-badge)
+
+![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/mighty_logger?style=for-the-badge)
+![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/mighty_logger?style=for-the-badge)
+![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/mighty_logger?label=%28pre-%29release%20date&style=for-the-badge)
+
+![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
+![Lines of code](https://img.shields.io/tokei/lines/github/Nakama3942/mighty_logger?style=for-the-badge)
+
+</div>
+
+# Mighty Logger
+
+### Content
+
+- [Qt_Сolored-logger](#mighty-logger)
+  - [Content](#content)
+  - [Preamble](#preamble)
+  - [Overview](#overview)
+  - [Important releases](#important-releases)
+  - [LICENSE](#license)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Additional functionality](#additional-functionality)
+  - [Data](#data)
+  - [Troubleshooting](#troubleshooting)
+  - [Authors](#authors)
+
+## Preamble
+
+<!--
+This library it was renamed to "Mighty logger" but before this library named is "Qt Colored logger". Old commits may search in this repository, but download old build may on next link: https://pypi.org/project/qt-colored-logger/ .
+-->
+
+> I often came across the opinion that it is better to use not standard output to the console, but full-fledged logging... However, the standard libraries do not provide exactly what I need... Therefore, I decided to make my own library! Which will implement the functionality I need.
+
+I was inspired by the [colored-logs](https://pypi.org/project/colored-logs/) library.
+
+---
+
+*This library has been renamed to "Mighty logger", but this library used to be called "Qt Colored logger". You can search for old commits in this repository, but you can download the old build from the [link](https://pypi.org/project/qt-colored-logger/).*
+
+- [Content](#content)
+
+## Overview
+
+The library implements the formation of a beautifully formatted colored text, similar to a log, which has all the necessary information:
+
+- Device name and registered profile, system name, etc. (this data is displayed only once at the beginning of the logging)
+- Log entry time
+- Log entry status
+- Log entry type
+- Entry message
+
+Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background, icons ~~and animations~~.
+
+- [Content](#content)
+
+## Important releases
+
+<details><summary>See the important releases (possible spoilers)</summary>
+
+- [x] v0.1.0 - First official release (complete basic HTML logger)
+- [x] v0.2.0 - Structural update (added basic console logger with HTML base)
+- [x] v0.3.0 - Background update (added background for log entries)
+- [x] v0.4.0 - Buffer update (added text buffer)
+- [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
+- [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
+- [ ] v0.6.0 - Progress update (added start of some log entries in threads (process))
+- [ ] v0.6.1 - Animation update (added animations in processes)
+- [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
+- [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
+- [ ] v0.7.2 - Search update (added search by log entry types)
+- [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
+- [ ] v1.0.0 - Completion of logger development (logger development completed)
+- [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
+
+</details>
+
+- [Content](#content)
+
+## LICENSE
+
+The full text of the license can be found at the following [link](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE).
+
+> Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+> 
+> Licensed under the Apache License, Version 2.0 (the "License");
+> you may not use this file except in compliance with the License.
+> You may obtain a copy of the License at
+> 
+>     http://www.apache.org/licenses/LICENSE-2.0
+> 
+> Unless required by applicable law or agreed to in writing, software
+> distributed under the License is distributed on an "AS IS" BASIS,
+> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+> See the License for the specific language governing permissions and
+
+- [Content](#content)
+
+## Installation
+
+Despite the fact that the library was originally developed for use in PyQt, it does not require PyQt to be installed, since this framework for outputting to Text fields, which support not only Plain Text, uses HTML and this library simply simplifies the logging process, since the creation process already formatted strings is registered in this library.
+
+To install the library, enter the command:
+
+```sh
+pip install mighty_logger
+```
+
+## Usage
+
+This is the simplest example of using the library:
+
+```python
+from mighty_logger import Logger
+from mighty_logger.src import StatusMessagePatterns
+
+if __name__ == "__main__":
+    logger = Logger(program_name="Test", console_width=115)
+    logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
+```
+
+The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
+
+> <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
+> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
+
+See the APPLYING.md file for more details.
+
+- [Content](#content)
+
+## *Additional functionality*
+
+*Additional functionality is also planned. Let's keep it a secret for now. Let it be a surprise.*
+
+- [Content](#content)
+
+## Data
+
+See the DATA.md file.
+
+- [Content](#content)
+
+## Troubleshooting
+
+All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
+
+- [Content](#content)
+
+## Authors
+
+<table align="center" style="border-width: 10; border-style: ridge">
+    <tr>
+        <td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
+        <!--<td></td>-->
+    </tr>
+<!--
+    <tr>
+        <td></td>
+        <td></td>
+    </tr>
+-->
+</table>
```

### Comparing `mighty_logger-0.5.0/mighty_logger/__init__.py` & `mighty_logger-0.5.1/mighty_logger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .powerful_logger import Logger
 
-__authot__ = "Kalynovsky 'Nakama3942' Valentin"
-__version__ = "0.5.0"
+__authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
+__version__ = "0.5.1"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.5.0/mighty_logger/basic/__init__.py` & `mighty_logger-0.5.1/mighty_logger/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.5.1/mighty_logger/basic/basic_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 					f"<span style='background-color: #{colors[1]};'>" +
 					f"<span style='color: #{colors[0]};'>-{self._program_name}?entry> " +
 					f"${platform.node()}^{os.getlogin()}" +
 					f"@{platform.system()}" +
 					f":{platform.version()}" +
 					":{}:{}".format(*platform.architecture()) +
 					f":{platform.machine()}" +
-					f"</span></span><br>"
+					f"</span></span>"
 			)
 		else:
 			return (
 					f"{colors[1]}" +
 					f"{colors[0]}-{self._program_name}?entry> " +
 					f"${platform.node()}^{os.getlogin()}" +
 					f"@{platform.system()}" +
@@ -64,24 +64,28 @@
 					f":{platform.machine()}" +
 					f"{GetAnsiFormat('reset/on')}"
 			)
 
 	def _assemble_entry(
 			self,
 			colors: list[str, str, str, str, str, str],
+			animation: list,
+			icon: str,
 			status_message_text: str,
 			message_type: str,
 			message_text: str,
 			env: str,
 			local_settings: dict
 	) -> str:
 		"""
 		A method that assemble an entry into a string and returns it.
 
 		:param colors: 6 colors that the method uses to assemble the string
+		:param animation: Animation of entry
+		:param icon: Type icon
 		:param status_message_text: Status message
 		:param message_type: Entry type
 		:param message_text: Entry message
 		:param env: For what environment is the string formed?
 		:param local_settings: Settings for the string of the current entry
 		:return: the formed entry string
 		"""
@@ -94,30 +98,32 @@
 		status_type_entry = local_settings['status_type_local_entry'] if 'status_type_local_entry' in local_settings else self._settings['status_type_global_entry']
 		message_entry = local_settings['message_local_entry'] if 'message_local_entry' in local_settings else self._settings['message_global_entry']
 		if env == LogEnvironments.HTML:
 			return (
 					(f"<b>" if bold else "") +
 					(f"<i>" if italic else "") +
 					f"<span style='background-color: #{colors[5]};'>" +
-					f"<span style='color: #{colors[4]};'>-?entry> </span>" +
+					f"<span style='color: #{colors[4]};'>-?entry> {animation[0]}</span>" +  # todo Must add animation
 					(f"<span style='color: #{colors[0]};'>*{datetime.datetime.now()} </span>" if time_entry else "") +
+					f"<div style='display: inline-block; white-space: pre; tab-size: 4'>{icon}&#9;</div>" +
 					(f"<span style='color: #{colors[1]};'>#STATUS: </span>" if status_entry else "") +
 					(f"<span style='color: #{colors[2]};'>{status_message_text} </span>" if status_message_entry else "") +
 					(f"<span style='color: #{colors[3]};'>{message_type} - </span>" if status_type_entry else "") +
 					(f"<span style='color: #{colors[4]};'>{message_text}</span></span>" if message_entry else "") +
 					(f"</i>" if italic else "") +
-					(f"</b>" if bold else "") + "<br>"
+					(f"</b>" if bold else "")
 			)
 		else:
 			return (
 					(f"{GetAnsiFormat('bold/on')}" if bold else "") +
 					(f"{GetAnsiFormat('italic/on')}" if italic else "") +
 					(f"{GetAnsiFormat('invert/on')}" if invert else "") +
 					f"{colors[5]}" +
-					f"{colors[4]}-?entry> " +
+					f"{colors[4]}-?entry> {animation[0]}" +  # todo Must add animation
 					(f"{colors[0]}*{datetime.datetime.now()} " if time_entry else "") +
+					f"{icon}\t" +
 					(f"{colors[1]}#STATUS: " if status_entry else "") +
 					(f"{colors[2]}{status_message_text} " if status_message_entry else "") +
 					(f"{colors[3]}{message_type} - " if status_type_entry else "") +
 					(f"{colors[4]}{message_text}" if message_entry else "") +
 					f"{GetAnsiFormat('reset/on')}"
 			)
```

### Comparing `mighty_logger-0.5.0/mighty_logger/basic/exceptions.py` & `mighty_logger-0.5.1/mighty_logger/basic/exceptions.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger/basic/patterns.py` & `mighty_logger-0.5.1/mighty_logger/basic/patterns.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger/basic/text_buffer_type.py` & `mighty_logger-0.5.1/mighty_logger/basic/text_buffer_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 
 from abc import ABC, abstractmethod
 
 class TextBufferType(ABC):
 	def __init__(self) -> None:
 		self._text_buffer: list[str] = []
 
-	def __lshift__(self, other) -> None:
+	def __lshift__(self, entry: str) -> None:
 		"""
 		Used to add a string to the end of the buffer.
 
-		:param other: The line to be added
+		:param entry: The line to be added
 		"""
-		self.append(f"{other}")
+		self.append(f"{entry}")
 
-	def __rshift__(self, other) -> None:
+	def __rshift__(self, entry: str) -> None:
 		"""
 		Used to save a buffer to the file.
 
-		:param other: The name of the file where you want to save the buffer
+		:param entry: The name of the file where you want to save the buffer
 		"""
-		self.save(other)
+		self.save(entry)
 
 	def get_data(self) -> list:
 		"""
 		Returns a list of strings from a text buffer.
 
 		:return: a list of text buffer lines
 		"""
@@ -89,8 +89,8 @@
 	@abstractmethod
 	def update_console(self) -> None:
 		"""
 		Refreshes the console, erasing output text and outputting an updated buffer.
 		"""
 		raise NotImplementedError("Method update_console() is not implemented in the base class.")
 
-	# todo abstractmethod remove(), clear(), -open_save() or load()-
+	# todo v0.7.0 abstractmethod remove(), clear(), -open_save() or load()-
```

### Comparing `mighty_logger-0.5.0/mighty_logger/powerful_logger.py` & `mighty_logger-0.5.1/mighty_logger/powerful_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 """
 
 from mighty_logger.basic.basic_logger import BasicLogger
 from mighty_logger.basic.exceptions import ColorException, CombinationException, ReCreationException
 from mighty_logger.basic.text_buffer_type import TextBufferType
 from mighty_logger.src.color_picker import AnsiColor, HexColor, Dec2Ansi, Dec2Hex
 from mighty_logger.src.log_environment import LogEnvironments
+from mighty_logger.src.status_variables import StatusMessageType
+from mighty_logger.text.icon_set import IconSetType, IconSet1
 from mighty_logger.text.text_buffer import BasicTextBuffer, TextBuffer
 
 class Logger(BasicLogger):
 	"""
 	The Logger class is a class that implements the functionality
 	of logging the work of software in different directions.\n
 	It has a color output of information, settings for the operation of the log.
@@ -41,26 +43,28 @@
 
 	def __init__(
 			self,
 			*,
 			program_name: str = "Unknown",
 			log_environment: str = LogEnvironments.CONSOLE,
 			console_width: int = 60,
+			icon_set: IconSetType = IconSet1(),
 			time_global_entry: bool = True,
 			status_global_entry: bool = True,
 			status_message_global_entry: bool = True,
 			status_type_global_entry: bool = True,
 			message_global_entry: bool = True,
 			global_bold_font: bool = False,
 			global_italic_font: bool = False,
 			global_invert_font: bool = False,
 			global_background: bool = False,
 	) -> None:
 		if not hasattr(self, "_ColorScheme"):
 			super().__init__(program_name)
+			self._icon_set = icon_set
 			self._settings["global_bold_font"] = global_bold_font
 			self._settings["global_italic_font"] = global_italic_font
 			self._settings["global_invert_font"] = global_invert_font
 			self._settings["time_global_entry"] = time_global_entry
 			self._settings["status_global_entry"] = status_global_entry
 			self._settings["status_message_global_entry"] = status_message_global_entry
 			self._settings["status_type_global_entry"] = status_type_global_entry
@@ -70,25 +74,25 @@
 			self.global_background = global_background
 			self._color_scheme_init()
 			if self._environment == LogEnvironments.CONSOLE:
 				if TextBuffer._instance is not None:
 					self._buffer = TextBuffer._instance
 					self.notice(
 						message_text="An existing logger was taken into use",
-						status_message_text="Note",
+						status_message=StatusMessageType("Note"),
 						local_settings={"italic": True}
 					)
 				else:
 					self._buffer = TextBuffer(console_width)
 			else:
 				if BasicTextBuffer._instance is not None:
 					self._buffer = BasicTextBuffer._instance
 					self.notice(
 						message_text="An existing logger was taken into use",
-						status_message_text="Note",
+						status_message=StatusMessageType("Note"),
 						local_settings={"italic": True}
 					)
 				else:
 					self._buffer = BasicTextBuffer()
 			self._initial_log()
 		else:
 			raise ReCreationException("Logger class object already created")
@@ -340,14 +344,25 @@
 				self._ColorScheme['INITIAL_COLOR'][self.global_background],
 				self._ColorScheme['INITIAL_BACKGROUND'][self.global_background]
 			], self._environment
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
+	# def set_animation(self):
+	# 	pass
+
+	def set_icons(self, icon_set: IconSetType):
+		"""
+		Changes the current icon set used by the Logger.
+
+		:param icon_set: Icon set to use
+		"""
+		self._icon_set = icon_set
+
 	def set_color(self, *, logger_color_name: str, color_value: list[int, int, int], foreground: bool = True, background: bool = False) -> None:
 		"""
 		A method that sets the ANSI escape code color in the color table of the logger.
 		May throw a ColorException if the given color is not in the table.
 		The logger color table stores the following keys: see /docs/DATA.md/"Logger Color Scheme".\n
 		Boolean flags: If foreground is set to True, then the color of the foreground text will change
 		with/without a background (it all depends on the background flag). If in this case background
@@ -379,22 +394,22 @@
 		The Text Buffer object is created in the class constructor and this
 		method is used to access it. It returns a buffer.
 
 		:return: a text buffer object
 		"""
 		return self._buffer
 
-	#todo сделать конвертер из Console в HTML и наоборот
+	#todo v0.7.1 сделать конвертер из Console в HTML и наоборот
 
-	def debug(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def debug(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -402,26 +417,26 @@
 			[
 				self._ColorScheme['DEBUG_TIME'][background],
 				self._ColorScheme['DEBUG_STATUS'][background],
 				self._ColorScheme['DEBUG_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_DEBUG'][background],
 				self._ColorScheme['DEBUG_MESSAGE'][background],
 				self._ColorScheme['DEBUG_BACKGROUND'][background],
-			], status_message_text, "%DEBUG", message_text, self._environment, local_settings
+			], [""], self._icon_set.debug, status_message.current_status_message, "%DEBUG", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def debug_performance(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def debug_performance(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Performance debugging information logging:
 		Can be used to log entry the execution time of operations or other
 		performance information while the application is being debugged.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -429,26 +444,26 @@
 			[
 				self._ColorScheme['DEBUG_PERFORMANCE_TIME'][background],
 				self._ColorScheme['DEBUG_PERFORMANCE_STATUS'][background],
 				self._ColorScheme['DEBUG_PERFORMANCE_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_DEBUG_PERFORMANCE'][background],
 				self._ColorScheme['DEBUG_PERFORMANCE_MESSAGE'][background],
 				self._ColorScheme['DEBUG_PERFORMANCE_BACKGROUND'][background],
-			], status_message_text, "%DEBUG PERFORMANCE", message_text, self._environment, local_settings
+			], [""], self._icon_set.debug_performance, status_message.current_status_message, "%DEBUG PERFORMANCE", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def performance(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def performance(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Performance information logging:
 		Can be used to log entry the execution time of operations or
 		other application performance information.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -456,26 +471,26 @@
 			[
 				self._ColorScheme['PERFORMANCE_TIME'][background],
 				self._ColorScheme['PERFORMANCE_STATUS'][background],
 				self._ColorScheme['PERFORMANCE_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_PERFORMANCE'][background],
 				self._ColorScheme['PERFORMANCE_MESSAGE'][background],
 				self._ColorScheme['PERFORMANCE_BACKGROUND'][background],
-			], status_message_text, "%PERFORMANCE", message_text, self._environment, local_settings
+			], [""], self._icon_set.performance, status_message.current_status_message, "%PERFORMANCE", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def event(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def event(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Event information logging:
 		Can be used to log entry specific events in the application,
 		such as button presses or mouse cursor movements.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -483,26 +498,26 @@
 			[
 				self._ColorScheme['EVENT_TIME'][background],
 				self._ColorScheme['EVENT_STATUS'][background],
 				self._ColorScheme['EVENT_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_EVENT'][background],
 				self._ColorScheme['EVENT_MESSAGE'][background],
 				self._ColorScheme['EVENT_BACKGROUND'][background],
-			], status_message_text, "~EVENT", message_text, self._environment, local_settings
+			], [""], self._icon_set.event, status_message.current_status_message, "~EVENT", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def audit(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def audit(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Audit information logging:
 		Can be used to log entry changes in the system, such as creating or
 		deleting users, as well as changes in security settings.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -510,25 +525,25 @@
 			[
 				self._ColorScheme['AUDIT_TIME'][background],
 				self._ColorScheme['AUDIT_STATUS'][background],
 				self._ColorScheme['AUDIT_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_AUDIT'][background],
 				self._ColorScheme['AUDIT_MESSAGE'][background],
 				self._ColorScheme['AUDIT_BACKGROUND'][background],
-			], status_message_text, "~AUDIT", message_text, self._environment, local_settings
+			], [""], self._icon_set.audit, status_message.current_status_message, "~AUDIT", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def metrics(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def metrics(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Metrics information logging:
 		Can be used to log entry metrics to track application performance and identify issues.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -536,26 +551,26 @@
 			[
 				self._ColorScheme['METRICS_TIME'][background],
 				self._ColorScheme['METRICS_STATUS'][background],
 				self._ColorScheme['METRICS_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_METRICS'][background],
 				self._ColorScheme['METRICS_MESSAGE'][background],
 				self._ColorScheme['METRICS_BACKGROUND'][background],
-			], status_message_text, "~METRICS", message_text, self._environment, local_settings
+			], [""], self._icon_set.metrics, status_message.current_status_message, "~METRICS", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def user(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def user(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		User information logging:
 		Can be used to log entry custom logs to store additional information
 		that may be useful for diagnosing problems.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -563,25 +578,25 @@
 			[
 				self._ColorScheme['USER_TIME'][background],
 				self._ColorScheme['USER_STATUS'][background],
 				self._ColorScheme['USER_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_USER'][background],
 				self._ColorScheme['USER_MESSAGE'][background],
 				self._ColorScheme['USER_BACKGROUND'][background],
-			], status_message_text, "~USER", message_text, self._environment, local_settings
+			], [""], self._icon_set.user, status_message.current_status_message, "~USER", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def message(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def message(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Message information logging:
 		Can be used for the usual output of ordinary messages about the program's operation.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -589,25 +604,25 @@
 			[
 				self._ColorScheme['MESSAGE_TIME'][background],
 				self._ColorScheme['MESSAGE_STATUS'][background],
 				self._ColorScheme['MESSAGE_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_MESSAGE'][background],
 				self._ColorScheme['MESSAGE_MESSAGE'][background],
 				self._ColorScheme['MESSAGE_BACKGROUND'][background],
-			], status_message_text, "@MESSAGE", message_text, self._environment, local_settings
+			], [""], self._icon_set.message, status_message.current_status_message, "@MESSAGE", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def info(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def info(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Default information logging:
 		Can be used to log entry messages with specific content about the operation of the program.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -615,25 +630,25 @@
 			[
 				self._ColorScheme['INFO_TIME'][background],
 				self._ColorScheme['INFO_STATUS'][background],
 				self._ColorScheme['INFO_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_INFO'][background],
 				self._ColorScheme['INFO_MESSAGE'][background],
 				self._ColorScheme['INFO_BACKGROUND'][background],
-			], status_message_text, "@INFO", message_text, self._environment, local_settings
+			], [""], self._icon_set.info, status_message.current_status_message, "@INFO", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def notice(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
+	def notice(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = None, local_settings: dict = None) -> None:
 		"""
 		Notice information logging:
 		Can be used to flag important events that might be missed with a normal logging level.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		background = local_background if local_background is not None else self.global_background
@@ -641,75 +656,75 @@
 			[
 				self._ColorScheme['NOTICE_TIME'][background],
 				self._ColorScheme['NOTICE_STATUS'][background],
 				self._ColorScheme['NOTICE_STATUS_MESSAGE'][background],
 				self._ColorScheme['TYPE_NOTICE'][background],
 				self._ColorScheme['NOTICE_MESSAGE'][background],
 				self._ColorScheme['NOTICE_BACKGROUND'][background],
-			], status_message_text, "@NOTICE", message_text, self._environment, local_settings
+			], [""], self._icon_set.notice, status_message.current_status_message, "@NOTICE", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def warning(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def warning(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Warning information logging:
 		Can be used to log entry warnings that the program may work with unpredictable results.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		self._buffer << self._assemble_entry(
 			[
 				self._ColorScheme['WARNING_TIME'][local_background],
 				self._ColorScheme['WARNING_STATUS'][local_background],
 				self._ColorScheme['WARNING_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_WARNING'][local_background],
 				self._ColorScheme['WARNING_MESSAGE'][local_background],
 				self._ColorScheme['WARNING_BACKGROUND'][local_background],
-			], status_message_text, "!WARNING", message_text, self._environment, local_settings
+			], [""], self._icon_set.warning, status_message.current_status_message, "!WARNING", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def error(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def error(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Error information logging:
 		Used to log entry errors and crashes in the program.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		self._buffer << self._assemble_entry(
 			[
 				self._ColorScheme['ERROR_TIME'][local_background],
 				self._ColorScheme['ERROR_STATUS'][local_background],
 				self._ColorScheme['ERROR_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_ERROR'][local_background],
 				self._ColorScheme['ERROR_MESSAGE'][local_background],
 				self._ColorScheme['ERROR_BACKGROUND'][local_background],
-			], status_message_text, "!!ERROR", message_text, self._environment, local_settings
+			], [""], self._icon_set.error, status_message.current_status_message, "!!ERROR", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def critical(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def critical(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Critical error information logging:
 		Used to log entry for critical and unpredictable program failures.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		if not 'bold' in local_settings:
@@ -718,63 +733,63 @@
 			[
 				self._ColorScheme['CRITICAL_TIME'][local_background],
 				self._ColorScheme['CRITICAL_STATUS'][local_background],
 				self._ColorScheme['CRITICAL_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_CRITICAL'][local_background],
 				self._ColorScheme['CRITICAL_MESSAGE'][local_background],
 				self._ColorScheme['CRITICAL_BACKGROUND'][local_background],
-			], status_message_text, "!!!@CRITICAL", message_text, self._environment, local_settings
+			], [""], self._icon_set.critical, status_message.current_status_message, "!!!@CRITICAL", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def start_process(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def start_process(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Stub.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
-		# if local_settings is None:
-		# 	local_settings = {}
-		# self._buffer << self._assemble_entry(
-		# 	[
-		# 		self._ColorScheme['PROGRESS_TIME'][local_background],
-		# 		self._ColorScheme['PROGRESS_STATUS'][local_background],
-		# 		self._ColorScheme['PROGRESS_STATUS_MESSAGE'][local_background],
-		# 		self._ColorScheme['TYPE_PROGRESS'][local_background],
-		# 		self._ColorScheme['PROGRESS_MESSAGE'][local_background],
-		# 		self._ColorScheme['PROGRESS_BACKGROUND'][local_background],
-		# 	], status_message_text, "&PROGRESS [*******.............] - 37%", message_text, self._environment, local_settings
-		# )
-		# if self._environment == LogEnvironments.CONSOLE:
-		# 	self._buffer.update_console()
-		pass
+		if local_settings is None:
+			local_settings = {}
+		self._buffer << self._assemble_entry(
+			[
+				self._ColorScheme['PROGRESS_TIME'][local_background],
+				self._ColorScheme['PROGRESS_STATUS'][local_background],
+				self._ColorScheme['PROGRESS_STATUS_MESSAGE'][local_background],
+				self._ColorScheme['TYPE_PROGRESS'][local_background],
+				self._ColorScheme['PROGRESS_MESSAGE'][local_background],
+				self._ColorScheme['PROGRESS_BACKGROUND'][local_background],
+			], [""], self._icon_set.process, status_message.current_status_message, "&PROGRESS [*******.............] - 37%", message_text, self._environment, local_settings
+		)
+		if self._environment == LogEnvironments.CONSOLE:
+			self._buffer.update_console()
+		# pass
 		# Must run on a thread
 
-	def stop_process(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def stop_process(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Stub.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		pass
 		# Make transition to SUCCESS or FAIL
 
-	def success(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def success(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Success information logging:
 		Used to log entry a message about the success of the process.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		if not 'italic' in local_settings:
@@ -783,25 +798,25 @@
 			[
 				self._ColorScheme['SUCCESS_TIME'][local_background],
 				self._ColorScheme['SUCCESS_STATUS'][local_background],
 				self._ColorScheme['SUCCESS_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_SUCCESS'][local_background],
 				self._ColorScheme['SUCCESS_MESSAGE'][local_background],
 				self._ColorScheme['SUCCESS_BACKGROUND'][local_background],
-			], status_message_text, "&SUCCESS", message_text, self._environment, local_settings
+			], [""], self._icon_set.success, status_message.current_status_message, "&SUCCESS", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
 
-	def fail(self, *, status_message_text: str = "...", message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
+	def fail(self, *, status_message: StatusMessageType = StatusMessageType("..."), message_text: str = "...", local_background: bool = True, local_settings: dict = None) -> None:
 		"""
 		Fail information logging:
 		Used to log entry a message about the failed execution of the process.
 
-		:param status_message_text: Log entry status message
+		:param status_message: Log entry status message
 		:param message_text: Log entry message
 		:param local_background: Display entry with background?
 		:param local_settings: Dictionary of local recording settings
 		"""
 		if local_settings is None:
 			local_settings = {}
 		if not 'italic' in local_settings:
@@ -810,11 +825,11 @@
 			[
 				self._ColorScheme['FAIL_TIME'][local_background],
 				self._ColorScheme['FAIL_STATUS'][local_background],
 				self._ColorScheme['FAIL_STATUS_MESSAGE'][local_background],
 				self._ColorScheme['TYPE_FAIL'][local_background],
 				self._ColorScheme['FAIL_MESSAGE'][local_background],
 				self._ColorScheme['FAIL_BACKGROUND'][local_background],
-			], status_message_text, "&FAIL", message_text, self._environment, local_settings
+			], [""], self._icon_set.fail, status_message.current_status_message, "&FAIL", message_text, self._environment, local_settings
 		)
 		if self._environment == LogEnvironments.CONSOLE:
 			self._buffer.update_console()
```

### Comparing `mighty_logger-0.5.0/mighty_logger/src/__init__.py` & `mighty_logger-0.5.1/mighty_logger/src/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 	Dec2Hex,\
 	Dec2Ansi,\
 	Hex2Dec,\
 	Hex2Ansi,\
 	Ansi2Dec,\
 	Ansi2Hex
 from .log_environment import LogEnvironments
+from .status_variables import StatusMessagePatterns
```

### Comparing `mighty_logger-0.5.0/mighty_logger/src/ansi_format.py` & `mighty_logger-0.5.1/mighty_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger/src/color_picker.py` & `mighty_logger-0.5.1/mighty_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger/src/log_environment.py` & `mighty_logger-0.5.1/mighty_logger/src/log_environment.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger/text/__init__.py` & `mighty_logger-0.5.1/mighty_logger/text/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from .icon_set import IconSetType, EmptyIconSet, IconSet1, IconSet2, IconSet3, IconSet4
 from .text_buffer import BasicTextBuffer, TextBuffer
```

### Comparing `mighty_logger-0.5.0/mighty_logger/text/text_buffer.py` & `mighty_logger-0.5.1/mighty_logger/text/text_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,19 @@
 		if number_string < len(self._text_buffer):
 			self._text_buffer[number_string] = f"{message}"
 		else:
 			self._text_buffer.extend([""] * (number_string - len(self._text_buffer)))
 			self.append(message)
 
 	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
-		# todo сделать очистку HTML в plain text
-		with open(name_file, "w") as text_buffer_file:
-			text_buffer_file.write('\n'.join(self._text_buffer))
+		with open(name_file, "w", encoding="utf-8") as text_buffer_file:
+			if clean:
+				text_buffer_file.write(self._text_buffer[0] + '\n' + '\n<br>'.join(self._text_buffer[1:]))
+			else:
+				text_buffer_file.write(self._text_buffer[0] + '\n' + '\n'.join(self._text_buffer[1:]))
 
 	def update_console(self) -> None:
 		super().update_console()
 
 class TextBuffer(Singleton, TextBufferType):
 	"""
 	A class with an advanced implementation of the console text buffer. It is not necessary to use it
@@ -101,15 +103,15 @@
 		else:
 			old_excess_console_strings = len(re.sub(r"\033\[.*?m", "", self._text_buffer[number_string])) // self.width
 			new_excess_console_strings = len(re.sub(r"\033\[.*?m", "", message)) // self.width
 			self._buffer_size += new_excess_console_strings - old_excess_console_strings
 			self._text_buffer[number_string] = f"{message}"
 
 	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
-		with open(name_file, "w") as text_buffer_file:
+		with open(name_file, "w", encoding="utf-8") as text_buffer_file:
 			if clean:
 				for item in self._text_buffer:
 					text_buffer_file.write("{}\n".format(re.sub(r"\033\[.*?m", "", item)))
 			else:
 				text_buffer_file.write('\n'.join(self._text_buffer))
 
 	def update_console(self) -> None:
```

### Comparing `mighty_logger-0.5.0/mighty_logger/text/~animation.py` & `mighty_logger-0.5.1/mighty_logger/text/~animation.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.5.0/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,175 +1,199 @@
 Metadata-Version: 2.1
-Name: mighty-logger
-Version: 0.5.0
+Name: mighty_logger
+Version: 0.5.1
 Summary: Powerful functional logger with support for qt programming
-Home-page: https://github.com/Nakama3942/qt_colored_logger
-Author: Kalynovsky 'Nakama3942' Valentin
+Home-page: https://github.com/Nakama3942/mighty_logger
+Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
-Project-URL: Releases, https://github.com/Nakama3942/qt_colored_logger/releases
+Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Logging
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
-[![template](https://img.shields.io/badge/Repository-template-darkred)](https://github.com/Nakama3942/template_rep)
-[![GitHub license](https://img.shields.io/github/license/Nakama3942/qt_colored_logger?color=gold&style=flat-square)](https://github.com/Nakama3942/qt_colored_logger/blob/master/LICENSE)
-
-![PyPI](https://img.shields.io/pypi/v/qt-colored-logger?color=yellow&logo=pypi&logoColor=white&style=flat-square)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/qt_colored_logger?label=latest%20release&logo=github&style=flat-square)
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/qt_colored_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=flat-square)
-![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/qt_colored_logger/v0.3.0?include_prereleases&style=flat-square)
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qt_colored_logger?style=flat-square)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/qt_colored_logger?style=flat-square)
-![PyPI - Format](https://img.shields.io/pypi/format/qt_colored_logger?label=PyPI%20format&style=flat-square)
-![PyPI - Status](https://img.shields.io/pypi/status/qt_colored_logger?label=PyPI%20status&style=flat-square)
-
-![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/qt_colored_logger?style=flat-square)
-![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/qt_colored_logger?style=flat-square)
-![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/qt_colored_logger?label=%28pre-%29release%20date&style=flat-square)
-
-![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/qt_colored_logger?color=darkgreen&style=flat-square)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/qt_colored_logger?color=darkgreen&style=flat-square)
-
-[![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CHANGELOG.md)
-[![CONTRIBUTING](https://img.shields.io/badge/here-CONTRIBUTING-indigo)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CONTRIBUTING.md)
-[![CODE_OF_CONDUCT](https://img.shields.io/badge/here-CODE_OF_CONDUCT-darkgreen)](https://github.com/Nakama3942/qt_colored_logger/blob/master/CODE_OF_CONDUCT.md)
-[![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange)](https://github.com/Nakama3942/qt_colored_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
+[![template](https://img.shields.io/badge/Repository-template-darkred?style=for-the-badge)](https://github.com/Nakama3942/template_rep)
+[![GitHub license](https://img.shields.io/github/license/Nakama3942/mighty_logger?color=gold&style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE)
+[![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/CHANGELOG.md)
+[![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
+
+![PyPI](https://img.shields.io/pypi/v/mighty-logger?color=yellow&logo=pypi&logoColor=white&style=for-the-badge)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?label=latest%20release&logo=github&style=for-the-badge)
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=for-the-badge)
+![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/mighty_logger/v0.5.0?include_prereleases&style=for-the-badge)
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mighty-logger?style=for-the-badge)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/mighty-logger?style=for-the-badge)
+![PyPI - Format](https://img.shields.io/pypi/format/mighty-logger?label=PyPI%20format&style=for-the-badge)
+![PyPI - Status](https://img.shields.io/pypi/status/mighty-logger?label=PyPI%20status&style=for-the-badge)
+
+![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/mighty_logger?style=for-the-badge)
+![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/mighty_logger?style=for-the-badge)
+![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/mighty_logger?label=%28pre-%29release%20date&style=for-the-badge)
+
+![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
+![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
+![Lines of code](https://img.shields.io/tokei/lines/github/Nakama3942/mighty_logger?style=for-the-badge)
 
 </div>
 
 # Mighty Logger
+
 ### Content
+
 - [Qt_Сolored-logger](#mighty-logger)
-	- [Content](#content)
-	- [Preamble](#preamble)
-	- [Overview](#overview)
-    - [Important releases](#important-releases)
-	- [LICENSE](#license)
-	- [Installation](#installation)
-	- [Usage](#usage)
-	- [Additional functionality](#additional-functionality)
-	- [Data](#data)
-	- [Troubleshooting](#troubleshooting)
-	- [Authors](#authors)
+  - [Content](#content)
+  - [Preamble](#preamble)
+  - [Overview](#overview)
+  - [Important releases](#important-releases)
+  - [LICENSE](#license)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Additional functionality](#additional-functionality)
+  - [Data](#data)
+  - [Troubleshooting](#troubleshooting)
+  - [Authors](#authors)
 
 ## Preamble
-I often came across the opinion that it is better to use not standard output to the console, but full-fledged logging... However, the standard libraries do not provide exactly what I need... Therefore, I decided to make my own library! Which will implement the functionality I need.
+
+<!--
+This library it was renamed to "Mighty logger" but before this library named is "Qt Colored logger". Old commits may search in this repository, but download old build may on next link: https://pypi.org/project/qt-colored-logger/ .
+-->
+
+> I often came across the opinion that it is better to use not standard output to the console, but full-fledged logging... However, the standard libraries do not provide exactly what I need... Therefore, I decided to make my own library! Which will implement the functionality I need.
 
 I was inspired by the [colored-logs](https://pypi.org/project/colored-logs/) library.
 
+---
+
+*This library has been renamed to "Mighty logger", but this library used to be called "Qt Colored logger". You can search for old commits in this repository, but you can download the old build from the [link](https://pypi.org/project/qt-colored-logger/).*
+
 - [Content](#content)
 
 ## Overview
+
 The library implements the formation of a beautifully formatted colored text, similar to a log, which has all the necessary information:
+
 - Device name and registered profile, system name, etc. (this data is displayed only once at the beginning of the logging)
 - Log entry time
 - Log entry status
-- Description of the log entry status
 - Log entry type
 - Entry message
 
-Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background.
+Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background, icons ~~and animations~~.
 
 - [Content](#content)
 
 ## Important releases
+
 <details><summary>See the important releases (possible spoilers)</summary>
 
 - [x] v0.1.0 - First official release (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
-- [ ] v0.5.1 - Symbols update (added hint symbols near log entries types)
+- [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [ ] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [ ] v0.7.0 - Animation update (added animations in processes)
-- [ ] v0.8.0 - Search update (added search by log entry types)
-- [ ] v0.8.1 - Extension update (made wheel format and instruction of toml)
+- [ ] v0.6.1 - Animation update (added animations in processes)
+- [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
+- [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
+- [ ] v0.7.2 - Search update (added search by log entry types)
+- [ ] v0.7.3 - Extension update (made wheel format and instruction of toml)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
 ## LICENSE
-The full text of the license can be found at the following [link](https://github.com/Nakama3942/qt_colored_logger/blob/master/LICENSE).
+
+The full text of the license can be found at the following [link](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE).
 
 > Copyright © 2023 Kalynovsky Valentin. All rights reserved.
->
+> 
 > Licensed under the Apache License, Version 2.0 (the "License");
 > you may not use this file except in compliance with the License.
 > You may obtain a copy of the License at
->
+> 
 >     http://www.apache.org/licenses/LICENSE-2.0
->
+> 
 > Unless required by applicable law or agreed to in writing, software
 > distributed under the License is distributed on an "AS IS" BASIS,
 > WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 > See the License for the specific language governing permissions and
 
 - [Content](#content)
 
 ## Installation
+
 Despite the fact that the library was originally developed for use in PyQt, it does not require PyQt to be installed, since this framework for outputting to Text fields, which support not only Plain Text, uses HTML and this library simply simplifies the logging process, since the creation process already formatted strings is registered in this library.
 
 To install the library, enter the command:
+
 ```sh
 pip install mighty_logger
 ```
 
 ## Usage
+
 This is the simplest example of using the library:
+
 ```python
 from mighty_logger import Logger
+from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
-	logger = Logger(program_name="Test", console_width=115)
-	logger.message(status_message_text="Hooray", message_text="Hello world!")
+    logger = Logger(program_name="Test", console_width=115)
+    logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
 ```
 
 The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
+
 > <span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span><br>
-> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-04-09 12:37:07.198496 </span><span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
+> <span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry> </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span><br>
 
 See the APPLYING.md file for more details.
 
 - [Content](#content)
 
 ## *Additional functionality*
+
 *Additional functionality is also planned. Let's keep it a secret for now. Let it be a surprise.*
 
 - [Content](#content)
 
 ## Data
+
 See the DATA.md file.
 
 - [Content](#content)
 
 ## Troubleshooting
-All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/qt_colored_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/qt_colored_logger/blob/master/CODE_OF_CONDUCT.md).
+
+All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
 
 ## Authors
+
 <table align="center" style="border-width: 10; border-style: ridge">
-	<tr>
-		<td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
-		<!--<td></td>-->
-	</tr>
+    <tr>
+        <td align="center"><a href="https://github.com/Nakama3942"><img src="https://avatars.githubusercontent.com/u/73797846?s=400&u=a9b7688ac521d739825d7003a5bd599aab74cb76&v=4" width="150px;" alt=""/><br /><sub><b>Kalynovsky Valentin</b></sub></a><sub><br />"Ideological inspirer and Author"</sub></td>
+        <!--<td></td>-->
+    </tr>
 <!--
-	<tr>
-		<td></td>
-		<td></td>
-	</tr>
+    <tr>
+        <td></td>
+        <td></td>
+    </tr>
 -->
 </table>
```

### Comparing `mighty_logger-0.5.0/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.5.1/mighty_logger.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 mighty_logger/basic/exceptions.py
 mighty_logger/basic/patterns.py
 mighty_logger/basic/text_buffer_type.py
 mighty_logger/src/__init__.py
 mighty_logger/src/ansi_format.py
 mighty_logger/src/color_picker.py
 mighty_logger/src/log_environment.py
-mighty_logger/src/~status_variables.py
+mighty_logger/src/status_variables.py
 mighty_logger/text/__init__.py
+mighty_logger/text/icon_set.py
 mighty_logger/text/text_buffer.py
 mighty_logger/text/~animation.py
-mighty_logger/text/~icon_set.py
+test/test_console.py
+test/test_html.py
```

### Comparing `mighty_logger-0.5.0/setup.py` & `mighty_logger-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mighty_logger",
-    version="0.5.0",
+    version="0.5.1",
 
-    author="Kalynovsky 'Nakama3942' Valentin",
+    author="Kalynovsky 'Nakamura Akira' Valentin",
     author_email="nakama3942@gmail.com",
 
     description="Powerful functional logger with support for qt programming",
     long_description=readme,
     long_description_content_type="text/markdown",
 
-    url="https://github.com/Nakama3942/qt_colored_logger",
+    url="https://github.com/Nakama3942/mighty_logger",
 
     license="Apache License, Version 2.0, see LICENSE file",
 
     packages=[
         'mighty_logger',
         'mighty_logger.text',
         'mighty_logger.src',
@@ -53,11 +53,11 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.11",
         "Topic :: System :: Logging",
     ],
     project_urls={
-        'Releases': 'https://github.com/Nakama3942/qt_colored_logger/releases',
+        'Releases': 'https://github.com/Nakama3942/mighty_logger/releases',
     },
     python_requires='>=3.11',
 )
```

