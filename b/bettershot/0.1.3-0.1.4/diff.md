# Comparing `tmp/bettershot-0.1.3.tar.gz` & `tmp/bettershot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.3.tar", max compression
+gzip compressed data, was "bettershot-0.1.4.tar", max compression
```

## Comparing `bettershot-0.1.3.tar` & `bettershot-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.3/README.md
--rw-r--r--   0        0        0     1605 2023-06-08 02:25:30.332871 bettershot-0.1.3/bettershot/__init__.py
--rw-r--r--   0        0        0      301 2023-06-08 02:25:44.819804 bettershot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 bettershot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.4/README.md
+-rw-r--r--   0        0        0     1597 2023-06-08 02:29:40.938044 bettershot-0.1.4/bettershot/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-08 02:29:43.449984 bettershot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 bettershot-0.1.4/PKG-INFO
```

### Comparing `bettershot-0.1.3/bettershot/__init__.py` & `bettershot-0.1.4/bettershot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 import requests
 import json 
 from langchain.schema import (AIMessage, HumanMessage, SystemMessage)
 
 url = "https://bettershot-w6mm.zeet-berri.zeet.app/openai_listener"
 
 def log(messages, completion, openai_api_key): 
@@ -25,16 +25,16 @@
             # messages': [{'role': 'user', 'content': "Hey! how's it going?"}]
             raw_message = {"role": "system", "content": message.content}
         elif isinstance(message, HumanMessage):
             raw_message = {"role": "system", "content": message.content}
         elif isinstance(message, AIMessage):
             raw_message = {"role": "ai", "content": message.content}
         raw_messages.append(raw_message)
-    if isinstance(completion, SystemMessage):
-        raw_completion = {"choices":[{"message": {"content": completion.SystemMessage}}]}
+    if isinstance(completion, AIMessage):
+        raw_completion = {"choices":[{"message": {"content": completion.AIMessage}}]}
     payload = {
         "messages": raw_messages,
         "completion": raw_completion,
         "openai_api_key": openai_api_key
     }
     headers = {
         "Content-Type": "application/json",
```

