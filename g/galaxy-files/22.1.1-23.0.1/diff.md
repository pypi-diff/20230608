# Comparing `tmp/galaxy-files-22.1.1.tar.gz` & `tmp/galaxy-files-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-files-22.1.1.tar", last modified: Mon Aug 22 19:45:49 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/files/dist/.tmp-4kd67fqu/galaxy-files-23.0.1.tar", last modified: Thu Jun  8 17:38:42 2023, max compression
```

## Comparing `galaxy-files-22.1.1.tar` & `galaxy-files-23.0.1.tar`

### file list

```diff
@@ -1,67 +1,40 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.437770 galaxy-files-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      147 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-files-22.1.1/LICENSE.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       28 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1515 2022-08-22 19:45:49.437903 galaxy-files-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      322 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/README.rst
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.426463 galaxy-files-22.1.1/build_scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/build_scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/build_scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/build_scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.426953 galaxy-files-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.427209 galaxy-files-22.1.1/galaxy/files/
--rw-r--r--   0 mvandenb   (501) staff       (20)    12851 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.431053 galaxy-files-22.1.1/galaxy/files/sources/
--rw-r--r--   0 mvandenb   (501) staff       (20)     8614 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3034 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/_pyfilesystem2.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      467 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/anvil.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      494 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/basespace.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      487 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/dropbox.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      477 2022-08-18 15:49:02.000000 galaxy-files-22.1.1/galaxy/files/sources/ftp.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1988 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/galaxy.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1011 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/googlecloudstorage.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      617 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/googledrive.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      480 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/onedata.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5867 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/posix.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      435 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/s3.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3177 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/s3fs.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      536 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/ssh.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      477 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/sources/webdav.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.431329 galaxy-files-22.1.1/galaxy/files/unittest_utils/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1246 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/galaxy/files/unittest_utils/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      426 2022-08-22 19:45:29.000000 galaxy-files-22.1.1/galaxy/project_galaxy_files.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.433057 galaxy-files-22.1.1/galaxy_files.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1515 2022-08-22 19:45:48.000000 galaxy-files-22.1.1/galaxy_files.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1669 2022-08-22 19:45:49.000000 galaxy-files-22.1.1/galaxy_files.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:48.000000 galaxy-files-22.1.1/galaxy_files.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:45:48.000000 galaxy-files-22.1.1/galaxy_files.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:48.000000 galaxy-files-22.1.1/galaxy_files.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       33 2022-08-22 19:45:48.000000 galaxy-files-22.1.1/galaxy_files.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:48.000000 galaxy-files-22.1.1/galaxy_files.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       34 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/requirements.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:49.444697 galaxy-files-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2823 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)       16 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.433299 galaxy-files-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:49.437555 galaxy-files-22.1.1/tests/files/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:13.000000 galaxy-files-22.1.1/tests/files/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6166 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      308 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/tests/files/basespace_file_sources_conf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)      128 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/tests/files/dropbox_file_sources_conf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)      533 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/tests/files/gcsfs_file_sources_conf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)      375 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/tests/files/googledrive_file_sources_conf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)      187 2022-08-18 15:49:03.000000 galaxy-files-22.1.1/tests/files/onedata_file_sources_conf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)      108 2022-03-24 19:47:13.000000 galaxy-files-22.1.1/tests/files/s3_file_sources_conf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     1349 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_basespace.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      515 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_dropbox.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      640 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_gcsfs.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      608 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_googledrive.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      600 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_onedata.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    14286 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_posix.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      575 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_s3.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3019 2022-08-22 19:45:28.000000 galaxy-files-22.1.1/tests/files/test_webdav.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      160 2022-03-24 19:47:14.000000 galaxy-files-22.1.1/tests/files/webdav_user_file_sources_conf.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-files-23.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/files/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/_pyfilesystem2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/anvil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/basespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/files/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/uris.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-files-22.1.1/LICENSE.txt` & `galaxy-files-23.0.1/LICENSE.txt`

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

### Comparing `galaxy-files-22.1.1/PKG-INFO` & `galaxy-files-23.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 22.1.1
-Summary: Galaxy File Source Framework and Default Plugins
+Version: 23.0.1
+Summary: Galaxy file source framework and default plugins
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
-License-File: LICENSE.txt
 
 
 .. image:: https://badge.fury.io/py/galaxy-files.svg
    :target: https://pypi.org/project/galaxy-files/
 
 
 
 Overview
 --------
 
 The Galaxy_ file sources framework and default plugins.
 
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
-22.1.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
+
+No recorded changes since last release
+
+-------------------
+22.1.1 (2022-08-22)
+-------------------
 
 * Initial standalone release of this package.
