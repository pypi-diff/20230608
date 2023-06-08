# Comparing `tmp/brainbox-0.0.5.tar.gz` & `tmp/brainbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainbox-0.0.5.tar", last modified: Thu Oct 27 15:07:34 2022, max compression
+gzip compressed data, was "brainbox-0.0.6.tar", last modified: Thu Jun  8 16:35:46 2023, max compression
```

## Comparing `brainbox-0.0.5.tar` & `brainbox-0.0.6.tar`

### file list

```diff
@@ -1,61 +1,67 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.144877 brainbox-0.0.5/
--rw-r--r--   0 home       (501) staff       (20)     1068 2021-07-14 10:57:17.000000 brainbox-0.0.5/LICENSE.md
--rw-r--r--   0 home       (501) staff       (20)      485 2022-10-27 15:07:34.144937 brainbox-0.0.5/PKG-INFO
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.136764 brainbox-0.0.5/brainbox/
--rw-r--r--   0 home       (501) staff       (20)        0 2021-02-09 10:40:44.000000 brainbox-0.0.5/brainbox/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.137957 brainbox-0.0.5/brainbox/datasets/
--rw-r--r--   0 home       (501) staff       (20)      249 2022-07-14 13:24:42.000000 brainbox-0.0.5/brainbox/datasets/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     6477 2022-10-04 16:07:50.000000 brainbox-0.0.5/brainbox/datasets/base.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.138497 brainbox-0.0.5/brainbox/datasets/implementations/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.5/brainbox/datasets/implementations/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1511 2022-06-01 11:16:20.000000 brainbox-0.0.5/brainbox/datasets/implementations/singer.py
--rw-r--r--   0 home       (501) staff       (20)     5977 2022-10-04 15:57:25.000000 brainbox-0.0.5/brainbox/datasets/implementations/taylor.py
--rw-r--r--   0 home       (501) staff       (20)     5585 2022-10-27 14:59:45.000000 brainbox-0.0.5/brainbox/datasets/transforms.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.139169 brainbox-0.0.5/brainbox/models/
--rw-r--r--   0 home       (501) staff       (20)       50 2022-06-01 11:02:04.000000 brainbox-0.0.5/brainbox/models/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1738 2022-08-27 10:57:49.000000 brainbox-0.0.5/brainbox/models/model.py
--rw-r--r--   0 home       (501) staff       (20)     2248 2022-09-08 13:04:03.000000 brainbox-0.0.5/brainbox/models/weight_init.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.139602 brainbox-0.0.5/brainbox/physiology/
--rw-r--r--   0 home       (501) staff       (20)      158 2022-10-11 10:14:49.000000 brainbox-0.0.5/brainbox/physiology/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.140247 brainbox-0.0.5/brainbox/physiology/neural/
--rw-r--r--   0 home       (501) staff       (20)       46 2022-10-27 14:43:04.000000 brainbox-0.0.5/brainbox/physiology/neural/__init__.py
--rw-r--r--   0 home       (501) staff       (20)      714 2022-10-27 14:59:44.000000 brainbox-0.0.5/brainbox/physiology/neural/correlation.py
--rw-r--r--   0 home       (501) staff       (20)     1472 2022-10-27 14:43:04.000000 brainbox-0.0.5/brainbox/physiology/neural/rdm.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.140681 brainbox-0.0.5/brainbox/physiology/rfs/
--rw-r--r--   0 home       (501) staff       (20)       19 2022-05-30 04:52:59.000000 brainbox-0.0.5/brainbox/physiology/rfs/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.141219 brainbox-0.0.5/brainbox/physiology/rfs/gabor/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.5/brainbox/physiology/rfs/gabor/__init__.py
--rw-r--r--   0 home       (501) staff       (20)    11574 2022-07-14 14:23:54.000000 brainbox-0.0.5/brainbox/physiology/rfs/gabor/fit.py
--rw-r--r--   0 home       (501) staff       (20)     6960 2022-07-14 14:26:14.000000 brainbox-0.0.5/brainbox/physiology/rfs/gabor/query.py
--rw-r--r--   0 home       (501) staff       (20)     3304 2022-05-30 04:52:59.000000 brainbox-0.0.5/brainbox/physiology/rfs/rfs.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.142298 brainbox-0.0.5/brainbox/physiology/spiking/
--rw-r--r--   0 home       (501) staff       (20)      155 2022-05-30 04:44:08.000000 brainbox-0.0.5/brainbox/physiology/spiking/__init__.py
--rw-r--r--   0 home       (501) staff       (20)      994 2022-05-30 04:52:59.000000 brainbox-0.0.5/brainbox/physiology/spiking/burst.py
--rw-r--r--   0 home       (501) staff       (20)     1473 2022-06-07 20:59:50.000000 brainbox-0.0.5/brainbox/physiology/spiking/isi.py
--rw-r--r--   0 home       (501) staff       (20)     1916 2022-10-27 14:59:45.000000 brainbox-0.0.5/brainbox/physiology/spiking/rate.py
--rw-r--r--   0 home       (501) staff       (20)     1619 2022-06-07 21:17:20.000000 brainbox-0.0.5/brainbox/physiology/spiking/synchrony.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.143139 brainbox-0.0.5/brainbox/physiology/tuning/
--rw-r--r--   0 home       (501) staff       (20)       40 2022-07-13 13:42:58.000000 brainbox-0.0.5/brainbox/physiology/tuning/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     9738 2022-07-15 12:03:41.000000 brainbox-0.0.5/brainbox/physiology/tuning/fit.py
--rw-r--r--   0 home       (501) staff       (20)     3064 2022-10-27 14:59:45.000000 brainbox-0.0.5/brainbox/physiology/tuning/fitters.py
--rw-r--r--   0 home       (501) staff       (20)     9174 2022-10-27 14:43:04.000000 brainbox-0.0.5/brainbox/physiology/tuning/query.py
--rw-r--r--   0 home       (501) staff       (20)     2363 2022-05-30 04:52:59.000000 brainbox-0.0.5/brainbox/physiology/util.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.144046 brainbox-0.0.5/brainbox/trainer/
--rw-r--r--   0 home       (501) staff       (20)      408 2022-06-01 11:02:43.000000 brainbox-0.0.5/brainbox/trainer/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1248 2022-08-27 21:50:53.000000 brainbox-0.0.5/brainbox/trainer/query.py
--rw-r--r--   0 home       (501) staff       (20)     6532 2022-10-09 18:29:44.000000 brainbox-0.0.5/brainbox/trainer/trainer.py
--rw-r--r--   0 home       (501) staff       (20)     1785 2022-10-27 14:43:04.000000 brainbox-0.0.5/brainbox/trainer/validator.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.137332 brainbox-0.0.5/brainbox.egg-info/
--rw-r--r--   0 home       (501) staff       (20)      485 2022-10-27 15:07:34.000000 brainbox-0.0.5/brainbox.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     1440 2022-10-27 15:07:34.000000 brainbox-0.0.5/brainbox.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2022-10-27 15:07:34.000000 brainbox-0.0.5/brainbox.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       43 2022-10-27 15:07:34.000000 brainbox-0.0.5/brainbox.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)       15 2022-10-27 15:07:34.000000 brainbox-0.0.5/brainbox.egg-info/top_level.txt
--rw-r--r--   0 home       (501) staff       (20)       93 2022-05-30 06:26:36.000000 brainbox-0.0.5/pyproject.toml
--rw-r--r--   0 home       (501) staff       (20)      577 2022-10-27 15:07:34.145235 brainbox-0.0.5/setup.cfg
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.144217 brainbox-0.0.5/tests/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.5/tests/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-10-27 15:07:34.144629 brainbox-0.0.5/tests/physiology/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.5/tests/physiology/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1557 2022-05-30 04:52:59.000000 brainbox-0.0.5/tests/physiology/test_spiking.py
--rw-r--r--   0 home       (501) staff       (20)     1439 2022-05-30 04:52:59.000000 brainbox-0.0.5/tests/physiology/test_util.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620986 brainbox-0.0.6/
+-rw-r--r--   0 home       (501) staff       (20)     1068 2021-07-14 10:57:17.000000 brainbox-0.0.6/LICENSE.md
+-rw-r--r--   0 home       (501) staff       (20)      485 2023-06-08 16:35:46.621052 brainbox-0.0.6/PKG-INFO
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.610231 brainbox-0.0.6/brainbox/
+-rw-r--r--   0 home       (501) staff       (20)       95 2023-02-22 17:29:14.000000 brainbox-0.0.6/brainbox/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.611664 brainbox-0.0.6/brainbox/datasets/
+-rw-r--r--   0 home       (501) staff       (20)      291 2022-11-01 19:02:15.000000 brainbox-0.0.6/brainbox/datasets/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     7111 2023-04-24 11:06:24.000000 brainbox-0.0.6/brainbox/datasets/base.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.612465 brainbox-0.0.6/brainbox/datasets/implementations/
+-rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/brainbox/datasets/implementations/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1511 2022-06-01 11:16:20.000000 brainbox-0.0.6/brainbox/datasets/implementations/singer.py
+-rw-r--r--   0 home       (501) staff       (20)     5977 2023-04-13 11:08:34.000000 brainbox-0.0.6/brainbox/datasets/implementations/taylor.py
+-rw-r--r--   0 home       (501) staff       (20)     7192 2023-06-01 15:44:40.000000 brainbox-0.0.6/brainbox/datasets/transforms.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.613247 brainbox-0.0.6/brainbox/models/
+-rw-r--r--   0 home       (501) staff       (20)       50 2022-06-01 11:02:04.000000 brainbox-0.0.6/brainbox/models/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1738 2023-04-25 14:47:43.000000 brainbox-0.0.6/brainbox/models/model.py
+-rw-r--r--   0 home       (501) staff       (20)     2248 2023-01-19 11:19:22.000000 brainbox-0.0.6/brainbox/models/weight_init.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.613708 brainbox-0.0.6/brainbox/physiology/
+-rw-r--r--   0 home       (501) staff       (20)      157 2023-05-31 14:22:23.000000 brainbox-0.0.6/brainbox/physiology/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.614394 brainbox-0.0.6/brainbox/physiology/neural/
+-rw-r--r--   0 home       (501) staff       (20)       46 2022-10-27 14:43:04.000000 brainbox-0.0.6/brainbox/physiology/neural/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1979 2023-03-23 16:58:09.000000 brainbox-0.0.6/brainbox/physiology/neural/correlation.py
+-rw-r--r--   0 home       (501) staff       (20)     1743 2023-03-16 16:42:25.000000 brainbox-0.0.6/brainbox/physiology/neural/rdm.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.614921 brainbox-0.0.6/brainbox/physiology/rfs/
+-rw-r--r--   0 home       (501) staff       (20)       19 2022-05-30 04:52:59.000000 brainbox-0.0.6/brainbox/physiology/rfs/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.615545 brainbox-0.0.6/brainbox/physiology/rfs/gabor/
+-rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/brainbox/physiology/rfs/gabor/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)    11574 2023-06-02 11:59:50.000000 brainbox-0.0.6/brainbox/physiology/rfs/gabor/fit.py
+-rw-r--r--   0 home       (501) staff       (20)     6962 2023-06-02 12:43:09.000000 brainbox-0.0.6/brainbox/physiology/rfs/gabor/query.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.616122 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-06-01 17:12:08.000000 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)    10189 2023-06-02 13:59:42.000000 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/fit.py
+-rw-r--r--   0 home       (501) staff       (20)     5121 2023-06-02 12:44:44.000000 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/query.py
+-rw-r--r--   0 home       (501) staff       (20)     3303 2023-06-02 12:54:56.000000 brainbox-0.0.6/brainbox/physiology/rfs/rfs.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.617859 brainbox-0.0.6/brainbox/physiology/spiking/
+-rw-r--r--   0 home       (501) staff       (20)      172 2023-05-31 14:23:15.000000 brainbox-0.0.6/brainbox/physiology/spiking/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)      994 2022-05-30 04:52:59.000000 brainbox-0.0.6/brainbox/physiology/spiking/burst.py
+-rw-r--r--   0 home       (501) staff       (20)     1473 2023-05-31 14:21:02.000000 brainbox-0.0.6/brainbox/physiology/spiking/isi.py
+-rw-r--r--   0 home       (501) staff       (20)     1350 2023-05-18 11:53:28.000000 brainbox-0.0.6/brainbox/physiology/spiking/metric.py
+-rw-r--r--   0 home       (501) staff       (20)     1916 2022-10-27 14:59:45.000000 brainbox-0.0.6/brainbox/physiology/spiking/rate.py
+-rw-r--r--   0 home       (501) staff       (20)     1619 2022-06-07 21:17:20.000000 brainbox-0.0.6/brainbox/physiology/spiking/synchrony.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.618726 brainbox-0.0.6/brainbox/physiology/tuning/
+-rw-r--r--   0 home       (501) staff       (20)       40 2022-07-13 13:42:58.000000 brainbox-0.0.6/brainbox/physiology/tuning/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     9769 2023-02-22 17:29:15.000000 brainbox-0.0.6/brainbox/physiology/tuning/fit.py
+-rw-r--r--   0 home       (501) staff       (20)     3064 2022-10-27 14:59:45.000000 brainbox-0.0.6/brainbox/physiology/tuning/fitters.py
+-rw-r--r--   0 home       (501) staff       (20)     9228 2022-11-25 15:50:08.000000 brainbox-0.0.6/brainbox/physiology/tuning/query.py
+-rw-r--r--   0 home       (501) staff       (20)     2363 2022-05-30 04:52:59.000000 brainbox-0.0.6/brainbox/physiology/util.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620055 brainbox-0.0.6/brainbox/trainer/
+-rw-r--r--   0 home       (501) staff       (20)      537 2023-02-27 11:23:54.000000 brainbox-0.0.6/brainbox/trainer/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     5616 2023-03-22 15:49:51.000000 brainbox-0.0.6/brainbox/trainer/crossval.py
+-rw-r--r--   0 home       (501) staff       (20)     1248 2023-03-25 08:45:35.000000 brainbox-0.0.6/brainbox/trainer/query.py
+-rw-r--r--   0 home       (501) staff       (20)     6822 2023-06-08 08:37:21.000000 brainbox-0.0.6/brainbox/trainer/trainer.py
+-rw-r--r--   0 home       (501) staff       (20)     2097 2023-05-08 16:21:07.000000 brainbox-0.0.6/brainbox/trainer/validator.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.611009 brainbox-0.0.6/brainbox.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)      485 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     1634 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       43 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)       15 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/top_level.txt
+-rw-r--r--   0 home       (501) staff       (20)       93 2022-05-30 06:26:36.000000 brainbox-0.0.6/pyproject.toml
+-rw-r--r--   0 home       (501) staff       (20)      577 2023-06-08 16:35:46.621377 brainbox-0.0.6/setup.cfg
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620289 brainbox-0.0.6/tests/
+-rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/tests/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620723 brainbox-0.0.6/tests/physiology/
+-rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/tests/physiology/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1557 2022-05-30 04:52:59.000000 brainbox-0.0.6/tests/physiology/test_spiking.py
+-rw-r--r--   0 home       (501) staff       (20)     1439 2022-05-30 04:52:59.000000 brainbox-0.0.6/tests/physiology/test_util.py
```

### Comparing `brainbox-0.0.5/LICENSE.md` & `brainbox-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/datasets/base.py` & `brainbox-0.0.6/brainbox/datasets/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 import torch
 
 
+class BasicBBDataset(torch.utils.data.Dataset):
+    def __init__(self, train, transform):
+        self._train = train
+        self._transform = transform
+
+    def __getitem__(self, i):
+        x, y = self.get_item(i)
+
+        if self._transform is not None:
+            x = self._transform(x)
+
+        return x, y
+
+    @property
+    def hyperparams(self):
+        hyperparams = {"name": self.__class__.__name__, "train": self._train}
+
+        if self._transform is not None:
+            hyperparams["transform"] = self._transform.hyperparams
+
+        return hyperparams
+
+    def get_item(self, i):
+        raise NotImplementedError
+
+
 class BBDataset(torch.utils.data.Dataset):
     def __init__(
         self,
         root,
         train=True,
         preprocess=None,
         transform=None,
```

### Comparing `brainbox-0.0.5/brainbox/datasets/implementations/singer.py` & `brainbox-0.0.6/brainbox/datasets/implementations/singer.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/datasets/implementations/taylor.py` & `brainbox-0.0.6/brainbox/datasets/implementations/taylor.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/models/model.py` & `brainbox-0.0.6/brainbox/models/model.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/models/weight_init.py` & `brainbox-0.0.6/brainbox/models/weight_init.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/neural/rdm.py` & `brainbox-0.0.6/brainbox/physiology/neural/rdm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 import torch
 import scipy
 import numpy as np
 
 # Adapted from Patrick Mineault (https://github.com/patrickmineault/your-head-is-there-to-move-you-around)
 
 
-def compute_rdm(X):
-    assert len(X.shape) == 2
-    return 1 - np.corrcoef(X)
+def compute_rdm(x):
+    # x: stimuli x neurons
+    assert len(x.shape) == 2
+    return torch.Tensor(1 - np.corrcoef(x))
+
+
+def rdm_distance(x, y, method="spearman"):
+    rdm_x = compute_rdm(x)
+    rdm_y = compute_rdm(y)
+    mean_deviation = compute_rdm_distance_from_rdms(rdm_x, rdm_y, method)
+
+    return mean_deviation
 
 
 def bootstrap_rdm_distance(X, Y, method="spearman", nboot=100):
     rdm_X = compute_rdm(X)
     rdm_Y = compute_rdm(Y)
-    mean_deviation = compute_rdm_distance(rdm_X, rdm_Y, method)
+    mean_deviation = compute_rdm_distance_from_rdms(rdm_X, rdm_Y, method)
     std_deviation = np.std(
         [
-            compute_rdm_distance(
+            compute_rdm_distance_from_rdms(
                 rdm_X,
                 compute_rdm(
                     Y[:, np.random.randint(low=0, high=Y.shape[1], size=Y.shape[1])]
                 ),
                 method,
             )
             for _ in range(nboot)
         ]
     )
 
     return mean_deviation, std_deviation
 
 
-def compute_rdm_distance(rdm_X, rdm_Y, method="spearman"):
+def compute_rdm_distance_from_rdms(rdm_X, rdm_Y, method="spearman"):
     assert rdm_X.shape[0] == rdm_X.shape[1]
     assert rdm_Y.shape[0] == rdm_Y.shape[1]
     assert rdm_X.shape == rdm_Y.shape
 
     ii, jj = np.triu_indices(rdm_X.shape[0], k=1)
     if method == "pearson":
         corr = np.corrcoef(rdm_X[ii, jj], rdm_Y[ii, jj])
```

### Comparing `brainbox-0.0.5/brainbox/physiology/rfs/gabor/fit.py` & `brainbox-0.0.6/brainbox/physiology/rfs/gabor/fit.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/rfs/gabor/query.py` & `brainbox-0.0.6/brainbox/physiology/rfs/gabor/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
         return temporal_profiles, rr
 
     def _query_cc(self, min_cc):
         return self._params_df["cc"] > min_cc
 
     def _query_location(self):
-        query = (0 < self._params_df["x0"]) & (self._params_df["x0"] < self._rf_size)
-        query &= (0 < self._params_df["y0"]) & (self._params_df["y0"] < self._rf_size)
+        query = (0 <= self._params_df["x0"]) & (self._params_df["x0"] < self._rf_size)
+        query &= (0 <= self._params_df["y0"]) & (self._params_df["y0"] < self._rf_size)
 
         return query
 
     def _query_envelope(self, min_env):
         query = self._params_df["sigmax"] > min_env
         query &= self._params_df["sigmay"] > min_env
```

### Comparing `brainbox-0.0.5/brainbox/physiology/rfs/rfs.py` & `brainbox-0.0.6/brainbox/physiology/rfs/rfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     t = power_at_timesteps.argmax().item()
     spatial_rf = spatiotemporal_rf[t]
 
     return spatial_rf
 
 
 def get_all_highest_power_spatial_rf(spatiotemporal_rfs):
-
     """
     Obtain the spatial RFs with largest mean power from the provided set of spatiotemporal RFs. The mean power is
     calculated as the mean over both spatial dimensions of the squared values of the spatial RFs at every time step.
 
     :param spatiotemporal_rfs: A tensor of shape n_units x rf_len x rf_w x rf_h
     :return: A tensor of shape n_units x rf_w x rf_h
     """
```

### Comparing `brainbox-0.0.5/brainbox/physiology/spiking/burst.py` & `brainbox-0.0.6/brainbox/physiology/spiking/burst.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/spiking/isi.py` & `brainbox-0.0.6/brainbox/physiology/spiking/isi.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/spiking/rate.py` & `brainbox-0.0.6/brainbox/physiology/spiking/rate.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/spiking/synchrony.py` & `brainbox-0.0.6/brainbox/physiology/spiking/synchrony.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/tuning/fit.py` & `brainbox-0.0.6/brainbox/physiology/tuning/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
             self.duration,
             self.dt,
             batch_size=response_batch,
             device=device,
         )
         torch.save(gratings.cpu(), os.path.join(path, "gratings.pt"))
         torch.save(unit_responses.cpu(), os.path.join(path, "unit_responses.pt"))
-
         self.compute_and_save_spectral_analysis(spectral_path, unit_responses)
 
     def probe(self, path, batch_size=1024, device="cuda"):
         def populate_mean_model_responses(batch_gratings, model_output_list):
             batch_gratings = torch.stack(batch_gratings).to(device)
             model_outputs = self.model(batch_gratings)
             model_outputs = model_outputs.mean(dim=2)
@@ -195,16 +194,17 @@
 
         if unit_id is not None:
             return self.model(gratings.unsqueeze(0))[0, int(unit_id)]
         else:
             batch_response_to_preferred_grating = []
 
             for i in range(
-                self._tuning_query.n_units // batch_size
-                + self._tuning_query.n_units % batch_size
+                self._tuning_query.n_units // batch_size + 1
+                if self._tuning_query.n_units % batch_size > 0
+                else 0
             ):
                 batch_gratings = gratings[i * batch_size : (i + 1) * batch_size]
                 batch_response_to_preferred_grating.append(self.model(batch_gratings))
 
             response_to_preferred_grating = torch.cat(
                 batch_response_to_preferred_grating
             )
```

### Comparing `brainbox-0.0.5/brainbox/physiology/tuning/fitters.py` & `brainbox-0.0.6/brainbox/physiology/tuning/fitters.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/physiology/tuning/query.py` & `brainbox-0.0.6/brainbox/physiology/tuning/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,19 @@
             if os.path.exists(os.path.join(path, "spectral.csv"))
             else None
         )
         self._probes_df = pd.read_csv(probe_path)
         self._spectral_df = (
             pd.read_csv(spectral_path) if spectral_path is not None else None
         )
