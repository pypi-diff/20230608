# Comparing `tmp/jsonQM-0.2.3.tar.gz` & `tmp/jsonQM-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/william/Documents/API Query language/dist/tmp11wlu70y/jsonQM-0.2.3.tar", last modified: Tue Jun  6 21:44:13 2023, max compression
+gzip compressed data, was "jsonQM-0.3.3.tar", last modified: Wed Jun  7 23:33:00 2023, max compression
```

## Comparing `jsonQM-0.2.3.tar` & `jsonQM-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:44:13.000000 jsonQM-0.2.3/
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM/
--rw-rw-r--   0 william   (1000) william   (1000)      620 2023-06-06 20:29:37.000000 jsonQM-0.2.3/jsonQM/model.py
--rw-rw-r--   0 william   (1000) william   (1000)     1246 2023-06-06 21:42:47.000000 jsonQM-0.2.3/jsonQM/modelserializer.py
--rw-rw-r--   0 william   (1000) william   (1000)       70 2023-06-06 21:42:40.000000 jsonQM-0.2.3/jsonQM/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)       38 2023-06-06 21:44:13.000000 jsonQM-0.2.3/setup.cfg
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/
--rw-rw-r--   0 william   (1000) william   (1000)      207 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/SOURCES.txt
--rw-rw-r--   0 william   (1000) william   (1000)        7 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/top_level.txt
--rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)        1 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/dependency_links.txt
--rw-rw-r--   0 william   (1000) william   (1000)     1957 2023-06-06 21:05:46.000000 jsonQM-0.2.3/README.md
--rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:44:13.000000 jsonQM-0.2.3/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)     1061 2023-06-06 08:49:52.000000 jsonQM-0.2.3/LICENSE
--rw-rw-r--   0 william   (1000) william   (1000)     1008 2023-06-06 21:43:12.000000 jsonQM-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.688119 jsonQM-0.3.3/
+-rw-rw-rw-   0        0        0     1067 2023-06-07 21:14:44.000000 jsonQM-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     4308 2023-06-07 23:33:00.685108 jsonQM-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3762 2023-06-07 23:27:03.000000 jsonQM-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.658110 jsonQM-0.3.3/jsonQM/
+-rw-rw-rw-   0        0        0       72 2023-06-07 21:14:44.000000 jsonQM-0.3.3/jsonQM/__init__.py
+-rw-rw-rw-   0        0        0     2060 2023-06-07 23:11:45.000000 jsonQM-0.3.3/jsonQM/model.py
+-rw-rw-rw-   0        0        0     2003 2023-06-07 23:22:05.000000 jsonQM-0.3.3/jsonQM/modelserializer.py
+drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.679119 jsonQM-0.3.3/jsonQM.egg-info/
+-rw-rw-rw-   0        0        0     4308 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 23:33:00.688119 jsonQM-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-06-07 23:32:35.000000 jsonQM-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.681109 jsonQM-0.3.3/tests/
+-rw-rw-rw-   0        0        0     3359 2023-06-07 22:52:55.000000 jsonQM-0.3.3/tests/test_model.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsonQM-0.2.3/LICENSE` & `jsonQM-0.3.3/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 William A. Lim
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 William A. Lim
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

