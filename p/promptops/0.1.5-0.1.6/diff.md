# Comparing `tmp/promptops-0.1.5.tar.gz` & `tmp/promptops-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptops-0.1.5.tar", last modified: Thu May 25 18:39:37 2023, max compression
+gzip compressed data, was "promptops-0.1.6.tar", last modified: Wed Jun  7 22:03:36 2023, max compression
```

## Comparing `promptops-0.1.5.tar` & `promptops-0.1.6.tar`

### file list

```diff
@@ -1,92 +1,103 @@
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.324385 promptops-0.1.5/
--rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.5/LICENSE.txt
--rw-r--r--   0 vasily     (501) staff       (20)     1929 2023-05-25 18:39:37.324543 promptops-0.1.5/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1292 2023-05-24 14:55:10.000000 promptops-0.1.5/README.md
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.300650 promptops-0.1.5/local_runner/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/__init__.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.302274 promptops-0.1.5/local_runner/comms/
--rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/http_reporter.py
--rw-r--r--   0 vasily     (501) staff       (20)     1368 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/ws.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.302813 promptops-0.1.5/local_runner/config/
--rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/config/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/config/config.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.303370 promptops-0.1.5/local_runner/creds/
--rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/creds/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/creds/creds.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.303842 promptops-0.1.5/local_runner/exec/
--rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/exec/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/exec/manager.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.304710 promptops-0.1.5/local_runner/handler/
--rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/handler/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/handler/censor.py
--rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/handler/handler.py
--rw-r--r--   0 vasily     (501) staff       (20)     1233 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.305474 promptops-0.1.5/local_runner/registration/
--rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/registration/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/registration/registration.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.306163 promptops-0.1.5/local_runner/tokens/
--rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/tokens/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/tokens/issuer.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.311293 promptops-0.1.5/promptops/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/corrections.py
--rw-r--r--   0 vasily     (501) staff       (20)      394 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/feedback.py
--rw-r--r--   0 vasily     (501) staff       (20)     3836 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/history.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.316155 promptops-0.1.5/promptops/loading/
--rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/base.py
--rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/context.py
--rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/pong.py
--rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/progress.py
--rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/promptops.py
--rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/simple.py
--rw-r--r--   0 vasily     (501) staff       (20)     7060 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/main.py
--rw-r--r--   0 vasily     (501) staff       (20)       28 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/nux.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.318122 promptops-0.1.5/promptops/query/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/query/explanation.py
--rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query/messages.py
--rw-r--r--   0 vasily     (501) staff       (20)    16123 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/query/query.py
--rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.318899 promptops-0.1.5/promptops/recipes/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/recipes/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     6435 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/recipes/creation.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.319703 promptops-0.1.5/promptops/scrub_secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/scrub_secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/scrub_secrets/scrub.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.320467 promptops-0.1.5/promptops/secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/secrets/scrub.py
--rw-r--r--   0 vasily     (501) staff       (20)      326 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/settings.py
--rw-r--r--   0 vasily     (501) staff       (20)     2292 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/settings_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.322954 promptops-0.1.5/promptops/shells/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3367 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/shells/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/bash.py
--rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/common.py
--rw-r--r--   0 vasily     (501) staff       (20)     1635 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/fish.py
--rw-r--r--   0 vasily     (501) staff       (20)     1789 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/zsh.py
--rw-r--r--   0 vasily     (501) staff       (20)     2543 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/similarity.py
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/trace.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.324069 promptops-0.1.5/promptops/ui/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui/prompts.py
--rw-r--r--   0 vasily     (501) staff       (20)     7026 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui/selections.py
--rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui.py
--rw-r--r--   0 vasily     (501) staff       (20)     3990 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/user.py
--rw-r--r--   0 vasily     (501) staff       (20)       22 2023-05-25 18:38:54.000000 promptops-0.1.5/promptops/version.py
--rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/version_check.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.313501 promptops-0.1.5/promptops.egg-info/
--rw-r--r--   0 vasily     (501) staff       (20)     1929 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1937 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/SOURCES.txt
--rw-r--r--   0 vasily     (501) staff       (20)        1 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/dependency_links.txt
--rw-r--r--   0 vasily     (501) staff       (20)      120 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/entry_points.txt
--rw-r--r--   0 vasily     (501) staff       (20)      209 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/requires.txt
--rw-r--r--   0 vasily     (501) staff       (20)       23 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/top_level.txt
--rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.5/pyproject.toml
--rw-r--r--   0 vasily     (501) staff       (20)       78 2023-05-25 18:39:37.325199 promptops-0.1.5/setup.cfg
--rw-r--r--   0 vasily     (501) staff       (20)     1967 2023-05-24 14:41:57.000000 promptops-0.1.5/setup.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.969483 promptops-0.1.6/
+-rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.6/LICENSE.txt
+-rw-r--r--   0 vasily     (501) staff       (20)     2255 2023-06-07 22:03:36.969644 promptops-0.1.6/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     1618 2023-06-07 21:55:02.000000 promptops-0.1.6/README.md
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.943019 promptops-0.1.6/local_runner/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/__init__.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.944510 promptops-0.1.6/local_runner/comms/
+-rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/comms/http_reporter.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.6/local_runner/comms/ws.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.945187 promptops-0.1.6/local_runner/config/
+-rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/config/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/config/config.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.945777 promptops-0.1.6/local_runner/creds/
+-rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/creds/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/creds/creds.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.946278 promptops-0.1.6/local_runner/exec/
+-rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/exec/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/exec/manager.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.947046 promptops-0.1.6/local_runner/handler/
+-rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/handler/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/handler/censor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/handler/handler.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.6/local_runner/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.947653 promptops-0.1.6/local_runner/registration/
+-rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/registration/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/registration/registration.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.948334 promptops-0.1.6/local_runner/tokens/
+-rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/tokens/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.6/local_runner/tokens/issuer.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.952869 promptops-0.1.6/promptops/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/corrections.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/feedback.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.955747 promptops-0.1.6/promptops/gitaware/
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/gitaware/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      632 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/gitaware/project.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/history.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.957085 promptops-0.1.6/promptops/index/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2692 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/content.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/entry_point.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/index/index_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.959503 promptops-0.1.6/promptops/loading/
+-rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/context.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/pong.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/progress.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/promptops.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/loading/simple.py
+-rw-r--r--   0 vasily     (501) staff       (20)     8515 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.961698 promptops-0.1.6/promptops/query/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.6/promptops/query/explanation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/query/git_repo.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query/messages.py
+-rw-r--r--   0 vasily     (501) staff       (20)    18387 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/query/query.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/query.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.962814 promptops-0.1.6/promptops/recipes/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/recipes/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     8841 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/recipes/creation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     5466 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/recipes/terraform.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.963623 promptops-0.1.6/promptops/scrub_secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/scrub_secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/scrub_secrets/scrub.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.964439 promptops-0.1.6/promptops/secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/secrets/scrub.py
+-rw-r--r--   0 vasily     (501) staff       (20)      364 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/settings.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2440 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/settings_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.966886 promptops-0.1.6/promptops/shells/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/shells/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4861 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/shells/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/shells/bash.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/shells/common.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1946 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/shells/fish.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2767 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/shells/zsh.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2902 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/similarity.py
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/trace.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.969034 promptops-0.1.6/promptops/ui/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/ui/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/ui/input.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/ui/prompts.py
+-rw-r--r--   0 vasily     (501) staff       (20)     8990 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/ui/selections.py
+-rw-r--r--   0 vasily     (501) staff       (20)      460 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/ui/vim.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/ui.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/user.py
+-rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-07 21:55:02.000000 promptops-0.1.6/promptops/version.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.6/promptops/version_check.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-07 22:03:36.955040 promptops-0.1.6/promptops.egg-info/
+-rw-r--r--   0 vasily     (501) staff       (20)     2255 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2199 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/SOURCES.txt
+-rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/dependency_links.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/entry_points.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      209 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/requires.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-07 22:03:36.000000 promptops-0.1.6/promptops.egg-info/top_level.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.6/pyproject.toml
+-rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-07 22:03:36.970219 promptops-0.1.6/setup.cfg
+-rw-r--r--   0 vasily     (501) staff       (20)     1967 2023-05-24 14:41:57.000000 promptops-0.1.6/setup.py
```

### Comparing `promptops-0.1.5/LICENSE.txt` & `promptops-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/PKG-INFO` & `promptops-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.5
+Version: 0.1.6
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
@@ -20,41 +20,53 @@
 <img src="https://github.com/promptops/cli/raw/main/media/default.png" />
 
 # Features
 
 - find the right command without leaving the terminal
 - `um` can index your history to find commands you've run before
 - `um` instantly learns from your corrections
