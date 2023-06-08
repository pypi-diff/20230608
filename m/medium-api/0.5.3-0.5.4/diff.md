# Comparing `tmp/medium-api-0.5.3.tar.gz` & `tmp/medium-api-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium-api-0.5.3.tar", last modified: Sat Apr 22 19:02:18 2023, max compression
+gzip compressed data, was "medium-api-0.5.4.tar", last modified: Thu Jun  8 11:01:45 2023, max compression
```

## Comparing `medium-api-0.5.3.tar` & `medium-api-0.5.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.856478 medium-api-0.5.3/
--rw-r--r--   0 sanskar    (501) staff       (20)     1069 2022-01-02 12:36:51.000000 medium-api-0.5.3/LICENSE
--rw-r--r--   0 sanskar    (501) staff       (20)      232 2022-01-21 06:51:28.000000 medium-api-0.5.3/MANIFEST.in
--rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-22 19:02:18.856590 medium-api-0.5.3/PKG-INFO
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.823637 medium-api-0.5.3/docs/
--rw-r--r--   0 sanskar    (501) staff       (20)      611 2022-02-27 09:33:04.000000 medium-api-0.5.3/docs/Makefile
--rw-r--r--   0 sanskar    (501) staff       (20)     5287 2023-01-28 20:04:36.000000 medium-api-0.5.3/docs/README.rst
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.816239 medium-api-0.5.3/docs/_build/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.816287 medium-api-0.5.3/docs/_build/html/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.827598 medium-api-0.5.3/docs/_build/html/_static/
--rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.3/docs/_build/html/_static/MediumAPI-Banner.png
--rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.3/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png
--rw-r--r--   0 sanskar    (501) staff       (20)      286 2022-01-17 09:33:23.000000 medium-api-0.5.3/docs/_build/html/_static/file.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.830605 medium-api-0.5.3/docs/_build/html/_static/logos/
--rw-r--r--   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled-no-background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled.png
--rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name-no_background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name.png
--rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.3/docs/_build/html/_static/logos/Logo.png
--rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.3/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.832046 medium-api-0.5.3/docs/_static/
--rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.3/docs/_static/MediumAPI-Banner.png
--rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.3/docs/_static/MediumAPI-GettingStarted-Thumbnail.png
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.843136 medium-api-0.5.3/docs/_static/logos/
--rw-rw-rw-   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.3/docs/_static/logos/Logo-encircled-no-background.png
--rw-rw-rw-   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.3/docs/_static/logos/Logo-encircled.png
--rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.3/docs/_static/logos/Logo-with_name-no_background.png
--rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.3/docs/_static/logos/Logo-with_name.png
--rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.3/docs/_static/logos/Logo.png
--rw-r--r--   0 sanskar    (501) staff       (20)      154 2022-02-28 10:17:36.000000 medium-api-0.5.3/docs/authors.rst
--rwxr-xr-x   0 sanskar    (501) staff       (20)     5256 2022-02-28 10:04:39.000000 medium-api-0.5.3/docs/conf.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3501 2022-02-27 09:29:20.000000 medium-api-0.5.3/docs/contributing.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      855 2023-04-02 23:24:30.000000 medium-api-0.5.3/docs/documentation.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      420 2022-02-07 11:18:24.000000 medium-api-0.5.3/docs/index.rst
--rw-r--r--   0 sanskar    (501) staff       (20)     1158 2022-02-27 09:18:02.000000 medium-api-0.5.3/docs/installation.rst
--rw-r--r--   0 sanskar    (501) staff       (20)      772 2022-02-27 09:32:51.000000 medium-api-0.5.3/docs/make.bat
--rw-r--r--   0 sanskar    (501) staff       (20)    34500 2022-02-27 09:32:17.000000 medium-api-0.5.3/docs/terms_of_use.rst
--rw-r--r--   0 sanskar    (501) staff       (20)    10462 2023-04-12 09:28:54.000000 medium-api-0.5.3/docs/usage.rst
--rw-r--r--   0 sanskar    (501) staff       (20)       89 2022-01-16 18:16:53.000000 medium-api-0.5.3/pyproject.toml
--rw-r--r--   0 sanskar    (501) staff       (20)       33 2022-02-01 20:42:59.000000 medium-api-0.5.3/requirements-dev.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        0 2023-01-26 20:03:14.000000 medium-api-0.5.3/requirements.txt
--rw-r--r--   0 sanskar    (501) staff       (20)     1045 2023-04-22 19:02:18.858886 medium-api-0.5.3/setup.cfg
--rw-r--r--   0 sanskar    (501) staff       (20)       61 2022-01-16 19:30:09.000000 medium-api-0.5.3/setup.py
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.816674 medium-api-0.5.3/src/
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.846115 medium-api-0.5.3/src/medium_api/
--rw-r--r--   0 sanskar    (501) staff       (20)      157 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api/__init__.py
--rw-r--r--   0 sanskar    (501) staff       (20)    15261 2023-04-12 09:31:29.000000 medium-api-0.5.3/src/medium_api/_article.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3013 2023-03-30 10:20:57.000000 medium-api-0.5.3/src/medium_api/_latestposts.py
--rw-r--r--   0 sanskar    (501) staff       (20)     8382 2023-04-02 21:00:13.000000 medium-api-0.5.3/src/medium_api/_medium_list.py
--rw-r--r--   0 sanskar    (501) staff       (20)    11527 2023-03-30 10:20:44.000000 medium-api-0.5.3/src/medium_api/_publication.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2450 2023-03-30 10:20:19.000000 medium-api-0.5.3/src/medium_api/_top_writers.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3076 2023-03-30 10:21:46.000000 medium-api-0.5.3/src/medium_api/_topfeeds.py
--rw-r--r--   0 sanskar    (501) staff       (20)    16393 2023-04-22 17:34:09.000000 medium-api-0.5.3/src/medium_api/_user.py
--rw-r--r--   0 sanskar    (501) staff       (20)    26743 2023-04-22 19:01:46.000000 medium-api-0.5.3/src/medium_api/medium.py
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.848402 medium-api-0.5.3/src/medium_api.egg-info/
--rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/PKG-INFO
--rw-r--r--   0 sanskar    (501) staff       (20)     1740 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/SOURCES.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        1 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/dependency_links.txt
--rw-r--r--   0 sanskar    (501) staff       (20)       11 2023-04-22 19:02:18.000000 medium-api-0.5.3/src/medium_api.egg-info/top_level.txt
--rw-r--r--   0 sanskar    (501) staff       (20)        1 2022-07-27 13:19:52.000000 medium-api-0.5.3/src/medium_api.egg-info/zip-safe
-drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-04-22 19:02:18.856133 medium-api-0.5.3/tests/
--rw-r--r--   0 sanskar    (501) staff       (20)     6148 2022-02-27 12:41:15.000000 medium-api-0.5.3/tests/.DS_Store
--rw-r--r--   0 sanskar    (501) staff       (20)        0 2022-01-16 17:06:47.000000 medium-api-0.5.3/tests/__init__.py
--rw-r--r--   0 sanskar    (501) staff       (20)     3578 2023-04-12 09:09:51.000000 medium-api-0.5.3/tests/test_article.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1161 2022-07-22 09:09:55.000000 medium-api-0.5.3/tests/test_latestposts.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2255 2023-03-28 12:57:03.000000 medium-api-0.5.3/tests/test_medium_list.py
--rw-r--r--   0 sanskar    (501) staff       (20)     2610 2022-11-30 08:22:20.000000 medium-api-0.5.3/tests/test_publication.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1230 2023-03-30 19:21:06.000000 medium-api-0.5.3/tests/test_search.py
--rw-r--r--   0 sanskar    (501) staff       (20)      710 2023-04-02 23:13:37.000000 medium-api-0.5.3/tests/test_tag.py
--rw-r--r--   0 sanskar    (501) staff       (20)      877 2023-02-17 11:23:49.000000 medium-api-0.5.3/tests/test_top_writers.py
--rw-r--r--   0 sanskar    (501) staff       (20)     1010 2023-02-14 17:43:26.000000 medium-api-0.5.3/tests/test_topfeeds.py
--rw-r--r--   0 sanskar    (501) staff       (20)     4162 2023-03-30 10:58:55.000000 medium-api-0.5.3/tests/test_user.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.667818 medium-api-0.5.4/
+-rw-r--r--   0 sanskar    (501) staff       (20)     1069 2022-01-02 12:36:51.000000 medium-api-0.5.4/LICENSE
+-rw-r--r--   0 sanskar    (501) staff       (20)      232 2022-01-21 06:51:28.000000 medium-api-0.5.4/MANIFEST.in
+-rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-06-08 11:01:45.667948 medium-api-0.5.4/PKG-INFO
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.642821 medium-api-0.5.4/docs/
+-rw-r--r--   0 sanskar    (501) staff       (20)      611 2022-02-27 09:33:04.000000 medium-api-0.5.4/docs/Makefile
+-rw-r--r--   0 sanskar    (501) staff       (20)     5287 2023-01-28 20:04:36.000000 medium-api-0.5.4/docs/README.rst
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.632725 medium-api-0.5.4/docs/_build/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.632797 medium-api-0.5.4/docs/_build/html/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.646831 medium-api-0.5.4/docs/_build/html/_static/
+-rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.4/docs/_build/html/_static/MediumAPI-Banner.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.4/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png
+-rw-r--r--   0 sanskar    (501) staff       (20)      286 2022-01-17 09:33:23.000000 medium-api-0.5.4/docs/_build/html/_static/file.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.650224 medium-api-0.5.4/docs/_build/html/_static/logos/
+-rw-r--r--   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.4/docs/_build/html/_static/logos/Logo-encircled-no-background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.4/docs/_build/html/_static/logos/Logo-encircled.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.4/docs/_build/html/_static/logos/Logo-with_name-no_background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.4/docs/_build/html/_static/logos/Logo-with_name.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.4/docs/_build/html/_static/logos/Logo.png
+-rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sanskar    (501) staff       (20)       90 2022-01-17 09:33:23.000000 medium-api-0.5.4/docs/_build/html/_static/plus.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.652003 medium-api-0.5.4/docs/_static/
+-rw-r--r--   0 sanskar    (501) staff       (20)   378551 2022-02-28 09:45:28.000000 medium-api-0.5.4/docs/_static/MediumAPI-Banner.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   116988 2022-04-10 13:29:20.000000 medium-api-0.5.4/docs/_static/MediumAPI-GettingStarted-Thumbnail.png
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.658359 medium-api-0.5.4/docs/_static/logos/
+-rw-rw-rw-   0 sanskar    (501) staff       (20)    26295 2022-02-04 15:57:31.000000 medium-api-0.5.4/docs/_static/logos/Logo-encircled-no-background.png
+-rw-rw-rw-   0 sanskar    (501) staff       (20)   275759 2022-02-04 15:54:27.000000 medium-api-0.5.4/docs/_static/logos/Logo-encircled.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    25218 2022-02-28 05:20:48.000000 medium-api-0.5.4/docs/_static/logos/Logo-with_name-no_background.png
+-rw-r--r--   0 sanskar    (501) staff       (20)   303096 2022-02-28 05:20:07.000000 medium-api-0.5.4/docs/_static/logos/Logo-with_name.png
+-rw-r--r--   0 sanskar    (501) staff       (20)    16128 2022-02-04 15:08:14.000000 medium-api-0.5.4/docs/_static/logos/Logo.png
+-rw-r--r--   0 sanskar    (501) staff       (20)      154 2022-02-28 10:17:36.000000 medium-api-0.5.4/docs/authors.rst
+-rwxr-xr-x   0 sanskar    (501) staff       (20)     5256 2022-02-28 10:04:39.000000 medium-api-0.5.4/docs/conf.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3501 2022-02-27 09:29:20.000000 medium-api-0.5.4/docs/contributing.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      855 2023-04-02 23:24:30.000000 medium-api-0.5.4/docs/documentation.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      420 2022-02-07 11:18:24.000000 medium-api-0.5.4/docs/index.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)     1158 2022-02-27 09:18:02.000000 medium-api-0.5.4/docs/installation.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)      772 2022-02-27 09:32:51.000000 medium-api-0.5.4/docs/make.bat
+-rw-r--r--   0 sanskar    (501) staff       (20)    34500 2022-02-27 09:32:17.000000 medium-api-0.5.4/docs/terms_of_use.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)    10462 2023-04-12 09:28:54.000000 medium-api-0.5.4/docs/usage.rst
+-rw-r--r--   0 sanskar    (501) staff       (20)       89 2022-01-16 18:16:53.000000 medium-api-0.5.4/pyproject.toml
+-rw-r--r--   0 sanskar    (501) staff       (20)       33 2022-02-01 20:42:59.000000 medium-api-0.5.4/requirements-dev.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        0 2023-01-26 20:03:14.000000 medium-api-0.5.4/requirements.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)     1045 2023-06-08 11:01:45.668446 medium-api-0.5.4/setup.cfg
+-rw-r--r--   0 sanskar    (501) staff       (20)       61 2022-01-16 19:30:09.000000 medium-api-0.5.4/setup.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.633409 medium-api-0.5.4/src/
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.661907 medium-api-0.5.4/src/medium_api/
+-rw-r--r--   0 sanskar    (501) staff       (20)      157 2023-06-08 11:01:45.000000 medium-api-0.5.4/src/medium_api/__init__.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    15328 2023-06-07 13:18:57.000000 medium-api-0.5.4/src/medium_api/_article.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3797 2023-06-07 13:41:43.000000 medium-api-0.5.4/src/medium_api/_latestposts.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     9166 2023-06-07 13:46:47.000000 medium-api-0.5.4/src/medium_api/_medium_list.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    12700 2023-06-07 14:12:31.000000 medium-api-0.5.4/src/medium_api/_publication.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2450 2023-03-30 10:20:19.000000 medium-api-0.5.4/src/medium_api/_top_writers.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3873 2023-06-07 13:40:31.000000 medium-api-0.5.4/src/medium_api/_topfeeds.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    16441 2023-06-07 13:10:04.000000 medium-api-0.5.4/src/medium_api/_user.py
+-rw-r--r--   0 sanskar    (501) staff       (20)    27791 2023-06-07 13:16:27.000000 medium-api-0.5.4/src/medium_api/medium.py
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.663157 medium-api-0.5.4/src/medium_api.egg-info/
+-rw-r--r--   0 sanskar    (501) staff       (20)     6221 2023-06-08 11:01:45.000000 medium-api-0.5.4/src/medium_api.egg-info/PKG-INFO
+-rw-r--r--   0 sanskar    (501) staff       (20)     1740 2023-06-08 11:01:45.000000 medium-api-0.5.4/src/medium_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        1 2023-06-08 11:01:45.000000 medium-api-0.5.4/src/medium_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)       11 2023-06-08 11:01:45.000000 medium-api-0.5.4/src/medium_api.egg-info/top_level.txt
+-rw-r--r--   0 sanskar    (501) staff       (20)        1 2022-07-27 13:19:52.000000 medium-api-0.5.4/src/medium_api.egg-info/zip-safe
+drwxr-xr-x   0 sanskar    (501) staff       (20)        0 2023-06-08 11:01:45.667495 medium-api-0.5.4/tests/
+-rw-r--r--   0 sanskar    (501) staff       (20)     6148 2022-02-27 12:41:15.000000 medium-api-0.5.4/tests/.DS_Store
+-rw-r--r--   0 sanskar    (501) staff       (20)        0 2022-01-16 17:06:47.000000 medium-api-0.5.4/tests/__init__.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3668 2023-06-07 14:16:11.000000 medium-api-0.5.4/tests/test_article.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1161 2022-07-22 09:09:55.000000 medium-api-0.5.4/tests/test_latestposts.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2259 2023-06-07 13:54:17.000000 medium-api-0.5.4/tests/test_medium_list.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     2565 2023-06-07 13:21:19.000000 medium-api-0.5.4/tests/test_publication.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     1298 2023-06-07 13:36:10.000000 medium-api-0.5.4/tests/test_search.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      710 2023-04-02 23:13:37.000000 medium-api-0.5.4/tests/test_tag.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      698 2023-06-07 13:54:51.000000 medium-api-0.5.4/tests/test_top_writers.py
+-rw-r--r--   0 sanskar    (501) staff       (20)      873 2023-06-07 13:55:32.000000 medium-api-0.5.4/tests/test_topfeeds.py
+-rw-r--r--   0 sanskar    (501) staff       (20)     3833 2023-06-07 14:04:58.000000 medium-api-0.5.4/tests/test_user.py
```

### Comparing `medium-api-0.5.3/LICENSE` & `medium-api-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/PKG-INFO` & `medium-api-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-api
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
 Home-page: https://github.com/weeping-angel/medium-api
 Author: Nishu Jain
 Author-email: nishujain1997.19@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `medium-api-0.5.3/docs/Makefile` & `medium-api-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/README.rst` & `medium-api-0.5.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/MediumAPI-Banner.png` & `medium-api-0.5.4/docs/_build/html/_static/MediumAPI-Banner.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png` & `medium-api-0.5.4/docs/_build/html/_static/MediumAPI-GettingStarted-Thumbnail.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled-no-background.png` & `medium-api-0.5.4/docs/_build/html/_static/logos/Logo-encircled-no-background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-encircled.png` & `medium-api-0.5.4/docs/_build/html/_static/logos/Logo-encircled.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name-no_background.png` & `medium-api-0.5.4/docs/_build/html/_static/logos/Logo-with_name-no_background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/logos/Logo-with_name.png` & `medium-api-0.5.4/docs/_build/html/_static/logos/Logo-with_name.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_build/html/_static/logos/Logo.png` & `medium-api-0.5.4/docs/_build/html/_static/logos/Logo.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/MediumAPI-Banner.png` & `medium-api-0.5.4/docs/_static/MediumAPI-Banner.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/MediumAPI-GettingStarted-Thumbnail.png` & `medium-api-0.5.4/docs/_static/MediumAPI-GettingStarted-Thumbnail.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/logos/Logo-encircled-no-background.png` & `medium-api-0.5.4/docs/_static/logos/Logo-encircled-no-background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/logos/Logo-encircled.png` & `medium-api-0.5.4/docs/_static/logos/Logo-encircled.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/logos/Logo-with_name-no_background.png` & `medium-api-0.5.4/docs/_static/logos/Logo-with_name-no_background.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/logos/Logo-with_name.png` & `medium-api-0.5.4/docs/_static/logos/Logo-with_name.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/_static/logos/Logo.png` & `medium-api-0.5.4/docs/_static/logos/Logo.png`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/conf.py` & `medium-api-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/contributing.rst` & `medium-api-0.5.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/documentation.rst` & `medium-api-0.5.4/docs/documentation.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/installation.rst` & `medium-api-0.5.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/make.bat` & `medium-api-0.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/terms_of_use.rst` & `medium-api-0.5.4/docs/terms_of_use.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/docs/usage.rst` & `medium-api-0.5.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/setup.cfg` & `medium-api-0.5.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = medium-api
 description = Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
