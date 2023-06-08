# Comparing `tmp/fsrs4anki_optimizer-3.23.0.tar.gz` & `tmp/fsrs4anki_optimizer-3.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.23.0.tar", last modified: Thu Jun  8 19:32:14 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.23.1.tar", last modified: Thu Jun  8 20:49:25 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.23.0.tar` & `fsrs4anki_optimizer-3.23.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-06-08 19:32:14.789601 fsrs4anki_optimizer-3.23.0/
--rw-r--r--   0 jarrettye   (501) staff       (20)      162 2023-06-08 19:32:14.789471 fsrs4anki_optimizer-3.23.0/PKG-INFO
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-06-08 19:32:14.788297 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer/
--rw-r--r--   0 jarrettye   (501) staff       (20)       34 2023-05-10 15:30:52.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 jarrettye   (501) staff       (20)     3940 2023-05-10 15:30:52.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 jarrettye   (501) staff       (20)    43276 2023-06-08 18:38:48.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 jarrettye   (501) staff       (20)        0 2023-06-08 19:32:14.789306 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 jarrettye   (501) staff       (20)      162 2023-06-08 19:32:14.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 jarrettye   (501) staff       (20)      344 2023-06-08 19:32:14.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)        1 2023-06-08 19:32:14.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)      126 2023-06-08 19:32:14.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)       20 2023-06-08 19:32:14.000000 fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 jarrettye   (501) staff       (20)      469 2023-06-08 19:31:47.000000 fsrs4anki_optimizer-3.23.0/pyproject.toml
--rw-r--r--   0 jarrettye   (501) staff       (20)       38 2023-06-08 19:32:14.789642 fsrs4anki_optimizer-3.23.0/setup.cfg
--rw-r--r--   0 jarrettye   (501) staff       (20)       37 2023-06-08 19:24:00.000000 fsrs4anki_optimizer-3.23.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43276 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:49:25.000000 fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:49:25.701580 fsrs4anki_optimizer-3.23.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 20:49:06.000000 fsrs4anki_optimizer-3.23.1/setup.py
```

### Comparing `fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.23.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.23.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files identical despite different names*