-
-
```

### Comparing `galaxy-files-22.1.1/galaxy/files/__init__.py` & `galaxy-files-23.0.1/galaxy/files/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import logging
 import os
 from collections import (
     defaultdict,
     namedtuple,
 )
-from typing import Set
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Set,
+)
 
 from galaxy import exceptions
-from galaxy.util import (
-    plugin_config
-)
+from galaxy.util import plugin_config
 from galaxy.util.dictifiable import Dictifiable
 
 log = logging.getLogger(__name__)
 
-FileSourcePath = namedtuple('FileSourcePath', ['file_source', 'path'])
+FileSourcePath = namedtuple("FileSourcePath", ["file_source", "path"])
 
 
 class ConfiguredFileSources:
     """Load plugins and resolve Galaxy URIs to FileSource objects."""
 
-    def __init__(self, file_sources_config: 'ConfiguredFileSourcesConfig', conf_file=None, conf_dict=None, load_stock_plugins=False):
+    def __init__(
+        self,
+        file_sources_config: "ConfiguredFileSourcesConfig",
+        conf_file=None,
+        conf_dict=None,
+        load_stock_plugins=False,
+    ):
         self._file_sources_config = file_sources_config
         self._plugin_classes = self._file_source_plugins_dict()
         file_sources = []
         if conf_file is not None:
             file_sources = self._load_plugins_from_file(conf_file)
         elif conf_dict is not None:
             plugin_source = plugin_config.plugin_source_from_dict(conf_dict)
@@ -35,22 +45,22 @@
         if load_stock_plugins:
             stock_file_source_conf_dict = []
 
             def _ensure_loaded(plugin_type):
                 for file_source in file_sources:
                     if file_source.plugin_type == plugin_type:
                         return
-                stock_file_source_conf_dict.append({'type': plugin_type})
+                stock_file_source_conf_dict.append({"type": plugin_type})
 
             if file_sources_config.ftp_upload_dir is not None:
-                _ensure_loaded('gxftp')
+                _ensure_loaded("gxftp")
             if file_sources_config.library_import_dir is not None:
-                _ensure_loaded('gximport')
+                _ensure_loaded("gximport")
             if file_sources_config.user_library_import_dir is not None:
-                _ensure_loaded('gxuserimport')
+                _ensure_loaded("gxuserimport")
             if stock_file_source_conf_dict:
                 stock_plugin_source = plugin_config.plugin_source_from_dict(stock_file_source_conf_dict)
                 # insert at begining instead of append so FTP and library import appear
                 # at the top of the list (presumably the most common options). Admins can insert
                 # these explicitly for greater control.
                 file_sources = self._parse_plugin_source(stock_plugin_source) + file_sources
 
@@ -59,19 +69,20 @@
 
     def _load_plugins_from_file(self, conf_file):
         plugin_source = plugin_config.plugin_source_from_path(conf_file)
         return self._parse_plugin_source(plugin_source)
 
     def _file_source_plugins_dict(self):
         import galaxy.files.sources
-        return plugin_config.plugins_dict(galaxy.files.sources, 'plugin_type')
+
+        return plugin_config.plugins_dict(galaxy.files.sources, "plugin_type")
 
     def _parse_plugin_source(self, plugin_source):
         extra_kwds = {
-            'file_sources_config': self._file_sources_config,
+            "file_sources_config": self._file_sources_config,
         }
         return plugin_config.load_plugins(
             self._plugin_classes,
             plugin_source,
             extra_kwds,
             dict_to_list_key="id",
         )
