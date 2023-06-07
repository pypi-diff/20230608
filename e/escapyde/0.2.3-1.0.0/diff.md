# Comparing `tmp/escapyde-0.2.3.tar.gz` & `tmp/escapyde-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escapyde-0.2.3.tar", max compression
+gzip compressed data, was "escapyde-1.0.0.tar", max compression
```

## Comparing `escapyde-0.2.3.tar` & `escapyde-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     5155 2023-06-07 13:27:18.292448 escapyde-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-06-07 13:27:18.292448 escapyde-0.2.3/LICENSE
--rw-r--r--   0        0        0      754 2023-06-07 13:27:18.292448 escapyde-0.2.3/README.md
--rw-r--r--   0        0        0      124 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/__init__.py
--rw-r--r--   0        0        0     2623 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/ansi.py
--rw-r--r--   0        0        0     2434 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/colours.py
--rw-r--r--   0        0        0        0 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/examples/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-07 13:27:18.292448 escapyde-0.2.3/escapyde/examples/text.py
--rw-r--r--   0        0        0        0 2023-06-07 13:27:18.292448 escapyde-0.2.3/py.typed
--rw-r--r--   0        0        0     4515 2023-06-07 13:27:18.292448 escapyde-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 escapyde-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     5930 2023-06-07 22:17:59.444503 escapyde-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-07 22:17:59.444503 escapyde-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3153 2023-06-07 22:17:59.444503 escapyde-1.0.0/README.md
+-rw-r--r--   0        0        0      124 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/__init__.py
+-rw-r--r--   0        0        0     5302 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/ansi.py
+-rw-r--r--   0        0        0     2557 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/colours.py
+-rw-r--r--   0        0        0      386 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/config.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/examples/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/examples/text.py
+-rw-r--r--   0        0        0     1098 2023-06-07 22:17:59.444503 escapyde-1.0.0/escapyde/validators.py
+-rw-r--r--   0        0        0        0 2023-06-07 22:17:59.444503 escapyde-1.0.0/py.typed
+-rw-r--r--   0        0        0     4527 2023-06-07 22:17:59.444503 escapyde-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 escapyde-1.0.0/PKG-INFO
```

### Comparing `escapyde-0.2.3/CHANGELOG.md` & `escapyde-1.0.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -45,39 +45,68 @@
 - Updated localisation files
 
 -->
 
 <!--
 _______________________________________________________________________________
 
-## [0.2.3] - 2023-06-07
+## [1.0.0] - 2023-06-08
 
-Remembered to include `py.typed` in the package, and fixed a bug with the
-`escape_format` function. Furthermore, identified a major bug with chained
-escapes, which will be fixed in the next major update as it may require breaking
-changes.
+Completely overhauled the `escapyde.ansi.AnsiEscape` class. This release breaks
+backwards compatibility with manual use of the class, however use of the
+provided colour shortcuts is not affected. `README.md` has also been updated.
 
 ### Added
 
-- Added `py.typed` - this time for real
-- Added unit tests
+- Added support for chaining formatting options
+- Added new validators
+- Added new examples to `README.md`, with screenshots
+- New unit tests
+- `SECURITY.md`
 
 ### Changed
 
 - Updated dependencies
+- Moved screenshots to an asset directory
+- `escapyde.ansi.AnsiEscape` now works a lot differently
 
 ### Fixed
 
-- Fixed a bug where `escape_format` was forcing any replaced substrings to be
-  lowercase. The casing in the output now matches the input.
+- Fixed chaining escape sequences
 
 -->
 
 _______________________________________________________________________________
 
+## [1.0.0] - 2023-06-08
+
+Completely overhauled the `escapyde.ansi.AnsiEscape` class. This release breaks
+backwards compatibility with manual use of the class, however use of the
+provided colour shortcuts is not affected. `README.md` has also been updated.
+
+### Added
+
+- Added support for chaining formatting options
+- Added new validators
+- Added new examples to `README.md`, with screenshots
+- New unit tests
+- `SECURITY.md`
+
+### Changed
+
+- Updated dependencies
+- Moved screenshots to an asset directory
+- `escapyde.ansi.AnsiEscape` now works a lot differently
+
+### Fixed
+
+- Fixed chaining escape sequences
+
+_______________________________________________________________________________
+
 ## [0.2.3] - 2023-06-07
 
 Remembered to include `py.typed` in the package, and fixed a bug with the
 `escape_format` function. Furthermore, identified a major bug with chained
 escapes, which will be fixed in the next major update as it may require breaking
 changes.
```

### Comparing `escapyde-0.2.3/LICENSE` & `escapyde-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.3/escapyde/examples/text.py` & `escapyde-1.0.0/escapyde/examples/text.py`

 * *Files identical despite different names*

### Comparing `escapyde-0.2.3/pyproject.toml` & `escapyde-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['poetry-core>=1.2.0', 'wheel',]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = 'escapyde'
-version = '0.2.3'
+version = '1.0.0'
 description = "Yet another ANSI escape sequence library for Python - now modernised!"
 
 authors = ["Lari Liuhamo <lari.liuhamo+pypi@gmail.com>",]
 maintainers = ["Lari Liuhamo <lari.liuhamo+pypi@gmail.com>",]
 
 include = ['CHANGELOG.md', 'LICENSE', 'py.typed',]
 license = 'MIT'
@@ -25,15 +25,15 @@
     'terminal',
     'escape',
     'sequence',
     'colour',
     'color',
 ]
 classifiers = [
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
```