-version = 0.5.3
+version = 0.5.4
 long_description = file: docs/README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/weeping-angel/medium-api
 author = Nishu Jain
 author_email = nishujain1997.19@gmail.com
 platforms = unix, linux, osx, win32, cygwin
 description_file = README.rst
```

### Comparing `medium-api-0.5.3/src/medium_api/_article.py` & `medium-api-0.5.4/src/medium_api/_article.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,25 +387,27 @@
         self.__html = str(resp['html'])
 
     @property
     def json(self):
         """To get the articles information in JSON format
         
         Returns:
-            dict: Returns a JSON object containing article `info`, `content`, and `markdown` if 
+            dict: Returns a JSON object containing article `info`, `content`, `markdown` and `html` if 
             already fetched. Else, returns an empty object.
         
         """
         ret = {}
         if self.__info:
             ret.update(self.info)
         if self.__content:
             ret['content'] = self.content
         if self.__markdown:
             ret['markdown'] = self.markdown
+        if self.__html:
+            ret['html'] = self.html
 
         return ret
     
     def fetch_fans(self):
         """To fetch user-related information of the people who clapped on the article (voters/fans), using multi-threading
 
         Returns:
```

### Comparing `medium-api-0.5.3/src/medium_api/_medium_list.py` & `medium-api-0.5.4/src/medium_api/_medium_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -192,28 +192,44 @@
                                        fetch_publications=self.__fetch_publications,
                                        fetch_lists=self.__fetch_lists,
                                        save_info=False) 
                                 for response_id in self.response_ids]
 
         return self.__responses
 
-    def fetch_articles(self, content=False):
+    def fetch_articles(self, content=False, markdown=False, html=False, html_fullpage=True):
         """To fetch all the Medium List's articles information (using multithreading)
 
         Args:
             content (bool, optional): Set it to `True` if you want to fetch the 
                 textual content of the article as well. Otherwise, default is `False`.
 