@@ -100,29 +111,37 @@
         # validate a URI against Galaxy's configuration, environment, and the current
         # user. Throw appropriate exception if there is a problem with the files source
         # referenced by the URI.
         if uri.startswith("gxuserimport://"):
             user_login = user_context.email
             user_base_dir = self._file_sources_config.user_library_import_dir
             if user_base_dir is None:
-                raise exceptions.ConfigDoesNotAllowException('The configuration of this Galaxy instance does not allow upload from user directories.')
+                raise exceptions.ConfigDoesNotAllowException(
+                    "The configuration of this Galaxy instance does not allow upload from user directories."
+                )
             full_import_dir = os.path.join(user_base_dir, user_login)
             if not os.path.exists(full_import_dir):
-                raise exceptions.ObjectNotFound('Your user import directory does not exist.')
+                raise exceptions.ObjectNotFound("Your user import directory does not exist.")
         elif uri.startswith("gximport://"):
             base_dir = self._file_sources_config.library_import_dir
             if base_dir is None:
-                raise exceptions.ConfigDoesNotAllowException('The configuration of this Galaxy instance does not allow usage of import directory.')
+                raise exceptions.ConfigDoesNotAllowException(
+                    "The configuration of this Galaxy instance does not allow usage of import directory."
+                )
         elif uri.startswith("gxftp://"):
             user_ftp_base_dir = self._file_sources_config.ftp_upload_dir
             if user_ftp_base_dir is None:
-                raise exceptions.ConfigDoesNotAllowException('The configuration of this Galaxy instance does not allow upload from FTP directories.')
+                raise exceptions.ConfigDoesNotAllowException(
+                    "The configuration of this Galaxy instance does not allow upload from FTP directories."
+                )
             user_ftp_dir = user_context.ftp_dir
             if not user_ftp_dir or not os.path.exists(user_ftp_dir):
-                raise exceptions.ObjectNotFound('Your FTP directory does not exist, attempting to upload files to it may cause it to be created.')
+                raise exceptions.ObjectNotFound(
+                    "Your FTP directory does not exist, attempting to upload files to it may cause it to be created."
+                )
 
     def get_file_source(self, id_prefix, scheme):
         for file_source in self._file_sources:
             # gxfiles uses prefix to find plugin, other scheme are assumed to have
             # at most one file_source.
             if scheme != file_source.get_scheme():
                 continue
@@ -141,52 +160,73 @@
 
     def get_schemes(self):
         schemes = set()
         for file_source in self._file_sources:
             schemes.add(file_source.get_scheme())
         return schemes
 
-    def plugins_to_dict(self, for_serialization=False, user_context=None):
+    def plugins_to_dict(
+        self, for_serialization: bool = False, user_context: Optional["FileSourceDictifiable"] = None
+    ) -> List[Dict[str, Any]]:
         rval = []
         for file_source in self._file_sources:
             if not file_source.user_has_access(user_context):
                 continue
             el = file_source.to_dict(for_serialization=for_serialization, user_context=user_context)
             rval.append(el)
         return rval
 
-    def to_dict(self, for_serialization=False, user_context=None):
+    def to_dict(
+        self, for_serialization: bool = False, user_context: Optional["FileSourceDictifiable"] = None
+    ) -> Dict[str, Any]:
         return {
-            'file_sources': self.plugins_to_dict(for_serialization=for_serialization, user_context=user_context),
-            'config': self._file_sources_config.to_dict()
+            "file_sources": self.plugins_to_dict(for_serialization=for_serialization, user_context=user_context),
+            "config": self._file_sources_config.to_dict(),
         }
 
     @staticmethod
     def from_app_config(config):
         config_file = config.file_sources_config_file
-        if not os.path.exists(config_file):
+        config_dict = None
+        if not config_file or not os.path.exists(config_file):
             config_file = None
+            config_dict = config.file_sources
         file_sources_config = ConfiguredFileSourcesConfig.from_app_config(config)
