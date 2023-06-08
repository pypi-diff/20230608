# Comparing `tmp/torrentool-1.1.1.tar.gz` & `tmp/torrentool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torrentool-1.1.1.tar", last modified: Sat Feb 20 10:34:48 2021, max compression
+gzip compressed data, was "torrentool-1.2.0.tar", last modified: Thu Jun  8 13:39:33 2023, max compression
```

## Comparing `torrentool-1.1.1.tar` & `torrentool-1.2.0.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/
--rw-rw-r--   0 idle      (1000) idle      (1000)      133 2021-02-20 10:34:48.000000 torrentool-1.1.1/setup.cfg
--rw-rw-r--   0 idle      (1000) idle      (1000)      189 2016-10-23 10:37:21.000000 torrentool-1.1.1/AUTHORS
--rw-rw-r--   0 idle      (1000) idle      (1000)     1502 2021-02-07 02:49:57.000000 torrentool-1.1.1/LICENSE
--rw-rw-r--   0 idle      (1000) idle      (1000)     2150 2021-02-07 02:49:34.000000 torrentool-1.1.1/README.rst
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool/
--rw-rw-r--   0 idle      (1000) idle      (1000)     3131 2020-06-18 12:38:15.000000 torrentool-1.1.1/torrentool/cli.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      103 2021-02-20 10:34:38.000000 torrentool-1.1.1/torrentool/__init__.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     6525 2021-02-19 07:50:38.000000 torrentool-1.1.1/torrentool/bencode.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     2543 2020-06-18 12:54:46.000000 torrentool-1.1.1/torrentool/utils.py
--rw-rw-r--   0 idle      (1000) idle      (1000)    12232 2021-02-19 07:50:38.000000 torrentool-1.1.1/torrentool/torrent.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      761 2016-10-30 07:27:52.000000 torrentool-1.1.1/torrentool/exceptions.py
--rw-rw-r--   0 idle      (1000) idle      (1000)      239 2020-09-26 01:14:55.000000 torrentool-1.1.1/torrentool/api.py
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool/repo/
--rw-rw-r--   0 idle      (1000) idle      (1000)      350 2016-08-30 09:13:49.000000 torrentool-1.1.1/torrentool/repo/open_trackers.ini
--rw-rw-r--   0 idle      (1000) idle      (1000)     1440 2020-10-22 11:42:14.000000 torrentool-1.1.1/setup.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1368 2021-02-20 10:34:38.000000 torrentool-1.1.1/CHANGELOG
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool.egg-info/
--rw-rw-r--   0 idle      (1000) idle      (1000)       52 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool.egg-info/entry_points.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)       11 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool.egg-info/top_level.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool.egg-info/dependency_links.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        1 2015-10-21 17:55:12.000000 torrentool-1.1.1/torrentool.egg-info/not-zip-safe
--rw-rw-r--   0 idle      (1000) idle      (1000)      853 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool.egg-info/SOURCES.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)     3400 2021-02-20 10:34:48.000000 torrentool-1.1.1/torrentool.egg-info/PKG-INFO
--rw-rw-r--   0 idle      (1000) idle      (1000)      342 2016-12-14 14:55:15.000000 torrentool-1.1.1/MANIFEST.in
--rw-rw-r--   0 idle      (1000) idle      (1000)     3400 2021-02-20 10:34:48.000000 torrentool-1.1.1/PKG-INFO
--rw-rw-r--   0 idle      (1000) idle      (1000)      464 2016-08-30 16:03:05.000000 torrentool-1.1.1/INSTALL
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/tests/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/tests/datafixtures/
--rw-rw-r--   0 idle      (1000) idle      (1000)      222 2015-10-23 14:39:21.000000 torrentool-1.1.1/tests/datafixtures/test_file.torrent
--rw-rw-r--   0 idle      (1000) idle      (1000)      489 2016-08-30 14:53:34.000000 torrentool-1.1.1/tests/datafixtures/test_dir.torrent
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/tests/datafixtures/torrtest/
--rw-rw-r--   0 idle      (1000) idle      (1000)        4 2015-10-20 15:31:14.000000 torrentool-1.1.1/tests/datafixtures/torrtest/root.txt
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/tests/datafixtures/torrtest/sub1/
-drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2021-02-20 10:34:48.000000 torrentool-1.1.1/tests/datafixtures/torrtest/sub1/sub2/
--rw-rw-r--   0 idle      (1000) idle      (1000)        4 2015-10-20 15:31:14.000000 torrentool-1.1.1/tests/datafixtures/torrtest/sub1/sub2/sub22.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)       11 2015-10-25 09:39:18.000000 torrentool-1.1.1/tests/datafixtures/torrtest/sub1/sub2/кириллица.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        0 2015-10-25 09:39:29.000000 torrentool-1.1.1/tests/datafixtures/torrtest/sub1/sub2/empty.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)        4 2015-10-20 15:31:14.000000 torrentool-1.1.1/tests/datafixtures/torrtest/sub1/sub11.txt
--rw-rw-r--   0 idle      (1000) idle      (1000)     2978 2021-02-19 07:50:38.000000 torrentool-1.1.1/tests/test_bencode.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1386 2020-06-19 10:33:58.000000 torrentool-1.1.1/tests/test_etc.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     1597 2020-06-19 10:21:18.000000 torrentool-1.1.1/tests/conftest.py
--rw-rw-r--   0 idle      (1000) idle      (1000)     5724 2020-06-19 10:44:03.000000 torrentool-1.1.1/tests/test_torrent.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.884045 torrentool-1.2.0/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      267 2023-06-08 13:36:01.000000 torrentool-1.2.0/AUTHORS
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1457 2023-06-08 13:39:27.000000 torrentool-1.2.0/CHANGELOG
+-rw-rw-r--   0 idle      (1000) idle      (1000)      464 2016-08-30 16:03:05.000000 torrentool-1.2.0/INSTALL
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1502 2022-02-04 12:56:58.000000 torrentool-1.2.0/LICENSE
+-rw-rw-r--   0 idle      (1000) idle      (1000)      342 2016-12-14 14:55:15.000000 torrentool-1.2.0/MANIFEST.in
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2883 2023-06-08 13:39:33.888045 torrentool-1.2.0/PKG-INFO
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2105 2022-05-15 06:11:16.000000 torrentool-1.2.0/README.rst
+-rw-rw-r--   0 idle      (1000) idle      (1000)      110 2023-06-08 13:39:33.888045 torrentool-1.2.0/setup.cfg
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1529 2022-05-15 06:07:01.000000 torrentool-1.2.0/setup.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.876045 torrentool-1.2.0/tests/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1625 2023-06-08 13:36:01.000000 torrentool-1.2.0/tests/conftest.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.880045 torrentool-1.2.0/tests/datafixtures/
+-rw-r--r--   0 idle      (1000) idle      (1000)    11530 2023-03-29 15:10:33.000000 torrentool-1.2.0/tests/datafixtures/88.torrent
+-rw-rw-r--   0 idle      (1000) idle      (1000)    58660 2021-05-18 11:04:50.000000 torrentool-1.2.0/tests/datafixtures/a.torrent
+-rw-rw-r--   0 idle      (1000) idle      (1000)   236831 2022-05-06 00:54:20.000000 torrentool-1.2.0/tests/datafixtures/temp.torrent
+-rw-rw-r--   0 idle      (1000) idle      (1000)   236936 2022-05-15 06:13:15.000000 torrentool-1.2.0/tests/datafixtures/temp.zip
+-rw-rw-r--   0 idle      (1000) idle      (1000)      502 2023-06-08 13:36:01.000000 torrentool-1.2.0/tests/datafixtures/test_dir.torrent
+-rw-rw-r--   0 idle      (1000) idle      (1000)      222 2015-10-23 14:39:21.000000 torrentool-1.2.0/tests/datafixtures/test_file.torrent
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.880045 torrentool-1.2.0/tests/datafixtures/torrtest/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        4 2015-10-20 15:31:14.000000 torrentool-1.2.0/tests/datafixtures/torrtest/root.txt
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.880045 torrentool-1.2.0/tests/datafixtures/torrtest/sub1/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        4 2015-10-20 15:31:14.000000 torrentool-1.2.0/tests/datafixtures/torrtest/sub1/sub11.txt
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.880045 torrentool-1.2.0/tests/datafixtures/torrtest/sub1/sub2/
+-rw-rw-r--   0 idle      (1000) idle      (1000)        0 2015-10-25 09:39:29.000000 torrentool-1.2.0/tests/datafixtures/torrtest/sub1/sub2/empty.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        4 2015-10-20 15:31:14.000000 torrentool-1.2.0/tests/datafixtures/torrtest/sub1/sub2/sub22.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)       11 2015-10-25 09:39:18.000000 torrentool-1.2.0/tests/datafixtures/torrtest/sub1/sub2/кириллица.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2978 2021-02-19 07:50:38.000000 torrentool-1.2.0/tests/test_bencode.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1386 2020-06-19 10:33:58.000000 torrentool-1.2.0/tests/test_etc.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     6234 2023-06-08 13:36:01.000000 torrentool-1.2.0/tests/test_torrent.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.884045 torrentool-1.2.0/torrentool/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      103 2023-06-08 13:39:27.000000 torrentool-1.2.0/torrentool/__init__.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      239 2020-09-26 01:14:55.000000 torrentool-1.2.0/torrentool/api.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     6776 2023-04-01 02:04:15.000000 torrentool-1.2.0/torrentool/bencode.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     3131 2020-06-18 12:38:15.000000 torrentool-1.2.0/torrentool/cli.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)      761 2016-10-30 07:27:52.000000 torrentool-1.2.0/torrentool/exceptions.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.884045 torrentool-1.2.0/torrentool/repo/
+-rw-rw-r--   0 idle      (1000) idle      (1000)      350 2016-08-30 09:13:49.000000 torrentool-1.2.0/torrentool/repo/open_trackers.ini
+-rw-rw-r--   0 idle      (1000) idle      (1000)    12550 2023-06-08 13:36:01.000000 torrentool-1.2.0/torrentool/torrent.py
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2543 2020-06-18 12:54:46.000000 torrentool-1.2.0/torrentool/utils.py
+drwxrwxr-x   0 idle      (1000) idle      (1000)        0 2023-06-08 13:39:33.884045 torrentool-1.2.0/torrentool.egg-info/
+-rw-rw-r--   0 idle      (1000) idle      (1000)     2883 2023-06-08 13:39:33.000000 torrentool-1.2.0/torrentool.egg-info/PKG-INFO
+-rw-rw-r--   0 idle      (1000) idle      (1000)     1005 2023-06-08 13:39:33.000000 torrentool-1.2.0/torrentool.egg-info/SOURCES.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2023-06-08 13:39:33.000000 torrentool-1.2.0/torrentool.egg-info/dependency_links.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)       52 2023-06-08 13:39:33.000000 torrentool-1.2.0/torrentool.egg-info/entry_points.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)        1 2015-10-21 17:55:12.000000 torrentool-1.2.0/torrentool.egg-info/not-zip-safe
+-rw-rw-r--   0 idle      (1000) idle      (1000)       13 2023-06-08 13:39:33.000000 torrentool-1.2.0/torrentool.egg-info/requires.txt
+-rw-rw-r--   0 idle      (1000) idle      (1000)       11 2023-06-08 13:39:33.000000 torrentool-1.2.0/torrentool.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `torrentool-1.1.1/LICENSE` & `torrentool-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2015-2021, Igor `idle sign` Starikov
+Copyright (c) 2015-2022, Igor `idle sign` Starikov
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `torrentool-1.1.1/README.rst` & `torrentool-1.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 
 .. image:: https://img.shields.io/pypi/l/torrentool.svg
     :target: https://pypi.python.org/pypi/torrentool
 
 .. image:: https://img.shields.io/coveralls/idlesign/torrentool/master.svg
     :target: https://coveralls.io/r/idlesign/torrentool
 
