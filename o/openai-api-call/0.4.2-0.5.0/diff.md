# Comparing `tmp/openai_api_call-0.4.2.tar.gz` & `tmp/openai_api_call-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.4.2.tar", last modified: Tue Jun  6 15:13:35 2023, max compression
+gzip compressed data, was "openai_api_call-0.5.0.tar", last modified: Thu Jun  8 08:07:45 2023, max compression
```

## Comparing `openai_api_call-0.4.2.tar` & `openai_api_call-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:13:35.450256 openai_api_call-0.4.2/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 15:13:35.000000 openai_api_call-0.4.2/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:13:35.454256 openai_api_call-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-06 15:13:24.000000 openai_api_call-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:07:45.020647 openai_api_call-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-08 08:07:45.020647 openai_api_call-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:07:45.020647 openai_api_call-0.5.0/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:07:45.020647 openai_api_call-0.5.0/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 08:07:44.000000 openai_api_call-0.5.0/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:07:45.020647 openai_api_call-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 08:07:35.000000 openai_api_call-0.5.0/setup.py
```

### Comparing `openai_api_call-0.4.2/LICENSE` & `openai_api_call-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.2/PKG-INFO` & `openai_api_call-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.4.2
+Version: 0.5.0
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -185,23 +185,44 @@
                               [{'role': 'user', 'content': 'hello!'}, 
                                {'role': 'assistant', 'content': '你好, how can I assist you today?'}]]
         # load the last message only
         chat_msgs = load_chats(checkpoint, last_message_only=True)
         assert chat_msgs == ["", "hello!", "你好, how can I assist you today?"]
         ```
         
+        In general, one can create a function `msg2chat` and use `process_chats` to process the data:
+        
+        ```python
+        def msg2chat(msg):
+            chat = Chat(api_key=api_key)
+            chat.system("You are a helpful translator for numbers.")
+            chat.user(f"Please translate the digit to Roman numerals: {msg}")
+            chat.getresponse()
+        
+        checkpath = "tmp.log"
+        # first part of the data
+        msgs = ["1", "2", "3"]
+        chats = process_chats(msgs, msg2chat, checkpath, clearfile=True)
+        assert len(chats) == 3
+        assert all([len(chat) == 3 for chat in chats])
+        # continue the process
+        msgs = msgs + ["4", "5", "6"]
+        continue_chats = process_chats(msgs, msg2chat, checkpath)
+        ```
+        
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
         - Since version `0.3.0`, you can use different API Key to send requests.
         - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
+        - Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
 Keywords: openai_api_call
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `openai_api_call-0.4.2/README.md` & `openai_api_call-0.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -177,16 +177,37 @@
                       [{'role': 'user', 'content': 'hello!'}, 
                        {'role': 'assistant', 'content': '你好, how can I assist you today?'}]]
 # load the last message only
 chat_msgs = load_chats(checkpoint, last_message_only=True)
 assert chat_msgs == ["", "hello!", "你好, how can I assist you today?"]
 ```
 
+In general, one can create a function `msg2chat` and use `process_chats` to process the data:
+
+```python
+def msg2chat(msg):
+    chat = Chat(api_key=api_key)
+    chat.system("You are a helpful translator for numbers.")
+    chat.user(f"Please translate the digit to Roman numerals: {msg}")
+    chat.getresponse()
+
+checkpath = "tmp.log"
+# first part of the data
+msgs = ["1", "2", "3"]
+chats = process_chats(msgs, msg2chat, checkpath, clearfile=True)
+assert len(chats) == 3
+assert all([len(chat) == 3 for chat in chats])
+# continue the process
+msgs = msgs + ["4", "5", "6"]
+continue_chats = process_chats(msgs, msg2chat, checkpath)
+```
+
 ## License
 
 This package is licensed under the MIT license. See the LICENSE file for more details.
 
 ## update log
 
 - Since version `0.2.0`, `Chat` type is used to handle data
 - Since version `0.3.0`, you can use different API Key to send requests.
-- Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
+- Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
+- Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
```

### Comparing `openai_api_call-0.4.2/openai_api_call/__init__.py` & `openai_api_call-0.5.0/openai_api_call/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.4.2'
+__version__ = '0.5.0'
 
-import os
-from .chattool import Chat, Resp, chat_completion, usage_status, load_chats
+import os, requests
+from .chattool import Chat, Resp, chat_completion, usage_status
+from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
-import requests
 from . import request
 
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
     api_key = os.environ.get('OPENAI_API_KEY')
     # skip checking the validity of the API key
```

### Comparing `openai_api_call-0.4.2/openai_api_call/chattool.py` & `openai_api_call-0.5.0/openai_api_call/chattool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # The object that stores the chat log
 