-        return ConfiguredFileSources(file_sources_config, config_file, load_stock_plugins=True)
+        return ConfiguredFileSources(
+            file_sources_config, conf_file=config_file, conf_dict=config_dict, load_stock_plugins=True
+        )
 
     @staticmethod
     def from_dict(as_dict):
         if as_dict is not None:
             sources_as_dict = as_dict["file_sources"]
             config_as_dict = as_dict["config"]
             file_sources_config = ConfiguredFileSourcesConfig.from_dict(config_as_dict)
         else:
             sources_as_dict = []
             file_sources_config = ConfiguredFileSourcesConfig()
         return ConfiguredFileSources(file_sources_config, conf_dict=sources_as_dict)
 
 
-class ConfiguredFileSourcesConfig:
+class NullConfiguredFileSources(ConfiguredFileSources):
+    def __init__(
+        self,
+    ):
+        super().__init__(ConfiguredFileSourcesConfig())
+
 
-    def __init__(self, symlink_allowlist=None, library_import_dir=None, user_library_import_dir=None, ftp_upload_dir=None, ftp_upload_purge=True):
+class ConfiguredFileSourcesConfig:
+    def __init__(
+        self,
+        symlink_allowlist=None,
+        library_import_dir=None,
+        user_library_import_dir=None,
+        ftp_upload_dir=None,
+        ftp_upload_purge=True,
+    ):
         symlink_allowlist = symlink_allowlist or []
         self.symlink_allowlist = symlink_allowlist
         self.library_import_dir = library_import_dir
         self.user_library_import_dir = user_library_import_dir
         self.ftp_upload_dir = ftp_upload_dir
         self.ftp_upload_purge = ftp_upload_purge
 
@@ -200,39 +240,39 @@
         kwds["user_library_import_dir"] = getattr(config, "user_library_import_dir", None)
         kwds["ftp_upload_dir"] = getattr(config, "ftp_upload_dir", None)
         kwds["ftp_upload_purge"] = getattr(config, "ftp_upload_purge", True)
         return ConfiguredFileSourcesConfig(**kwds)
 
     def to_dict(self):
         return {
-            'symlink_allowlist': self.symlink_allowlist,
-            'library_import_dir': self.library_import_dir,
-            'user_library_import_dir': self.user_library_import_dir,
-            'ftp_upload_dir': self.ftp_upload_dir,
-            'ftp_upload_purge': self.ftp_upload_purge,
+            "symlink_allowlist": self.symlink_allowlist,
+            "library_import_dir": self.library_import_dir,
+            "user_library_import_dir": self.user_library_import_dir,
+            "ftp_upload_dir": self.ftp_upload_dir,
+            "ftp_upload_purge": self.ftp_upload_purge,
         }
 
     @staticmethod
     def from_dict(as_dict):
         return ConfiguredFileSourcesConfig(
-            symlink_allowlist=as_dict['symlink_allowlist'],
-            library_import_dir=as_dict['library_import_dir'],
-            user_library_import_dir=as_dict['user_library_import_dir'],
-            ftp_upload_dir=as_dict['ftp_upload_dir'],
-            ftp_upload_purge=as_dict['ftp_upload_purge'],
+            symlink_allowlist=as_dict["symlink_allowlist"],
+            library_import_dir=as_dict["library_import_dir"],
+            user_library_import_dir=as_dict["user_library_import_dir"],
+            ftp_upload_dir=as_dict["ftp_upload_dir"],
+            ftp_upload_purge=as_dict["ftp_upload_purge"],
         )
 
 
 class FileSourceDictifiable(Dictifiable):
-    dict_collection_visible_keys = ('email', 'username', 'ftp_dir', 'preferences', 'is_admin')
+    dict_collection_visible_keys = ("email", "username", "ftp_dir", "preferences", "is_admin")
 
-    def to_dict(self, view='collection', value_mapper=None):
+    def to_dict(self, view="collection", value_mapper=None):
         rval = super().to_dict(view=view, value_mapper=value_mapper)
-        rval['role_names'] = list(self.role_names)
-        rval['group_names'] = list(self.group_names)
+        rval["role_names"] = list(self.role_names)
+        rval["group_names"] = list(self.group_names)
         return rval
 
     @property
     def role_names(self) -> Set[str]:
         raise NotImplementedError
 
     @property