-.. image:: https://img.shields.io/travis/idlesign/torrentool/master.svg
-    :target: https://travis-ci.org/idlesign/torrentool
-
 
 Description
 -----------
 
 *The tool to work with torrent files.*
 
-Works on Python 3.6+.
+Works on Python 3.7+.
 
 Includes:
 
-* Command line interface (requires ``click`` package to be installed)
-* Torrent utils (file creation, read and modification)
-* Bencoding utils (decoder, encoder)
+* Command line interface. Requires ``click`` package to be installed.
+
+  Use ``pip install torrentool[cli]`` to install this dependency automatically.
+* Torrent utils (file creation, read and modification).
+* Bencoding utils (decoder, encoder).
 
 
 Using CLI
 ~~~~~~~~~
 
 .. code-block:: bash
```

### Comparing `torrentool-1.1.1/torrentool/cli.py` & `torrentool-1.2.0/torrentool/cli.py`

 * *Files identical despite different names*

### Comparing `torrentool-1.1.1/torrentool/bencode.py` & `torrentool-1.2.0/torrentool/bencode.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,15 +156,22 @@
                         # for non-standard .torrent files.
                         string = string.decode(errors='replace')
 
                 stack_items.append(string)
                 encoded = encoded[last_char_idx:]
 
             elif char == 'e':  # End of a dictionary or a list.
