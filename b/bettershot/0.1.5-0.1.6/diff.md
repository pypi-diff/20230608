# Comparing `tmp/bettershot-0.1.5.tar.gz` & `tmp/bettershot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.5.tar", max compression
+gzip compressed data, was "bettershot-0.1.6.tar", max compression
```

## Comparing `bettershot-0.1.5.tar` & `bettershot-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.5/README.md
--rw-r--r--   0        0        0     1595 2023-06-08 02:33:03.607433 bettershot-0.1.5/bettershot/__init__.py
--rw-r--r--   0        0        0      301 2023-06-08 02:33:07.704712 bettershot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 bettershot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.6/README.md
+-rw-r--r--   0        0        0     1595 2023-06-08 02:43:56.731715 bettershot-0.1.6/bettershot/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-08 02:43:54.711289 bettershot-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 bettershot-0.1.6/PKG-INFO
```

### Comparing `bettershot-0.1.5/bettershot/__init__.py` & `bettershot-0.1.6/bettershot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 import requests
 import json 
 from langchain.schema import (AIMessage, HumanMessage, SystemMessage)
 
 url = "https://bettershot-w6mm.zeet-berri.zeet.app/openai_listener"
 
 def log(messages, completion, openai_api_key):
```