+- `um workflow` can help you provision infrastructure
 - simple interface to clarify your question or provide more context
-- free to use
 
 # Installation
 
-## pip (preferred)
+## Linux - Ubuntu
+```shell
+curl -fsSL -o ubuntu-installer.sh https://raw.githubusercontent.com/promptops/cli/main/ubuntu-installer.sh
+chmod 700 ubuntu-installer.sh
+./ubuntu-installer.sh
+```
 
-Make sure you have python 3.9 or more recent
+## MacOS - Homebrew
 
 ```shell
-pip3 install promptops
+brew install promptops/promptops/promptops-cli
 ```
 
-## homebrew (MacOS only)
+## pip 
+
+Make sure you have python 3.10 or more recent
+[python.org downloads](https://www.python.org/downloads/)
 
 ```shell
-brew install promptops/promptops/promptops-cli
+pip3 install promptops
 ```
 
 # Usage
 
 ## um
 
 ```shell
 um <question>
 ```
 
+```shell
+um workflow <multi-stepped-prompt>
+```
+
 ## local runner
 
 ```shell
 promptops runner
 ```
 
 # Examples
@@ -75,15 +87,15 @@
 <img src="https://github.com/promptops/cli/raw/main/media/clarify.png" />
 
 # Development setup
 
 create virtual env
 
 ```shell
-python3 -m venv ./venv
+python3.10 -m venv ./venv
 . ./venv/bin/activate
 ```
 
 install dependencies
 
 ```shell
 pip install -r requirements.txt
```

### Comparing `promptops-0.1.5/README.md` & `promptops-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,41 +3,53 @@
 <img src="https://github.com/promptops/cli/raw/main/media/default.png" />
 
 # Features
 
 - find the right command without leaving the terminal
 - `um` can index your history to find commands you've run before
 - `um` instantly learns from your corrections
+- `um workflow` can help you provision infrastructure
 - simple interface to clarify your question or provide more context
-- free to use
 
 # Installation
 
-## pip (preferred)
+## Linux - Ubuntu
+```shell
+curl -fsSL -o ubuntu-installer.sh https://raw.githubusercontent.com/promptops/cli/main/ubuntu-installer.sh
+chmod 700 ubuntu-installer.sh
+./ubuntu-installer.sh
+```
 
-Make sure you have python 3.9 or more recent
+## MacOS - Homebrew
 
 ```shell
-pip3 install promptops
+brew install promptops/promptops/promptops-cli
 ```
 
-## homebrew (MacOS only)
+## pip 
+
+Make sure you have python 3.10 or more recent
+[python.org downloads](https://www.python.org/downloads/)
 
 ```shell
-brew install promptops/promptops/promptops-cli
+pip3 install promptops
 ```
 
 # Usage
 
 ## um
 
 ```shell
 um <question>
 ```
 
+```shell
+um workflow <multi-stepped-prompt>
+```
+
 ## local runner
 
 ```shell
 promptops runner
 ```
 
 # Examples
@@ -58,15 +70,15 @@
 <img src="https://github.com/promptops/cli/raw/main/media/clarify.png" />
 
 # Development setup
 
 create virtual env
 
 ```shell
-python3 -m venv ./venv
+python3.10 -m venv ./venv
 . ./venv/bin/activate
 ```
 
 install dependencies
 
 ```shell
 pip install -r requirements.txt
```

### Comparing `promptops-0.1.5/local_runner/comms/dtos.py` & `promptops-0.1.6/local_runner/comms/dtos.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/comms/http_reporter.py` & `promptops-0.1.6/local_runner/comms/http_reporter.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/comms/ws.py` & `promptops-0.1.6/local_runner/comms/ws.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,38 @@
 
 
 class Listener:
     def __init__(self, handler: Callable):
         self.handler = handler
 
     async def listen(self, url: str, get_token: Callable):
-        async with websockets.connect(url) as websocket:
-            auth_needed = True
-            while True:
-                if auth_needed:
-                    token = get_token()
-                    await websocket.send(json.dumps({
-                        "__action__": "authorize",
-                        "token": token
-                    }))
-                message = await websocket.recv()
-                data = json.loads(message)
+        while True:
+            async with websockets.connect(url) as websocket:
+                auth_needed = True
+                while True:
+                    if auth_needed:
+                        token = get_token()
+                        await websocket.send(json.dumps({
+                            "__action__": "authorize",
+                            "token": token
+                        }))
+                    try:
+                        message = await websocket.recv()
+                    except websockets.ConnectionClosed:
+                        print("connection closed, reconnecting...")
+                        break
+                    data = json.loads(message)
 
-                action = data.get("__action__")
-                if action:
-                    if action == "authorization_success":
-                        print("Ready")
-                        auth_needed = False
-                    elif action in ["no_authorization", "authorization_failure"]:
-                        raise ValueError(f"{action}: {data.get('__text__')}")
+                    action = data.get("__action__")
+                    if action:
+                        if action == "authorization_success":
+                            print("Ready")
+                            auth_needed = False
+                        elif action in ["no_authorization", "authorization_failure"]:
+                            raise ValueError(f"{action}: {data.get('__text__')}")
+                        else:
+                            raise ValueError(f"Unknown action: {action}")
                     else:
-                        raise ValueError(f"Unknown action: {action}")
-                else:
-                    try:
-                        await self.handler(data, websocket)
-                    except Exception as e:
-                        logging.error("error handling message", exc_info=e)
+                        try:
+                            await self.handler(data, websocket)
+                        except Exception as e:
+                            logging.error("error handling message", exc_info=e)
```

### Comparing `promptops-0.1.5/local_runner/config/config.py` & `promptops-0.1.6/local_runner/config/config.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/creds/creds.py` & `promptops-0.1.6/local_runner/creds/creds.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/exec/manager.py` & `promptops-0.1.6/local_runner/exec/manager.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/handler/handler.py` & `promptops-0.1.6/local_runner/handler/handler.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/main.py` & `promptops-0.1.6/local_runner/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import sys
 
 import requests
 
 from local_runner.comms import Listener, HttpReporter
 from local_runner import config
 from local_runner.tokens import Issuer
 from local_runner import creds
@@ -13,15 +14,19 @@
 
 async def _main():
     cfg = config.default()
     try:
         c = creds.default(cfg.credentials_file)
     except creds.NotFoundError:
         print("Credentials not found. Initiating pairing...")
-        c = await asyncio.wait_for(register(cfg.registration_url, cfg.registration_code_rotation), cfg.registration_timeout)
+        try:
+            c = await asyncio.wait_for(register(cfg.registration_url, cfg.registration_code_rotation), cfg.registration_timeout)
+        except asyncio.TimeoutError:
+            print("Pairing timed out")
+            sys.exit(1)
         creds.store(cfg.credentials_file, c)
 
     issuer = Issuer(c)
     mgr = exec.Manager(2)
     mgr.start()
 
     session = requests.Session()
```

### Comparing `promptops-0.1.5/local_runner/registration/registration.py` & `promptops-0.1.6/local_runner/registration/registration.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/local_runner/tokens/issuer.py` & `promptops-0.1.6/local_runner/tokens/issuer.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/corrections.py` & `promptops-0.1.6/promptops/corrections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/history.py` & `promptops-0.1.6/promptops/history.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,24 +61,30 @@
         cmd = item["text"]
         vector = np.array(item["embeddings"])
         items.append((cmd, vector))
 
     return items
 
 
-def index_history(show_progress: bool = None):
+def index_history(show_progress: bool = None, max_history: int = 1000):
     progress = None
     if show_progress:
         from promptops.loading.progress import ProgressSpinner
 
         progress = ProgressSpinner(100)
         progress.increment(1)
 
     db = get_history_db()
-    prev_commands = get_shell().get_full_history()
+    if max_history > 0:
+        prev_commands = get_shell().get_recent_history(max_history + 1)
+    else:
+        prev_commands = get_shell().get_full_history()
+    has_more = len(prev_commands) > max_history > 0
+    if max_history > 0:
+        prev_commands = prev_commands[-max_history:]
 
     if show_progress:
         progress.increment(3)
 
     indexed_commands = {obj if isinstance(obj, str) else obj["cmd"] for obj in db.objects}
     delta = list(set(prev_commands) - indexed_commands)
     batch_size = 32
@@ -90,29 +96,30 @@
         progress.increment(4)
     if show_progress:
         progress.increment(2)
 
     if len(delta) == 0:
         if show_progress:
             progress.set(100)
-        return
-
-    progress_inc = (100 - 6) // (len(delta) / batch_size)
+        return has_more
 
+    start_progress = 6
     for i in range(0, len(delta), batch_size):
-        for cmd, vector in embedding_batch(delta[i : i + batch_size]):
+        for cmd, vector in embedding_batch(delta[i: i + batch_size]):
             db.add(vector, {"cmd": cmd, "ignore": False})
         if show_progress:
-            progress.increment(progress_inc)
+            progress.set(start_progress + (i + batch_size) / len(delta) * (100 - start_progress))
 
     db.save(os.path.expanduser(settings.history_db_path))
 
     if show_progress:
         progress.set(100)
 
+    return has_more
+
 
 def update_history():
     if settings.index_history:
         index_history()
 
 
 def add(cmd: str, return_code: int):
```

### Comparing `promptops-0.1.5/promptops/loading/base.py` & `promptops-0.1.6/promptops/loading/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/loading/pong.py` & `promptops-0.1.6/promptops/loading/pong.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/loading/progress.py` & `promptops-0.1.6/promptops/loading/progress.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/loading/promptops.py` & `promptops-0.1.6/promptops/loading/promptops.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/loading/simple.py` & `promptops-0.1.6/promptops/loading/simple.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/main.py` & `promptops-0.1.6/promptops/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from promptops import settings
 from promptops import settings_store
 from promptops import version_check
 from promptops import query
 from promptops import user
 from promptops.recipes.creation import workflow_entrypoint
+from promptops.index.entry_point import entry_point as index_entry_point
 
 ENDPOINT_ENV = "PROMPTOPS_ENDPOINT"
 
 
 def runner_mode(args):
     from promptops.feedback import feedback
 
@@ -123,18 +124,35 @@
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO, format="%(message)s")
     version_check.version_check()
     if not registered or args.config:
         user.register()
+        args.history_context = settings.history_context
     else:
         from promptops import history
 
         history.update_history()
+
+    if args.question and len(args.question) > 0:
+        if args.question[0] == 'workflow':
+            return workflow_entrypoint(args)
+        elif args.question[0] == 'index':
+            # index subcommand
+            subparser = ArgumentParser(
+                prog=f"{alias} index",
+                usage=f"{alias} index [action]",
+                description=f"{alias} index: manage the indexed data",
+            )
+            subparser.add_argument("action", choices=["list", "add", "remove", "test"], help="list or update the index")
+            subparser.add_argument("--source", help="the source to add or remove")
+            subparser.add_argument("--query", help="query to test with")
+            sub_args = subparser.parse_args(args.question[1:])
+            return index_entry_point(sub_args)
     query.query_mode(args)
 
 
 def entry_main():
     # Set the global exception handler
     sys.excepthook = handle_exception(sys.excepthook)
 
@@ -180,14 +198,20 @@
     parser_runner = subparsers.add_parser("runner", help="run commands from slack")
     parser_runner.set_defaults(func=runner_mode)
 
     parser_workflow = subparsers.add_parser("workflow", help="run a complex or multi-stepped script")
     parser_workflow.add_argument("question", nargs=REMAINDER, help="the question to generate scripts for")
     parser_workflow.set_defaults(func=workflow_entrypoint)
 
+    parser_index = subparsers.add_parser("index", help="manage the indexed data")
+    parser_index.add_argument("action", choices=["list", "add", "remove", "test"], help="list or update the index")
+    parser_index.add_argument("--source", help="the source to add or remove")
+    parser_index.add_argument("--query", help="query to test with")
+    parser_index.set_defaults(func=index_entry_point)
+
     args = parser.parse_args()
 
     registered = user.has_registered()
 
     if not hasattr(args, "func"):
         if args.version:
             from promptops.version import __version__
@@ -196,27 +220,29 @@
 
             r = version_check.version_check()
             if not r.update_required:
                 print("latest version:", r.latest_version)
             sys.exit(0)
         if args.config:
             user.register()
+            args.history_context = settings.history_context
             sys.exit(0)
 
         parser.print_help()
         return
 
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO, format="%(message)s")
 
     version_check.version_check()
     if not registered:
         user.register()