-                compress_stack()
+                try:
+                    compress_stack()
+
+                except IndexError as e:
+                    raise BencodeDecodingError(
+                        f'Unable to parse the rest of the data: "{encoded.decode(errors="replace")[:60]}"'
+                    ) from e
+
                 encoded = encoded[1:]
 
             else:
                 raise BencodeDecodingError(f'Unable to interpret `{char}` char.')
 
         if len(stack_items) == 1:
             stack_items = stack_items.pop()
```

### Comparing `torrentool-1.1.1/torrentool/utils.py` & `torrentool-1.2.0/torrentool/utils.py`

 * *Files identical despite different names*

### Comparing `torrentool-1.1.1/torrentool/torrent.py` & `torrentool-1.2.0/torrentool/torrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,24 @@
     def comment(self) -> Optional[str]:
         """Optional. Free-form textual comments of the author."""
         return self._struct.get('comment')
 
     @comment.setter
     def comment(self, val: str):
         self._struct['comment'] = val
+    
+    @property
+    def source(self) -> Optional[str]:
+        """Optional. Often used by private trackers to create a unique infohash to prevent peer-leak."""
+        return self._struct.get('info').get("source")
 
+    @source.setter
+    def source(self, val: str):
+        self._struct['info']['source'] = val
+    
     @property
     def creation_date(self) -> Optional[datetime]:
         """Optional. The creation time of the torrent, in standard UNIX epoch format. UTC."""
 
         date = self._struct.get('creation date')
         if date is not None:
             date = datetime.utcfromtimestamp(int(date))
