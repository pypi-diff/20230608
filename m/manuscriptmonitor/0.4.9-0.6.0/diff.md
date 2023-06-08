# Comparing `tmp/ManuscriptMonitor-0.4.9.tar.gz` & `tmp/manuscriptmonitor-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ManuscriptMonitor-0.4.9.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ManuscriptMonitor-0.4.9.tar` & `manuscriptmonitor-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2022-02-28 23:37:46.940250 ManuscriptMonitor-0.4.9/manuscriptmonitor/__init__.py
--rw-r--r--   0        0        0       96 2022-02-28 23:37:46.941200 ManuscriptMonitor-0.4.9/manuscriptmonitor/__main__.py
--rw-r--r--   0        0        0     4402 2023-04-12 16:56:01.048335 ManuscriptMonitor-0.4.9/manuscriptmonitor/ManuscriptMonitor.py
--rw-r--r--   0        0        0      540 2023-04-12 16:55:35.658818 ManuscriptMonitor-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      804 2023-04-12 16:56:06.161397 ManuscriptMonitor-0.4.9/setup.py
--rw-r--r--   0        0        0      613 2023-04-12 16:56:06.162485 ManuscriptMonitor-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/manuscriptmonitor/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/manuscriptmonitor/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/manuscriptmonitor/__main__.py
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/manuscriptmonitor/manuscriptmonitor.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 manuscriptmonitor-0.6.0/PKG-INFO
```