+        args.history_context = settings.history_context
     else:
         from promptops import history
 
         history.update_history()
     args.func(args)
```

### Comparing `promptops-0.1.5/promptops/query/explanation.py` & `promptops-0.1.6/promptops/query/explanation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/query/messages.py` & `promptops-0.1.6/promptops/query/messages.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/query/query.py` & `promptops-0.1.6/promptops/query/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 from promptops import similarity
 from promptops import corrections
 from promptops.corrections import get_correction
 from promptops.feedback import feedback
 from promptops import history
 from promptops import settings_store
 from promptops import scrub_secrets
+from promptops import shells
+from promptops.index import index_store
+from promptops import gitaware
 from .dtos import Result
 from .explanation import get_explanation, ReturningThread
 from . import messages
 
 
 def deduplicate(results: list[Result]):
     results_set = set()
@@ -39,35 +42,67 @@
         if result.script in results_set:
             continue
         results_set.add(result.script)
         final_results.append(result)
     return final_results
 
 
+def printer(pipe, func):
+    for line in iter(pipe.readline, b''):
+        line_decoded = line.decode()
+        sys.stdout.write(line_decoded)
+        sys.stdout.flush()
+        func(line)
+    pipe.close()
+
+
 def run(cmd: Result) -> (int, Optional[str]):
     if cmd.lang == "shell":