```

### Comparing `torrentool-1.1.1/torrentool/exceptions.py` & `torrentool-1.2.0/torrentool/exceptions.py`

 * *Files identical despite different names*

### Comparing `torrentool-1.1.1/setup.py` & `torrentool-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     author_email='idlesign@yandex.ru',
 
     packages=['torrentool'],
     include_package_data=True,
     zip_safe=False,
 
     install_requires=[],
+    extras_require={'cli': ['click']},
     setup_requires=[] + PYTEST_RUNNER,
     tests_require=[
         'pytest',
         'pytest-datafixtures',
         'pytest-responsemock',
     ],
 
@@ -43,13 +44,14 @@
 
     classifiers=[
         # As in https://pypi.python.org/pypi?:action=list_classifiers
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: BSD License'
     ],
 )
```

### Comparing `torrentool-1.1.1/CHANGELOG` & `torrentool-1.2.0/CHANGELOG`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 torrentool changelog
 ====================
 
 
+v1.2.0 [2023-06-08]
+-------------------
++ Add 'source' property for Torrent (see #27).
+
+
 v1.1.1 [2021-02-20]
 -------------------
 * Better handling for bogus string encodings in .torrent files (see #2).
 
 
 v1.1.0 [2020-06-19]
 -------------------
```

### Comparing `torrentool-1.1.1/torrentool.egg-info/SOURCES.txt` & `torrentool-1.2.0/torrentool.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 README.rst
 setup.cfg
 setup.py
 tests/conftest.py
 tests/test_bencode.py
 tests/test_etc.py
 tests/test_torrent.py
