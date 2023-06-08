# Comparing `tmp/mona-openai-0.0.5.tar.gz` & `tmp/mona-openai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.5.tar", last modified: Wed May 31 08:24:09 2023, max compression
+gzip compressed data, was "mona-openai-0.0.6.tar", last modified: Mon Jun  5 07:44:12 2023, max compression
```

## Comparing `mona-openai-0.0.5.tar` & `mona-openai-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.728045 mona-openai-0.0.5/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.5/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-31 08:24:09.727876 mona-openai-0.0.5/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     9162 2023-05-25 05:50:33.000000 mona-openai-0.0.5/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.724794 mona-openai-0.0.5/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.5/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.725672 mona-openai-0.0.5/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3121 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.726194 mona-openai-0.0.5/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     7675 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     5091 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/endpoint_wrapping.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/wrapping_getter.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.5/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.5/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    16315 2023-05-31 08:23:40.000000 mona-openai-0.0.5/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.727177 mona-openai-0.0.5/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-05-31 01:28:56.000000 mona-openai-0.0.5/mona_openai/util/async_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.5/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/oop_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/openai_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/stream_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/tokens_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.5/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.725322 mona-openai-0.0.5/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-31 08:24:02.000000 mona-openai-0.0.5/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.5/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-31 08:24:09.728080 mona-openai-0.0.5/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.727683 mona-openai-0.0.5/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.5/tests/test_chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    20103 2023-05-31 08:23:40.000000 mona-openai-0.0.5/tests/test_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.5/tests/test_privacy_analyzer.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      852 2023-05-25 05:50:33.000000 mona-openai-0.0.5/tests/test_textual_analyzer.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.007846 mona-openai-0.0.6/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.6/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-06-05 07:44:12.007618 mona-openai-0.0.6/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9162 2023-05-25 05:50:33.000000 mona-openai-0.0.6/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.003346 mona-openai-0.0.6/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.6/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.004917 mona-openai-0.0.6/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3121 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.005513 mona-openai-0.0.6/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7675 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5091 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.6/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.6/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17096 2023-06-05 07:07:51.000000 mona-openai-0.0.6/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.006605 mona-openai-0.0.6/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-06-01 06:55:43.000000 mona-openai-0.0.6/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.6/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.6/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.6/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.004350 mona-openai-0.0.6/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-06-05 07:44:11.000000 mona-openai-0.0.6/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-06-05 07:44:12.000000 mona-openai-0.0.6/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-06-05 07:44:11.000000 mona-openai-0.0.6/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-06-05 07:44:11.000000 mona-openai-0.0.6/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-06-05 07:44:11.000000 mona-openai-0.0.6/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-06-05 07:44:02.000000 mona-openai-0.0.6/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.6/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-06-05 07:44:12.007886 mona-openai-0.0.6/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-06-05 07:44:12.007380 mona-openai-0.0.6/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.6/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    20103 2023-06-01 06:55:43.000000 mona-openai-0.0.6/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.6/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      852 2023-05-25 05:50:33.000000 mona-openai-0.0.6/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.0.5/LICENSE` & `mona-openai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/PKG-INFO` & `mona-openai-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mona-openai-0.0.5/README.md` & `mona-openai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/analysis/privacy.py` & `mona-openai-0.0.6/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/analysis/textual.py` & `mona-openai-0.0.6/mona_openai/analysis/textual.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/endpoints/chat_completion.py` & `mona-openai-0.0.6/mona_openai/endpoints/chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/endpoints/completion.py` & `mona-openai-0.0.6/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/endpoints/endpoint_wrapping.py` & `mona-openai-0.0.6/mona_openai/endpoints/endpoint_wrapping.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/endpoints/wrapping_getter.py` & `mona-openai-0.0.6/mona_openai/endpoints/wrapping_getter.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/mona_client.py` & `mona-openai-0.0.6/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/mona_openai.py` & `mona-openai-0.0.6/mona_openai/mona_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import logging
 from copy import deepcopy
 from types import MappingProxyType
 
 from mona_sdk import MonaSingleMessage
 
 from .endpoints.wrapping_getter import get_endpoint_wrapping
 from .mona_client import get_mona_clients
@@ -68,14 +69,32 @@
         message=message,
         contextClass=context_class,
         contextId=context_id,
         exportTimestamp=export_timestamp,
     )
 
 
+def _init_mona_class(client, context_class_name, openai_endpoint_name):
+    response = client.create_openai_context_class(
+        context_class_name, openai_endpoint_name
+    )
+    error_message = response.get("error_message")
+    if error_message:
+        logging.warning(
+            f"Problem initializing Mona context class '{context_class_name}':"
+            f" {error_message}"
+        )
+    else:
+        logging.info(
+            f"Made sure Mona context class '{context_class_name}' "
+            "is initialised"
+        )
+    return response
+
+
 # TODO(itai): Consider creating some sturct (as NamedTuple or dataclass) for
 #   the specs param.
 
 
 def monitor(
     openai_class,
     mona_creds,
@@ -139,14 +158,16 @@
 
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
     base_class = get_endpoint_wrapping(
         openai_class.__name__, specs
     ).wrap_class(openai_class)
 
+    _init_mona_class(client, context_class, openai_class.__name__)
+
     # TODO(itai): Add call to Mona servers to init the context class if it
     #   isn't inited yet once we have the relevant endpoint for this.
 
     class MonitoredOpenAI(base_class):
         """
         A mona-monitored version of an openai API class.
         """
@@ -330,14 +351,15 @@
             """
             return (client, async_client)
 
     return type(base_class.__name__, (MonitoredOpenAI,), {})
 
 
 def get_rest_monitor(
+    # TODO(itai): Consider understanding endpoint name from complete url.
     openai_endpoint_name,
     mona_creds,
     context_class,
     specs=EMPTY_DICT,
     mona_clients_getter=get_mona_clients,
 ):
     """
@@ -346,14 +368,16 @@
     endpoints directly). This isn't a wrapper for any http requesting
     library and doesn't call the OpenAI API for you - it's just an easy
     logging client to log requests, responses and exceptions.
     """
 
     client, async_client = mona_clients_getter(mona_creds)
 
+    _init_mona_class(client, context_class, openai_endpoint_name)
+
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
     wrapping_logic = get_endpoint_wrapping(openai_endpoint_name, specs)
 
     class RestClient:
         """
         This will be the returned Mona logging class. We follow
```

### Comparing `mona-openai-0.0.5/mona_openai/util/async_util.py` & `mona-openai-0.0.6/mona_openai/util/async_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/util/func_util.py` & `mona-openai-0.0.6/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/util/oop_util.py` & `mona-openai-0.0.6/mona_openai/util/oop_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/util/stream_util.py` & `mona-openai-0.0.6/mona_openai/util/stream_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/util/tokens_util.py` & `mona-openai-0.0.6/mona_openai/util/tokens_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai/util/validation_util.py` & `mona-openai-0.0.6/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.0.6/mona_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mona-openai-0.0.5/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.0.6/mona_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/pyproject.toml` & `mona-openai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mona-openai-0.0.5/tests/test_chat_completion.py` & `mona-openai-0.0.6/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/tests/test_completion.py` & `mona-openai-0.0.6/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/tests/test_privacy_analyzer.py` & `mona-openai-0.0.6/tests/test_privacy_analyzer.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.5/tests/test_textual_analyzer.py` & `mona-openai-0.0.6/tests/test_textual_analyzer.py`

 * *Files identical despite different names*

