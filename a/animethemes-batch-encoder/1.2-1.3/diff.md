# Comparing `tmp/animethemes-batch-encoder-1.2.tar.gz` & `tmp/animethemes-batch-encoder-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-batch-encoder-1.2.tar", last modified: Fri May 19 05:04:25 2023, max compression
+gzip compressed data, was "animethemes-batch-encoder-1.3.tar", last modified: Thu Jun  8 04:12:49 2023, max compression
```

## Comparing `animethemes-batch-encoder-1.2.tar` & `animethemes-batch-encoder-1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 05:04:25.590101 animethemes-batch-encoder-1.2/
--rw-rw-rw-   0        0        0     1088 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/LICENSE
--rw-rw-rw-   0        0        0     4321 2023-05-19 05:04:25.589100 animethemes-batch-encoder-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3418 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 05:04:25.581579 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     4321 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-19 05:04:25.000000 animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 05:04:25.589100 animethemes-batch-encoder-1.2/batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     6993 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    12970 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     3814 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     2527 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      711 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     5615 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6594 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-04-24 23:52:30.000000 animethemes-batch-encoder-1.2/batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-05-19 05:04:25.590101 animethemes-batch-encoder-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-05-19 05:02:46.000000 animethemes-batch-encoder-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:49.972211 animethemes-batch-encoder-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-08 04:12:49.972211 animethemes-batch-encoder-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:49.968211 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 04:12:49.000000 animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:49.968211 animethemes-batch-encoder-1.3/batch_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_bitrate_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_encode_webm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_encoding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_loudnorm_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_seek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_seek_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_source_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/batch_encoder/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 04:12:49.972211 animethemes-batch-encoder-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 04:12:42.000000 animethemes-batch-encoder-1.3/setup.py
```

### Comparing `animethemes-batch-encoder-1.2/PKG-INFO` & `animethemes-batch-encoder-1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,104 @@
-Metadata-Version: 2.1
-Name: animethemes-batch-encoder
-Version: 1.2
-Summary: Generate/Execute FFmpeg commands for files in acting directory
-Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
-Author: AnimeThemes
-Author-email: admin@animethemes.moe
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-### Description
-
-Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
-
-Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
-
-Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
-
-### Install
-
-**Requirements:**
-
-* FFmpeg
-* Python >= 3.6
-
-**Install:**
-
-    pip install animethemes-batch-encoder
-
-### Usage
-
-        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
-
-**Mode**
-
-`--mode 1` generates commands from input files in the current directory.
-
-The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
-
-`--mode 2` executes commands from file in the current directory line-by-line.
-
-By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
-
-`--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
-
-The `--file` argument will be ignored in this case.
-
-**File**
-
-The file that commands are written to or read from.
-
-By default, the program will write to or read from `commands.txt` in the current directory.
-
-**Config File**
-
-The configuration file in which our encoding properties are defined.
-
-By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
-
-Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
-
-**Encoding Properties**
-
-`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
-
-`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
-
-Available bitrate control modes are:
-
-* `CBR` Constant Bitrate Mode
-* `VBR` Variable Bitrate Mode
-* `CQ` Constrained Quality Mode
-
-`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
-
-`Threads` is the number of threads used to encode. Default is 4.
-
-`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
-
-`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
-
-`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
-
-`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
-
-**Logging**
-
-Determines the level of the logging for the program.
-
-`--loglevel error` will only output error messages.
-
-`--loglevel info` will output error messages and script progression info messages.
-
-`--loglevel debug` will output all messages, including variable dumps.
+Metadata-Version: 2.1
+Name: animethemes-batch-encoder
+Version: 1.3
+Summary: Generate/Execute FFmpeg commands for files in acting directory
+Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
+Author: AnimeThemes
+Author-email: admin@animethemes.moe
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Description
+
+Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
+
+Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
+
+Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
+
+### Install
+
+**Requirements:**
+
+* FFmpeg
+* Python >= 3.6
+
+**Install:**
+
+    pip install animethemes-batch-encoder
+
+### Usage
+
+        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+
+**Mode**
+
+`--mode 1` generates commands from input files in the current directory.
+
+The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time, output file name and new audio filters.
+
+`--mode 2` executes commands from file in the current directory line-by-line.
+
+By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
+
+`--mode 3` generates commands from input files in the current directory and executes the commands sequentially.
+
+**File**
+
+The file that commands are written to or read from.
+
+By default, the program will write to or read from `commands.txt` in the current directory.
+
+**Config File**
+
+The configuration file in which our encoding properties are defined.
+
+By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
+
+Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+
+**Encoding Properties**
+
+`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
+
+`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
+
+Available bitrate control modes are:
+
+* `CBR` Constant Bitrate Mode
+* `VBR` Variable Bitrate Mode
+* `CQ` Constrained Quality Mode
+
+`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
+
+`Threads` is the number of threads used to encode. Default is 4.
+
+`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
+
+`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
+
+`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
+
+`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
+
+**Logging**
+
+Determines the level of the logging for the program.
+
+`--loglevel error` will only output error messages.
+
+`--loglevel info` will output error messages and script progression info messages.
+
+`--loglevel debug` will output all messages, including variable dumps.
```

### Comparing `animethemes-batch-encoder-1.2/README.md` & `animethemes-batch-encoder-1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,82 @@
-### Description
-
-Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
-
-Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
-
-Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
-
-### Install
-
-**Requirements:**
-
-* FFmpeg
-* Python >= 3.6
-
-**Install:**
-
-    pip install animethemes-batch-encoder
-
-### Usage
-
-        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
-
-**Mode**
-
-`--mode 1` generates commands from input files in the current directory.
-
-The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
-
-`--mode 2` executes commands from file in the current directory line-by-line.
-
-By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
-
-`--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
-
-The `--file` argument will be ignored in this case.
-
-**File**
-
-The file that commands are written to or read from.
-
-By default, the program will write to or read from `commands.txt` in the current directory.
-
-**Config File**
-
-The configuration file in which our encoding properties are defined.
-
-By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
-
-Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
-
-**Encoding Properties**
-
-`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
-
-`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
-
-Available bitrate control modes are:
-
-* `CBR` Constant Bitrate Mode
-* `VBR` Variable Bitrate Mode
-* `CQ` Constrained Quality Mode
-
-`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
-
-`Threads` is the number of threads used to encode. Default is 4.
-
-`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
-
-`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
-
-`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
-
-`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
-
-**Logging**
-
-Determines the level of the logging for the program.
-
-`--loglevel error` will only output error messages.
-
-`--loglevel info` will output error messages and script progression info messages.
-
-`--loglevel debug` will output all messages, including variable dumps.
+### Description
+
+Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
+
+Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
+
+Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
+
+### Install
+
+**Requirements:**
+
+* FFmpeg
+* Python >= 3.6
+
+**Install:**
+
+    pip install animethemes-batch-encoder
+
+### Usage
+
+        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+
+**Mode**
+
+`--mode 1` generates commands from input files in the current directory.
+
+The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time, output file name and new audio filters.
+
+`--mode 2` executes commands from file in the current directory line-by-line.
+
+By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
+
+`--mode 3` generates commands from input files in the current directory and executes the commands sequentially.
+
+**File**
+
+The file that commands are written to or read from.
+
+By default, the program will write to or read from `commands.txt` in the current directory.
+
+**Config File**
+
+The configuration file in which our encoding properties are defined.
+
+By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
+
+Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+
+**Encoding Properties**
+
+`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
+
+`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
+
+Available bitrate control modes are:
+
+* `CBR` Constant Bitrate Mode
+* `VBR` Variable Bitrate Mode
+* `CQ` Constrained Quality Mode
+
+`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
+
+`Threads` is the number of threads used to encode. Default is 4.
+
+`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
+
+`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
+
+`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
+
+`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
+
+**Logging**
+
+Determines the level of the logging for the program.
+
+`--loglevel error` will only output error messages.
+
+`--loglevel info` will output error messages and script progression info messages.
+
+`--loglevel debug` will output all messages, including variable dumps.
```

### Comparing `animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/PKG-INFO` & `animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,104 @@
-Metadata-Version: 2.1
-Name: animethemes-batch-encoder
-Version: 1.2
-Summary: Generate/Execute FFmpeg commands for files in acting directory
-Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
-Author: AnimeThemes
-Author-email: admin@animethemes.moe
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-### Description
-
-Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
-
-Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
-
-Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
-
-### Install
-
-**Requirements:**
-
-* FFmpeg
-* Python >= 3.6
-
-**Install:**
-
-    pip install animethemes-batch-encoder
-
-### Usage
-
-        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
-
-**Mode**
-
-`--mode 1` generates commands from input files in the current directory.
-
-The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time and output file name.
-
-`--mode 2` executes commands from file in the current directory line-by-line.
-
-By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
-
-`--mode 3` generates commands from input files in the current directory and executes the commands sequentially without writing to file.
-
-The `--file` argument will be ignored in this case.
-
-**File**
-
-The file that commands are written to or read from.
-
-By default, the program will write to or read from `commands.txt` in the current directory.
-
-**Config File**
-
-The configuration file in which our encoding properties are defined.
-
-By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
-
-Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
-
-**Encoding Properties**
-
-`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
-
-`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
-
-Available bitrate control modes are:
-
-* `CBR` Constant Bitrate Mode
-* `VBR` Variable Bitrate Mode
-* `CQ` Constrained Quality Mode
-
-`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
-
-`Threads` is the number of threads used to encode. Default is 4.
-
-`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
-
-`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
-
-`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
-
-`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
-
-**Logging**
-
-Determines the level of the logging for the program.
-
-`--loglevel error` will only output error messages.
-
-`--loglevel info` will output error messages and script progression info messages.
-
-`--loglevel debug` will output all messages, including variable dumps.
+Metadata-Version: 2.1
+Name: animethemes-batch-encoder
+Version: 1.3
+Summary: Generate/Execute FFmpeg commands for files in acting directory
+Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
+Author: AnimeThemes
+Author-email: admin@animethemes.moe
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Description
+
+Generate and execute collection of FFmpeg commands sequentially from external file to produce WebMs that meet [AnimeThemes.moe](https://animethemes.moe/) encoding standards.
+
+Take advantage of sleep, work, or any other time that we cannot actively monitor the encoding process to produce a set of encodes for later quality checking and/or tweaking for additional encodes.
+
+Ideally we are iterating over a combination of filters and settings, picking the best one at the end.
+
+### Install
+
+**Requirements:**
+
+* FFmpeg
+* Python >= 3.6
+
+**Install:**
+
+    pip install animethemes-batch-encoder
+
+### Usage
+
+        python -m batch_encoder [-h] --mode [{1,2,3}] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+
+**Mode**
+
+`--mode 1` generates commands from input files in the current directory.
+
+The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time, output file name and new audio filters.
+
+`--mode 2` executes commands from file in the current directory line-by-line.
+
+By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
+
+`--mode 3` generates commands from input files in the current directory and executes the commands sequentially.
+
+**File**
+
+The file that commands are written to or read from.
+
+By default, the program will write to or read from `commands.txt` in the current directory.
+
+**Config File**
+
+The configuration file in which our encoding properties are defined.
+
+By default, the program will write to or read from `batch_encoder.ini` in the user config directory of appname `batch_encoder` and author `AnimeThemes`.
+
+Example: `C:\Users\paranarimasu\AppData\Local\AnimeThemes\batch_encoder\batch_encoder.ini`
+
+**Encoding Properties**
+
+`AllowedFileTypes` is a comma-separated listing of file extensions that will be considered for source file candidates.
+
+`EncodingModes` is a comma-separated listing of [bitrate control modes](https://developers.google.com/media/vp9/bitrate-modes) for inclusion and ordering of commands.
+
+Available bitrate control modes are:
+
+* `CBR` Constant Bitrate Mode
+* `VBR` Variable Bitrate Mode
+* `CQ` Constrained Quality Mode
+
+`CRFs` is a comma-separated listing of ordered CRF values to use with `VBR` and/or `CQ` bitrate control modes.
+
+`Threads` is the number of threads used to encode. Default is 4.
+
+`LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
+
+`AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
+
+`IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
+
+`VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
+
+**Logging**
+
+Determines the level of the logging for the program.
+
+`--loglevel error` will only output error messages.
+
+`--loglevel info` will output error messages and script progression info messages.
+
+`--loglevel debug` will output all messages, including variable dumps.
```