+tests/datafixtures/88.torrent
+tests/datafixtures/a.torrent
+tests/datafixtures/temp.torrent
+tests/datafixtures/temp.zip
 tests/datafixtures/test_dir.torrent
 tests/datafixtures/test_file.torrent
 tests/datafixtures/torrtest/root.txt
 tests/datafixtures/torrtest/sub1/sub11.txt
 tests/datafixtures/torrtest/sub1/sub2/empty.txt
 tests/datafixtures/torrtest/sub1/sub2/sub22.txt
 tests/datafixtures/torrtest/sub1/sub2/кириллица.txt
@@ -25,9 +29,10 @@
 torrentool/torrent.py
 torrentool/utils.py
 torrentool.egg-info/PKG-INFO
 torrentool.egg-info/SOURCES.txt
 torrentool.egg-info/dependency_links.txt
 torrentool.egg-info/entry_points.txt
 torrentool.egg-info/not-zip-safe
+torrentool.egg-info/requires.txt
 torrentool.egg-info/top_level.txt
 torrentool/repo/open_trackers.ini
```

### Comparing `torrentool-1.1.1/torrentool.egg-info/PKG-INFO` & `torrentool-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: torrentool
-Version: 1.1.1
+Version: 1.2.0
 Summary: The tool to work with torrent files.
 Home-page: https://github.com/idlesign/torrentool
 Author: Igor `idle sign` Starikov
 Author-email: idlesign@yandex.ru
 License: BSD 3-Clause License
-Description: torrentool
-        ==========
-        https://github.com/idlesign/torrentool
-        
-        .. image:: https://img.shields.io/pypi/v/torrentool.svg
-            :target: https://pypi.python.org/pypi/torrentool
-        
-        .. image:: https://img.shields.io/pypi/l/torrentool.svg
-            :target: https://pypi.python.org/pypi/torrentool
-        
-        .. image:: https://img.shields.io/coveralls/idlesign/torrentool/master.svg
-            :target: https://coveralls.io/r/idlesign/torrentool
-        
-        .. image:: https://img.shields.io/travis/idlesign/torrentool/master.svg
-            :target: https://travis-ci.org/idlesign/torrentool
-        
-        
-        Description
-        -----------
-        
-        *The tool to work with torrent files.*
-        
-        Works on Python 3.6+.
-        
-        Includes:
-        
-        * Command line interface (requires ``click`` package to be installed)
-        * Torrent utils (file creation, read and modification)
-        * Bencoding utils (decoder, encoder)
-        
-        
-        Using CLI
-        ~~~~~~~~~
-        
-        .. code-block:: bash
-        
-            ; Make .torrent out of `video.mkv`
-            $ torrentool torrent create /home/my/files_here/video.mkv
-        
-            ; Make .torrent out of entire `/home/my/files_here` dir,
-            ; and put some open trackers announce URLs into it,
-            ; and publish file on torrent caching service, so it is ready to share.
-            $ torrentool torrent create /home/my/files_here --open_trackers --cache
-        
-            ; Print out existing file info.
-            $ torrentool torrent info /home/my/some.torrent
-        
-        
-        Use command line ``--help`` switch to know more.
-        
-        .. note:: Some commands require ``requests`` package to be installed.
-        
-        
-        From your Python code
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: python
-        
-            from torrentool.api import Torrent
-        
-            # Reading and modifying an existing file.
-            my_torrent = Torrent.from_file('/home/idle/some.torrent')
-            my_torrent.total_size  # Total files size in bytes.
-            my_torrent.magnet_link  # Magnet link for you.
-            my_torrent.comment = 'Your torrents are mine.'  # Set a comment.
-            my_torrent.to_file()  # Save changes.
-        
-            # Or we can create a new torrent from a directory.
-            new_torrent = Torrent.create_from('/home/idle/my_stuff/')  # or it could have been a single file
-            new_torrent.announce_urls = 'udp://tracker.openbittorrent.com:80'
-            new_torrent.to_file('/home/idle/another.torrent')
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
+Provides-Extra: cli
+License-File: LICENSE
+License-File: AUTHORS
+
+torrentool
+==========
+https://github.com/idlesign/torrentool
+
+.. image:: https://img.shields.io/pypi/v/torrentool.svg
+    :target: https://pypi.python.org/pypi/torrentool
+
+.. image:: https://img.shields.io/pypi/l/torrentool.svg
+    :target: https://pypi.python.org/pypi/torrentool
+
+.. image:: https://img.shields.io/coveralls/idlesign/torrentool/master.svg
+    :target: https://coveralls.io/r/idlesign/torrentool
+
+
+Description
+-----------
+
+*The tool to work with torrent files.*
+
+Works on Python 3.7+.
+
+Includes:
+
+* Command line interface. Requires ``click`` package to be installed.
+
+  Use ``pip install torrentool[cli]`` to install this dependency automatically.
+* Torrent utils (file creation, read and modification).
+* Bencoding utils (decoder, encoder).
+
+
+Using CLI
+~~~~~~~~~
+
+.. code-block:: bash
+
+    ; Make .torrent out of `video.mkv`
+    $ torrentool torrent create /home/my/files_here/video.mkv
+
+    ; Make .torrent out of entire `/home/my/files_here` dir,
+    ; and put some open trackers announce URLs into it,
+    ; and publish file on torrent caching service, so it is ready to share.
+    $ torrentool torrent create /home/my/files_here --open_trackers --cache
+
+    ; Print out existing file info.
+    $ torrentool torrent info /home/my/some.torrent
+
+
+Use command line ``--help`` switch to know more.
+
+.. note:: Some commands require ``requests`` package to be installed.
+
+
+From your Python code
+~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    from torrentool.api import Torrent
+
+    # Reading and modifying an existing file.
+    my_torrent = Torrent.from_file('/home/idle/some.torrent')
+    my_torrent.total_size  # Total files size in bytes.
+    my_torrent.magnet_link  # Magnet link for you.
+    my_torrent.comment = 'Your torrents are mine.'  # Set a comment.
+    my_torrent.to_file()  # Save changes.
+
+    # Or we can create a new torrent from a directory.
+    new_torrent = Torrent.create_from('/home/idle/my_stuff/')  # or it could have been a single file
+    new_torrent.announce_urls = 'udp://tracker.openbittorrent.com:80'
+    new_torrent.to_file('/home/idle/another.torrent')
+
+
+
```

### Comparing `torrentool-1.1.1/PKG-INFO` & `torrentool-1.2.0/torrentool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: torrentool
-Version: 1.1.1
+Version: 1.2.0
 Summary: The tool to work with torrent files.
 Home-page: https://github.com/idlesign/torrentool
 Author: Igor `idle sign` Starikov
 Author-email: idlesign@yandex.ru
 License: BSD 3-Clause License