-        proc = subprocess.run(
+        process = subprocess.Popen(
             cmd.script, shell=True, start_new_session=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
-        if proc.stdout and len(proc.stdout) > 0:
-            sys.stdout.write(proc.stdout.decode("utf-8"))
-        if proc.stderr and len(proc.stderr) > 0:
-            sys.stdout.write(proc.stderr.decode("utf-8"))
+        stdout = []
+        stderr = []
+
+        thread_out = threading.Thread(target=printer, args=[process.stdout, lambda line: stdout.append(line.decode())])
+        thread_err = threading.Thread(target=printer, args=[process.stderr, lambda line: stderr.append(line.decode())])
+
+        thread_out.start()
+        thread_err.start()
+        thread_out.join()
+        thread_err.join()
+
+        sys.stdout.write("\n")
         sys.stdout.flush()
 
-        history.add(scrub_secrets.scrub_line(".bash_history", cmd.script), proc.returncode)
-        return proc.returncode, proc.stderr.decode("utf-8")
+        process.wait()
+
+        history.add(scrub_secrets.scrub_line(".bash_history", cmd.script), process.returncode)
+        return process.returncode, "".join(stderr)
     else:
         raise NotImplementedError(f"{cmd.lang} not implemented yet")
 
 
 def corrections_search(embedding):
     db = corrections.get_db()
     similar = db.search(embedding, k=3, min_similarity=0.8)
-    return [(corrections.QATuple.from_dict(s), score) for s, score in similar]
+    return list(filter(lambda c: c[0].corrected is not None, [(corrections.QATuple.from_dict(s), score) for s, score in similar]))
+
+
+def search_indexed_fragments(embedding, current_dir: str) -> list[index_store.SearchResult]:
+    store = index_store.IndexStore(os.path.expanduser(settings.user_index_root))
+
+    def accept_source(meta: index_store.ItemMetadata):
+        if meta.item_type != "file":
+            return True
+        dirname = os.path.dirname(meta.item_location)
+        return current_dir.startswith(dirname)
+
+    similar = store.search(embedding, k=3, min_similarity=0.7, accept_source=accept_source)
+    return similar
 
 
 def make_revise_option():
     return "\x1b[3m💭️ don't see what you're looking for? try providing more context\x1b[0m"
 
 
 ORIGIN_SYMBOLS = {"history": "📖", "promptops": "✨"}
@@ -81,15 +116,15 @@
 class ConfirmResult:
     result: Result = None
     confirmed: str = ""
     question: str = None
     options: list = None
 
 
-def revise_loop(questions: list[str], prev_results: list[list[str]]) -> ConfirmResult:
+def revise_loop(questions: list[str], prev_results: list[list[str]], history_context: list[str]) -> ConfirmResult:
     embedding = similarity.embedding(text="\n".join(questions))
     update_lock = threading.Lock()
     corrected_results = []
 
     similar_corrections = corrections_search(embedding)
     logging.debug("found %d similar corrections", len(similar_corrections))
     if len(similar_corrections) > 0:
@@ -106,25 +141,37 @@
         Result(script=r if isinstance(r, str) else r["cmd"], explanation="loaded from shell history", origin="history")
         for r, _ in history_results
     ]
 
     results = corrected_results + history_results
     results = deduplicate(results)
 
+    relevant_indexed_data = search_indexed_fragments(embedding, os.getcwd())
+    if len(relevant_indexed_data) > 0:
+        print("  found information that might be relevant to your question in:")
+        printed = set()
+        for r in relevant_indexed_data:
+            if r.item.item_location in printed:
+                continue
+            print(f"  ● {r.item.item_location}")
+            printed.add(r.item.item_location)
+        print()
+
     ui = None
     tasks = [
         ReturningThread(
             query,
             kwargs=dict(
                 q=questions[-1],
                 prev_questions=questions[:-1],
                 corrected_results=[qa for qa, _ in similar_corrections],
                 prev_results=prev_results,
                 similar_history=[r.script for r in history_results],
-                history_context=[],
+                history_context=history_context,
+                relevant_indexed_data=relevant_indexed_data,
             ),
             daemon=True,
         )
     ]
     num_running = len(tasks)
 
     def update_results(extra):
@@ -229,15 +276,15 @@
                         target=_explain_and_done,
                         kwargs=dict(
                             result=selected,
                             prev_questions=questions[:-1],
                             prev_results=prev_results,
                             corrected_results=[qa for qa, _ in similar_corrections],
                             similar_history=[r.script for r in history_results],
-                            history_context=[],
+                            history_context=history_context,
                         ),
                         daemon=True,
                     )
                     pt = ReturningThread(
                         target=_confirm_and_done,
                         args=(selected.script, False),
                         kwargs=dict(
@@ -271,15 +318,15 @@
             elif confirmed == prompts.EXIT:
                 raise KeyboardInterrupt()
             return ConfirmResult(result=selected, confirmed=confirmed)
 
 
 def correction_loop(prompt: str, command: str, error: str) -> Optional[Result]:
     selected = prompts.confirm(
-        f"looks like the command failed (return code was not 0), would you like us to attempt to fix it?"
+        f"It looks like the command failed, would you like us to attempt to fix it using the stderr output?"
     )
     if selected == prompts.GO_BACK:
         return None
     elif selected == prompts.EXIT:
         raise KeyboardInterrupt()
 
     with loading_animation(Simple("thinking...")):
@@ -301,14 +348,18 @@
         raise KeyboardInterrupt()
 
     print()
     return selected
 
 
 def do_query(question: str):
+    if git_root := gitaware.git_root():
+        from .git_repo import offer_to_index
+        offer_to_index(git_root)
+
     question = question.strip()
     if question == "":
         feedback({"event": "empty-initial-query"})
         for i in range(2):
             if i > 0:
                 print("please enter a question")
             bottom_toolbar = HTML("<b>[enter]</b> confirm <b>[ctrl+c]</b> exit")
@@ -324,17 +375,18 @@
 
     questions = [question]
     prev_results = []
 
     print()
 
     def input_loop():
+        history_context = shells.get_shell().get_recent_history(settings.history_context) if settings.history_context else []
         while True:
             try:
-                results = revise_loop(questions, prev_results)
+                results = revise_loop(questions, prev_results, history_context)
                 if results.result:
                     return results.result, results.confirmed
                 else:
                     print()
                     feedback({"event": "revise"})
                     questions.append(results.question)
                     prev_results.append(results.options)
@@ -345,35 +397,35 @@
 
     try:
         cmd, confirmed = input_loop()
     except KeyboardInterrupt:
         feedback({"event": "cancelled"})
         sys.exit(1)
 
-    if cmd.script != confirmed or len(questions) > 1:
+    if (cmd.script != confirmed or len(questions) > 1) and confirmed:
         # the user corrected the script
         db = corrections.get_db()
         q = "\n".join(questions)
         vector = similarity.embedding(text=q)
         db.add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=confirmed).to_dict())
         logging.debug("added correction to db")
         db.save(os.path.expanduser(settings.corrections_db_path))
         feedback({"event": "corrected"})
 
     feedback({"event": "run"})
     revised_cmd = copy(cmd)
     revised_cmd.script = confirmed
