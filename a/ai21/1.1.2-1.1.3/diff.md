# Comparing `tmp/ai21-1.1.2.tar.gz` & `tmp/ai21-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.1.2.tar", last modified: Thu Jun  8 08:06:20 2023, max compression
+gzip compressed data, was "ai21-1.1.3.tar", last modified: Thu Jun  8 14:35:03 2023, max compression
```

## Comparing `ai21-1.1.2.tar` & `ai21-1.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.737883 ai21-1.1.2/
--rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.2/LICENSE
--rw-r--r--   0 etang      (501) staff       (20)     3930 2023-06-08 08:06:20.737962 ai21-1.1.2/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     2996 2023-06-08 08:05:25.000000 ai21-1.1.2/README.md
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.732529 ai21-1.1.2/ai21/
--rw-r--r--   0 etang      (501) staff       (20)     2209 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/AWS_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      885 2023-06-07 13:39:06.000000 ai21-1.1.2/ai21/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/ai21_object.py
--rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/ai21_studio_client.py
--rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/api_resources.py
--rw-r--r--   0 etang      (501) staff       (20)     1923 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/bedrock_client.py
--rw-r--r--   0 etang      (501) staff       (20)      246 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/constants.py
--rw-r--r--   0 etang      (501) staff       (20)     3084 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/errors.py
--rw-r--r--   0 etang      (501) staff       (20)     4033 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/http_client.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.736054 ai21-1.1.2/ai21/modules/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/completion.py
--rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/custom_model.py
--rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/dataset.py
--rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/destination.py
--rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/experimental.py
--rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/gec.py
--rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/improvements.py
--rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/paraphrase.py
--rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/question_answering.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.737724 ai21-1.1.2/ai21/modules/resources/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/segmentation.py
--rw-r--r--   0 etang      (501) staff       (20)     1164 2023-06-08 08:05:25.000000 ai21-1.1.2/ai21/modules/summarize.py
--rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/tokenization.py
--rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/utils.py
--rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-08 08:05:25.000000 ai21-1.1.2/ai21/version.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.733444 ai21-1.1.2/ai21.egg-info/
--rw-r--r--   0 etang      (501) staff       (20)     3930 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/requires.txt
--rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-08 08:06:20.738197 ai21-1.1.2/setup.cfg
--rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-07 10:54:53.000000 ai21-1.1.2/setup.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.828075 ai21-1.1.3/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1065 2023-03-25 06:53:34.000000 ai21-1.1.3/LICENSE
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4095 2023-06-08 14:35:03.828182 ai21-1.1.3/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3161 2023-06-08 14:21:53.000000 ai21-1.1.3/README.md
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.823254 ai21-1.1.3/ai21/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2209 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/AWS_utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      885 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/ai21_object.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2055 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/ai21_studio_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/api_resources.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1923 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/bedrock_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      246 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/constants.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3084 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/errors.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4034 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/http_client.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.826472 ai21-1.1.3/ai21/modules/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2009 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/completion.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/custom_model.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/dataset.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      445 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/destination.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1801 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/experimental.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      986 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/gec.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      925 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/improvements.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1000 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/paraphrase.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1104 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/question_answering.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.827901 ai21-1.1.3/ai21/modules/resources/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1605 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2059 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      915 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/segmentation.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1164 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/summarize.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      693 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/modules/tokenization.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3038 2023-06-08 14:30:41.000000 ai21-1.1.3/ai21/utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-06-08 14:34:42.000000 ai21-1.1.3/ai21/version.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-06-08 14:35:03.824090 ai21-1.1.3/ai21.egg-info/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     4095 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1070 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       40 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/requires.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-06-08 14:35:03.000000 ai21-1.1.3/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      155 2023-06-08 14:35:03.828492 ai21-1.1.3/setup.cfg
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      600 2023-06-08 14:21:53.000000 ai21-1.1.3/setup.py
```

### Comparing `ai21-1.1.2/LICENSE` & `ai21-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/PKG-INFO` & `ai21-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.2
+Version: 1.1.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
         
         ## API Keys
-        API key can be set globally, using ai21.api_key, or alternatively - be passed to any function call 
+        API key can be set globally, using ai21.api_key, or alternatively - be passed to any function call
         as a named argument. For example - ai21.Dataset.get(api_key=api_key)
         
         ## Installation:
         `pip install -U ai21`
         
         ## Client customization