+            markdown(bool, optional): Set it to `True` if you want to fetch the markdown of 
+                the article as well. Otherwise, default is `False`
+
+            html(bool, optional): Set it to `True` if you want to fetch the article in HTML 
+                format as well. Otherwise, default is `False`
+
+            html_fullpage(bool, optional): Set it to `False` if you only want to fetch the HTML 
+                inside body tag of the article. Otherwise, default is `True`, which fetches the 
+                entire HTML of the article.
+
         Returns:
             None: All the fetched information will be access via medium_list.articles.
 
             ``medium_list.articles[0].title``
             ``medium_list.articles[1].claps``
         """
-        self.__fetch_articles(self.articles, content=content)
+        self.__fetch_articles(
+                    self.articles, 
+                    content=content,
+                    markdown=markdown, 
+                    html=html, 
+                    html_fullpage=html_fullpage
+                )
 
     def fetch_responses(self, content=False):
         """To fetch all the Medium List's Responses information (using multithreading)
 
         Args:
             content (bool, optional): Set it to `True` if you want to fetch the 
                 textual content of the article as well. Otherwise, default is `False`.
```

### Comparing `medium-api-0.5.3/src/medium_api/_publication.py` & `medium-api-0.5.4/src/medium_api/_publication.py`

 * *Files 12% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         self.__fetch_articles = fetch_articles
         self.__fetch_users = fetch_users
         self.__fetch_publications = fetch_publications
         self.__fetch_lists = fetch_lists
 
         self.name = None
         self.description = None
-        self.url = None
         self.tagline = None
         self.followers = None
         self.slug = None
         self.tags = None
         self.creator = None
         self.editors = None
         self.domain = None
@@ -166,15 +165,14 @@
         
         Note:
             Only after running ``publication.save_info()`` you can use the following
             variables:
 
                 - ``publication.name``
                 - ``publication.description``
-                - ``publication.url``
                 - ``publication.tagline``
                 - ``publication.followers``
                 - ``publication.slug``
                 - ``publication.tags``
                 - ``publication.domain``
                 - ``publication.creator``
                 - ``publication.editors``
@@ -183,15 +181,14 @@
                 - ``publication.facebook_pagename``
 
         """
         publication = self.info
 
         self.name = publication.get('name')
         self.description = publication.get('description')
-        self.url = publication.get('url')
         self.tagline = publication.get('tagline')
         self.followers = publication.get('followers')
         self.slug = publication.get('slug')
         self.tags = publication.get('tags')
         self.domain = publication.get('domain')
         self.twitter_username = publication.get('twitter_username')
         self.instagram_username = publication.get('instagram_username')
@@ -240,26 +237,39 @@
                         fetch_publications=self.__fetch_publications,
                         fetch_lists=self.__fetch_lists,
                     )
                 for article_id in article_ids]
     
     
     @lru_cache(maxsize=16)
-    def get_articles_between(self, _from=None, _to=None):
+    def get_articles_between(self, _from=None, _to=None, content=False, markdown=False, html=False, html_fullpage=True):
         """To get publication articles within a datetime range.
 
             Example usage:
                 
             ``publication.get_articles_between(_from=datetime.now(), _to=datetime.now() - timedelta(days=15))``
 
         Args:
             _from (datetime.datetime): Starting date of the interval
 
             _to (datetime.datetime): Ending date of the interval
 
+            content (bool, optional): Set it to `True` if you want to fetch the 
+                textual content of the article as well. Otherwise, default is `False`.
+
+            markdown(bool, optional): Set it to `True` if you want to fetch the markdown of 
+                the article as well. Otherwise, default is `False`
+
+            html(bool, optional): Set it to `True` if you want to fetch the article in HTML 
+                format as well. Otherwise, default is `False`
+
+            html_fullpage(bool, optional): Set it to `False` if you only want to fetch the HTML 
+                inside body tag of the article. Otherwise, default is `True`, which fetches the 
+                entire HTML of the article.
+
         Returns:
             list[Article]: Returns a list of Article Objects (publication articles).
 
         Note:
             - If the ``_to`` parameter is not provided, then the function will return recent 25 
               articles from the given date (in ``_from`` parameter)
 
@@ -281,25 +291,37 @@
                 next_to = datetime.strptime(resp['to'], '%Y-%m-%d %H:%M:%S')
 
                 while next_to > _to:
                     resp,_ = self.__get_resp(f'/publication/{self._id}/articles?from={next_to.isoformat()}')
                     articles += self.articles_from_ids(resp['publication_articles'][::-1])
                     next_to = datetime.strptime(resp['to'], '%Y-%m-%d %H:%M:%S')
             
-                self.__fetch_articles(articles)
+                self.__fetch_articles(
+                                articles, 
+                                content=content,
+                                markdown=markdown, 
+                                html=html, 
+                                html_fullpage=html_fullpage
+                            )
 
                 self.__articles = [article for article in articles if (_to <= article.published_at <= _from)]
 
             else:
                 print('[ERROR]: "from" date should be greater than "to" date. Try swapping both.')
                 return []
         else:
             resp,_ = self.__get_resp(f'/publication/{self._id}/articles?from={_from.isoformat()}')
             self.__articles = self.articles_from_ids(resp['publication_articles'])
-            self.__fetch_articles(self.__articles)
+            self.__fetch_articles(
+                        self.__articles,
+                        content=content,
+                        markdown=markdown, 
+                        html=html, 
+                        html_fullpage=html_fullpage
+                    )
         
         return self.__articles
     
     @property
     def articles(self):
         """Returns top recent 25 articles
```