-Description: torrentool
-        ==========
-        https://github.com/idlesign/torrentool
-        
-        .. image:: https://img.shields.io/pypi/v/torrentool.svg
-            :target: https://pypi.python.org/pypi/torrentool
-        
-        .. image:: https://img.shields.io/pypi/l/torrentool.svg
-            :target: https://pypi.python.org/pypi/torrentool
-        
-        .. image:: https://img.shields.io/coveralls/idlesign/torrentool/master.svg
-            :target: https://coveralls.io/r/idlesign/torrentool
-        
-        .. image:: https://img.shields.io/travis/idlesign/torrentool/master.svg
-            :target: https://travis-ci.org/idlesign/torrentool
-        
-        
-        Description
-        -----------
-        
-        *The tool to work with torrent files.*
-        
-        Works on Python 3.6+.
-        
-        Includes:
-        
-        * Command line interface (requires ``click`` package to be installed)
-        * Torrent utils (file creation, read and modification)
-        * Bencoding utils (decoder, encoder)
-        
-        
-        Using CLI
-        ~~~~~~~~~
-        
-        .. code-block:: bash
-        
-            ; Make .torrent out of `video.mkv`
-            $ torrentool torrent create /home/my/files_here/video.mkv
-        
-            ; Make .torrent out of entire `/home/my/files_here` dir,
-            ; and put some open trackers announce URLs into it,
-            ; and publish file on torrent caching service, so it is ready to share.
-            $ torrentool torrent create /home/my/files_here --open_trackers --cache
-        
-            ; Print out existing file info.
-            $ torrentool torrent info /home/my/some.torrent
-        
-        
-        Use command line ``--help`` switch to know more.
-        
-        .. note:: Some commands require ``requests`` package to be installed.
-        
-        
-        From your Python code
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code-block:: python
-        
-            from torrentool.api import Torrent
-        
-            # Reading and modifying an existing file.
-            my_torrent = Torrent.from_file('/home/idle/some.torrent')
-            my_torrent.total_size  # Total files size in bytes.
-            my_torrent.magnet_link  # Magnet link for you.
-            my_torrent.comment = 'Your torrents are mine.'  # Set a comment.
-            my_torrent.to_file()  # Save changes.
-        
-            # Or we can create a new torrent from a directory.
-            new_torrent = Torrent.create_from('/home/idle/my_stuff/')  # or it could have been a single file
-            new_torrent.announce_urls = 'udp://tracker.openbittorrent.com:80'
-            new_torrent.to_file('/home/idle/another.torrent')
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
+Provides-Extra: cli
+License-File: LICENSE
+License-File: AUTHORS
+
+torrentool
+==========
+https://github.com/idlesign/torrentool
+
+.. image:: https://img.shields.io/pypi/v/torrentool.svg
+    :target: https://pypi.python.org/pypi/torrentool
+
+.. image:: https://img.shields.io/pypi/l/torrentool.svg
+    :target: https://pypi.python.org/pypi/torrentool
+
+.. image:: https://img.shields.io/coveralls/idlesign/torrentool/master.svg
+    :target: https://coveralls.io/r/idlesign/torrentool
+
+
+Description
+-----------
+
+*The tool to work with torrent files.*
+
+Works on Python 3.7+.
+
+Includes:
+
+* Command line interface. Requires ``click`` package to be installed.
+
+  Use ``pip install torrentool[cli]`` to install this dependency automatically.
+* Torrent utils (file creation, read and modification).
+* Bencoding utils (decoder, encoder).
+
+
+Using CLI
+~~~~~~~~~
+
+.. code-block:: bash
+
+    ; Make .torrent out of `video.mkv`
+    $ torrentool torrent create /home/my/files_here/video.mkv
+
+    ; Make .torrent out of entire `/home/my/files_here` dir,
+    ; and put some open trackers announce URLs into it,
+    ; and publish file on torrent caching service, so it is ready to share.
+    $ torrentool torrent create /home/my/files_here --open_trackers --cache
+
+    ; Print out existing file info.
+    $ torrentool torrent info /home/my/some.torrent
+
+
+Use command line ``--help`` switch to know more.
+
+.. note:: Some commands require ``requests`` package to be installed.
+
+
+From your Python code
+~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: python
+
+    from torrentool.api import Torrent
+
+    # Reading and modifying an existing file.
+    my_torrent = Torrent.from_file('/home/idle/some.torrent')
+    my_torrent.total_size  # Total files size in bytes.
+    my_torrent.magnet_link  # Magnet link for you.
+    my_torrent.comment = 'Your torrents are mine.'  # Set a comment.
+    my_torrent.to_file()  # Save changes.
+
+    # Or we can create a new torrent from a directory.
+    new_torrent = Torrent.create_from('/home/idle/my_stuff/')  # or it could have been a single file
+    new_torrent.announce_urls = 'udp://tracker.openbittorrent.com:80'
+    new_torrent.to_file('/home/idle/another.torrent')
+
+
+
```

### Comparing `torrentool-1.1.1/tests/test_bencode.py` & `torrentool-1.2.0/tests/test_bencode.py`

 * *Files identical despite different names*

### Comparing `torrentool-1.1.1/tests/test_etc.py` & `torrentool-1.2.0/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `torrentool-1.1.1/tests/conftest.py` & `torrentool-1.2.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 {'length': 11, 'path': ['sub1', 'sub2', 'кириллица.txt']},
                 {'length': 4, 'path': ['sub1', 'sub2', 'sub22.txt']}
             ],
             'name': 'torrtest',
             'piece length': 32768,
             'pieces': b'?\x9ew\xc1A\x84\x8d\x8b\xb7\x91\x19\xe3(\x1e\x1ex\x1e\xde\xa8\xdc',
             'private': 0,
+            'source': 'GIT'
         }
     }
 
 
 @pytest.fixture(scope='session')
 def struct_torr_file():
     return {
```