-        The ai21 namespace has parameters that one can set globally, and they will 
-        be used by all the following client calls. 
-        One can also pass each of these parameters as a named argument. 
-        If a parameter is overridden globally, and also passed as a named argument - 
+        The ai21 namespace has parameters that one can set globally, and they will
+        be used by all the following client calls.
+        One can also pass each of these parameters as a named argument.
+        If a parameter is overridden globally, and also passed as a named argument -
         the passed named argument will be used with the following client calls.
         The supported parameters are described below:
         ```text
         * api_key (str) - the key to be used for the Authorization header
         * organization (str) - this information is sent as part of the user-agent
         * application (str) - this information is sent as part of the user-agent
         * api_version (str) - the api version. (i.e. v1 / v2). Default=v1
         * api_host (str) - the api host. Default=https://api.ai21.com
         * timeout_sec (int) - the number of seconds the client must wait before cutting the connection. Default=30
         * num_retries (int) - the number of attempts to retry a failure response. Default=0 (no retries)
         * log_level (str) - debug / info / error (Default=error)
         ```
         ### Retry on Failure
         By default, there is no retry on failures. If setting the num_retries parameter
-        to an integer greater than 0, then all the following client calls will retry up to the specified 
+        to an integer greater than 0, then all the following client calls will retry up to the specified
         number of times on the following http error codes: 429, 500, 503.
         
         ### Documentation & resources
         https://docs.ai21.com/
         
         ## Usage
         
         ### Studio API
-        In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
+        In the following example, an AI21 API client is used with an API key and a timeout parameter set globally.
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
         ```python
         import ai21
         
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
-        response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
+        response = ai21.Completion.execute(model="j2-ultra", prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.", maxTokens=200)
         print(response)
         ```
         
         ### AWS Client
         This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
         To activate this option, make sure to install with the extra AWS dependencies:
```

### Comparing `ai21-1.1.2/README.md` & `ai21-1.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # AI21 Studio Client
 Python client for the AI21 Studio API
 
 ## API Keys
-API key can be set globally, using ai21.api_key, or alternatively - be passed to any function call 
+API key can be set globally, using ai21.api_key, or alternatively - be passed to any function call
 as a named argument. For example - ai21.Dataset.get(api_key=api_key)
 
 ## Installation:
 `pip install -U ai21`
 
 ## Client customization
-The ai21 namespace has parameters that one can set globally, and they will 
-be used by all the following client calls. 
-One can also pass each of these parameters as a named argument. 
-If a parameter is overridden globally, and also passed as a named argument - 
+The ai21 namespace has parameters that one can set globally, and they will
+be used by all the following client calls.
+One can also pass each of these parameters as a named argument.
+If a parameter is overridden globally, and also passed as a named argument -
 the passed named argument will be used with the following client calls.
 The supported parameters are described below:
 ```text
 * api_key (str) - the key to be used for the Authorization header
 * organization (str) - this information is sent as part of the user-agent
 * application (str) - this information is sent as part of the user-agent
 * api_version (str) - the api version. (i.e. v1 / v2). Default=v1
 * api_host (str) - the api host. Default=https://api.ai21.com
 * timeout_sec (int) - the number of seconds the client must wait before cutting the connection. Default=30
 * num_retries (int) - the number of attempts to retry a failure response. Default=0 (no retries)
 * log_level (str) - debug / info / error (Default=error)
 ```
 ### Retry on Failure
 By default, there is no retry on failures. If setting the num_retries parameter
-to an integer greater than 0, then all the following client calls will retry up to the specified 
+to an integer greater than 0, then all the following client calls will retry up to the specified
 number of times on the following http error codes: 429, 500, 503.
 
 ### Documentation & resources
 https://docs.ai21.com/
 
 ## Usage
 
 ### Studio API
-In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
+In the following example, an AI21 API client is used with an API key and a timeout parameter set globally.
 This example uses a simple completion call with only prompt and maxTokens arguments supplied
 (all other completion settings are set to their defaults):
 ```python
 import ai21
 
 ai21.api_key = 'my_api_key'
 ai21.timeout_sec = 20
-response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
+response = ai21.Completion.execute(model="j2-ultra", prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.", maxTokens=200)
 print(response)
 ```
 
 ### AWS Client
 This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
 To activate this option, make sure to install with the extra AWS dependencies:
```

### Comparing `ai21-1.1.2/ai21/AWS_utils.py` & `ai21-1.1.3/ai21/AWS_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/__init__.py` & `ai21-1.1.3/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/ai21_object.py` & `ai21-1.1.3/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/ai21_studio_client.py` & `ai21-1.1.3/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/bedrock_client.py` & `ai21-1.1.3/ai21/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/errors.py` & `ai21-1.1.3/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/http_client.py` & `ai21-1.1.3/ai21/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 from requests.adapters import HTTPAdapter, Retry, RetryError
 
 from ai21.errors import BadRequest, Unauthorized, UnprocessableEntity, TooManyRequests, ServerError, ServiceUnavailable, \
     APIError
 from ai21.utils import log_info, log_error
 