-    rc, stdout = run(revised_cmd)
+    rc, stderr = run(revised_cmd)
     feedback({"event": "finished", "rc": rc})
 
     while rc != 0:
-        corrected_cmd = correction_loop("\n".join(questions), revised_cmd.script, stdout)
+        corrected_cmd = correction_loop("\n".join(questions), revised_cmd.script, stderr)
         if not corrected_cmd:
             return
-        rc, stdout = run(corrected_cmd)
+        rc, stderr = run(corrected_cmd)
         if rc == 0:
             db = corrections.get_db()
             q = "\n".join(questions)
             vector = similarity.embedding(text=q)
             db.add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=corrected_cmd.script).to_dict())
             logging.debug("added correction to db")
             db.save(os.path.expanduser(settings.corrections_db_path))
@@ -406,25 +458,33 @@
     *,
     q: str,
     prev_questions: list[str],
     prev_results: list[list[str]],
     corrected_results: list[corrections.QATuple],
     history_context: list[str],
     similar_history: list[str],
+    relevant_indexed_data: list[index_store.SearchResult],
 ) -> list[Result]:
     req = {
         "query": q,
         "prev_questions": prev_questions,
         "prev_suggestions": prev_results,
         "context": {
             "history": history_context,
             "similar": similar_history,
             "corrections": [
                 (qa.question, scrub_secrets.scrub_line("~/.bash_history", qa.corrected)) for qa in corrected_results
             ],
+            "user_data": [
+                {
+                    "source_type": r.item.item_type,
+                    "source": r.item.item_location,
+                    "fragment": r.fragment.fragment,
+                } for r in relevant_indexed_data
+            ]
         },
         "model": settings.model,
         "trace_id": trace.trace_id,
         "platform": sys.platform,
         "shell": os.environ.get("SHELL"),
     }
     logging.debug("query with request: %s", req)
```

### Comparing `promptops-0.1.5/promptops/query.py` & `promptops-0.1.6/promptops/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/scrub_secrets/scrub.py` & `promptops-0.1.6/promptops/scrub_secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/secrets/scrub.py` & `promptops-0.1.6/promptops/secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/settings_store.py` & `promptops-0.1.6/promptops/settings_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import os
 
 from promptops import settings
 
 
 config_file_path = "~/.promptops/cli-config.json"
 
@@ -71,8 +72,11 @@
     return diff_keys | {key for key in common_keys if dict1[key] != dict2[key]}
 
 
 def is_changed() -> bool:
     data = _build_data()
     diff_keys = dict_diff_keys(data, _loaded_data or {})
     diff_keys.discard("endpoint")
+    logging.debug(f"diff_keys: {diff_keys}")
+    logging.debug("data: %s", data)
+    logging.debug("_loaded_data: %s", _loaded_data)
     return len(diff_keys) > 0
```

### Comparing `promptops-0.1.5/promptops/shells/bash.py` & `promptops-0.1.6/promptops/shells/bash.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/shells/common.py` & `promptops-0.1.6/promptops/shells/common.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/shells/fish.py` & `promptops-0.1.6/promptops/shells/fish.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .base import Shell
 from .base import reverse_readline, accept_command
 from promptops.scrub_secrets import scrub_lines
 import os
+import logging
 
 
 def _is_start_line(line):
     return line.startswith("- cmd: ")
 
 
 class Fish(Shell):
@@ -19,25 +20,31 @@
 
     def _get_cmds_from_lines(self, lines):
         commands = []
         for line in lines:
             if _is_start_line(line):
                 cmd = line.split("- cmd: ")[1].rstrip()
                 # unescape see https://stackoverflow.com/a/57192592