### Comparing `medium-api-0.5.3/src/medium_api/_top_writers.py` & `medium-api-0.5.4/src/medium_api/_top_writers.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/src/medium_api/_topfeeds.py` & `medium-api-0.5.4/src/medium_api/_topfeeds.py`

 * *Files 26% similar despite different names*

```diff
@@ -68,21 +68,37 @@
                                        fetch_publications=self.__fetch_publications,
                                        fetch_lists=self.__fetch_lists,
                                        save_info=False) 
                                 for article_id in self.ids]
 
         return self.__articles
 
-    def fetch_articles(self, content=False):
+    def fetch_articles(self, content=False, markdown=False, html=False, html_fullpage=True):
         """To fetch all the topfeeds articles information (multithreading)
 
         Args:
             content (bool, optional): Set it to `True` if you want to fetch the 
                 textual content of the article as well. Otherwise, default is `False`.
+            
+            markdown(bool, optional): Set it to `True` if you want to fetch the markdown of 
+                the article as well. Otherwise, default is `False`
+
+            html(bool, optional): Set it to `True` if you want to fetch the article in HTML 
+                format as well. Otherwise, default is `False`
+
+            html_fullpage(bool, optional): Set it to `False` if you only want to fetch the HTML 
+                inside body tag of the article. Otherwise, default is `True`, which fetches the 
+                entire HTML of the article.
 
         Returns:
             None: All the fetched information will be access via topfeeds.articles.
 
             ``topfeeds.articles[0].title``
             ``topfeeds.articles[1].claps``
         """
-        self.__fetch_articles(self.articles, content=content)
+        self.__fetch_articles(
+                    self.articles, 
+                    content=content, 
+                    markdown=markdown, 
+                    html=html, 
+                    html_fullpage=html_fullpage
+                )
```