-DEFAULT_TIMEOUT_SEC = 30
+DEFAULT_TIMEOUT_SEC = 300
 DEFAULT_NUM_RETRIES = 0
 RETRY_BACK_OFF_FACTOR = 0.5
 TIME_BETWEEN_RETRIES = 1000
 RETRY_ERROR_CODES = (429, 500, 503)
 RETRY_METHOD_WHITELIST = ['GET', 'POST', 'PUT']
```

### Comparing `ai21-1.1.2/ai21/modules/completion.py` & `ai21-1.1.3/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/custom_model.py` & `ai21-1.1.3/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/dataset.py` & `ai21-1.1.3/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/experimental.py` & `ai21-1.1.3/ai21/modules/experimental.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/gec.py` & `ai21-1.1.3/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/improvements.py` & `ai21-1.1.3/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/paraphrase.py` & `ai21-1.1.3/ai21/modules/paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/question_answering.py` & `ai21-1.1.3/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/resources/ai21_module.py` & `ai21-1.1.3/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/resources/execution_utils.py` & `ai21-1.1.3/ai21/modules/resources/execution_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/resources/nlp_task.py` & `ai21-1.1.3/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/segmentation.py` & `ai21-1.1.3/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/summarize.py` & `ai21-1.1.3/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/modules/tokenization.py` & `ai21-1.1.3/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21/utils.py` & `ai21-1.1.3/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/ai21.egg-info/PKG-INFO` & `ai21-1.1.3/ai21.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.2
+Version: 1.1.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
         
         ## API Keys
-        API key can be set globally, using ai21.api_key, or alternatively - be passed to any function call 
+        API key can be set globally, using ai21.api_key, or alternatively - be passed to any function call
         as a named argument. For example - ai21.Dataset.get(api_key=api_key)
         
         ## Installation:
         `pip install -U ai21`
         
         ## Client customization
-        The ai21 namespace has parameters that one can set globally, and they will 
-        be used by all the following client calls. 
-        One can also pass each of these parameters as a named argument. 
-        If a parameter is overridden globally, and also passed as a named argument - 
+        The ai21 namespace has parameters that one can set globally, and they will
+        be used by all the following client calls.
+        One can also pass each of these parameters as a named argument.
+        If a parameter is overridden globally, and also passed as a named argument -
         the passed named argument will be used with the following client calls.
         The supported parameters are described below:
         ```text
         * api_key (str) - the key to be used for the Authorization header
         * organization (str) - this information is sent as part of the user-agent
         * application (str) - this information is sent as part of the user-agent
         * api_version (str) - the api version. (i.e. v1 / v2). Default=v1
         * api_host (str) - the api host. Default=https://api.ai21.com
         * timeout_sec (int) - the number of seconds the client must wait before cutting the connection. Default=30
         * num_retries (int) - the number of attempts to retry a failure response. Default=0 (no retries)
         * log_level (str) - debug / info / error (Default=error)
         ```
         ### Retry on Failure
         By default, there is no retry on failures. If setting the num_retries parameter
-        to an integer greater than 0, then all the following client calls will retry up to the specified 
+        to an integer greater than 0, then all the following client calls will retry up to the specified
         number of times on the following http error codes: 429, 500, 503.
         
         ### Documentation & resources
         https://docs.ai21.com/
         
         ## Usage
         
         ### Studio API
-        In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
+        In the following example, an AI21 API client is used with an API key and a timeout parameter set globally.
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
         ```python
         import ai21
         
         ai21.api_key = 'my_api_key'
         ai21.timeout_sec = 20
-        response = ai21.Completion.execute(model="j1-large", prompt="hello world", maxTokens=20)
+        response = ai21.Completion.execute(model="j2-ultra", prompt="Write a news release in the voice of a global banking conglomerate announcing an unprecedented building campaign to expand and rebuild their corporate headquarters in Alpha Centauri.", maxTokens=200)
         print(response)
         ```
         
         ### AWS Client
         This python SDK can also be used to invoke Jurassic models as a SageMaker (SM) endpoint or as an AWS Bedrock API.
         To activate this option, make sure to install with the extra AWS dependencies:
```

### Comparing `ai21-1.1.2/ai21.egg-info/SOURCES.txt` & `ai21-1.1.3/ai21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai21-1.1.2/setup.py` & `ai21-1.1.3/setup.py`

 * *Files identical despite different names*