### Comparing `animethemes-batch-encoder-1.2/animethemes_batch_encoder.egg-info/SOURCES.txt` & `animethemes-batch-encoder-1.3/animethemes_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/__main__.py` & `animethemes-batch-encoder-1.3/batch_encoder/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,148 @@
-from ._encode_webm import EncodeWebM
-from ._encoding_config import EncodingConfig
-from ._seek_collector import SeekCollector
-from ._source_file import SourceFile
-from ._utils import commandfile_arg_type
-from ._utils import configfile_arg_type
-from appdirs import AppDirs
-
-import argparse
-import configparser
-import logging
-import os
-import shutil
-import subprocess
-import sys
-
-
-def main():
-    # Load/Validate Arguments
-    parser = argparse.ArgumentParser(prog='batch_encoder',
-                                     description='Generate/Execute FFmpeg commands for files in acting directory',
-                                     formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument('--mode', nargs='?', type=int, choices=[1, 2, 3], required=True,
-                        help='1: Generate commands and write to file\n'
-                             '2: Execute commands from file\n'
-                             '3: Generate and execute commands')
-    parser.add_argument('--file', nargs='?', default='commands.txt', type=commandfile_arg_type,
-                        help='1: Name of file commands are written to (default: commands.txt)\n'
-                             '2: Name of file commands are executed from (default: commands.txt)\n'
-                             '3: Unused')
-    parser.add_argument('--configfile', nargs='?', default='batch_encoder.ini', type=configfile_arg_type,
-                        help='Name of config file (default: batch_encoder.ini)\n'
-                             'If the file does not exist, default configuration will be written\n'
-                             'The file is expected to exist in the same directory as this script')
-    parser.add_argument('--loglevel', nargs='?', default='info', choices=['debug', 'info', 'error'],
-                        help='Set logging level')
-    args = parser.parse_args()
-
-    # Logging Config
-    logging.basicConfig(stream=sys.stdout, level=logging.getLevelName(args.loglevel.upper()),
-                        format='%(levelname)s: %(message)s')
-
-    # Env Check: Check that dependencies are installed
-    if shutil.which('ffmpeg') is None:
-        logging.error('FFmpeg is required')
-        sys.exit()
-
-    if shutil.which('ffprobe') is None:
-        logging.error('FFprobe is required')
-        sys.exit()
-
-    # Write default config file if it doesn't exist
-    config = configparser.ConfigParser()
-    dirs = AppDirs('batch_encoder', 'AnimeThemes')
-    config_file = os.path.join(dirs.user_config_dir, args.configfile)
-    if not os.path.exists(config_file):
-        config['Encoding'] = {EncodingConfig.config_allowed_filetypes: EncodingConfig.default_allowed_filetypes,
-                              EncodingConfig.config_encoding_modes: EncodingConfig.default_encoding_modes,
-                              EncodingConfig.config_crfs: EncodingConfig.default_crfs,
-                              EncodingConfig.config_threads: EncodingConfig.default_threads,
-                              EncodingConfig.config_limit_size_enable: EncodingConfig.default_limit_size_enable,
-                              EncodingConfig.config_alternate_source_files: EncodingConfig.default_alternate_source_files,
-                              EncodingConfig.config_include_unfiltered: EncodingConfig.default_include_unfiltered,
-                              EncodingConfig.config_default_video_stream: '',
-                              EncodingConfig.config_default_audio_stream: ''}
-        config['VideoFilters'] = EncodingConfig.default_video_filters
-
-        os.makedirs(os.path.dirname(config_file), exist_ok=True)
-        with open(config_file, 'w', encoding='utf8') as f:
-            config.write(f)
-
-    # Load config file
-    config.read(config_file)
-    encoding_config = EncodingConfig.from_config(config)
-
-    commands = []
-
-    # Generate commands from source file candidates in current directory
-    if args.mode == 1 or args.mode == 3:
-        source_file_candidates = [f for f in os.listdir('.') if f.endswith(tuple(encoding_config.allowed_filetypes))]
-
-        if not source_file_candidates:
-            logging.error('No source file candidates in current directory')
-            sys.exit()
-
-        for source_file_candidate in source_file_candidates:
-            if SourceFile.yes_or_no(source_file_candidate):
-                try:
-                    source_file = SourceFile.from_file(source_file_candidate, encoding_config)
-
-                    is_collector_valid = False
-                    seek_collector = None
-                    while not is_collector_valid:
-                        seek_collector = SeekCollector(source_file)
-                        is_collector_valid = seek_collector.is_valid()
-
-                    for seek in seek_collector.get_seek_list():
-                        logging.info(f'Generating commands with seek ss: \'{seek.ss}\', to: \'{seek.to}\'')
-                        encode_webm = EncodeWebM(source_file, seek)
-                        load_commands = encode_webm.get_commands(encoding_config)
-                        commands = commands + load_commands
-                except KeyboardInterrupt:
-                    logging.info(f'Exiting from inclusion of file \'{source_file_candidate}\' after keyboard interrupt')
-        
-        # Alternate lines per source files
-        if encoding_config.alternate_source_files == True:
-            output_list = []
-            lines_per_source = len(load_commands)
-            for i in range(lines_per_source):
-                output_list.append(commands[i])
-                for k in range(1, len(commands) // lines_per_source):
-                    output_list.append(commands[i + lines_per_source * k])
-
-            commands = output_list
-
-    # Write commands to file
-    if args.mode == 1:
-        logging.info(f'Writing {len(commands)} commands to file \'{args.file}\'...')
-        with open(args.file, mode='w', encoding='utf8') as f:
-            for command in commands:
-                f.write(command + '\n')
-
-    # Read and execute commands from file
-    if args.mode == 2:
-        if not os.path.isfile(args.file):
-            logging.error(f'File \'{args.file}\' does not exist')
-            sys.exit()
-
-        with open(args.file, mode='r', encoding='utf8') as f:
-            for command in f:
-                commands.append(command)
-
-        logging.info(f'Reading {len(commands)} commands from file \'{args.file}\'...')
-
-        for command in commands:
-            subprocess.call(command, shell=True)
-
-    # Execute commands in memory
-    if args.mode == 3:
-        logging.info(f'Executing {len(commands)} commands...')
-        for command in commands:
-            subprocess.call(command, shell=True)
-
-
-if __name__ == '__main__':
-    try:
-        main()
-    except KeyboardInterrupt:
+from ._encode_webm import EncodeWebM
+from ._encoding_config import EncodingConfig
+from ._seek_collector import SeekCollector
+from ._source_file import SourceFile
+from ._utils import commandfile_arg_type
+from ._utils import configfile_arg_type
+from appdirs import AppDirs
+
+import argparse
+import configparser
+import logging
+import os
+import shutil
+import subprocess
+import sys
+
+
+def main():
+    # Load/Validate Arguments
+    parser = argparse.ArgumentParser(prog='batch_encoder',
+                                     description='Generate/Execute FFmpeg commands for files in acting directory',
+                                     formatter_class=argparse.RawTextHelpFormatter)
+    parser.add_argument('--mode', nargs='?', type=int, choices=[1, 2, 3], required=True,
+                        help='1: Generate commands and write to file\n'
+                             '2: Execute commands from file\n'
+                             '3: Generate and execute commands')
+    parser.add_argument('--file', nargs='?', default='commands.txt', type=commandfile_arg_type,
+                        help='1: Name of file commands are written to (default: commands.txt)\n'
+                             '2: Name of file commands are executed from (default: commands.txt)\n'
+                             '3: Name of file commands are written to (default: commands.txt)')
+    parser.add_argument('--configfile', nargs='?', default='batch_encoder.ini', type=configfile_arg_type,
+                        help='Name of config file (default: batch_encoder.ini)\n'
+                             'If the file does not exist, default configuration will be written\n'
+                             'The file is expected to exist in the same directory as this script')
+    parser.add_argument('--loglevel', nargs='?', default='info', choices=['debug', 'info', 'error'],
+                        help='Set logging level')
+    args = parser.parse_args()
+
+    # Logging Config
+    logging.basicConfig(stream=sys.stdout, level=logging.getLevelName(args.loglevel.upper()),
+                        format='%(levelname)s: %(message)s')
+
+    # Env Check: Check that dependencies are installed
+    if shutil.which('ffmpeg') is None:
+        logging.error('FFmpeg is required')
+        sys.exit()
+
+    if shutil.which('ffprobe') is None:
+        logging.error('FFprobe is required')
+        sys.exit()
+
+    # Write default config file if it doesn't exist
+    config = configparser.ConfigParser()
+    dirs = AppDirs('batch_encoder', 'AnimeThemes')
+    config_file = os.path.join(dirs.user_config_dir, args.configfile)
+    if not os.path.exists(config_file):
+        config['Encoding'] = {EncodingConfig.config_allowed_filetypes: EncodingConfig.default_allowed_filetypes,
+                              EncodingConfig.config_encoding_modes: EncodingConfig.default_encoding_modes,
+                              EncodingConfig.config_crfs: EncodingConfig.default_crfs,
+                              EncodingConfig.config_threads: EncodingConfig.default_threads,
+                              EncodingConfig.config_limit_size_enable: EncodingConfig.default_limit_size_enable,
+                              EncodingConfig.config_alternate_source_files: EncodingConfig.default_alternate_source_files,
+                              EncodingConfig.config_include_unfiltered: EncodingConfig.default_include_unfiltered,
+                              EncodingConfig.config_default_video_stream: '',
+                              EncodingConfig.config_default_audio_stream: ''}
+        config['VideoFilters'] = EncodingConfig.default_video_filters
+
+        os.makedirs(os.path.dirname(config_file), exist_ok=True)
+        with open(config_file, 'w', encoding='utf8') as f:
+            config.write(f)
+
+    # Load config file
+    config.read(config_file)
+    encoding_config = EncodingConfig.from_config(config)
+
+    commands = []
+
+    # Generate commands from source file candidates in current directory
+    if args.mode == 1 or args.mode == 3:
+        source_file_candidates = [f for f in os.listdir('.') if f.endswith(tuple(encoding_config.allowed_filetypes))]
+
+        if not source_file_candidates:
+            logging.error('No source file candidates in current directory')
+            sys.exit()
+
+        for source_file_candidate in source_file_candidates:
+            if SourceFile.yes_or_no(source_file_candidate):
+                try:
+                    source_file = SourceFile.from_file(source_file_candidate, encoding_config)
+
+                    is_collector_valid = False
+                    seek_collector = None
+                    while not is_collector_valid:
+                        seek_collector = SeekCollector(source_file)
+                        is_collector_valid = seek_collector.is_valid()
+
+                    for seek in seek_collector.get_seek_list():
+                        logging.info(f'Generating commands with seek ss: \'{seek.ss}\', to: \'{seek.to}\'')
+                        encode_webm = EncodeWebM(source_file, seek)
+                        load_commands = encode_webm.get_commands(encoding_config)
+                        commands = commands + load_commands
+                except KeyboardInterrupt:
+                    logging.info(f'Exiting from inclusion of file \'{source_file_candidate}\' after keyboard interrupt')
+        
+        # Alternate lines per source files
+        if encoding_config.alternate_source_files == True:
+            output_list = []
+            lines_per_source = len(load_commands)
+            for i in range(lines_per_source):
+                output_list.append(commands[i])
+                for k in range(1, len(commands) // lines_per_source):
+                    output_list.append(commands[i + lines_per_source * k])
+
+            commands = output_list
+
+        # Write commands to file
+        logging.info(f'Writing {len(commands)} commands to file \'{args.file}\'...')
+        with open(args.file, mode='w', encoding='utf8') as f:
+            for command in commands:
+                f.write(command + '\n')
+
+        # Execute commands in memory and write commands to file if requested
+        if args.mode == 3:
+            logging.info(f'Executing {len(commands)} commands...')
+            for command in commands:
+                subprocess.call(command, shell=True)
+
+
+    # Read and execute commands from file
+    if args.mode == 2:
+        if not os.path.isfile(args.file):
+            logging.error(f'File \'{args.file}\' does not exist')
+            sys.exit()
+
+        with open(args.file, mode='r', encoding='utf8') as f:
+            for command in f:
+                commands.append(command)
+
+        logging.info(f'Reading {len(commands)} commands from file \'{args.file}\'...')
+
+        for command in commands:
+            subprocess.call(command, shell=True)
+
+if __name__ == '__main__':
+    try:
+        main()
+    except KeyboardInterrupt:
         logging.error('Exiting after keyboard interrupt')
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_bitrate_mode.py` & `animethemes-batch-encoder-1.3/batch_encoder/_bitrate_mode.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import enum
-
-
-# The Bitrate Mode Enumerated List
-# Bitrate Mode determines the rate control argument values for our commands
-# Further Reading: https://developers.google.com/media/vp9/bitrate-modes
-class BitrateMode(enum.Enum):
-    def __new__(cls, value, first_pass_rate_control, second_pass_rate_control):
-        obj = object.__new__(cls)
-        obj._value_ = value
-        obj.first_pass_rate_control = first_pass_rate_control
-        obj.second_pass_rate_control = second_pass_rate_control
-        return obj
-
-    # Constant Bitrate Mode
-    CBR = (0, lambda cbr_bitrate, cbr_max_bitrate, crf: f'-b:v {cbr_bitrate} -maxrate {cbr_max_bitrate} -qcomp 0.3',
-           lambda cbr_bitrate, cbr_max_bitrate,
-           crf: f'-b:v {cbr_bitrate} -maxrate {cbr_max_bitrate} -bufsize 6000k -qcomp 0.3')
-    # Variable Bitrate Mode / Constant Quality Mode
-    VBR = (1, lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v 0 -qcomp 0.7',
-           lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v 0 -qcomp 0.7')
-    # Constrained Quality Mode
-    CQ = (2, lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v {cbr_bitrate} -qcomp 0.7',
-          lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v {cbr_bitrate} -qcomp 0.7')
+import enum
+
+
+# The Bitrate Mode Enumerated List
+# Bitrate Mode determines the rate control argument values for our commands
+# Further Reading: https://developers.google.com/media/vp9/bitrate-modes
+class BitrateMode(enum.Enum):
+    def __new__(cls, value, first_pass_rate_control, second_pass_rate_control):
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.first_pass_rate_control = first_pass_rate_control
+        obj.second_pass_rate_control = second_pass_rate_control
+        return obj
+
+    # Constant Bitrate Mode
+    CBR = (0, lambda cbr_bitrate, cbr_max_bitrate, crf: f'-b:v {cbr_bitrate} -maxrate {cbr_max_bitrate} -qcomp 0.3',
+           lambda cbr_bitrate, cbr_max_bitrate,
+           crf: f'-b:v {cbr_bitrate} -maxrate {cbr_max_bitrate} -bufsize 6000k -qcomp 0.3')
+    # Variable Bitrate Mode / Constant Quality Mode
+    VBR = (1, lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v 0 -qcomp 0.7',
+           lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v 0 -qcomp 0.7')
+    # Constrained Quality Mode
+    CQ = (2, lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v {cbr_bitrate} -qcomp 0.7',
+          lambda cbr_bitrate, cbr_max_bitrate, crf: f'-crf {crf} -b:v {cbr_bitrate} -qcomp 0.7')
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_colorspace.py` & `animethemes-batch-encoder-1.3/batch_encoder/_colorspace.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import enum
-import logging
-
-
-# The Colorspace Enumerated List
-# Parse color data from file to provide arguments for the encoded file
-class Colorspace(enum.Enum):
-    def __new__(cls, colorspace, color_primaries, color_trc):
-        value = len(cls.__members__) + 1
-        obj = object.__new__(cls)
-        obj._value_ = value
-        obj.colorspace = colorspace
-        obj.color_primaries = color_primaries
-        obj.color_trc = color_trc
-        return obj
-
-    HD = ('bt709', 'bt709', 'bt709')
-    NTSC = ('smpte170m', 'smpte170m', 'smpte170m')
-    PAL = ('bt470bg', 'bt470bg', 'gamma28')
-
-    # The color data arguments for our encode
-    def get_args(self):
-        return f'-colorspace {self.colorspace} -color_primaries {self.color_primaries} -color_trc {self.color_trc}'
-
-    @staticmethod
-    def value_of(source_file):
-        # Method 1: Carry over color data from source if specified
-        source_colorspace = source_file.video_format['streams'][0].get('color_space', '')
-        source_color_primaries = source_file.video_format['streams'][0].get('color_primaries', '')
-        source_color_trc = source_file.video_format['streams'][0].get('color_transfer', '')
-        logging.debug(
-            f'[Colorspace.value_of] source_colorspace: {source_colorspace}, '
-            f'source_color_primaries: {source_color_primaries}, '
-            f'source_color_trc: {source_color_trc}')
-
-        for colorspace_candidate in Colorspace:
-            if (
-                    source_colorspace == colorspace_candidate.colorspace
-                    or source_color_primaries == colorspace_candidate.color_primaries
-                    or source_color_trc == colorspace_candidate.color_trc
-            ):
-                logging.debug(f'[Colorspace.value_of] carryover colorspace \'{colorspace_candidate.name}\' from source')
-                return colorspace_candidate
-
-        # Method 2: Infer color date from source file resolution
-        resolution = int(source_file.video_format['streams'][0]['height'])
-
-        if resolution >= 720:
-            logging.debug(f'[Colorspace.value_of] colorspace: \'{Colorspace.HD.name}\', resolution: \'{resolution}\'')
-            return Colorspace.HD
-        elif resolution >= 576:
-            logging.debug(f'[Colorspace.value_of] colorspace: \'{Colorspace.PAL.name}\', resolution: \'{resolution}\'')
-            return Colorspace.PAL
-        else:
-            logging.debug(f'[Colorspace.value_of] colorspace: \'{Colorspace.NTSC.name}\', resolution: \'{resolution}\'')
-            return Colorspace.NTSC
+import enum
+import logging
+
+
+# The Colorspace Enumerated List
+# Parse color data from file to provide arguments for the encoded file
+class Colorspace(enum.Enum):
+    def __new__(cls, colorspace, color_primaries, color_trc):
+        value = len(cls.__members__) + 1
+        obj = object.__new__(cls)
+        obj._value_ = value
+        obj.colorspace = colorspace
+        obj.color_primaries = color_primaries
+        obj.color_trc = color_trc
+        return obj
+
+    HD = ('bt709', 'bt709', 'bt709')
+    NTSC = ('smpte170m', 'smpte170m', 'smpte170m')
+    PAL = ('bt470bg', 'bt470bg', 'gamma28')
+
+    # The color data arguments for our encode
+    def get_args(self):
+        return f'-colorspace {self.colorspace} -color_primaries {self.color_primaries} -color_trc {self.color_trc}'
+
+    @staticmethod
+    def value_of(source_file):
+        # Method 1: Carry over color data from source if specified
+        source_colorspace = source_file.video_format['streams'][0].get('color_space', '')
+        source_color_primaries = source_file.video_format['streams'][0].get('color_primaries', '')
+        source_color_trc = source_file.video_format['streams'][0].get('color_transfer', '')
+        logging.debug(
+            f'[Colorspace.value_of] source_colorspace: {source_colorspace}, '
+            f'source_color_primaries: {source_color_primaries}, '
+            f'source_color_trc: {source_color_trc}')
+
+        for colorspace_candidate in Colorspace:
+            if (
+                    source_colorspace == colorspace_candidate.colorspace
+                    or source_color_primaries == colorspace_candidate.color_primaries
+                    or source_color_trc == colorspace_candidate.color_trc
+            ):
+                logging.debug(f'[Colorspace.value_of] carryover colorspace \'{colorspace_candidate.name}\' from source')
+                return colorspace_candidate
+
+        # Method 2: Infer color date from source file resolution
+        resolution = int(source_file.video_format['streams'][0]['height'])
+
+        if resolution >= 720:
+            logging.debug(f'[Colorspace.value_of] colorspace: \'{Colorspace.HD.name}\', resolution: \'{resolution}\'')
+            return Colorspace.HD
+        elif resolution >= 576:
+            logging.debug(f'[Colorspace.value_of] colorspace: \'{Colorspace.PAL.name}\', resolution: \'{resolution}\'')
+            return Colorspace.PAL
+        else:
+            logging.debug(f'[Colorspace.value_of] colorspace: \'{Colorspace.NTSC.name}\', resolution: \'{resolution}\'')
+            return Colorspace.NTSC
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_encode_webm.py` & `animethemes-batch-encoder-1.3/batch_encoder/_encode_webm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,239 +1,248 @@
-from ._bitrate_mode import BitrateMode
-from ._colorspace import Colorspace
-from ._loudnorm_filter import LoudnormFilter
-from ._utils import string_to_seconds
-
-import logging
-
-
-# The class that generates FFmpeg commands for the specific cut in the source file
-# We generate common argument values that can be determined programmatically and then use our config to produce commands
-class EncodeWebM:
-    def __init__(self, source_file, seek):
-        self.source_file = source_file
-        self.seek = seek
-        self.loudnorm_filter = LoudnormFilter.from_seek(self.seek)
-        self.g = self.get_keyframe_interval()
-        self.audio_bitrate = self.get_audio_bitrate()
-        self.cbr_bitrate = self.get_cbr_bitrate()
-        self.cbr_max_bitrate = self.get_cbr_max_bitrate()
-        self.colorspace = Colorspace.value_of(self.source_file)
-
-    # We want at least 10 keyframes in our encode and consistency in our interval
-    def get_keyframe_interval(self):
-        source_file_duration = float(self.source_file.file_format['format']['duration'])
-
-        start_time = string_to_seconds(self.seek.ss) if self.seek.ss else 0
-        end_time = string_to_seconds(self.seek.to) if self.seek.to else source_file_duration
-        duration = end_time - start_time
-
-        logging.debug(
-            f'[EncodeWebm.get_keyframe_interval] '
-            f'duration: \'{duration}\', '
-            f'end_time: \'{end_time}\', '
-            f'start_time: \'{start_time}\'')
-
-        if duration < 60:
-            return 96
-        elif duration < 120:
-            return 120
-        else:
-            return 240
-
-    # Audio must use a default bitrate of 192 kbps
-    # Audio must use a bitrate of 320 kbps if the source bitrate is > 320 kbps
-    def get_audio_bitrate(self):
-        audio_bitrate = int(self.source_file.audio_format['format']['bit_rate'])
-
-        logging.debug(f'[EncodeWebm.get_audio_bitrate] audio_bitrate: \'{audio_bitrate}\'')
-
-        if audio_bitrate > 320000:
-            return '320k'
-        else:
-            return '192k'
-
-    # Approximation of target average bitrate near file size limit
-    def get_cbr_bitrate(self):
-        resolution = int(self.source_file.video_format['streams'][0]['height'])
-
-        logging.debug(f'[EncodeWebm.get_cbr_bitrate] resolution: \'{resolution}\'')
-
-        if resolution >= 1080:
-            return '5600k'
-        elif resolution >= 720:
-            return '3700k'
-        elif resolution >= 576:
-            return '3200k'
-        else:
-            return '2400k'
-
-    # Approximation of max overall bitrate near file size limit
-    def get_cbr_max_bitrate(self):
-        resolution = int(self.source_file.video_format['streams'][0]['height'])
-
-        logging.debug(f'[EncodeWebm.get_cbr_max_bitrate] resolution: \'{resolution}\'')
-
-        if resolution >= 1080:
-            return '6400k'
-        elif resolution >= 720:
-            return '4200k'
-        elif resolution >= 576:
-            return '3700k'
-        else:
-            return '3200k'
-
-    # Limiting file size based on resolution and duration
-    def get_limit_file_size(self, video_filters=''):
-        source_file_duration = float(self.source_file.file_format['format']['duration'])
-
-        start_time = string_to_seconds(self.seek.ss) if self.seek.ss else 0
-        end_time = string_to_seconds(self.seek.to) if self.seek.to else source_file_duration
-        duration = end_time - start_time
-
-        for filter in video_filters.split(','):
-            if 'scale=-1:' in filter:
-                resolution = int(filter.split(':')[1])
-                break
-            else:
-                resolution = int(self.source_file.video_format['streams'][0]['height'])
-        
-        logging.debug(f'[EncodeWebm.get_limit_file_size] resolution: \'{resolution}\'')
-
-        max_allowed_bitrate = resolution * 6100 + 475000
-        max_allowed_size = max_allowed_bitrate * duration
-        limit_size = max_allowed_size / 8
-
-        return str(round(limit_size))
-
-    # First-pass encode
-    def get_first_pass(self, encoding_mode, crf=None, threads=4):
-        return f'ffmpeg {self.seek.get_seek_string()} ' \
-               f'-pass 1 -passlogfile {self.seek.output_name} ' \
-               f'-map 0:v:{self.source_file.selected_video_stream} ' \
-               f'-map 0:a:{self.source_file.selected_audio_stream} ' \
-               f'-c:v libvpx-vp9 ' \
-               f'{encoding_mode.first_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
-               f'-cpu-used 4 -g {self.g} -threads {threads} -tile-columns 6 -frame-parallel 0 -auto-alt-ref 1 ' \
-               f'-lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p {self.colorspace.get_args()} -an -sn -f webm -y NUL'
-
-    # Second-pass encode
-    def get_second_pass(self, encoding_mode, crf=None, threads=4, video_filters='', limit_size_enable=True, webm_filename=''):
-        limit_size = '-fs ' + EncodeWebM.get_limit_file_size(self, video_filters=video_filters) + ' ' if limit_size_enable else ''
-        return f'ffmpeg {self.seek.get_seek_string()} ' \
-               f'-pass 2 -passlogfile {self.seek.output_name} ' \
-               f'-map 0:v:{self.source_file.selected_video_stream} ' \
-               f'-map 0:a:{self.source_file.selected_audio_stream} ' \
-               f'-c:v libvpx-vp9 ' \
-               f'{encoding_mode.second_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
-               f'-cpu-used 0 -g {self.g} -threads {threads} {self.get_audio_filters()}{video_filters} -tile-columns 6 ' \
-               f'-frame-parallel 0 -auto-alt-ref 1 -lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p ' \
-               f'{self.colorspace.get_args()} ' \
-               f'-c:a libopus -b:a {self.audio_bitrate} -ar 48k ' \
-               f'{limit_size}' \
-               f'-map_metadata:g -1 -map_metadata:s:v -1 -map_metadata:s:a -1 -map_chapters -1 -sn -f webm -y {webm_filename}.webm'
-
-    # Build audio filtergraph for encodes
-    def get_audio_filters(self):
-        audio_filters = []
-        self.source_file.apply_audio_resampling(audio_filters)
-        audio_filters.append(self.loudnorm_filter.get_normalization_filter())
-        return '-af ' + ','.join(audio_filters)
-
-    # Build video filtergraph for encodes
-    @staticmethod
-    def get_video_filters(config_filter=None):
-        video_filters = []
-
-        if config_filter is not None:
-            video_filters.append(config_filter)
-
-        if not video_filters:
-            return ''
-
-        return ' -vf ' + ','.join(video_filters)
-
-    # Build unique WebM filename for encodes
-    def get_webm_filename(self, crf=None, cbr_bitrate=None, filter_name=None):
-        webm_filename = self.seek.output_name
-
-        if crf is not None:
-            webm_filename += f'-{crf}'
-
-        if cbr_bitrate is not None:
-            webm_filename += f'-{self.cbr_bitrate}'
-
-        if filter_name is not None:
-            webm_filename += f'-{filter_name}'
-
-        return webm_filename
-
-    # Get list of commands in sequence specified by configuration file
-    # Sequencing - 1. Encoding Mode, 2: CRF, 3: Filter mapping
-    def get_commands(self, encoding_config):
-        file_commands = []
-
-        logging.debug(
-            f'[EncodeWebm.get_commands] encoding_modes: \'{encoding_config.encoding_modes}\', '
-            f'crfs: \'{encoding_config.crfs}\', '
-            f'include_unfiltered: \'{encoding_config.include_unfiltered}\', '
-            f'video_filters: \'{encoding_config.video_filters}\'')
-
-        for encoding_mode in encoding_config.encoding_modes:
-            if BitrateMode.CBR.name == encoding_mode.upper():
-                file_commands.append(self.get_first_pass(BitrateMode.CBR, threads=encoding_config.threads))
-                if encoding_config.include_unfiltered:
-                    file_commands.append(self.get_second_pass(BitrateMode.CBR,
-                                                              threads=encoding_config.threads,
-                                                              video_filters=EncodeWebM.get_video_filters(),
-                                                              limit_size_enable=encoding_config.limit_size_enable,
-                                                              webm_filename=self.get_webm_filename(
-                                                                  cbr_bitrate=self.cbr_bitrate)))
-                for filter_name, filter_value in encoding_config.video_filters:
-                    file_commands.append(self.get_second_pass(BitrateMode.CBR,
-                                                              threads=encoding_config.threads,
-                                                              video_filters=EncodeWebM.get_video_filters(
-                                                                  config_filter=filter_value),
-                                                              limit_size_enable=encoding_config.limit_size_enable,
-                                                              webm_filename=self.get_webm_filename(
-                                                                  cbr_bitrate=self.cbr_bitrate,
-                                                                  filter_name=filter_name)))
-            elif BitrateMode.VBR.name == encoding_mode.upper():
-                for crf in encoding_config.crfs:
-                    file_commands.append(self.get_first_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads))
-                    if encoding_config.include_unfiltered:
-                        file_commands.append(
-                            self.get_second_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads, video_filters=EncodeWebM.get_video_filters(),
-                                                 limit_size_enable=encoding_config.limit_size_enable,
-                                                 webm_filename=self.get_webm_filename(crf=crf)))
-                    for filter_name, filter_value in encoding_config.video_filters:
-                        file_commands.append(self.get_second_pass(BitrateMode.VBR, crf=crf,
-                                                                  threads=encoding_config.threads,
-                                                                  video_filters=EncodeWebM.get_video_filters(
-                                                                      config_filter=filter_value),
-                                                                  limit_size_enable=encoding_config.limit_size_enable,
-                                                                  webm_filename=self.get_webm_filename(
-                                                                      crf=crf,
-                                                                      filter_name=filter_name)))
-            elif BitrateMode.CQ.name == encoding_mode.upper():
-                for crf in encoding_config.crfs:
-                    file_commands.append(self.get_first_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads))
-                    if encoding_config.include_unfiltered:
-                        file_commands.append(
-                            self.get_second_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads, video_filters=self.get_video_filters(),
-                                                 limit_size_enable=encoding_config.limit_size_enable,
-                                                 webm_filename=self.get_webm_filename(crf=crf,
-                                                                                      cbr_bitrate=self.cbr_bitrate)))
-                    for filter_name, filter_value in encoding_config.video_filters:
-                        file_commands.append(self.get_second_pass(BitrateMode.CQ, crf=crf,
-                                                                  threads=encoding_config.threads,
-                                                                  video_filters=EncodeWebM.get_video_filters(
-                                                                      config_filter=filter_value),
-                                                                  limit_size_enable=encoding_config.limit_size_enable,
-                                                                  webm_filename=self.get_webm_filename(
-                                                                      crf=crf,
-                                                                      cbr_bitrate=self.cbr_bitrate,
-                                                                      filter_name=filter_name)))
-
-        logging.debug(f'[EncodeWebm.get_commands] # of file_commands: \'{len(file_commands)}\'')
-        
+from ._bitrate_mode import BitrateMode
+from ._colorspace import Colorspace
+from ._loudnorm_filter import LoudnormFilter
+from ._utils import string_to_seconds
+
+import logging
+
+
+# The class that generates FFmpeg commands for the specific cut in the source file
+# We generate common argument values that can be determined programmatically and then use our config to produce commands
+class EncodeWebM:
+    def __init__(self, source_file, seek):
+        self.source_file = source_file
+        self.seek = seek
+        self.loudnorm_filter = LoudnormFilter.from_seek(self.seek)
+        self.g = self.get_keyframe_interval()
+        self.audio_bitrate = self.get_audio_bitrate()
+        self.cbr_bitrate = self.get_cbr_bitrate()
+        self.cbr_max_bitrate = self.get_cbr_max_bitrate()
+        self.colorspace = Colorspace.value_of(self.source_file)
+
+    # We want at least 10 keyframes in our encode and consistency in our interval
+    def get_keyframe_interval(self):
+        source_file_duration = float(self.source_file.file_format['format']['duration'])
+
+        start_time = string_to_seconds(self.seek.ss) if self.seek.ss else 0
+        end_time = string_to_seconds(self.seek.to) if self.seek.to else source_file_duration
+        duration = end_time - start_time
+
+        logging.debug(
+            f'[EncodeWebm.get_keyframe_interval] '
+            f'duration: \'{duration}\', '
+            f'end_time: \'{end_time}\', '
+            f'start_time: \'{start_time}\'')
+
+        if duration < 60:
+            return 96
+        elif duration < 120:
+            return 120
+        else:
+            return 240
+
+    # Audio must use a default bitrate of 192 kbps
+    # Audio must use a bitrate of 320 kbps if the source bitrate is > 320 kbps
+    def get_audio_bitrate(self):
+        audio_bitrate = int(self.source_file.audio_format['format']['bit_rate'])
+
+        logging.debug(f'[EncodeWebm.get_audio_bitrate] audio_bitrate: \'{audio_bitrate}\'')
+
+        if audio_bitrate > 320000:
+            return '320k'
+        else:
+            return '192k'
+
+    # Approximation of target average bitrate near file size limit
+    def get_cbr_bitrate(self):
+        resolution = int(self.source_file.video_format['streams'][0]['height'])
+
+        logging.debug(f'[EncodeWebm.get_cbr_bitrate] resolution: \'{resolution}\'')
+
+        if resolution >= 1080:
+            return '5600k'
+        elif resolution >= 720:
+            return '3700k'
+        elif resolution >= 576:
+            return '3200k'
+        else:
+            return '2400k'
+
+    # Approximation of max overall bitrate near file size limit
+    def get_cbr_max_bitrate(self):
+        resolution = int(self.source_file.video_format['streams'][0]['height'])
+
+        logging.debug(f'[EncodeWebm.get_cbr_max_bitrate] resolution: \'{resolution}\'')
+
+        if resolution >= 1080:
+            return '6400k'
+        elif resolution >= 720:
+            return '4200k'
+        elif resolution >= 576:
+            return '3700k'
+        else:
+            return '3200k'
+
+    # Limiting file size based on resolution and duration
+    def get_limit_file_size(self, video_filters=''):
+        source_file_duration = float(self.source_file.file_format['format']['duration'])
+
+        start_time = string_to_seconds(self.seek.ss) if self.seek.ss else 0
+        end_time = string_to_seconds(self.seek.to) if self.seek.to else source_file_duration
+        duration = end_time - start_time
+
+        for filter in video_filters.split(','):
+            if 'scale=-1:' in filter:
+                resolution = int(filter.split(':')[1])
+                break
+            else:
+                resolution = int(self.source_file.video_format['streams'][0]['height'])
+        
+        logging.debug(f'[EncodeWebm.get_limit_file_size] resolution: \'{resolution}\'')
+
+        max_allowed_bitrate = resolution * 6100 + 475000
+        max_allowed_size = max_allowed_bitrate * duration
+        limit_size = max_allowed_size / 8
+
+        return str(round(limit_size))
+    
+    # Command to preview a seek
+    def preview_seek(self, webm_filename=''):
+        return f'ffmpeg {self.seek.get_seek_string()} ' \
+               f'{self.get_audio_filters()} ' \
+               f'-vcodec copy -c:a aac -b:a 128k -sn -f mp4 {webm_filename}.mp4'
+
+    # First-pass encode
+    def get_first_pass(self, encoding_mode, crf=None, threads=4):
+        return f'ffmpeg {self.seek.get_seek_string()} ' \
+               f'-pass 1 -passlogfile {self.seek.output_name} ' \
+               f'-map 0:v:{self.source_file.selected_video_stream} ' \
+               f'-map 0:a:{self.source_file.selected_audio_stream} ' \
+               f'-c:v libvpx-vp9 ' \
+               f'{encoding_mode.first_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
+               f'-cpu-used 4 -g {self.g} -threads {threads} -tile-columns 6 -frame-parallel 0 -auto-alt-ref 1 ' \
+               f'-lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p {self.colorspace.get_args()} -an -sn -f webm -y NUL'
+
+    # Second-pass encode
+    def get_second_pass(self, encoding_mode, crf=None, threads=4, video_filters='', limit_size_enable=True, webm_filename=''):
+        limit_size = '-fs ' + EncodeWebM.get_limit_file_size(self, video_filters=video_filters) + ' ' if limit_size_enable else ''
+        return f'ffmpeg {self.seek.get_seek_string()} ' \
+               f'-pass 2 -passlogfile {self.seek.output_name} ' \
+               f'-map 0:v:{self.source_file.selected_video_stream} ' \
+               f'-map 0:a:{self.source_file.selected_audio_stream} ' \
+               f'-c:v libvpx-vp9 ' \
+               f'{encoding_mode.second_pass_rate_control(self.cbr_bitrate, self.cbr_max_bitrate, crf)} ' \
+               f'-cpu-used 0 -g {self.g} -threads {threads} {self.get_audio_filters()}{video_filters} -tile-columns 6 ' \
+               f'-frame-parallel 0 -auto-alt-ref 1 -lag-in-frames 25 -row-mt 1 -pix_fmt yuv420p ' \
+               f'{self.colorspace.get_args()} ' \
+               f'-c:a libopus -b:a {self.audio_bitrate} -ar 48k ' \
+               f'{limit_size}' \
+               f'-map_metadata:g -1 -map_metadata:s:v -1 -map_metadata:s:a -1 -map_chapters -1 -sn -f webm -y {webm_filename}.webm'
+
+    # Build audio filtergraph for encodes
+    def get_audio_filters(self):
+        audio_filters = []
+        self.source_file.apply_audio_resampling(audio_filters)
+        audio_filters.append(self.loudnorm_filter.get_normalization_filter())
+        audio_filters.append(self.seek.new_audio_filter) if self.seek.new_audio_filter.strip() != '' else None
+        return '-af ' + ','.join(audio_filters)
+
+    # Build video filtergraph for encodes
+    @staticmethod
+    def get_video_filters(config_filter=None):
+        video_filters = []
+
+        if config_filter is not None:
+            video_filters.append(config_filter)
+
+        if not video_filters:
+            return ''
+
+        return ' -vf ' + ','.join(video_filters)
+
+    # Build unique WebM filename for encodes
+    def get_webm_filename(self, crf=None, cbr_bitrate=None, filter_name=None):
+        webm_filename = self.seek.output_name
+
+        if crf is not None:
+            webm_filename += f'-{crf}'
+
+        if cbr_bitrate is not None:
+            webm_filename += f'-{self.cbr_bitrate}'
+
+        if filter_name is not None:
+            webm_filename += f'-{filter_name}'
+
+        return webm_filename
+
+    # Get list of commands in sequence specified by configuration file
+    # Sequencing - 1. Encoding Mode, 2: CRF, 3: Filter mapping
+    def get_commands(self, encoding_config):
+        file_commands = []
+
+        logging.debug(
+            f'[EncodeWebm.get_commands] encoding_modes: \'{encoding_config.encoding_modes}\', '
+            f'crfs: \'{encoding_config.crfs}\', '
+            f'include_unfiltered: \'{encoding_config.include_unfiltered}\', '
+            f'video_filters: \'{encoding_config.video_filters}\'')
+        
+        file_commands.append(self.preview_seek(webm_filename=self.get_webm_filename()))
+
+        for encoding_mode in encoding_config.encoding_modes:
+            if BitrateMode.CBR.name == encoding_mode.upper():
+                file_commands.append(self.get_first_pass(BitrateMode.CBR, threads=encoding_config.threads))
+                if encoding_config.include_unfiltered:
+                    file_commands.append(self.get_second_pass(BitrateMode.CBR,
+                                                              threads=encoding_config.threads,
+                                                              video_filters=EncodeWebM.get_video_filters(),
+                                                              limit_size_enable=encoding_config.limit_size_enable,
+                                                              webm_filename=self.get_webm_filename(
+                                                                  cbr_bitrate=self.cbr_bitrate)))
+                for filter_name, filter_value in encoding_config.video_filters:
+                    file_commands.append(self.get_second_pass(BitrateMode.CBR,
+                                                              threads=encoding_config.threads,
+                                                              video_filters=EncodeWebM.get_video_filters(
+                                                                  config_filter=filter_value),
+                                                              limit_size_enable=encoding_config.limit_size_enable,
+                                                              webm_filename=self.get_webm_filename(
+                                                                  cbr_bitrate=self.cbr_bitrate,
+                                                                  filter_name=filter_name)))
+            elif BitrateMode.VBR.name == encoding_mode.upper():
+                for crf in encoding_config.crfs:
+                    file_commands.append(self.get_first_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads))
+                    if encoding_config.include_unfiltered:
+                        file_commands.append(
+                            self.get_second_pass(BitrateMode.VBR, crf=crf, threads=encoding_config.threads, video_filters=EncodeWebM.get_video_filters(),
+                                                 limit_size_enable=encoding_config.limit_size_enable,
+                                                 webm_filename=self.get_webm_filename(crf=crf)))
+                    for filter_name, filter_value in encoding_config.video_filters:
+                        file_commands.append(self.get_second_pass(BitrateMode.VBR, crf=crf,
+                                                                  threads=encoding_config.threads,
+                                                                  video_filters=EncodeWebM.get_video_filters(
+                                                                      config_filter=filter_value),
+                                                                  limit_size_enable=encoding_config.limit_size_enable,
+                                                                  webm_filename=self.get_webm_filename(
+                                                                      crf=crf,
+                                                                      filter_name=filter_name)))
+            elif BitrateMode.CQ.name == encoding_mode.upper():
+                for crf in encoding_config.crfs:
+                    file_commands.append(self.get_first_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads))
+                    if encoding_config.include_unfiltered:
+                        file_commands.append(
+                            self.get_second_pass(BitrateMode.CQ, crf=crf, threads=encoding_config.threads, video_filters=self.get_video_filters(),
+                                                 limit_size_enable=encoding_config.limit_size_enable,
+                                                 webm_filename=self.get_webm_filename(crf=crf,
+                                                                                      cbr_bitrate=self.cbr_bitrate)))
+                    for filter_name, filter_value in encoding_config.video_filters:
+                        file_commands.append(self.get_second_pass(BitrateMode.CQ, crf=crf,
+                                                                  threads=encoding_config.threads,
+                                                                  video_filters=EncodeWebM.get_video_filters(
+                                                                      config_filter=filter_value),
+                                                                  limit_size_enable=encoding_config.limit_size_enable,
+                                                                  webm_filename=self.get_webm_filename(
+                                                                      crf=crf,
+                                                                      cbr_bitrate=self.cbr_bitrate,
+                                                                      filter_name=filter_name)))
+
+        logging.debug(f'[EncodeWebm.get_commands] # of file_commands: \'{len(file_commands)}\'')
+        
         return file_commands
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_encoding_config.py` & `animethemes-batch-encoder-1.3/batch_encoder/_encoding_config.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from ._bitrate_mode import BitrateMode
-
-
-class EncodingConfig:
-    # Config keys
-    config_allowed_filetypes = 'AllowedFileTypes'
-    config_encoding_modes = 'EncodingModes'
-    config_crfs = 'CRFs'
-    config_threads = 'Threads'
-    config_limit_size_enable = 'LimitSizeEnable'
-    config_alternate_source_files = 'AlternateSourceFiles'
-    config_include_unfiltered = 'IncludeUnfiltered'
-
-    # Default Config keys
-    config_default_video_stream = 'DefaultVideoStream'
-    config_default_audio_stream = 'DefaultAudioStream'
-
-    # Default config values
-    default_allowed_filetypes = '.avi,.m2ts,.mkv,.mp4,.wmv'
-    default_encoding_modes = f'{BitrateMode.VBR.name},{BitrateMode.CBR.name}'
-    default_crfs = '12,15,18,21,24'
-    default_threads = '4'
-    default_limit_size_enable = True
-    default_alternate_source_files = False
-    default_include_unfiltered = True
-    default_video_filters = {'filtered': 'hqdn3d=0:0:3:3,gradfun,unsharp',
-                             'lightdenoise': 'hqdn3d=0:0:3:3',
-                             'heavydenoise': 'hqdn3d=1.5:1.5:6:6',
-                             'unsharp': 'unsharp'}
-
-    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
-                 default_audio_stream):
-        self.allowed_filetypes = allowed_filetypes
-        self.encoding_modes = encoding_modes
-        self.crfs = crfs
-        self.threads = threads
-        self.limit_size_enable = limit_size_enable
-        self.alternate_source_files = alternate_source_files
-        self.include_unfiltered = include_unfiltered
-        self.video_filters = video_filters
-        self.default_video_stream = default_video_stream
-        self.default_audio_stream = default_audio_stream
-
-    @classmethod
-    def from_config(cls, config):
-        allowed_filetypes = config['Encoding'].get(EncodingConfig.config_allowed_filetypes,
-                                                   EncodingConfig.default_allowed_filetypes).split(',')
-        encoding_modes = config['Encoding'].get(EncodingConfig.config_encoding_modes,
-                                                EncodingConfig.default_encoding_modes).split(',')
-        crfs = config['Encoding'].get(EncodingConfig.config_crfs, EncodingConfig.default_crfs).split(',')
-        threads = config['Encoding'].get(EncodingConfig.config_threads,
-                                         EncodingConfig.default_threads)
-        limit_size_enable = config.getboolean('Encoding', EncodingConfig.config_limit_size_enable, fallback=EncodingConfig.default_limit_size_enable)
-        alternate_source_files = config.getboolean('Encoding', EncodingConfig.config_alternate_source_files, fallback=EncodingConfig.default_alternate_source_files)
-        include_unfiltered = config.getboolean('Encoding', EncodingConfig.config_include_unfiltered,
-                                               fallback=EncodingConfig.default_include_unfiltered)
-        video_filters = config.items('VideoFilters', EncodingConfig.default_video_filters)
-
-        default_video_stream = config['Encoding'].get(EncodingConfig.config_default_video_stream)
-        default_audio_stream = config['Encoding'].get(EncodingConfig.config_default_audio_stream)
-
-        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
-                   default_audio_stream)
-
-    def get_default_stream(self, stream_type):
-        if stream_type == 'video':
-            return self.default_video_stream
-        elif stream_type == 'audio':
-            return self.default_audio_stream
+from ._bitrate_mode import BitrateMode
+
+
+class EncodingConfig:
+    # Config keys
+    config_allowed_filetypes = 'AllowedFileTypes'
+    config_encoding_modes = 'EncodingModes'
+    config_crfs = 'CRFs'
+    config_threads = 'Threads'
+    config_limit_size_enable = 'LimitSizeEnable'
+    config_alternate_source_files = 'AlternateSourceFiles'
+    config_include_unfiltered = 'IncludeUnfiltered'
+
+    # Default Config keys
+    config_default_video_stream = 'DefaultVideoStream'
+    config_default_audio_stream = 'DefaultAudioStream'
+
+    # Default config values
+    default_allowed_filetypes = '.avi,.m2ts,.mkv,.mp4,.wmv'
+    default_encoding_modes = f'{BitrateMode.VBR.name},{BitrateMode.CBR.name}'
+    default_crfs = '12,15,18,21,24'
+    default_threads = '4'
+    default_limit_size_enable = True
+    default_alternate_source_files = False
+    default_include_unfiltered = True
+    default_video_filters = {'filtered': 'hqdn3d=0:0:3:3,gradfun,unsharp',
+                             'lightdenoise': 'hqdn3d=0:0:3:3',
+                             'heavydenoise': 'hqdn3d=1.5:1.5:6:6',
+                             'unsharp': 'unsharp'}
+
+    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
+                 default_audio_stream):
+        self.allowed_filetypes = allowed_filetypes
+        self.encoding_modes = encoding_modes
+        self.crfs = crfs
+        self.threads = threads
+        self.limit_size_enable = limit_size_enable
+        self.alternate_source_files = alternate_source_files
+        self.include_unfiltered = include_unfiltered
+        self.video_filters = video_filters
+        self.default_video_stream = default_video_stream
+        self.default_audio_stream = default_audio_stream
+
+    @classmethod
+    def from_config(cls, config):
+        allowed_filetypes = config['Encoding'].get(EncodingConfig.config_allowed_filetypes,
+                                                   EncodingConfig.default_allowed_filetypes).split(',')
+        encoding_modes = config['Encoding'].get(EncodingConfig.config_encoding_modes,
+                                                EncodingConfig.default_encoding_modes).split(',')
+        crfs = config['Encoding'].get(EncodingConfig.config_crfs, EncodingConfig.default_crfs).split(',')
+        threads = config['Encoding'].get(EncodingConfig.config_threads,
+                                         EncodingConfig.default_threads)
+        limit_size_enable = config.getboolean('Encoding', EncodingConfig.config_limit_size_enable, fallback=EncodingConfig.default_limit_size_enable)
+        alternate_source_files = config.getboolean('Encoding', EncodingConfig.config_alternate_source_files, fallback=EncodingConfig.default_alternate_source_files)
+        include_unfiltered = config.getboolean('Encoding', EncodingConfig.config_include_unfiltered,
+                                               fallback=EncodingConfig.default_include_unfiltered)
+        video_filters = config.items('VideoFilters', EncodingConfig.default_video_filters)
+
+        default_video_stream = config['Encoding'].get(EncodingConfig.config_default_video_stream)
+        default_audio_stream = config['Encoding'].get(EncodingConfig.config_default_audio_stream)
+
+        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
+                   default_audio_stream)
+
+    def get_default_stream(self, stream_type):
+        if stream_type == 'video':
+            return self.default_video_stream
+        elif stream_type == 'audio':
+            return self.default_audio_stream
         return None
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_loudnorm_filter.py` & `animethemes-batch-encoder-1.3/batch_encoder/_loudnorm_filter.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import json
-import logging
-import re
-import shlex
-import subprocess
-
-
-# The audio normalization filter for our encode
-class LoudnormFilter:
-    first_pass_filter = 'loudnorm=I=-16:LRA=20:TP=-1:dual_mono=true:linear=true:print_format=json'
-
-    def __init__(self, input_i, input_lra, input_tp, input_thresh, target_offset):
-        self.input_i = input_i
-        self.input_lra = input_lra
-        self.input_tp = input_tp
-        self.input_thresh = input_thresh
-        self.target_offset = target_offset
-
-    @classmethod
-    def from_seek(cls, seek):
-        logging.info('Retrieving loudness data...')
-        loudnorm_cmd = f'ffmpeg {seek.get_seek_string()} ' \
-                       f'-map 0:a:{seek.source_file.selected_audio_stream} ' \
-                       f'-af {LoudnormFilter.get_first_pass_filters(seek)} ' \
-                       f'-vn -sn -dn -f null /dev/null'
-        loudnorm_args = shlex.split(loudnorm_cmd)
-        loudnorm_output = subprocess.check_output(loudnorm_args, stderr=subprocess.STDOUT).decode('utf-8').strip()
-        loudnorm_stats = re.search('^{[^}]*}$', loudnorm_output, re.MULTILINE)
-        loudnorm_stats = json.loads(loudnorm_stats.group(0))
-
-        logging.debug(
-            f'[Loudnorm.__init__] input_i: \'{loudnorm_stats["input_i"]}\', '
-            f'input_lra: \'{loudnorm_stats["input_lra"]}\', '
-            f'input_tp: \'{loudnorm_stats["input_tp"]}\', '
-            f'input_thresh: \'{loudnorm_stats["input_thresh"]}\', '
-            f'target_offset: \'{loudnorm_stats["target_offset"]}\'')
-
-        return cls(loudnorm_stats['input_i'],
-                   loudnorm_stats['input_lra'],
-                   loudnorm_stats['input_tp'],
-                   loudnorm_stats['input_thresh'],
-                   loudnorm_stats['target_offset'])
-
-    # The audio normalization filter argument for our encode
-    def get_normalization_filter(self):
-        return f'loudnorm=I=-16:LRA=20:TP=-1:dual_mono=true:linear=true:' \
-               f'measured_I={self.input_i}:' \
-               f'measured_LRA={self.input_lra}:' \
-               f'measured_TP={self.input_tp}:' \
-               f'measured_thresh={self.input_thresh}:' \
-               f'offset={self.target_offset}'
-
-    @staticmethod
-    def get_first_pass_filters(seek):
-        audio_filters = []
-        seek.source_file.apply_audio_resampling(audio_filters)
-        audio_filters.append(LoudnormFilter.first_pass_filter)
-        return ','.join(audio_filters)
+import json
+import logging
+import re
+import shlex
+import subprocess
+
+
+# The audio normalization filter for our encode
+class LoudnormFilter:
+    first_pass_filter = 'loudnorm=I=-16:LRA=20:TP=-1:dual_mono=true:linear=true:print_format=json'
+
+    def __init__(self, input_i, input_lra, input_tp, input_thresh, target_offset):
+        self.input_i = input_i
+        self.input_lra = input_lra
+        self.input_tp = input_tp
+        self.input_thresh = input_thresh
+        self.target_offset = target_offset
+
+    @classmethod
+    def from_seek(cls, seek):
+        logging.info('Retrieving loudness data...')
+        loudnorm_cmd = f'ffmpeg {seek.get_seek_string()} ' \
+                       f'-map 0:a:{seek.source_file.selected_audio_stream} ' \
+                       f'-af {LoudnormFilter.get_first_pass_filters(seek)} ' \
+                       f'-vn -sn -dn -f null /dev/null'
+        loudnorm_args = shlex.split(loudnorm_cmd)
+        loudnorm_output = subprocess.check_output(loudnorm_args, stderr=subprocess.STDOUT).decode('utf-8').strip()
+        loudnorm_stats = re.search('^{[^}]*}$', loudnorm_output, re.MULTILINE)
+        loudnorm_stats = json.loads(loudnorm_stats.group(0))
+
+        logging.debug(
+            f'[Loudnorm.__init__] input_i: \'{loudnorm_stats["input_i"]}\', '
+            f'input_lra: \'{loudnorm_stats["input_lra"]}\', '
+            f'input_tp: \'{loudnorm_stats["input_tp"]}\', '
+            f'input_thresh: \'{loudnorm_stats["input_thresh"]}\', '
+            f'target_offset: \'{loudnorm_stats["target_offset"]}\'')
+
+        return cls(loudnorm_stats['input_i'],
+                   loudnorm_stats['input_lra'],
+                   loudnorm_stats['input_tp'],
+                   loudnorm_stats['input_thresh'],
+                   loudnorm_stats['target_offset'])
+
+    # The audio normalization filter argument for our encode
+    def get_normalization_filter(self):
+        return f'loudnorm=I=-16:LRA=20:TP=-1:dual_mono=true:linear=true:' \
+               f'measured_I={self.input_i}:' \
+               f'measured_LRA={self.input_lra}:' \
+               f'measured_TP={self.input_tp}:' \
+               f'measured_thresh={self.input_thresh}:' \
+               f'offset={self.target_offset}'
+
+    @staticmethod
+    def get_first_pass_filters(seek):
+        audio_filters = []
+        seek.source_file.apply_audio_resampling(audio_filters)
+        audio_filters.append(LoudnormFilter.first_pass_filter)
+        return ','.join(audio_filters)
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_seek.py` & `animethemes-batch-encoder-1.3/batch_encoder/_seek.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# The seek information for our encode
-class Seek:
-    def __init__(self, source_file, ss, to, output_name):
-        self.source_file = source_file
-        self.ss = ss
-        self.to = to
-        self.output_name = output_name
-
-    # The seek string arguments for our encode
-    def get_seek_string(self):
-        if len(self.ss) > 0 and len(self.to) > 0:
-            return f'-ss {self.ss} -to {self.to} -i "{self.source_file.file}"'
-        elif len(self.ss) > 0:
-            return f'-ss {self.ss} -i "{self.source_file.file}"'
-        elif len(self.to) > 0:
-            return f'-i "{self.source_file.file}" -to {self.to}'
-        else:
-            return f'-i "{self.source_file.file}"'
+# The seek information for our encode
+class Seek:
+    def __init__(self, source_file, ss, to, output_name, new_audio_filter):
+        self.source_file = source_file
+        self.ss = ss
+        self.to = to
+        self.output_name = output_name
+        self.new_audio_filter = new_audio_filter
+
+    # The seek string arguments for our encode
+    def get_seek_string(self):
+        if len(self.ss) > 0 and len(self.to) > 0:
+            return f'-ss {self.ss} -to {self.to} -i "{self.source_file.file}"'
+        elif len(self.ss) > 0:
+            return f'-ss {self.ss} -i "{self.source_file.file}"'
+        elif len(self.to) > 0:
+            return f'-i "{self.source_file.file}" -to {self.to}'
+        else:
+            return f'-i "{self.source_file.file}"'
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_source_file.py` & `animethemes-batch-encoder-1.3/batch_encoder/_source_file.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import json
-import logging
-import os
-import subprocess
-
-
-# Abstraction of the source file from which we are producing our encodes
-# We are prefetching properties of the source file audio/video streams to help determine encoding argument values
-class SourceFile:
-    format_args = ['ffprobe', '-v', 'quiet', '-print_format', 'json', '-show_streams', '-show_format', '-show_chapters']
-
-    def __init__(self, file, file_format, selected_video_stream, selected_audio_stream, video_format, audio_format):
-        self.file = file
-        self.file_format = file_format
-        self.selected_video_stream = selected_video_stream
-        self.selected_audio_stream = selected_audio_stream
-        self.video_format = video_format
-        self.audio_format = audio_format
-
-    @classmethod
-    def from_file(cls, file, encoding_config):
-        video_file = None
-        audio_file = None
-        try:
-            file_format = SourceFile.get_file_format(file)
-
-            selected_video_stream = SourceFile.get_default_stream(file_format, 'video', encoding_config)
-            if selected_video_stream is None:
-                selected_video_stream = SourceFile.get_selected_stream(file_format, 'video')
-
-            selected_audio_stream = SourceFile.get_default_stream(file_format, 'audio', encoding_config)
-            if selected_audio_stream is None:
-                selected_audio_stream = SourceFile.get_selected_stream(file_format, 'audio')
-
-            logging.info('Retrieving extracted audio/video stream/format data...')
-
-            video_file = '[Video]' + file
-            logging.debug(f'[SourceFile.from_file] video_file: \'{video_file}\'')
-            audio_file = '[Audio]' + file
-            logging.debug(f'[SourceFile.from_file] audio_file: \'{audio_file}\'')
-
-            demux_args = ['ffmpeg', '-i', file, '-v', 'quiet', '-y', '-sn', '-dn', '-map',
-                          f'0:v:{selected_video_stream}', '-vcodec', 'copy', video_file, '-map',
-                          f'0:a:{selected_audio_stream}', '-acodec', 'copy', audio_file]
-            subprocess.call(demux_args)
-
-            video_args = SourceFile.format_args + [video_file]
-            video_format = subprocess.check_output(video_args).decode('utf-8')
-            video_format = json.loads(video_format)
-
-            os.remove(video_file)
-            logging.debug(f'[SourceFile.from_file] video_file deleted: {not os.path.isfile(video_file)}')
-
-            audio_args = SourceFile.format_args + [audio_file]
-            audio_format = subprocess.check_output(audio_args).decode('utf-8')
-            audio_format = json.loads(audio_format)
-
-            os.remove(audio_file)
-            logging.debug(f'[SourceFile.from_file] audio_file deleted: {not os.path.isfile(audio_file)}')
-
-            return cls(file, file_format, selected_video_stream, selected_audio_stream, video_format, audio_format)
-        except KeyboardInterrupt:
-            logging.info('Attempting to delete temp files after keyboard interrupt')
-
-            if os.path.isfile(video_file):
-                os.remove(video_file)
-
-            if os.path.isfile(audio_file):
-                os.remove(audio_file)
-
-            raise
-
-    # Source file streams/formats
-    @staticmethod
-    def get_file_format(file):
-        logging.info('Retrieving source file stream/format data...')
-        format_args = SourceFile.format_args + [file]
-
-        file_format = subprocess.check_output(format_args).decode('utf-8')
-
-        return json.loads(file_format)
-
-    # Get the number of streams of the codec type (audio/video)
-    @staticmethod
-    def get_stream_count(file_format, target_codec_type):
-        count = 0
-
-        for stream in file_format['streams']:
-            if stream['codec_type'] == target_codec_type:
-                count += 1
-
-        logging.debug(f'[SourceFile.get_stream_count] target_codec_type: \'{target_codec_type}\', count: \'{count}\'')
-
-        return count
-
-    # Validate default stream selection before prompting the user to specify which stream to use
-    @staticmethod
-    def get_default_stream(file_format, stream_type, encoding_config):
-        # Exit early if default stream is not set
-        default_stream = encoding_config.get_default_stream(stream_type)
-        if not default_stream:
-            return None
-
-        stream_count = SourceFile.get_stream_count(file_format, stream_type)
-        try:
-            default_stream = int(default_stream)
-            if default_stream in range(stream_count):
-                return default_stream
-            logging.error(f'Default stream selection \'{default_stream}\' is invalid')
-        except ValueError:
-            logging.error(f'Default stream selection \'{default_stream}\' must be an integer')
-
-        return None
-
-    # If there exists more than one stream for a codec type (audio/video),
-    # we want the user to specify which stream to use
-    @staticmethod
-    def get_selected_stream(file_format, stream_type):
-        stream_count = SourceFile.get_stream_count(file_format, stream_type)
-        if stream_count <= 1:
-            return 0
-
-        streams = range(stream_count)
-        prompt_text = f'Select {stream_type} stream [0-{stream_count - 1}]: '
-        while True:
-            try:
-                selected_stream = int(input(prompt_text))
-                if selected_stream in streams:
-                    return selected_stream
-                logging.error('Stream selection is invalid')
-            except ValueError:
-                logging.error('Stream selection must be an integer')
-
-    # Include the source file candidate?
-    @staticmethod
-    def yes_or_no(file):
-        yes = {'yes', 'y', ''}
-        no = {'no', 'n'}
-        while True:
-            choice = input(f'Include file \'{file}\': ').lower()
-            if choice in yes:
-                return True
-            elif choice in no:
-                return False
-            else:
-                logging.error('Please respond with \'y\' or \'n\'')
-
-    # If our source file audio stream is not a 2-channel stereo layout, we need to resample it before normalization
-    def apply_audio_resampling(self, audio_filters):
-        channels = int(self.audio_format['streams'][0].get('channels', 2))
-        channel_layout = self.audio_format['streams'][0].get('channel_layout', 'stereo')
-        if channels != 2 or channel_layout != 'stereo':
-            audio_filters.append('aresample=ochl=stereo')
+import json
+import logging
+import os
+import subprocess
+
+
+# Abstraction of the source file from which we are producing our encodes
+# We are prefetching properties of the source file audio/video streams to help determine encoding argument values
+class SourceFile:
+    format_args = ['ffprobe', '-v', 'quiet', '-print_format', 'json', '-show_streams', '-show_format', '-show_chapters']
+
+    def __init__(self, file, file_format, selected_video_stream, selected_audio_stream, video_format, audio_format):
+        self.file = file
+        self.file_format = file_format
+        self.selected_video_stream = selected_video_stream
+        self.selected_audio_stream = selected_audio_stream
+        self.video_format = video_format
+        self.audio_format = audio_format
+
+    @classmethod
+    def from_file(cls, file, encoding_config):
+        video_file = None
+        audio_file = None
+        try:
+            file_format = SourceFile.get_file_format(file)
+
+            selected_video_stream = SourceFile.get_default_stream(file_format, 'video', encoding_config)
+            if selected_video_stream is None:
+                selected_video_stream = SourceFile.get_selected_stream(file_format, 'video')
+
+            selected_audio_stream = SourceFile.get_default_stream(file_format, 'audio', encoding_config)
+            if selected_audio_stream is None:
+                selected_audio_stream = SourceFile.get_selected_stream(file_format, 'audio')
+
+            logging.info('Retrieving extracted audio/video stream/format data...')
+
+            video_file = '[Video]' + file
+            logging.debug(f'[SourceFile.from_file] video_file: \'{video_file}\'')
+            audio_file = '[Audio]' + file
+            logging.debug(f'[SourceFile.from_file] audio_file: \'{audio_file}\'')
+
+            demux_args = ['ffmpeg', '-i', file, '-v', 'quiet', '-y', '-sn', '-dn', '-map',
+                          f'0:v:{selected_video_stream}', '-vcodec', 'copy', video_file, '-map',
+                          f'0:a:{selected_audio_stream}', '-acodec', 'copy', audio_file]
+            subprocess.call(demux_args)
+
+            video_args = SourceFile.format_args + [video_file]
+            video_format = subprocess.check_output(video_args).decode('utf-8')
+            video_format = json.loads(video_format)
+
+            os.remove(video_file)
+            logging.debug(f'[SourceFile.from_file] video_file deleted: {not os.path.isfile(video_file)}')
+
+            audio_args = SourceFile.format_args + [audio_file]
+            audio_format = subprocess.check_output(audio_args).decode('utf-8')
+            audio_format = json.loads(audio_format)
+
+            os.remove(audio_file)
+            logging.debug(f'[SourceFile.from_file] audio_file deleted: {not os.path.isfile(audio_file)}')
+
+            return cls(file, file_format, selected_video_stream, selected_audio_stream, video_format, audio_format)
+        except KeyboardInterrupt:
+            logging.info('Attempting to delete temp files after keyboard interrupt')
+
+            if os.path.isfile(video_file):
+                os.remove(video_file)
+
+            if os.path.isfile(audio_file):
+                os.remove(audio_file)
+
+            raise
+
+    # Source file streams/formats
+    @staticmethod
+    def get_file_format(file):
+        logging.info('Retrieving source file stream/format data...')
+        format_args = SourceFile.format_args + [file]
+
+        file_format = subprocess.check_output(format_args).decode('utf-8')
+
+        return json.loads(file_format)
+
+    # Get the number of streams of the codec type (audio/video)
+    @staticmethod
+    def get_stream_count(file_format, target_codec_type):
+        count = 0
+
+        for stream in file_format['streams']:
+            if stream['codec_type'] == target_codec_type:
+                count += 1
+
+        logging.debug(f'[SourceFile.get_stream_count] target_codec_type: \'{target_codec_type}\', count: \'{count}\'')
+
+        return count
+
+    # Validate default stream selection before prompting the user to specify which stream to use
+    @staticmethod
+    def get_default_stream(file_format, stream_type, encoding_config):
+        # Exit early if default stream is not set
+        default_stream = encoding_config.get_default_stream(stream_type)
+        if not default_stream:
+            return None
+
+        stream_count = SourceFile.get_stream_count(file_format, stream_type)
+        try:
+            default_stream = int(default_stream)
+            if default_stream in range(stream_count):
+                return default_stream
+            logging.error(f'Default stream selection \'{default_stream}\' is invalid')
+        except ValueError:
+            logging.error(f'Default stream selection \'{default_stream}\' must be an integer')
+
+        return None
+
+    # If there exists more than one stream for a codec type (audio/video),
+    # we want the user to specify which stream to use
+    @staticmethod
+    def get_selected_stream(file_format, stream_type):
+        stream_count = SourceFile.get_stream_count(file_format, stream_type)
+        if stream_count <= 1:
+            return 0
+
+        streams = range(stream_count)
+        prompt_text = f'Select {stream_type} stream [0-{stream_count - 1}]: '
+        while True:
+            try:
+                selected_stream = int(input(prompt_text))
+                if selected_stream in streams:
+                    return selected_stream
+                logging.error('Stream selection is invalid')
+            except ValueError:
+                logging.error('Stream selection must be an integer')
+
+    # Include the source file candidate?
+    @staticmethod
+    def yes_or_no(file):
+        yes = {'yes', 'y', ''}
+        no = {'no', 'n'}
+        while True:
+            choice = input(f'Include file \'{file}\': ').lower()
+            if choice in yes:
+                return True
+            elif choice in no:
+                return False
+            else:
+                logging.error('Please respond with \'y\' or \'n\'')
+
+    # If our source file audio stream is not a 2-channel stereo layout, we need to resample it before normalization
+    def apply_audio_resampling(self, audio_filters):
+        channels = int(self.audio_format['streams'][0].get('channels', 2))
+        channel_layout = self.audio_format['streams'][0].get('channel_layout', 'stereo')
+        if channels != 2 or channel_layout != 'stereo':
+            audio_filters.append('aresample=ochl=stereo')
```

### Comparing `animethemes-batch-encoder-1.2/batch_encoder/_utils.py` & `animethemes-batch-encoder-1.3/batch_encoder/_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import argparse
-import os
-import sys
-
-
-# Convert position to seconds, needed for integrity tests
-def string_to_seconds(time):
-    return sum(x * float(t) for x, t in zip([1, 60, 3600], reversed(time.split(':'))))
-
-
-# Validate Arguments: check that file can be written to
-def file_arg_type(arg_value):
-    if not os.access(arg_value, os.W_OK):
-        try:
-            open(arg_value, 'w').close()
-            os.remove(arg_value)
-        except OSError:
-            raise argparse.ArgumentTypeError(f'File \'{arg_value}\' cannot be created')
-    return arg_value
-
-
-# Validate Arguments: check that command file can be written to and is a TXT file type
-# New users were providing source files for this argument and overwriting them
-def commandfile_arg_type(arg_value):
-    file_arg_type(arg_value)
-    if not arg_value.endswith('.txt'):
-        raise argparse.ArgumentTypeError(f'Command File \'{arg_value}\' must use \'.txt\' file extension')
-    return arg_value
-
-
-# Validate Arguments: check that config file can be written to and is INI file type
-def configfile_arg_type(arg_value):
-    config_file = os.path.join(sys.path[0], arg_value)
-    file_arg_type(config_file)
-    if not arg_value.endswith('.ini'):
-        raise argparse.ArgumentTypeError(f'Config File \'{arg_value}\' must use \'.ini\' file extension')
-    return arg_value
+import argparse
+import os
+import sys
+
+
+# Convert position to seconds, needed for integrity tests
+def string_to_seconds(time):
+    return sum(x * float(t) for x, t in zip([1, 60, 3600], reversed(time.split(':'))))
+
+
+# Validate Arguments: check that file can be written to
+def file_arg_type(arg_value):
+    if not os.access(arg_value, os.W_OK):
+        try:
+            open(arg_value, 'w').close()
+            os.remove(arg_value)
+        except OSError:
+            raise argparse.ArgumentTypeError(f'File \'{arg_value}\' cannot be created')
+    return arg_value
+
+
+# Validate Arguments: check that command file can be written to and is a TXT file type
+# New users were providing source files for this argument and overwriting them
+def commandfile_arg_type(arg_value):
+    file_arg_type(arg_value)
+    if not arg_value.endswith('.txt'):
+        raise argparse.ArgumentTypeError(f'Command File \'{arg_value}\' must use \'.txt\' file extension')
+    return arg_value
+
+
+# Validate Arguments: check that config file can be written to and is INI file type
+def configfile_arg_type(arg_value):
+    config_file = os.path.join(sys.path[0], arg_value)
+    file_arg_type(config_file)
+    if not arg_value.endswith('.ini'):
+        raise argparse.ArgumentTypeError(f'Config File \'{arg_value}\' must use \'.ini\' file extension')
+    return arg_value
```

### Comparing `animethemes-batch-encoder-1.2/setup.py` & `animethemes-batch-encoder-1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-#!/usr/bin/env python3
-
-from setuptools import setup, find_packages
-
-with open('README.md') as f:
-    long_description = f.read()
-
-setup(
-    name='animethemes-batch-encoder',
-    version='1.2',
-    author='AnimeThemes',
-    author_email='admin@animethemes.moe',
-    url='https://github.com/AnimeThemes/animethemes-batch-encoder',
-    description='Generate/Execute FFmpeg commands for files in acting directory',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    packages=find_packages(),
-    classifiers=[
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        'appdirs',
-    ],
-)
+#!/usr/bin/env python3
+
+from setuptools import setup, find_packages
+
+with open('README.md') as f:
+    long_description = f.read()
+
+setup(
+    name='animethemes-batch-encoder',
+    version='1.3',
+    author='AnimeThemes',
+    author_email='admin@animethemes.moe',
+    url='https://github.com/AnimeThemes/animethemes-batch-encoder',
+    description='Generate/Execute FFmpeg commands for files in acting directory',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    packages=find_packages(),
+    classifiers=[
+        'Intended Audience :: Developers',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+    ],
+    python_requires='>=3.6',
+    install_requires=[
+        'appdirs',
+    ],
+)
```