-from typing import List, Dict, Union
+from typing import List, Dict, Union, Callable
 import openai_api_call
 from .response import Resp
 from .request import chat_completion, usage_status
 import signal, time, random
 import datetime
 import json
 import warnings
@@ -33,16 +33,15 @@
                 self._chat_log = [{"role": "user", "content": msg}]
             else:
                 self._chat_log = openai_api_call.default_prompt(msg)
         elif isinstance(msg, list):
             self._chat_log = msg.copy() # avoid changing the original list
         else:
             raise ValueError("msg should be a list of dict, a string or None")
-        if api_key is None:
-            self._api_key = openai_api_call.api_key
+        self._api_key = openai_api_call.api_key if api_key is None else api_key
     
     @property
     def api_key(self):
         """Get API key"""
         return self._api_key
     
     @api_key.setter
@@ -228,60 +227,8 @@
     def __eq__(self, chat: object) -> bool:
         if isinstance(chat, Chat):
             return self._chat_log == chat._chat_log
         return False
 
     def __getitem__(self, index):
         """Get the message at index"""
-        return self._chat_log[index]['content']
-
-def load_chats( checkpoint:str
-              , sep='\n'
-              , last_message_only:bool=False
-              , chat_log_only:bool=False
-              , chat_size:int=0):
-    """Load chats from a checkpoint file
-    
-    Args:
-        checkpoint (str): path to the checkpoint file
-        sep (str, optional): separator of chats. Defaults to '\n'.
-        last_message_only (bool, optional): whether to return the last message of each chat. Defaults to False.
-        chat_log_only (bool, optional): whether to return the chat log only. Defaults to False.
-        chat_size (int, optional): number of chats. Defaults to 0.
-
-    Returns:
-        list: chats
-    """
-    # load chats from the checkpoint file
-    with open(checkpoint, 'r', encoding='utf-8') as f:
-        txts = f.read().strip().split(sep)
-    chats = [json.loads(txt) for txt in txts]
-    # no chats
-    if not len(chats): return []
-    # number of chats
-    if chat_size == 0:
-        chat_size = len(chats)
-    # chats with chatid
-    if 'chatid' in chats[0]:
-        chatlogs = [None] * chat_size
-        for chat in chats:
-            idx = chat['chatid']
-            if idx >= chat_size:
-                warnings.warn(f"chatid {idx} is out of the default chat size {chat_size}")
-                chatlogs.extend([None] * (idx - chat_size + 1))
-                chat_size = idx + 1
-            chatlogs[idx] = chat['chatlog']
-    else:
-        # chats without chatid
-        chatlogs = chats
-    # last message of chats only
-    if last_message_only:
-        msgs = [None] * len(chatlogs)
-        for i, chat in enumerate(chatlogs):
-            if chat is None: continue
-            msgs[i] = chat[-1]['content'] if len(chat) else ""
-        return msgs
-    # chat log only
-    if chat_log_only:
-        return chatlogs
-    # return Chat class
-    return [Chat(chatlog) if chatlog is not None else None for chatlog in chatlogs]
+        return self._chat_log[index]['content']
```

### Comparing `openai_api_call-0.4.2/openai_api_call/proxy.py` & `openai_api_call-0.5.0/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.2/openai_api_call/request.py` & `openai_api_call-0.5.0/openai_api_call/request.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.2/openai_api_call/response.py` & `openai_api_call-0.5.0/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.4.2/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.5.0/openai_api_call.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.4.2
+Version: 0.5.0
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -185,23 +185,44 @@
                               [{'role': 'user', 'content': 'hello!'}, 
                                {'role': 'assistant', 'content': '你好, how can I assist you today?'}]]
         # load the last message only
         chat_msgs = load_chats(checkpoint, last_message_only=True)
         assert chat_msgs == ["", "hello!", "你好, how can I assist you today?"]
         ```
         
+        In general, one can create a function `msg2chat` and use `process_chats` to process the data:
+        
+        ```python
+        def msg2chat(msg):
+            chat = Chat(api_key=api_key)
+            chat.system("You are a helpful translator for numbers.")
+            chat.user(f"Please translate the digit to Roman numerals: {msg}")
+            chat.getresponse()
+        
+        checkpath = "tmp.log"
+        # first part of the data
+        msgs = ["1", "2", "3"]
+        chats = process_chats(msgs, msg2chat, checkpath, clearfile=True)
+        assert len(chats) == 3
+        assert all([len(chat) == 3 for chat in chats])
+        # continue the process
+        msgs = msgs + ["4", "5", "6"]
+        continue_chats = process_chats(msgs, msg2chat, checkpath)
+        ```
+        
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
         - Since version `0.3.0`, you can use different API Key to send requests.
         - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
+        - Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
 Keywords: openai_api_call
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `openai_api_call-0.4.2/setup.py` & `openai_api_call-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.4.2'
+VERSION = '0.5.0'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