### Comparing `torrentool-1.1.1/tests/test_torrent.py` & `torrentool-1.2.0/tests/test_torrent.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os.path import normpath, join
 from tempfile import mkdtemp
 from uuid import uuid4
 
 import pytest
 
 from torrentool.api import Torrent
-from torrentool.exceptions import TorrentError
+from torrentool.exceptions import TorrentError, BencodeDecodingError
 
 
 def test_create(datafix_dir, struct_torr_dir, struct_torr_file):
     fp = datafix_dir / 'torrtest' / 'root.txt'
     t = Torrent.create_from(str(fp))
     t.private = True
 
@@ -42,15 +42,15 @@
     assert files[0].length == 4
 
     assert t.total_size == 4
     assert t.name == 'root.txt'
     assert t.announce_urls == [['udp://123.123.123.123']]
     assert t.creation_date.isoformat() == '2015-10-21T17:40:05'
     assert t.comment is None
-
+    assert t.source is None
     hash_expected = '238967c8417cc6ccc378df16687d1958277f270b'
     assert t.info_hash == hash_expected
 
     magnet = t.magnet_link
     assert hash_expected in magnet
     assert 'btih' in magnet
     assert 'magnet:' in magnet
@@ -68,47 +68,51 @@
         (normpath('torrtest/sub1/sub2/кириллица.txt'), 11),
         (normpath('torrtest/sub1/sub2/sub22.txt'), 4)
     ]
     assert t.total_size == 23
     assert t.announce_urls == [['http://track1.org/1/', 'http://track2.org/2/']]
     assert t.creation_date.isoformat() == '2015-10-25T09:42:04'
     assert t.comment == 'примечание'
