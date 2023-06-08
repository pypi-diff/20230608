# Comparing `tmp/bettershot-0.1.2.tar.gz` & `tmp/bettershot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.2.tar", max compression
+gzip compressed data, was "bettershot-0.1.3.tar", max compression
```

## Comparing `bettershot-0.1.2.tar` & `bettershot-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.2/README.md
--rw-r--r--   0        0        0      481 2023-06-08 02:01:23.349820 bettershot-0.1.2/bettershot/__init__.py
--rw-r--r--   0        0        0      276 2023-06-08 02:01:15.121132 bettershot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 bettershot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.3/README.md
+-rw-r--r--   0        0        0     1605 2023-06-08 02:25:30.332871 bettershot-0.1.3/bettershot/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-08 02:25:44.819804 bettershot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 bettershot-0.1.3/PKG-INFO
```