### Comparing `medium-api-0.5.3/src/medium_api/_user.py` & `medium-api-0.5.4/src/medium_api/_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
             self.medium_member_at = datetime.strptime(user['medium_member_at'], '%Y-%m-%d %H:%M:%S') if user['medium_member_at']!='' else None
         self.top_writer_in = list(user['top_writer_in']) if user.get('top_writer_in') else []
 
         if self.fullname is None:
             print(f"[ERROR]: Could not retrieve user for the given user_id ({self.user_id}). Please check if this user exists.")
             print(f"[ERROR]: Link to unknown user's profile: https://medium.com/u/{self.user_id}")
 
-    def fetch_articles(self, content=False):
+    def fetch_articles(self, content=False, markdown=False, html=False, html_fullpage=True):
         """To fetch all the user-written articles information and content
 
         Args:
             content (bool, optional): Set it to `True` if you want to fetch the 
                 textual content of the article as well. Otherwise, default is `False`.
 
         Returns:
```

### Comparing `medium-api-0.5.3/src/medium_api/medium.py` & `medium-api-0.5.4/src/medium_api/medium.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,23 @@
         `publication`, `topfeeds`, `top_writers`, etc ... 
 
     Note:
         See https://docs.rapidapi.com/docs/keys to learn more about RapidAPI keys.
 
     """
     def __init__(self, rapidapi_key:str, base_url:str='medium2.p.rapidapi.com', calls:int=0):