-
-    hash_expected = 'c815be93f20bf8b12fed14bee35c14b19b1d1984'
+    assert t.source == 'GIT'
+    hash_expected = '669e5c550e4681d00239c5bdc4344e038f1f5c0e'
     assert t.info_hash == hash_expected
 
     magnet = t.magnet_link
     assert hash_expected in magnet
     assert 'btih' in magnet
     assert 'magnet:' in magnet
 
     magnet = t.get_magnet(detailed=True)
     assert (
-        magnet == 'magnet:?xt=urn:btih:c815be93f20bf8b12fed14bee35c14b19b1d1984'
+        magnet == 'magnet:?xt=urn:btih:669e5c550e4681d00239c5bdc4344e038f1f5c0e'
                   '&tr=http%3A%2F%2Ftrack1.org%2F1%2F&tr=http%3A%2F%2Ftrack2.org%2F2%2F'
     )
 
 
 def test_setters():
     t = Torrent()
 
     assert t.info_hash is None
     assert t.comment is None
+    assert t.source is None
     assert t.created_by is None
     assert t.creation_date is None
     assert t.total_size == 0
     assert t.announce_urls == []
     assert t.files == []
 
     t.name = 'mytorrent'
     assert t.name == 'mytorrent'
 
     t.comment = 'mycomment'
     assert t.comment == 'mycomment'
 
+    t.source = 'GIT'
+    assert t.source == 'GIT'
+
     t.created_by = 'some/1.0'
     assert t.created_by == 'some/1.0'
 
     now = datetime.now()
     t.creation_date = now
     assert t.creation_date == now.replace(microsecond=0)
 
@@ -179,14 +183,25 @@
 
 def test_from_string():
     torrstr = '4:spam'
     t = Torrent.from_string(torrstr)
     assert t._struct == 'spam'
 
 
+def test_bogus():
+
+    with pytest.raises(BencodeDecodingError) as e:
+        Torrent.from_string('4:spambogus: ending')
+    assert 'Unable to interpret `b` char.' in f'{e.value}'
+
+    with pytest.raises(BencodeDecodingError) as e:
+        Torrent.from_string('4:spamebogus: ending')
+    assert 'the rest of the data: "ebogus: ending"' in f'{e.value}'
+
+
 def test_to_file(torr_test_file):
     t0 = Torrent({})
 
     with pytest.raises(TorrentError):
         t0.to_file()
 
     t1 = Torrent.from_file(torr_test_file)
```