@@ -292,15 +332,14 @@
     def app_vault(self):
         """App vault namespace"""
         vault = self.trans.app.vault
         return vault or defaultdict(lambda: None)
 
 
 class DictFileSourcesUserContext(FileSourceDictifiable):
-
     def __init__(self, **kwd):
         self._kwd = kwd
 
     @property
     def email(self):
         return self._kwd.get("email")
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/__init__.py` & `galaxy-files-23.0.1/galaxy/files/sources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import os
 import time
-from typing import Set
-
-from typing_extensions import ClassVar
+from typing import (
+    ClassVar,
+    Set,
+)
 
 from galaxy.exceptions import (
     ConfigurationError,
     ItemAccessibilityException,
 )
 from galaxy.util.bool_expressions import (
     BooleanExpressionEvaluator,
@@ -16,16 +17,15 @@
 from galaxy.util.template import fill_template
 
 DEFAULT_SCHEME = "gxfiles"
 DEFAULT_WRITABLE = False
 
 
 class FilesSource(metaclass=abc.ABCMeta):
-    """
-    """
+    """ """
 
     @abc.abstractmethod
     def get_uri_root(self) -> str:
         """Return a prefix for the root (e.g. gxfiles://prefix/)."""
 
     @abc.abstractmethod
     def get_scheme(self) -> str:
@@ -44,17 +44,17 @@
     def list(self, source_path="/", recursive=False, user_context=None):
         """Return dictionary of 'Directory's and 'File's."""
 
     @abc.abstractmethod
     def realize_to(self, source_path, native_path, user_context=None):
         """Realize source path (relative to uri root) to local file system path."""
 
+    @abc.abstractmethod
     def write_from(self, target_path, native_path, user_context=None):
-        """Write file at native path to target_path (relative to uri root).
-        """
+        """Write file at native path to target_path (relative to uri root)."""
 
     @abc.abstractmethod
     def to_dict(self, for_serialization=False, user_context=None):
         """Return a dictified representation of this FileSource instance.
 
         If ``user_context`` is supplied, properties should be written so user
         context doesn't need to be present after the plugin is re-hydrated.
@@ -75,18 +75,15 @@
 
     def user_has_access(self, user_context) -> bool:
         if user_context is None and self.user_context_required:
             return False
         return (
             user_context is None
             or user_context.is_admin
-            or (
-                self._user_has_required_roles(user_context)
-                and self._user_has_required_groups(user_context)
-            )
+            or (self._user_has_required_roles(user_context) and self._user_has_required_groups(user_context))
         )
 
     @property
     def user_context_required(self) -> bool:
         return self.requires_roles is not None or self.requires_groups is not None
 
     def get_uri_root(self):
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/_pyfilesystem2.py` & `galaxy-files-23.0.1/galaxy/files/sources/_pyfilesystem2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import abc
 import functools
 import logging
 import os
-from typing import Any, Dict, List, Optional, Type
+from typing import (
+    Any,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Type,
+)
 
 import fs
 from fs.base import FS
-from typing_extensions import ClassVar
 
-from ..sources import BaseFilesSource
+from . import BaseFilesSource
 
 log = logging.getLogger(__name__)
 
 PACKAGE_MESSAGE = "FilesSource plugin is missing required Python PyFilesystem2 plugin package [%s]"
 
 
 class PyFilesystem2FilesSource(BaseFilesSource):
@@ -37,24 +43,24 @@
                 res: List[Dict[str, Any]] = []
                 for p, dirs, files in h.walk(path):
                     to_dict = functools.partial(self._resource_info_to_dict, p)
                     res.extend(map(to_dict, dirs))
                     res.extend(map(to_dict, files))
                 return res
             else:
-                res = h.scandir(path, namespaces=['details'])
+                res = h.scandir(path, namespaces=["details"])
                 to_dict = functools.partial(self._resource_info_to_dict, path)
                 return list(map(to_dict, res))
 
     def _realize_to(self, source_path, native_path, user_context=None):
-        with open(native_path, 'wb') as write_file:
+        with open(native_path, "wb") as write_file:
             self._open_fs(user_context=user_context).download(source_path, write_file)
 
     def _write_from(self, target_path, native_path, user_context=None):
-        with open(native_path, 'rb') as read_file:
+        with open(native_path, "rb") as read_file:
             openfs = self._open_fs(user_context=user_context)
             dirname = fs.path.dirname(target_path)
             if not openfs.isdir(dirname):
                 openfs.makedirs(dirname)
             openfs.upload(target_path, read_file)
 
     def _resource_info_to_dict(self, dir_path, resource_info):
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/galaxy.py` & `galaxy-files-23.0.1/galaxy/files/sources/galaxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Static Galaxy file sources - ftp and libraries."""
 
 from .posix import PosixFilesSource
 
 
 class UserFtpFilesSource(PosixFilesSource):
-    plugin_type = 'gxftp'
+    plugin_type = "gxftp"
 
     def __init__(self, label="FTP Directory", doc="Galaxy User's FTP Directory", root="${user.ftp_dir}", **kwd):
         posix_kwds = dict(
             id="_ftp",
             root=root,
             label=label,
             doc=doc,
@@ -24,17 +24,23 @@
         return None
 
     def get_scheme(self):
         return "gxftp"
 
 
 class LibraryImportFilesSource(PosixFilesSource):
-    plugin_type = 'gximport'
+    plugin_type = "gximport"
 
-    def __init__(self, label="Library Import Directory", doc="Galaxy's library import directory", root="${config.library_import_dir}", **kwd):
+    def __init__(
+        self,
+        label="Library Import Directory",
+        doc="Galaxy's library import directory",
+        root="${config.library_import_dir}",
+        **kwd,
+    ):
         posix_kwds = dict(
             id="_import",
             root=root,
             label=label,
             doc=doc,
         )
         posix_kwds.update(kwd)
@@ -44,17 +50,23 @@
         return None
 
     def get_scheme(self):
         return "gximport"
 
 
 class UserLibraryImportFilesSource(PosixFilesSource):
-    plugin_type = 'gxuserimport'
+    plugin_type = "gxuserimport"
 
-    def __init__(self, label="Library User Import Directory", doc="Galaxy's user library import directory", root="${config.user_library_import_dir}/${user.email}", **kwd):
+    def __init__(
+        self,
+        label="Library User Import Directory",
+        doc="Galaxy's user library import directory",
+        root="${config.user_library_import_dir}/${user.email}",
+        **kwd,
+    ):
         posix_kwds = dict(
             id="_userimport",
             root=root,
             label=label,
             doc=doc,
         )
         posix_kwds.update(kwd)
@@ -63,8 +75,8 @@
     def get_prefix(self):
         return None
 
     def get_scheme(self):
         return "gxuserimport"
 
 
-__all__ = ('UserFtpFilesSource', 'LibraryImportFilesSource', 'UserLibraryImportFilesSource')
+__all__ = ("UserFtpFilesSource", "LibraryImportFilesSource", "UserLibraryImportFilesSource")
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/googlecloudstorage.py` & `galaxy-files-23.0.1/galaxy/files/sources/googlecloudstorage.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 except ImportError:
     GCSFS = None
 
 from ._pyfilesystem2 import PyFilesystem2FilesSource
 
 
 class GoogleCloudStorageFilesSource(PyFilesystem2FilesSource):
-    plugin_type = 'googlecloudstorage'
+    plugin_type = "googlecloudstorage"
     required_module = GCSFS
     required_package = "fs-gcsfs"
 
     def _open_fs(self, user_context):
         props = self._serialization_props(user_context)
-        bucket_name = props.pop('bucket_name', None)
-        root_path = props.pop('root_path', None)
-        project = props.pop('project', None)
+        bucket_name = props.pop("bucket_name", None)
+        root_path = props.pop("root_path", None)
+        project = props.pop("project", None)
         args = {}
-        if props.get('anonymous'):
-            args['client'] = Client.create_anonymous_client()
-        elif props.get('token'):
-            args['client'] = Client(project=project, credentials=Credentials(**props))
+        if props.get("anonymous"):
+            args["client"] = Client.create_anonymous_client()
+        elif props.get("token"):
+            args["client"] = Client(project=project, credentials=Credentials(**props))
         handle = GCSFS(bucket_name, root_path=root_path, retry=0, **args)
         return handle
 
 
-__all__ = ('GoogleCloudStorageFilesSource',)
+__all__ = ("GoogleCloudStorageFilesSource",)
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/googledrive.py` & `galaxy-files-23.0.1/galaxy/files/sources/googledrive.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 except ImportError:
     GoogleDriveFS = None
 
 from ._pyfilesystem2 import PyFilesystem2FilesSource
 
 
 class GoogleDriveFilesSource(PyFilesystem2FilesSource):
-    plugin_type = 'googledrive'
+    plugin_type = "googledrive"
     required_module = GoogleDriveFS
     required_package = "fs.googledrivefs"
 
     def _open_fs(self, user_context):
         props = self._serialization_props(user_context)
         credentials = Credentials(**props)
         handle = GoogleDriveFS(credentials)
         return handle
 
 
-__all__ = ('GoogleDriveFilesSource',)
+__all__ = ("GoogleDriveFilesSource",)
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/posix.py` & `galaxy-files-23.0.1/galaxy/files/sources/posix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import functools
 import os
 import shutil
-from typing import Any, Dict, List
+from typing import (
+    Any,
+    Dict,
+    List,
+)
 
 from galaxy import exceptions
 from galaxy.util.path import (
     safe_contains,
     safe_path,
     safe_walk,
 )
-from ..sources import BaseFilesSource
+from . import BaseFilesSource
 
 DEFAULT_ENFORCE_SYMLINK_SECURITY = True
 DEFAULT_DELETE_ON_REALIZE = False
 DEFAULT_ALLOW_SUBDIR_CREATION = True
 
 
 class PosixFilesSource(BaseFilesSource):
-    plugin_type = 'posix'
+    plugin_type = "posix"
 
     # If this were a PyFilesystem2FilesSource all that would be needed would be,
     # but we couldn't enforce security our way I suspect.
     # def _open_fs(self):
     #    from fs.osfs import OSFS
     #    handle = OSFS(**self._props)
     #    return handle
@@ -32,19 +36,19 @@
         self.enforce_symlink_security = props.get("enforce_symlink_security", DEFAULT_ENFORCE_SYMLINK_SECURITY)
         self.delete_on_realize = props.get("delete_on_realize", DEFAULT_DELETE_ON_REALIZE)
         self.allow_subdir_creation = props.get("allow_subdir_creation", DEFAULT_ALLOW_SUBDIR_CREATION)
 
     def _list(self, path="/", recursive=True, user_context=None):
         dir_path = self._to_native_path(path, user_context=user_context)
         if not self._safe_directory(dir_path):
-            raise exceptions.ObjectNotFound(f'The specified directory does not exist [{dir_path}].')
+            raise exceptions.ObjectNotFound(f"The specified directory does not exist [{dir_path}].")
         if recursive:
             res: List[Dict[str, Any]] = []
             effective_root = self._effective_root(user_context)
-            for (p, dirs, files) in safe_walk(dir_path, allowlist=self._allowlist):
+            for p, dirs, files in safe_walk(dir_path, allowlist=self._allowlist):
                 rel_dir = os.path.relpath(p, effective_root)
                 to_dict = functools.partial(self._resource_info_to_dict, rel_dir, user_context=user_context)
                 res.extend(map(to_dict, dirs))
                 res.extend(map(to_dict, files))
             return res
         else:
             res = os.listdir(dir_path)
@@ -110,15 +114,17 @@
                 "uri": uri,
                 "path": rel_path,
             }
 
     def _safe_directory(self, directory):
         if self.enforce_symlink_security:
             if not safe_path(directory, allowlist=self._allowlist):
-                raise exceptions.ConfigDoesNotAllowException(f'directory ({directory}) is a symlink to a location not on the allowlist')
+                raise exceptions.ConfigDoesNotAllowException(
+                    f"directory ({directory}) is a symlink to a location not on the allowlist"
+                )
 
         if not os.path.exists(directory):
             return False
         return True
 
     def _serialization_props(self, user_context=None):
         return {
@@ -131,8 +137,8 @@
         }
 
     @property
     def _allowlist(self):
         return self._file_sources_config.symlink_allowlist
 
 
-__all__ = ('PosixFilesSource',)
+__all__ = ("PosixFilesSource",)
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/s3fs.py` & `galaxy-files-23.0.1/galaxy/files/sources/s3fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import functools
 import logging
 import os
-from typing import Any, Dict, List
+from typing import (
+    Any,
+    Dict,
+    List,
+)
 
 try:
     import s3fs
 except ImportError:
     s3fs = None
 
-from ..sources import BaseFilesSource
+from . import BaseFilesSource
 
 DEFAULT_ENFORCE_SYMLINK_SECURITY = True
 DEFAULT_DELETE_ON_REALIZE = False
 
 log = logging.getLogger(__name__)
 
 
 class S3FsFilesSource(BaseFilesSource):
-    plugin_type = 's3fs'
+    plugin_type = "s3fs"
 
     def __init__(self, **kwd):
         if s3fs is None:
             raise Exception("Package s3fs unavailable but required for this file source plugin.")
         props = self._parse_common_config_opts(kwd)
-        self._bucket = props.pop("bucket", '')
-        self._endpoint_url = props.pop('endpoint_url', None)
+        self._bucket = props.pop("bucket", "")
+        self._endpoint_url = props.pop("endpoint_url", None)
         assert self._endpoint_url or self._bucket
         self._props = props
 
     def _list(self, path="/", recursive=True, user_context=None):
         fs = self._open_fs(user_context=user_context)
         if recursive:
             res: List[Dict[str, Any]] = []
@@ -54,15 +58,15 @@
     def _bucket_path(self, path):
         if not path.startswith("/"):
             path = f"/{path}"
         return f"{self._bucket}{path}"
 
     def _open_fs(self, user_context=None):
         if self._endpoint_url:
-            self._props.update({'client_kwargs': {'endpoint_url': self._endpoint_url}})
+            self._props.update({"client_kwargs": {"endpoint_url": self._endpoint_url}})
         fs = s3fs.S3FileSystem(**self._props)
         return fs
 
     def _resource_info_to_dict(self, dir_path, resource_info):
         name = os.path.basename(resource_info["name"])
         path = os.path.join(dir_path, name)
         uri = self.uri_from_path(path)
@@ -83,8 +87,8 @@
         effective_props = {}
         for key, val in self._props.items():
             effective_props[key] = self._evaluate_prop(val, user_context=user_context)
         effective_props["bucket"] = self._bucket
         return effective_props
 
 
-__all__ = ('S3FsFilesSource',)
+__all__ = ("S3FsFilesSource",)
```

### Comparing `galaxy-files-22.1.1/galaxy/files/sources/ssh.py` & `galaxy-files-23.0.1/galaxy/files/sources/ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class SshFilesSource(PyFilesystem2FilesSource):
     plugin_type = "ssh"
     required_module = SSHFS
     required_package = "fs.sshfs"
 
     def _open_fs(self, user_context):
         props = self._serialization_props(user_context)
-        path = props.pop('path')
+        path = props.pop("path")
         handle = SSHFS(**props)
         if path:
             handle = handle.opendir(path)
         return handle
 
 
 __all__ = ("SshFilesSource",)
```

### Comparing `galaxy-files-22.1.1/galaxy_files.egg-info/PKG-INFO` & `galaxy-files-23.0.1/galaxy_files.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 22.1.1
-Summary: Galaxy File Source Framework and Default Plugins
+Version: 23.0.1
+Summary: Galaxy file source framework and default plugins
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
-License-File: LICENSE.txt
 
 
 .. image:: https://badge.fury.io/py/galaxy-files.svg
    :target: https://pypi.org/project/galaxy-files/
 
 
 
 Overview
 --------
 
 The Galaxy_ file sources framework and default plugins.
 
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
-22.1.0.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
+
+No recorded changes since last release
+
+-------------------
+22.1.1 (2022-08-22)
+-------------------
 
 * Initial standalone release of this package.
-
-
```

