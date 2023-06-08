# Comparing `tmp/ai21-1.1.1.tar.gz` & `tmp/ai21-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-1.1.1.tar", last modified: Wed Jun  7 14:19:30 2023, max compression
+gzip compressed data, was "ai21-1.1.2.tar", last modified: Thu Jun  8 08:06:20 2023, max compression
```

## Comparing `ai21-1.1.1.tar` & `ai21-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.906403 ai21-1.1.1/
--rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.1/LICENSE
--rw-r--r--   0 etang      (501) staff       (20)     3936 2023-06-07 14:19:30.906504 ai21-1.1.1/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     3002 2023-06-07 13:39:06.000000 ai21-1.1.1/README.md
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.900660 ai21-1.1.1/ai21/
--rw-r--r--   0 etang      (501) staff       (20)     2209 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/AWS_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      885 2023-06-07 13:39:06.000000 ai21-1.1.1/ai21/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/ai21_object.py
--rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/ai21_studio_client.py
--rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/api_resources.py
--rw-r--r--   0 etang      (501) staff       (20)     1923 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/bedrock_client.py
--rw-r--r--   0 etang      (501) staff       (20)      246 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/constants.py
--rw-r--r--   0 etang      (501) staff       (20)     3084 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/errors.py
--rw-r--r--   0 etang      (501) staff       (20)     4033 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/http_client.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.904543 ai21-1.1.1/ai21/modules/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/completion.py
--rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/custom_model.py
--rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/dataset.py
--rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/destination.py
--rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/experimental.py
--rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/gec.py
--rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/improvements.py
--rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/paraphrase.py
--rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/question_answering.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.906231 ai21-1.1.1/ai21/modules/resources/
--rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/__init__.py
--rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/resources/execution_utils.py
--rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.1/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/segmentation.py
--rw-r--r--   0 etang      (501) staff       (20)      910 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/summarize.py
--rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/modules/tokenization.py
--rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-07 10:54:53.000000 ai21-1.1.1/ai21/utils.py
--rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-07 14:18:08.000000 ai21-1.1.1/ai21/version.py
-drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-07 14:19:30.901693 ai21-1.1.1/ai21.egg-info/
--rw-r--r--   0 etang      (501) staff       (20)     3936 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/PKG-INFO
--rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/dependency_links.txt
--rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/requires.txt
--rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-07 14:19:30.000000 ai21-1.1.1/ai21.egg-info/top_level.txt
--rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-07 14:19:30.906770 ai21-1.1.1/setup.cfg
--rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-07 10:54:53.000000 ai21-1.1.1/setup.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.737883 ai21-1.1.2/
+-rw-r--r--   0 etang      (501) staff       (20)     1065 2023-05-22 10:53:48.000000 ai21-1.1.2/LICENSE
+-rw-r--r--   0 etang      (501) staff       (20)     3930 2023-06-08 08:06:20.737962 ai21-1.1.2/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     2996 2023-06-08 08:05:25.000000 ai21-1.1.2/README.md
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.732529 ai21-1.1.2/ai21/
+-rw-r--r--   0 etang      (501) staff       (20)     2209 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/AWS_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      885 2023-06-07 13:39:06.000000 ai21-1.1.2/ai21/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      971 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/ai21_object.py
+-rw-r--r--   0 etang      (501) staff       (20)     2055 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/ai21_studio_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      473 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/api_resources.py
+-rw-r--r--   0 etang      (501) staff       (20)     1923 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/bedrock_client.py
+-rw-r--r--   0 etang      (501) staff       (20)      246 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/constants.py
+-rw-r--r--   0 etang      (501) staff       (20)     3084 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/errors.py
+-rw-r--r--   0 etang      (501) staff       (20)     4033 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/http_client.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.736054 ai21-1.1.2/ai21/modules/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)     2009 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/completion.py
+-rw-r--r--   0 etang      (501) staff       (20)      856 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/custom_model.py
+-rw-r--r--   0 etang      (501) staff       (20)      646 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/dataset.py
+-rw-r--r--   0 etang      (501) staff       (20)      445 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/destination.py
+-rw-r--r--   0 etang      (501) staff       (20)     1801 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/experimental.py
+-rw-r--r--   0 etang      (501) staff       (20)      986 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/gec.py
+-rw-r--r--   0 etang      (501) staff       (20)      925 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/improvements.py
+-rw-r--r--   0 etang      (501) staff       (20)     1000 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/paraphrase.py
+-rw-r--r--   0 etang      (501) staff       (20)     1104 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/question_answering.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.737724 ai21-1.1.2/ai21/modules/resources/
+-rw-r--r--   0 etang      (501) staff       (20)        0 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/__init__.py
+-rw-r--r--   0 etang      (501) staff       (20)      585 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 etang      (501) staff       (20)      371 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     1605 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/resources/execution_utils.py
+-rw-r--r--   0 etang      (501) staff       (20)      352 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)     2059 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 etang      (501) staff       (20)      387 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      476 2023-05-22 10:53:48.000000 ai21-1.1.2/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 etang      (501) staff       (20)      915 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/segmentation.py
+-rw-r--r--   0 etang      (501) staff       (20)     1164 2023-06-08 08:05:25.000000 ai21-1.1.2/ai21/modules/summarize.py
+-rw-r--r--   0 etang      (501) staff       (20)      693 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/modules/tokenization.py
+-rw-r--r--   0 etang      (501) staff       (20)     3038 2023-06-07 10:54:53.000000 ai21-1.1.2/ai21/utils.py
+-rw-r--r--   0 etang      (501) staff       (20)       22 2023-06-08 08:05:25.000000 ai21-1.1.2/ai21/version.py
+drwxr-xr-x   0 etang      (501) staff       (20)        0 2023-06-08 08:06:20.733444 ai21-1.1.2/ai21.egg-info/
+-rw-r--r--   0 etang      (501) staff       (20)     3930 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 etang      (501) staff       (20)     1070 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 etang      (501) staff       (20)        1 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 etang      (501) staff       (20)       40 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/requires.txt
+-rw-r--r--   0 etang      (501) staff       (20)        5 2023-06-08 08:06:20.000000 ai21-1.1.2/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 etang      (501) staff       (20)      155 2023-06-08 08:06:20.738197 ai21-1.1.2/setup.cfg
+-rwxr-xr-x   0 etang      (501) staff       (20)      600 2023-06-07 10:54:53.000000 ai21-1.1.2/setup.py
```

### Comparing `ai21-1.1.1/LICENSE` & `ai21-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/PKG-INFO` & `ai21-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -35,15 +35,15 @@
         ```
         ### Retry on Failure
         By default, there is no retry on failures. If setting the num_retries parameter
         to an integer greater than 0, then all the following client calls will retry up to the specified 
         number of times on the following http error codes: 429, 500, 503.
         
         ### Documentation & resources
-        https://studio.ai21.com/docs
+        https://docs.ai21.com/
         
         ## Usage
         
         ### Studio API
         In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
```