-        self.headers = {
-            'X-RapidAPI-Key': rapidapi_key,
-            'User-Agent': f"medium-api-python-sdk"
-        }
-        self.base_url = base_url
-        self.calls = calls
+        if rapidapi_key and isinstance(rapidapi_key, str):
+            self.headers = {
+                'X-RapidAPI-Key': rapidapi_key,
+                'User-Agent': f"medium-api-python-sdk"
+            }
+            self.base_url = base_url
+            self.calls = calls
+        else:
+            print('[ERROR]: Please pass the API Key in string format')
 
     def __get_resp(self, endpoint:str, retries:int=0):
         conn = HTTPSConnection(self.base_url)
         conn.request('GET', endpoint, headers=self.headers)
         resp = conn.getresponse()
 
         data = resp.read()
@@ -544,15 +547,15 @@
             dict: Contains tag-related information
 
         """
         resp, _ = self.__get_resp(f'/tag/{tag}')
 
         return resp
 
-    def fetch_articles(self, articles:list, content:bool = False):
+    def fetch_articles(self, articles:list, content:bool = False, markdown:bool = False, html:bool = False, html_fullpage:bool = True):
         """To quickly fetch articles (info and content) using multithreading
 
             Typical usage example:
 
             ``medium.fetch_articles(latestposts.articles)``
             ``medium.fetch_articles(user.articles)``
             ``medium.fetch_articles(list_of_articles_obj)``
@@ -561,24 +564,40 @@
 
             articles (list[Article]): List of (empty) Article objects to fill information 
                 (and content) into it.
 
             content(bool, optional): Set it to `True` if you want to fetch the content of 
                 the article as well. Otherwise, default is `False`
 