-        self._gratings = torch.load(os.path.join(path, "gratings.pt"))
-        self._responses = torch.load(os.path.join(path, "unit_responses.pt"))
+        try:
+            self._gratings = torch.load(os.path.join(path, "gratings.pt"))
+            self._responses = torch.load(os.path.join(path, "unit_responses.pt"))
+        except:
+            pass
 
     @property
     def n_units(self):
         return len(self._probes_df.columns) - 3
 
     def build_sinusoid_from_spectral(self, unit_id):
         spectral_data = self._spectral_df.iloc[unit_id]
```

### Comparing `brainbox-0.0.5/brainbox/physiology/util.py` & `brainbox-0.0.6/brainbox/physiology/util.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/trainer/query.py` & `brainbox-0.0.6/brainbox/trainer/query.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/brainbox/trainer/trainer.py` & `brainbox-0.0.6/brainbox/trainer/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,14 @@
             self.train_dataset, self.batch_size, **loader_kwargs
         )
 
         self.optimizer = self.optimizer_func(
             self.model.parameters(), self.lr, **optimizer_kwargs
         )
         if self.scheduler_func is not None:
-            print("scheduler_func", scheduler_func)
-            print("self.scheduler_kwargs", self.scheduler_kwargs)
             self.scheduler = scheduler_func(self.optimizer, **self.scheduler_kwargs)
         else:
             self.scheduler = None
 
         # Register grad clippings
         if self.grad_clip_type == Trainer.GRAD_VALUE_CLIP_PRE:
 