### Comparing `ai21-1.1.1/README.md` & `ai21-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```
 ### Retry on Failure
 By default, there is no retry on failures. If setting the num_retries parameter
 to an integer greater than 0, then all the following client calls will retry up to the specified 
 number of times on the following http error codes: 429, 500, 503.
 
 ### Documentation & resources
-https://studio.ai21.com/docs
+https://docs.ai21.com/
 
 ## Usage
 
 ### Studio API
 In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
 This example uses a simple completion call with only prompt and maxTokens arguments supplied
 (all other completion settings are set to their defaults):
```

### Comparing `ai21-1.1.1/ai21/AWS_utils.py` & `ai21-1.1.2/ai21/AWS_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/__init__.py` & `ai21-1.1.2/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/ai21_object.py` & `ai21-1.1.2/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/ai21_studio_client.py` & `ai21-1.1.2/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/bedrock_client.py` & `ai21-1.1.2/ai21/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/errors.py` & `ai21-1.1.2/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/http_client.py` & `ai21-1.1.2/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/completion.py` & `ai21-1.1.2/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/custom_model.py` & `ai21-1.1.2/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/dataset.py` & `ai21-1.1.2/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/experimental.py` & `ai21-1.1.2/ai21/modules/experimental.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/gec.py` & `ai21-1.1.2/ai21/modules/gec.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/improvements.py` & `ai21-1.1.2/ai21/modules/improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/paraphrase.py` & `ai21-1.1.2/ai21/modules/paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/question_answering.py` & `ai21-1.1.2/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/resources/ai21_module.py` & `ai21-1.1.2/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/resources/execution_utils.py` & `ai21-1.1.2/ai21/modules/resources/execution_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/resources/nlp_task.py` & `ai21-1.1.2/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/segmentation.py` & `ai21-1.1.2/ai21/modules/segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/modules/summarize.py` & `ai21-1.1.2/ai21/modules/summarize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ai21.modules.resources.execution_utils import execute_studio_request
+from ai21.modules.destination import SageMakerDestination
+from ai21.modules.resources.execution_utils import execute_studio_request, execute_sm_request
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
 class Summarize(NLPTask):
     MODULE_NAME = 'summarize'
 
@@ -13,13 +14,16 @@
     @classmethod
     def _validate_params(cls, params):
         validate_mandatory_field(key='sourceType', call_name=cls.MODULE_NAME, params=params, validate_type=True,
                                  expected_type=str)
         validate_mandatory_field(key='source', call_name=cls.MODULE_NAME, params=params, validate_type=True,
                                  expected_type=str)
 
-
     @classmethod
     def _execute_studio_api(cls, params):
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
         return execute_studio_request(task_url=url, params=params)
+
+    @classmethod
+    def _execute_sm(cls, destination: SageMakerDestination, params):
+        return execute_sm_request(endpoint_name=destination.endpoint_name, params=params)
```

### Comparing `ai21-1.1.1/ai21/modules/tokenization.py` & `ai21-1.1.2/ai21/modules/tokenization.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21/utils.py` & `ai21-1.1.2/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/ai21.egg-info/PKG-INFO` & `ai21-1.1.2/ai21.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 1.1.1
+Version: 1.1.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: ai21 labs
 Author-email: support@ai21.com
 License: MIT
 Description: # AI21 Studio Client
         Python client for the AI21 Studio API
@@ -35,15 +35,15 @@
         ```
         ### Retry on Failure
         By default, there is no retry on failures. If setting the num_retries parameter
         to an integer greater than 0, then all the following client calls will retry up to the specified 
         number of times on the following http error codes: 429, 500, 503.
         
         ### Documentation & resources
-        https://studio.ai21.com/docs
+        https://docs.ai21.com/
         
         ## Usage
         
         ### Studio API
         In the following example, an AI21 API client is used with an API key and a timeout parameter set globally. 
         This example uses a simple completion call with only prompt and maxTokens arguments supplied
         (all other completion settings are set to their defaults):
```

### Comparing `ai21-1.1.1/ai21.egg-info/SOURCES.txt` & `ai21-1.1.2/ai21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai21-1.1.1/setup.py` & `ai21-1.1.2/setup.py`

 * *Files identical despite different names*