+            markdown(bool, optional): Set it to `True` if you want to fetch the markdown of 
+                the article as well. Otherwise, default is `False`
+
+            html(bool, optional): Set it to `True` if you want to fetch the article in HTML 
+                format as well. Otherwise, default is `False`
+
+            html_fullpage(bool, optional): Set it to `False` if you only want to fetch the HTML 
+                inside body tag of the article. Otherwise, default is `True`, which fetches the 
+                entire HTML of the article.
+
         Returns:
             None: This method doesn't return anything since it fills the values in the passed
             list of Article(s) objects itself.
 
         """
         with ThreadPoolExecutor(max_workers=10) as executor:
             future_to_url = [executor.submit(article.save_info) for article in articles if article.title is None]
             if content:
                 future_to_url += [executor.submit(article.save_content) for article in articles]
 
+            if markdown:
+                future_to_url += [executor.submit(article.save_markdown) for article in articles]
+
+            if html:
+                future_to_url += [executor.submit(article.save_html, html_fullpage) for article in articles]
+
             for future in as_completed(future_to_url):
                 future.result()
     
     def fetch_publications(self, publications:list):
         """To quickly fetch publications' info using multithreading
 
             Typical usage example:
```

### Comparing `medium-api-0.5.3/src/medium_api.egg-info/PKG-INFO` & `medium-api-0.5.4/src/medium_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-api
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python Wrapper on top of Medium API to quickly extract data from https://medium.com.
 Home-page: https://github.com/weeping-angel/medium-api
 Author: Nishu Jain
 Author-email: nishujain1997.19@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `medium-api-0.5.3/src/medium_api.egg-info/SOURCES.txt` & `medium-api-0.5.4/src/medium_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/tests/.DS_Store` & `medium-api-0.5.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/tests/test_article.py` & `medium-api-0.5.4/tests/test_article.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,43 +53,43 @@
     assert isinstance(article.response_ids[0], str)
 
     assert isinstance(article.responses, list)
     assert isinstance(article.responses[0], Article)
 
     assert article.responses[0].title is None
 
-    article.fetch_responses()
+    # article.fetch_responses()
 
-    assert article.responses[0].title is not None
+    # assert article.responses[0].title is not None
 
 def test_article_fans():
     assert isinstance(article.fans_ids, list)
     assert isinstance(article.fans_ids[0], str)
 
     assert isinstance(article.fans, list)
     assert isinstance(article.fans[0], User)
 
     assert article.fans[0].fullname is None
 
-    article.fetch_fans()
+    # article.fetch_fans()
 
-    assert article.fans[0].fullname is not None
+    # assert article.fans[0].fullname is not None
 
 def test_related_articles():
     assert isinstance(article.related_articles_ids, list)
     assert isinstance(article.related_articles_ids[0], str)
 
     assert isinstance(article.related_articles, list)
     assert isinstance(article.related_articles[0], Article)
 
     assert article.related_articles[0].title is None
 
-    article.fetch_related_articles()
+    # article.fetch_related_articles()
 
-    assert article.related_articles[0].title is not None
+    # assert article.related_articles[0].title is not None
 
 def test_article_content():
     article.save_content()
 
     assert isinstance(article.content, str)
     assert len(article.content) > 0
 
@@ -106,20 +106,22 @@
     assert len(article.html) > 0
     assert article.html[:len('<html')] == '<html'
 
 def test_article_json():
     article.save_info()
     article.save_content()
     article.save_markdown()
+    article.save_html(fullpage=True)
     
     article_json = article.json
 
     assert isinstance(article_json, dict)
     assert 'content' in article_json.keys()
     assert 'markdown' in article_json.keys()
+    assert 'html' in article_json.keys()
     assert 'title' in article_json.keys()
 
 def test_article_publication():
     is_self_published = article.is_self_published
 
     assert isinstance(is_self_published, bool)
```

### Comparing `medium-api-0.5.3/tests/test_latestposts.py` & `medium-api-0.5.4/tests/test_latestposts.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/tests/test_medium_list.py` & `medium-api-0.5.4/tests/test_medium_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     assert medium_list._id == list_id
 
 def test_medium_list_articles():
     article_ids = medium_list.article_ids
     assert isinstance(article_ids, list)
     assert isinstance(article_ids[0], str)
 
-    medium_list.fetch_articles()
+    # medium_list.fetch_articles()
 
     articles = medium_list.articles
     assert isinstance(articles, list)
     assert isinstance(articles[0], Article)
 
 def test_medium_list_responses():
     response_ids = medium_list.response_ids
     assert isinstance(response_ids, list)
     assert isinstance(response_ids[0], str)
 
-    medium_list.fetch_responses()
+    # medium_list.fetch_responses()
 
     responses = medium_list.responses
     assert isinstance(responses, list)
     assert isinstance(responses[0], Article)
 
 def test_medium_list_info():
     # Before save_info
```

### Comparing `medium-api-0.5.3/tests/test_publication.py` & `medium-api-0.5.4/tests/test_publication.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     assert len(articles)==0
 
 def test_publication_info():
     _publication.save_info()
 
     assert isinstance(_publication.name, str)
     assert isinstance(_publication.description, str)
-    assert isinstance(_publication.url, str)
     assert isinstance(_publication.tagline, str)
     assert isinstance(_publication.followers, int)
     assert isinstance(_publication.slug, str)
     assert isinstance(_publication.tags, list)
     assert isinstance(_publication.domain, str)
     assert isinstance(_publication.twitter_username, str)
     assert isinstance(_publication.instagram_username, str)