-                cmd = cmd.encode("latin-1", "backslashreplace").decode("unicode-escape")
-                if accept_command(cmd):
-                    commands.append(cmd)
+                try:
+                    cmd = cmd.encode("latin-1", "backslashreplace").decode("unicode-escape")
+                    if accept_command(cmd):
+                        commands.append(cmd)
+                except UnicodeDecodeError:
+                    logging.debug("UnicodeDecodeError at line: ", line)
         return commands
 
     def get_recent_history(self, look_back: int = 10):
         fname = os.path.expanduser(self.history_file)
         commands = []
         for line in reverse_readline(fname):
             if len(commands) >= look_back:
                 break
             if _is_start_line(line):
                 cmd = line.split("- cmd: ")[1].rstrip()
                 # unescape see https://stackoverflow.com/a/57192592
-                cmd = cmd.encode("latin-1", "backslashreplace").decode("unicode-escape")
-                if accept_command(cmd):
-                    commands.append(cmd)
+                try:
+                    cmd = cmd.encode("latin-1", "backslashreplace").decode("unicode-escape")
+                    if accept_command(cmd):
+                        commands.append(cmd)
+                except UnicodeDecodeError:
+                    logging.debug("UnicodeDecodeError at line: ", line)
         return scrub_lines(fname, list(reversed(commands)))
```

### Comparing `promptops-0.1.5/promptops/similarity.py` & `promptops-0.1.6/promptops/similarity.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,23 @@
         if len(self.vectors) == 0:
             return []
         scores = np.dot(vector, self.vectors.T).flatten()
         # rank results
         results = np.argsort(scores)[::-1]
         return [(self.objects[i], scores[i]) for i in results[:k] if scores[i] > min_similarity]
 
+    def argsearch(self, vector, k=1, min_similarity=0.8):
+        # compute cosine similarity
+        if len(self.vectors) == 0:
+            return []
+        scores = np.dot(vector, self.vectors.T).flatten()
+        # rank results
+        results = np.argsort(scores)[::-1]
+        return [(i, scores[i]) for i in results[:k] if scores[i] > min_similarity]
+
     def index(self, obj):
         return self.objects.index(obj)
 
     def remove(self, index):
         self.vectors = np.delete(self.vectors, index, axis=0)
         del self.objects[index]
```

### Comparing `promptops-0.1.5/promptops/ui/prompts.py` & `promptops-0.1.6/promptops/ui/prompts.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/ui/selections.py` & `promptops-0.1.6/promptops/ui/selections.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,32 +5,14 @@
 import typing
 from promptops.loading.simple import loader
 from prompt_toolkit.formatted_text import to_plain_text, ANSI
 import wcwidth
 import colorama
 
 
-def getch():
-    if sys.platform == "win32":
-        import msvcrt
-
-        return msvcrt.getwch()
-    else:
-        import tty
-        import termios
-
-        fd = sys.stdin.fileno()
-        old = termios.tcgetattr(fd)
-        try:
-            tty.setraw(fd)
-            return sys.stdin.read(1)
-        finally:
-            termios.tcsetattr(fd, termios.TCSADRAIN, old)
-
-
 FOOTER_SECTIONS = {
     "select": f"{colorama.Style.BRIGHT}[↑/↓]{colorama.Style.RESET_ALL} select",
     "confirm": f"{colorama.Style.BRIGHT}[enter]{colorama.Style.RESET_ALL} confirm",
     "cancel": f"{colorama.Style.BRIGHT}[ctrl+c]{colorama.Style.RESET_ALL} cancel",
     "copy": f"{colorama.Style.BRIGHT}[c]{colorama.Style.RESET_ALL} copy",
 }
 
@@ -41,106 +23,156 @@
         options: list[str],
         is_loading: bool,
         cursor="➜︎",
         show_timer=False,
         loading_text="getting you the best results ...",
         footer=" ".join([FOOTER_SECTIONS["select"], FOOTER_SECTIONS["confirm"], FOOTER_SECTIONS["cancel"]]),
         actions: dict[str, typing.Callable[[str, "UI"], None]] = None,
+        header=""
     ):
         self._selected = 0
         self._options = options
         self._is_loading = is_loading
         self._start = time.time()
         self._cursor = cursor
         self._footer = footer
+        self._header = header
         self._loading_line_index = None
         self._option_indexes = []
         self._thread = threading.Thread(target=self._loading_animation, daemon=True)
         self._show_timer = show_timer
         self._spinner = loader(loading_text)
         self._lock = threading.Lock()
         self._is_active = True
         self._actions = actions or {}
 
         self._lines_written = 0
+        self._raw_mode = False
+        self._old_stdin_attrs = None
+        self._offset = 0
+        self._estimated_lines = []
+        self._usable_lines = 0
         self.render()
         self._thread.start()
 
     def render(self):
         with self._lock:
+            if self._raw_mode:
+                import termios
+                fd = sys.stdin.fileno()
+                termios.tcsetattr(fd, termios.TCSADRAIN, self._old_stdin_attrs)
+
             # clean all the lines that were written
-            sys.stdout.write("\r\x1b[K")
+            sys.stdout.write("\x1b[2K")
             for _ in range(self._lines_written):
-                sys.stdout.write("\x1b[1A\x1b[K")
+                sys.stdout.write("\x1b[1A\x1b[2K")
+            sys.stdout.write("\r")
+
             size = os.get_terminal_size()
             width = size.columns
+            height = size.lines
+            extra_lines = 0
+            if self._header:
+                extra_lines += 2
+            if self._is_loading:
+                extra_lines += 1
+            if self._footer:
+                extra_lines += 2
+            self._usable_lines = height - extra_lines
             self._option_indexes = []
 
             current_line = 0
+            if self._header:
+                sys.stdout.write(f"{self._header}\n\n")
+                current_line += 2
+            option_lines = 0
             for i, option in enumerate(self._options):
                 self._option_indexes.append(current_line)
                 if i == self._selected:
                     text = f" {self._cursor} {self._get_formatted_text(option, True)}"
                 else:
                     text = f"   {self._get_formatted_text(option, False)}"
-                sys.stdout.write(f"\r{text}")
-                sys.stdout.write("\n\r")
+                estimated_lines = 0
                 for line in to_plain_text(ANSI(text)).split("\n"):
-                    current_line += 1
                     text_width = wcwidth.wcswidth(line)
-                    if text_width > width:
-                        current_line += text_width // width
+                    estimated_lines += 1  # we always write at least one line
+                    estimated_lines += text_width // width
+                self._estimated_lines.append(estimated_lines)
+                if i < self._offset:
+                    continue
+                option_lines += estimated_lines
+                if option_lines <= self._usable_lines:
+                    sys.stdout.write(f"{text}\n")
+                    current_line += estimated_lines
 
             if self._is_loading:
                 self._loading_line_index = current_line
                 if self._show_timer:
-                    sys.stdout.write(f"\r  {self._spinner(advance=False)} {(time.time() - self._start):.2f}s\n\r")
+                    sys.stdout.write(f"   {self._spinner(advance=False)} {(time.time() - self._start):.2f}s\n")
                 else:
-                    sys.stdout.write(f"\r  {self._spinner(advance=False)}\n\r")
+                    sys.stdout.write(f"   {self._spinner(advance=False)}\n")
                 current_line += 1
 
             if self._footer:
-                sys.stdout.write(f"\n\r{self._footer}")
+                sys.stdout.write(f"\n{self._footer}")
                 current_line += 1
 
             self._lines_written = current_line
 
             sys.stdout.flush()
+            if self._raw_mode:
+                import tty
+                fd = sys.stdin.fileno()
+                tty.setraw(fd)
 
     def _loading_animation(self):
         while True:
             with self._lock:
                 if self._is_loading:
-                    # sys.stdout.write("\x1b[s")
                     sys.stdout.write("\x1b7")
-                    sys.stdout.write(f"\x1b[{self._lines_written - self._loading_line_index}A\x1b[K")
+                    sys.stdout.write(f"\x1b[{self._lines_written - self._loading_line_index}A")
+                    sys.stdout.write("\x1b[2K\r")
                     if self._show_timer:
-                        sys.stdout.write(f"\r   {self._spinner()} {(time.time() - self._start):.2f}s\n\r")
+                        sys.stdout.write(f"   {self._spinner()} {(time.time() - self._start):.2f}s\n")
                     else:
-                        sys.stdout.write(f"\r   {self._spinner()}\n\r")
-                    # sys.stdout.write("\x1b[u")
+                        sys.stdout.write(f"   {self._spinner()}\n")
                     sys.stdout.write("\x1b8")
                     sys.stdout.flush()
 
             time.sleep(0.1)
 
     def select(self, index):
         if index == self._selected:
             return
         if len(self._options) == 0:
             return
+        if index < self._offset:
+            self._offset = index
+            self._selected = index
+            self.render()
+            return
+        elif index > self._selected:
+            # check if we need to scroll down
+            new_offset = self._offset
+            while sum(self._estimated_lines[new_offset: index + 1]) > self._usable_lines:
+                new_offset += 1
+            if self._offset != new_offset:
+                self._offset = new_offset
+                self._selected = index
+                self.render()
+                return
         with self._lock:
             sys.stdout.write("\x1b7")
             sys.stdout.write(f"\x1b[{self._lines_written - self._option_indexes[index]}A")
             sys.stdout.write(f"\r {self._cursor} {self._get_formatted_text(self._options[index], True)}")
             sys.stdout.write("\x1b8")
             sys.stdout.write("\x1b7")
             sys.stdout.write(f"\x1b[{self._lines_written - self._option_indexes[self._selected]}A")
-            sys.stdout.write(f"\r\x1b[K   {self._get_formatted_text(self._options[self._selected], False)}")
-            sys.stdout.write(f"\x1b[{self._lines_written}B\r")
+            sys.stdout.write(f"\r   {self._get_formatted_text(self._options[self._selected], False)}")
+            sys.stdout.write(f"\x1b[{self._lines_written}B")
             sys.stdout.write("\x1b8")
             sys.stdout.flush()
             self._selected = index
 
     @property
     def selected(self):
         return self._selected
@@ -168,25 +200,45 @@
             return
         self._options = options
         if self._selected >= len(self._options):
             self._selected = len(self._options) - 1
         self._is_loading = is_loading
         self.render()
 
+    def getch(self):
+        if sys.platform == "win32":
+            import msvcrt
+
+            return msvcrt.getwch()
+        else:
+            import tty
+            import termios
+
+            fd = sys.stdin.fileno()
+            old = termios.tcgetattr(fd)
+            self._old_stdin_attrs = old
+            try:
+                tty.setraw(fd)
+                self._raw_mode = True
+                return sys.stdin.read(1)
+            finally:
+                termios.tcsetattr(fd, termios.TCSADRAIN, old)
+                self._raw_mode = False
+
     def input(self):
         while True:
-            key = getch()
+            key = self.getch()
             if key == "\x03":
                 if self._footer:
                     sys.stdout.write("\r\x1b[K")
                 raise KeyboardInterrupt()
             elif key == "\x1b":
-                next_ch = getch()
+                next_ch = self.getch()
                 if next_ch == "[":
-                    last_ch = getch()
+                    last_ch = self.getch()
                     if last_ch == "A":
                         index = max(0, self._selected - 1)
                         self.select(index)
                     elif last_ch == "B":
                         index = min(len(self._options) - 1, self._selected + 1)
                         self.select(index)
             elif key in ["\r", "\n"]:
```

### Comparing `promptops-0.1.5/promptops/ui.py` & `promptops-0.1.6/promptops/ui.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops/user.py` & `promptops-0.1.6/promptops/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import sys
-from typing import Optional
 
 from promptops import settings
 import os
 import uuid
 from functools import lru_cache
+
+from promptops.shells import get_shell
 from promptops.ui.prompts import confirm, EXIT, GO_BACK
 from promptops.ui import selections
 from prompt_toolkit import print_formatted_text
 from prompt_toolkit.formatted_text import HTML
 import requests
 from promptops.trace import trace_id
-from promptops.settings_store import save, set_index_history
+from promptops import settings_store
 
 
 @lru_cache(maxsize=1)
 def user_id() -> str:
     real_path = os.path.expanduser(settings.user_id_path)
     if not os.path.exists(real_path):
         uid = f"user-{uuid.uuid4().hex}"
@@ -32,28 +33,28 @@
 
 
 def has_registered() -> bool:
     real_path = os.path.expanduser(settings.user_id_path)
     return os.path.exists(real_path)
 
 
-def config_flow() -> Optional[dict]:
+def config_flow() -> dict:
     config_selections = {}
 
     print()
     print_formatted_text(
         HTML("  👋 thanks for installing <ansigreen><b>um</b></ansigreen>! let's make sure you get the most out of it")
     )
     print()
 
     options = ["continue", "skip"]
     ui = selections.UI(options, is_loading=False)
     selection = ui.input()
     if selection == 1:
-        return
+        return config_selections
 
     print()
     print()
     print("  📖 indexing your history can greatly improve the speed and the quality of the suggestions")
     print_formatted_text(
         HTML(
             "  do you want to index your history? <b><i>we take special care to"
@@ -64,51 +65,62 @@
 
     options = ["confirm", "skip"]
     ui = selections.UI(options, is_loading=False)
     selection = ui.input()
     if selection != 1:
         from promptops.history import index_history
 
-        set_index_history(True)
-        index_history(show_progress=True)
+        settings_store.set_index_history(True)
+        initial_batch = 1000
+        has_more = index_history(show_progress=True, max_history=initial_batch)
         config_selections["loaded_history"] = True
+        if has_more:
+            print()
+            all_history = get_shell().get_full_history()
+            print_formatted_text(
+                HTML(
+                    f"  📖 we've indexed your last {initial_batch} commands, but there's {len(all_history) - initial_batch} more!"
+                )
+            )
+            print()
+            options = ["continue", "skip for now"]
+            ui = selections.UI(options, is_loading=False)
+            selection = ui.input()
+            if selection != 1:
+                index_history(show_progress=True, max_history=0)
 
     print()
     while True:
         print()
         context_size = 2
         print(
             f"  ↩️  say more with less! the number of previous commands to include"
             f" in the query context (default: {context_size})?"
         )
         print()
         options = ["confirm defaults", "change"]
         ui = selections.UI(options, is_loading=False)
         selection = ui.input()
         if selection == 0:
-            from promptops.settings_store import set_history_context
-
-            set_history_context(context_size)
+            settings_store.set_history_context(context_size)
             config_selections["context_size"] = context_size
             break
         else:
             while True:
                 choice = confirm(str(context_size)).strip()
                 if choice == GO_BACK:
                     break
                 if choice == EXIT:
-                    return
+                    return config_selections
                 if choice.isdigit():
                     # TODO: validate
                     break
             if choice == GO_BACK:
                 continue
-            from promptops.settings_store import set_history_context
-
-            set_history_context(int(choice))
+            settings_store.set_history_context(int(choice))
             config_selections["context_size"] = int(choice)
             break
 
     print()
     print("  🎉 all done! 🎉")
     print()
 
@@ -127,8 +139,8 @@
         settings.endpoint + "/installed",
         json={"trace_id": trace_id, "email": email, "platform": sys.platform, "python_version": sys.version},
         headers={"user-agent": user_agent()},
     )
     config = config_flow()
     config["trace_id"] = trace_id
     requests.post(settings.endpoint + "/config", json=config, headers={"user-agent": user_agent()})
-    save()
+    settings_store.save()
```

### Comparing `promptops-0.1.5/promptops/version_check.py` & `promptops-0.1.6/promptops/version_check.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.5/promptops.egg-info/PKG-INFO` & `promptops-0.1.6/promptops.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.5
+Version: 0.1.6
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
@@ -20,41 +20,53 @@
 <img src="https://github.com/promptops/cli/raw/main/media/default.png" />
 
 # Features
 
 - find the right command without leaving the terminal
 - `um` can index your history to find commands you've run before
 - `um` instantly learns from your corrections
+- `um workflow` can help you provision infrastructure
 - simple interface to clarify your question or provide more context
-- free to use
 
 # Installation
 
-## pip (preferred)
+## Linux - Ubuntu
+```shell
+curl -fsSL -o ubuntu-installer.sh https://raw.githubusercontent.com/promptops/cli/main/ubuntu-installer.sh
+chmod 700 ubuntu-installer.sh
+./ubuntu-installer.sh
+```
 
-Make sure you have python 3.9 or more recent
+## MacOS - Homebrew
 
 ```shell
-pip3 install promptops
+brew install promptops/promptops/promptops-cli
 ```
 
-## homebrew (MacOS only)
+## pip 
+
+Make sure you have python 3.10 or more recent
+[python.org downloads](https://www.python.org/downloads/)
 
 ```shell
-brew install promptops/promptops/promptops-cli
+pip3 install promptops
 ```
 
 # Usage
 
 ## um
 
 ```shell
 um <question>
 ```
 
+```shell
+um workflow <multi-stepped-prompt>
+```
+
 ## local runner
 
 ```shell
 promptops runner
 ```
 
 # Examples
@@ -75,15 +87,15 @@
 <img src="https://github.com/promptops/cli/raw/main/media/clarify.png" />
 
 # Development setup
 
 create virtual env
 
 ```shell
-python3 -m venv ./venv
+python3.10 -m venv ./venv
 . ./venv/bin/activate
 ```
 
 install dependencies
 
 ```shell
 pip install -r requirements.txt
```

### Comparing `promptops-0.1.5/promptops.egg-info/SOURCES.txt` & `promptops-0.1.6/promptops.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 local_runner/tokens/__init__.py
 local_runner/tokens/issuer.py
 promptops/__init__.py
 promptops/corrections.py
 promptops/feedback.py
 promptops/history.py
 promptops/main.py
-promptops/nux.py
 promptops/query.py
 promptops/settings.py
 promptops/settings_store.py
 promptops/similarity.py
 promptops/trace.py
 promptops/ui.py
 promptops/user.py
@@ -40,34 +39,44 @@
 promptops/version_check.py
 promptops.egg-info/PKG-INFO
 promptops.egg-info/SOURCES.txt
 promptops.egg-info/dependency_links.txt
 promptops.egg-info/entry_points.txt
 promptops.egg-info/requires.txt
 promptops.egg-info/top_level.txt
+promptops/gitaware/__init__.py
+promptops/gitaware/project.py
+promptops/index/__init__.py
+promptops/index/content.py
+promptops/index/entry_point.py
+promptops/index/index_store.py
 promptops/loading/__init__.py
 promptops/loading/base.py
 promptops/loading/context.py
 promptops/loading/pong.py
 promptops/loading/progress.py
 promptops/loading/promptops.py
 promptops/loading/simple.py
 promptops/query/__init__.py
 promptops/query/dtos.py
 promptops/query/explanation.py
+promptops/query/git_repo.py
 promptops/query/messages.py
 promptops/query/query.py
 promptops/recipes/__init__.py
 promptops/recipes/creation.py
+promptops/recipes/terraform.py
 promptops/scrub_secrets/__init__.py
 promptops/scrub_secrets/scrub.py
 promptops/secrets/__init__.py
 promptops/secrets/scrub.py
 promptops/shells/__init__.py
 promptops/shells/base.py
 promptops/shells/bash.py
 promptops/shells/common.py
 promptops/shells/fish.py
 promptops/shells/zsh.py
 promptops/ui/__init__.py
+promptops/ui/input.py
 promptops/ui/prompts.py
-promptops/ui/selections.py
+promptops/ui/selections.py
+promptops/ui/vim.py
```

### Comparing `promptops-0.1.5/setup.py` & `promptops-0.1.6/setup.py`

 * *Files identical despite different names*