@@ -89,14 +87,15 @@
         self.model = self.model.to(device)
         if dtype == torch.float:
             self.model = self.model.float()
         elif dtype == torch.half:
             self.model = self.model.half()
         self.model.train()
         self.date = datetime.today().strftime("%Y-%m-%d-%H:%M:%S")
+        self.exit = False
 
     @property
     def hyperparams(self):
         hyperparams = {
             "trainer": {
                 "date": self.date,
                 "n_epochs": self.n_epochs,
@@ -153,16 +152,25 @@
         if save:
             self.save_model()
 
     def train_for_single_epoch(self):
         epoch_loss = 0
 
         for batch_id, (data, target) in enumerate(self.train_data_loader):
-            data = data.to(self.device).type(self.dtype)
-            target = target.to(self.device).type(self.dtype)
+            if type(data) == list:
+                data = [element.to(self.device).type(self.dtype) for element in data]
+            else:
+                data = data.to(self.device).type(self.dtype)
+
+            if type(target) == list:
+                target = [
+                    element.to(self.device).type(self.dtype) for element in target
+                ]
+            else:
+                target = target.to(self.device).type(self.dtype)
 
             self.optimizer.zero_grad()
             output = self.model(data)
             loss = self.loss(output, target, self.model)
             epoch_loss += loss.item()
             loss.backward()
 
@@ -183,19 +191,21 @@
         if self.scheduler is not None:
             self.scheduler.step()
 
         return epoch_loss
 
     def train(self, save=False):
         if save:
-            os.mkdir(os.path.join(self.root, self.id))
+            os.makedirs(os.path.join(self.root, self.id))
 
         self.on_training_start(save)
 
         for epoch in range(self.n_epochs):
+            if self.exit:
+                break
             # Train the model
             start_time = time.time()
             epoch_loss = self.train_for_single_epoch()
             end_time = time.time()
             epoch_duration = end_time - start_time
             logger.info(
                 f"Completed epoch {epoch} with loss {epoch_loss} in {epoch_duration:.4f}s"
```

### Comparing `brainbox-0.0.5/brainbox/trainer/validator.py` & `brainbox-0.0.6/brainbox/trainer/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,16 +51,26 @@
 ):
     metric_list = []
 
     data_loader = torch.utils.data.DataLoader(dataset, batch_size)
 
     with torch.no_grad():
         for data, target in data_loader:
-            data = data.to(device).type(dtype)
-            target = target.to(device).type(dtype)
+            if type(data) == list:
+                data = [element.to(device).type(dtype) for element in data]
+            else:
+                data = data.to(device).type(dtype)
+
+            if type(target) == list:
+                target = [
+                    element.to(device).type(dtype) for element in target
+                ]
+            else:
+                target = target.to(device).type(dtype)
+
             if len(kwargs) > 0:
                 output = model(data, **kwargs)
             else:
                 output = model(data)
             metric_value = metric(output, target)
             metric_list.append(metric_value)
```

### Comparing `brainbox-0.0.5/brainbox.egg-info/SOURCES.txt` & `brainbox-0.0.6/brainbox.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,24 +22,29 @@
 brainbox/physiology/neural/correlation.py
 brainbox/physiology/neural/rdm.py
 brainbox/physiology/rfs/__init__.py
 brainbox/physiology/rfs/rfs.py
 brainbox/physiology/rfs/gabor/__init__.py
 brainbox/physiology/rfs/gabor/fit.py
 brainbox/physiology/rfs/gabor/query.py
+brainbox/physiology/rfs/gaussian/__init__.py
+brainbox/physiology/rfs/gaussian/fit.py
+brainbox/physiology/rfs/gaussian/query.py
 brainbox/physiology/spiking/__init__.py
 brainbox/physiology/spiking/burst.py
 brainbox/physiology/spiking/isi.py
+brainbox/physiology/spiking/metric.py
 brainbox/physiology/spiking/rate.py
 brainbox/physiology/spiking/synchrony.py
 brainbox/physiology/tuning/__init__.py
 brainbox/physiology/tuning/fit.py
 brainbox/physiology/tuning/fitters.py
 brainbox/physiology/tuning/query.py
 brainbox/trainer/__init__.py
+brainbox/trainer/crossval.py
 brainbox/trainer/query.py
 brainbox/trainer/trainer.py
 brainbox/trainer/validator.py
 tests/__init__.py
 tests/physiology/__init__.py
 tests/physiology/test_spiking.py
 tests/physiology/test_util.py
```

### Comparing `brainbox-0.0.5/setup.cfg` & `brainbox-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = brainbox
-version = 0.0.5
+version = 0.0.6
 author = Luke Taylor
 author_email = webstorms@gmail.com
 description = Simplifying the life of a computational neuroscientist.
 url = https://github.com/webstorms/BrainBox
 project_urls = 
 	Bug Tracker = https://github.com/webstorms/BrainBox/issues
 classifiers =
```

### Comparing `brainbox-0.0.5/tests/physiology/test_spiking.py` & `brainbox-0.0.6/tests/physiology/test_spiking.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.5/tests/physiology/test_util.py` & `brainbox-0.0.6/tests/physiology/test_util.py`

 * *Files identical despite different names*