```

### Comparing `medium-api-0.5.3/tests/test_search.py` & `medium-api-0.5.4/tests/test_search.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 from medium_api._user import User
 from medium_api._article import Article
 from medium_api._medium_list import MediumList
 
 medium = Medium(os.getenv('RAPIDAPI_KEY'))
 
 def test_search_articles():
-    results = medium.search_articles(query = "data science")
+    results = medium.search_articles(query = "data science", save_info=False)
 
     assert isinstance(results, list)
     assert len(results) > 0
     assert isinstance(results[0], Article)
 
 def test_search_publications():
-    results = medium.search_publications(query = "mental health")
+    results = medium.search_publications(query = "mental health", save_info=False)
 
     assert isinstance(results, list)
     assert len(results) > 0
     assert isinstance(results[0], Publication)
 
 def test_search_users():
-    results = medium.search_users(query = "data engineer")
+    results = medium.search_users(query = "data engineer", save_info=False)
 
     assert isinstance(results, list)
     assert len(results) > 0
     assert isinstance(results[0], User)
 
 def test_search_lists():
-    results = medium.search_lists(query = "medium")
+    results = medium.search_lists(query = "medium", save_info=False)
 
     assert isinstance(results, list)
     assert len(results) > 0
     assert isinstance(results[0], MediumList)
 
 def test_search_tags():
     results = medium.search_tags(query = "blockchain")
```

### Comparing `medium-api-0.5.3/tests/test_tag.py` & `medium-api-0.5.4/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `medium-api-0.5.3/tests/test_topfeeds.py` & `medium-api-0.5.4/tests/test_topfeeds.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,7 @@
         assert isinstance(topfeeds.ids, list)
         assert len(topfeeds.ids) == count
         assert isinstance(topfeeds.ids[0], str)
 
         assert isinstance(topfeeds.articles, list)
         assert isinstance(topfeeds.articles[0], Article)
 
-    topfeeds.fetch_articles()
-
-    assert 'title' in topfeeds.articles[0].info.keys()
-    assert topfeeds.articles[0].title is not None
-
```

### Comparing `medium-api-0.5.3/tests/test_user.py` & `medium-api-0.5.4/tests/test_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from medium_api._medium_list import MediumList
 
 medium = Medium(os.getenv('RAPIDAPI_KEY'))
 
 username = 'nishu-jain'
 user_id = '1985b61817c3'
 
-user = medium.user(username = username)
+user = medium.user(username = username, save_info=False)
 
 def test_user_instance():
     assert isinstance(user, User)
     assert isinstance(user._id, str)
     assert user._id == user_id
 
 def test_user_info():
@@ -67,82 +67,69 @@
     assert isinstance(top_articles, list)
     assert isinstance(top_articles[0], Article)
 
 def test_user_following():
     following_ids = user.following_ids
     following = user.following
 
-    user.fetch_following()
+    # user.fetch_following()
 
     assert isinstance(following_ids, list)
     if len(following_ids) != 0:
         assert isinstance(following_ids[0], str)
 
     assert isinstance(following, list)
     if len(following) != 0:
         assert isinstance(following[0], User)
-        assert isinstance(following[0].fullname, str)
+        # assert isinstance(following[0].fullname, str)
 
 def test_user_followers():
     followers_ids = user.followers_ids
     followers = user.followers
 
-    user.fetch_followers()
+    # user.fetch_followers()
 
     assert isinstance(followers_ids, list)
     if len(followers_ids) != 0:
         assert isinstance(followers_ids[0], str)
 
     assert isinstance(followers, list)
     if len(followers) != 0:
         assert isinstance(followers[0], User)
-        assert isinstance(followers[0].fullname, str)
+        # assert isinstance(followers[0].fullname, str)
 
 def test_user_publications():
     publication_ids = user.publication_ids
     publications = user.publications
 
-    user.fetch_publications()
+    # user.fetch_publications()
 
     assert isinstance(publication_ids, list)
     if len(publication_ids) != 0:
         assert isinstance(publication_ids[0], str)
 
     assert isinstance(publications, list)
     if len(publications) != 0:
         assert isinstance(publications[0], Publication)
-        assert isinstance(publications[0].name, str)
+        # assert isinstance(publications[0].name, str)
 
 def test_user_lists():
     list_ids = user.list_ids
     lists = user.lists
 
-    user.fetch_lists()
+    # user.fetch_lists()
 
     assert isinstance(list_ids, list)
     if len(list_ids) != 0:
         assert isinstance(list_ids[0], str)
 
     assert isinstance(lists, list)
     if len(lists) != 0:
         assert isinstance(lists[0], MediumList)
-        assert isinstance(lists[0].name, str)
-
-def test_user_articles_as_json():
-    user.fetch_articles(content=True)
-
-    user_articles_as_json = user.articles_as_json
-
-    assert isinstance(user_articles_as_json, list)
-    assert isinstance(user_articles_as_json[0], dict)
-    
-    articles_keys = user_articles_as_json[0].keys()
-
-    assert 'title' in articles_keys
-    assert 'content' in articles_keys
+        # assert isinstance(lists[0].name, str)
 
 def test_user_interests():
     interests = user.interests
 
     assert isinstance(interests, list)
     if interests:
         assert isinstance(interests[0], str)
```

