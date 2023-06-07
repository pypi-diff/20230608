# Comparing `tmp/alphawave-0.2.0.tar.gz` & `tmp/alphawave-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.0.tar", last modified: Wed Jun  7 00:29:06 2023, max compression
+gzip compressed data, was "alphawave-0.2.1.tar", last modified: Wed Jun  7 23:01:16 2023, max compression
```

## Comparing `alphawave-0.2.0.tar` & `alphawave-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.0/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 00:29:06.869218 alphawave-0.2.0/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.2.0/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-07 00:27:46.000000 alphawave-0.2.0/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-07 00:29:06.869218 alphawave-0.2.0/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.865218 alphawave-0.2.0/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10339 2023-06-06 23:37:53.000000 alphawave-0.2.0/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.2.0/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-06 01:24:12.000000 alphawave-0.2.0/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3211 2023-06-06 23:45:44.000000 alphawave-0.2.0/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.0/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6799 2023-06-04 16:26:58.000000 alphawave-0.2.0/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7626 2023-06-06 23:47:49.000000 alphawave-0.2.0/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-03 23:24:45.000000 alphawave-0.2.0/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      789 2023-06-07 00:22:15.000000 alphawave-0.2.0/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1505 2023-06-06 01:26:50.000000 alphawave-0.2.0/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.0/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1348 2023-06-06 23:25:38.000000 alphawave-0.2.0/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.0/src/alphawave/internalTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1251 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-07 00:29:06.000000 alphawave-0.2.0/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10353 2023-06-06 21:56:16.000000 alphawave-0.2.0/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1786 2023-06-06 02:43:58.000000 alphawave-0.2.0/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1625 2023-06-06 02:37:59.000000 alphawave-0.2.0/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1462 2023-06-06 21:01:10.000000 alphawave-0.2.0/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2168 2023-06-06 17:01:33.000000 alphawave-0.2.0/src/alphawave_agents/AskCommandTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1863 2023-06-06 22:06:08.000000 alphawave-0.2.0/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.0/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1076 2023-06-06 16:53:04.000000 alphawave-0.2.0/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1493 2023-06-06 21:06:39.000000 alphawave-0.2.0/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1956 2023-06-06 16:58:01.000000 alphawave-0.2.0/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3506 2023-06-06 21:03:30.000000 alphawave-0.2.0/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2453 2023-06-06 22:41:49.000000 alphawave-0.2.0/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.0/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.0/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-06 18:47:10.000000 alphawave-0.2.0/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 00:29:06.869218 alphawave-0.2.0/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14730 2023-06-06 23:10:09.000000 alphawave-0.2.0/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.0/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.1/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 23:01:16.295585 alphawave-0.2.1/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       57 2023-06-05 21:20:34.000000 alphawave-0.2.1/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      849 2023-06-07 23:01:03.000000 alphawave-0.2.1/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-07 23:01:16.295585 alphawave-0.2.1/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.291586 alphawave-0.2.1/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10346 2023-06-07 04:00:56.000000 alphawave-0.2.1/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1207 2023-06-04 00:33:26.000000 alphawave-0.2.1/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      711 2023-06-06 01:24:12.000000 alphawave-0.2.1/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3371 2023-06-07 22:30:30.000000 alphawave-0.2.1/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7887 2023-06-07 22:29:56.000000 alphawave-0.2.1/src/alphawave/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      545 2023-06-03 22:27:04.000000 alphawave-0.2.1/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7119 2023-06-07 22:32:28.000000 alphawave-0.2.1/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7669 2023-06-07 22:54:41.000000 alphawave-0.2.1/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2301 2023-06-07 21:51:05.000000 alphawave-0.2.1/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      789 2023-06-07 00:22:15.000000 alphawave-0.2.1/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1505 2023-06-06 01:26:50.000000 alphawave-0.2.1/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.1/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1348 2023-06-06 23:25:38.000000 alphawave-0.2.1/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.1/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.1/src/alphawave/jsonParser.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2745 2023-06-07 18:39:44.000000 alphawave-0.2.1/src/alphawave/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      670 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1316 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       86 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       27 2023-06-07 23:01:16.000000 alphawave-0.2.1/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    10353 2023-06-06 21:56:16.000000 alphawave-0.2.1/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1786 2023-06-06 02:43:58.000000 alphawave-0.2.1/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1625 2023-06-06 02:37:59.000000 alphawave-0.2.1/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1462 2023-06-06 21:01:10.000000 alphawave-0.2.1/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.1/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.1/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.1/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.1/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1956 2023-06-06 16:58:01.000000 alphawave-0.2.1/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3506 2023-06-07 02:19:55.000000 alphawave-0.2.1/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2453 2023-06-06 22:41:49.000000 alphawave-0.2.1/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.1/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.1/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1686 2023-06-06 18:47:10.000000 alphawave-0.2.1/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-07 23:01:16.295585 alphawave-0.2.1/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.1/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14653 2023-06-07 04:29:45.000000 alphawave-0.2.1/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.1/tests/testSchema.py
```

### Comparing `alphawave-0.2.0/LICENSE` & `alphawave-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/PKG-INFO` & `alphawave-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.0
+Version: 0.2.1
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.0/pyproject.toml` & `alphawave-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.2.0/src/alphawave/AlphaWave.py` & `alphawave-0.2.1/src/alphawave/AlphaWave.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 from alphawave.alphawaveTypes import  PromptCompletionClient, PromptCompletionOptions, PromptResponse,Validation, PromptResponseValidator 
 from alphawave.DefaultResponseValidator import DefaultResponseValidator
 from alphawave.MemoryFork import  MemoryFork
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse, Validation, PromptResponseValidator
 from alphawave.Colorize import Colorize
 import traceback
 
+"""
 @dataclass
 class AlphaWaveOptions:
     def __init__(self, client: PromptCompletionClient, prompt: PromptSection, prompt_options: PromptCompletionOptions, functions: Optional[PromptFunctions] = None, history_variable: Optional[str] = None, input_variable: Optional[str] = None, max_history_messages: Optional[int] = None, max_repair_attempts: Optional[int] = None, memory: Optional[PromptMemory] = None, tokenizer: Optional[Tokenizer] = None, validator: Optional[PromptResponseValidator] = None, logRepairs: Optional[bool] = None):
         self.client = client
         self.prompt = prompt
         self.prompt_options = prompt_options
         self.functions = functions
         self.history_variable = history_variable
         self.input_variable = input_variable
         self.max_history_messages = max_history_messages
         self.max_repair_attempts = max_repair_attempts
         self.tokenizer = tokenizer
         self.validator = validator
         self.logRepairs = logRepairs
-
+"""
 
 class AlphaWave(AsyncIOEventEmitter):
     def __init__(self, **kwargs):
         super().__init__()
         self.options = {
             'client': PromptCompletionClient,
             'prompt': PromptSection,
```

### Comparing `alphawave-0.2.0/src/alphawave/Colorize.py` & `alphawave-0.2.1/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.1/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.1/src/alphawave/JSONResponseValidator.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 class JSONResponseValidator(PromptResponseValidator):
     def __init__(self, schema=None, missing_json_feedback='No valid JSON objects were found in the response. Return a valid JSON object.'):
         self.schema = schema
         self.missing_json_feedback = missing_json_feedback
 
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts: int) -> Validation:
         message = response['message']
+        #print(f'***** JSON ResponseValidator \n{response}, \n {message}\n\n')
         text = message if isinstance(message, str) else message.get('content', '')
 
         # Parse the response text
         parsed = Response.parse_all_objects(text)
+        #print(f'***** JSON ResponseValidator Response.parse_all \n{parsed}n\n')
         if len(parsed) == 0:
             return {
                 'type': 'Validation',
                 'valid': False,
                 'feedback': self.missing_json_feedback
             }
```

### Comparing `alphawave-0.2.0/src/alphawave/MemoryFork.py` & `alphawave-0.2.1/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/OSClient.py` & `alphawave-0.2.1/src/alphawave/OpenAIClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,134 @@
-import requests
+import requests, time, copy
 from typing import Optional, Dict, Any, Union
-from promptrix import PromptFunctions, PromptMemory, PromptSection, Tokenizer
-from types import PromptCompletionClient, PromptCompletionOptions, PromptResponse
-from internals import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
-from internals import Colorize
+from dataclasses import dataclass, asdict
+from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
+from promptrix.SystemMessage import SystemMessage
+from promptrix.ConversationHistory import ConversationHistory
+from promptrix.AssistantMessage import AssistantMessage
+
+from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
+from alphawave.internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
+import alphawave.Colorize as Colorize
 
+@dataclass
 class OpenAIClientOptions:
-    def __init__(self, apiKey: str, organization: Optional[str] = None, endpoint: Optional[str] = None, logRequests: Optional[bool] = None):
+    def __init__(self, apiKey=None, organization = None, endpoint = None, logRequests = False):
         self.apiKey = apiKey
         self.organization = organization
         self.endpoint = endpoint
         self.logRequests = logRequests
 
 class OpenAIClient(PromptCompletionClient):
     DefaultEndpoint = 'https://api.openai.com'
     UserAgent = 'AlphaWave'
 
-    def __init__(self, options: OpenAIClientOptions):
-        self.options = options
-
-        if options.endpoint:
-            options.endpoint = options.endpoint.strip()
-            if options.endpoint.endswith('/'):
-                options.endpoint = options.endpoint[:-1]
-
-            if not options.endpoint.lower().startswith('https://'):
-                raise ValueError(f"Client created with an invalid endpoint of '{options.endpoint}'. The endpoint must be a valid HTTPS url.")
-
-        if not options.apiKey:
-            raise ValueError("Client created without an 'apiKey'.")
+    def __init__(self, **kwargs):
+        self.options = {'apiKey':None, 'organization':None, 'endpoint':None, 'logRequests':False}
+        self.options.update(kwargs)
+        if self.options['endpoint']:
+            self.options['endpoint'] = self.options['endpoint'].strip()
+            if self.options['endpoint'].endswith('/'):
+                self.options['endpoint'] = self.options['endpoint'][:-1]
+
+            if not self.options['endpoint'].lower().startswith('https://'):
+                raise ValueError(f"Client created with an invalid endpoint of '{options['endpoint']}'. The endpoint must be a valid HTTPS url.")
+
+        if not self.options['apiKey']:
+            print("Client created without an 'apiKey'.")
+            raise ValueError
 
         self._session = requests.Session()
 
-    def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
+    async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
         startTime = time.time()
-        max_input_tokens = options.max_input_tokens or 1024
-        if options.completion_type == 'text':
+        max_input_tokens = 1024
+        if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
+            max_input_tokens = options.max_input_tokens
+        if hasattr(options, 'completion_type') and options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            if self.options.logRequests:
+            if self.options['logRequests']:
                 print(Colorize.title('PROMPT:'))
                 print(Colorize.output(result.output))
 
             request = self.copyOptionsToRequest(CreateCompletionRequest({
-                'model': options.model,
-                'prompt': result.output,
+                'model': self.options['model'],
+                'prompt': result['output'],
             }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createCompletion(request)
-            if self.options.logRequests:
+            if self.options['logRequests']:
                 print(Colorize.title('RESPONSE:'))
                 print(Colorize.value('statuse', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
                 print(Colorize.output(response.json()))
 
             if response.status_code < 300:
                 completion = response.json().get('choices')[0]
                 return {'status': 'success', 'message': {'role': 'assistant', 'content': completion.get('text', '')}}
             elif response.status_code == 429:
-                if self.options.logRequests:
+                if self.options['logRequests']:
                     print(Colorize.title('HEADERS:'))
                     print(Colorize.output(response.headers))
                 return {'status': 'rate_limited', 'message': 'The text completion API returned a rate limit error.'}
             else:
                 return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status_code}: {response.reason}"}
         else:
-            result = prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
+            result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            if self.options.logRequests:
+            if self.options['logRequests']:
                 print(Colorize.title('CHAT PROMPT:'))
                 print(Colorize.output(result.output))
-
-            request = self.copyOptionsToRequest(CreateChatCompletionRequest({
-                'model': options.model,
-                'messages': result.output,
-            }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
+            request = self.copyOptionsToRequest(CreateChatCompletionRequest(model=options.model, messages=result.output), options,
+                                                    ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createChatCompletion(request)
-            if self.options.logRequests:
+            if self.options['logRequests']:
                 print(Colorize.title('CHAT RESPONSE:'))
                 print(Colorize.value('statuse', response.status_code))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
                 print(Colorize.output(response.json()))
 
             if response.status_code < 300:
                 completion = response.json().get('choices')[0]
                 return {'status': 'success', 'message': completion.get('message', {'role': 'assistant', 'content': ''})}
             elif response.status_code == 429:
-                if self.options.logRequests:
+                if self.options['logRequests']:
                     print(Colorize.title('HEADERS:'))
                     print(Colorize.output(response.headers))
                 return {'status': 'rate_limited', 'message': 'The chat completion API returned a rate limit error.'}
             else:
                 return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status_code}: {response.reason}"}
 
     def addRequestHeaders(self, headers: Dict[str, str], options: OpenAIClientOptions):
-        headers['Authorization'] = f"Bearer {options.apiKey}"
-        if options.organization:
-            headers['OpenAI-Organization'] = options.organization
+        headers['Authorization'] = f"Bearer {options['apiKey']}"
+        if options['organization']:
+            headers['OpenAI-Organization'] = options['organization']
 
     def copyOptionsToRequest(self, target: Dict[str, Any], src: Any, fields: list) -> Dict[str, Any]:
         for field in fields:
-            if field in src:
-                target[field] = src[field]
+            if hasattr(src, field) and getattr(src, field) is not None:
+                setattr(target,field, getattr(src,field))
         return target
 
     def createCompletion(self, request: CreateCompletionRequest) -> requests.Response:
-        url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/completions"
+        url = f"{self.options['endpoint'] or self.DefaultEndpoint}/v1/completions"
         return self.post(url, request)
 
     def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
-        url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/chat/completions"
+        url = f"{self.options['endpoint'] or self.DefaultEndpoint}/v1/chat/completions"
         return self.post(url, request)
 
     def post(self, url: str, body: object) -> requests.Response:
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
         self.addRequestHeaders(requestHeaders, self.options)
-        return self._session.post(url, json=body, headers=requestHeaders)
+        jsonbody = asdict(body)
+        keys = list(jsonbody.keys())
+        for key in keys:
+            if jsonbody[key] is None:
+                del jsonbody[key]
+        return self._session.post(url, json=jsonbody, headers=requestHeaders)
+
```

### Comparing `alphawave-0.2.0/src/alphawave/OpenAIClient.py` & `alphawave-0.2.1/src/alphawave/OSClient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,137 @@
-import requests, time, copy
-from typing import Optional, Dict, Any, Union
+import requests
 from dataclasses import dataclass, asdict
+from typing import Optional, Dict, Any, Union
+import time
+import json
+import asyncio
 from promptrix.promptrixTypes import PromptFunctions, PromptMemory, PromptSection, Tokenizer
 from promptrix.SystemMessage import SystemMessage
 from promptrix.ConversationHistory import ConversationHistory
 from promptrix.AssistantMessage import AssistantMessage
 
 from alphawave.alphawaveTypes import PromptCompletionClient, PromptCompletionOptions, PromptResponse
 from alphawave.internalTypes import ChatCompletionRequestMessage, CreateChatCompletionRequest, CreateChatCompletionResponse, CreateCompletionRequest, CreateCompletionResponse
 import alphawave.Colorize as Colorize
+import alphawave.utilityV2 as ut
+import alphawave.LLMClient as client
 
 @dataclass
-class OpenAIClientOptions:
-    def __init__(self, apiKey=None, organization = None, endpoint = None, logRequests = False):
+class OSClientOptions:
+    def __init__(self, apiKey, organization = None, endpoint = None, logRequests = None):
         self.apiKey = apiKey
         self.organization = organization
         self.endpoint = endpoint
         self.logRequests = logRequests
 
-class OpenAIClient(PromptCompletionClient):
+@dataclass
+class Response:
+    status_code: int
+    text: str
+    headers: Dict[str,str] = None
+    reason: str = ''
+    
+class OSClient(PromptCompletionClient):
     DefaultEndpoint = 'https://api.openai.com'
     UserAgent = 'AlphaWave'
 
     def __init__(self, **kwargs):
         self.options = {'apiKey':None, 'organization':None, 'endpoint':None, 'logRequests':False}
         self.options.update(kwargs)
         if self.options['endpoint']:
-            self.options['endpoint'] = options['endpoint'].strip()
-            if options['endpoint'].endswith('/'):
-                options['endpoint'] = options['endpoint'][:-1]
+            self.options['endpoint'] = self.options['endpoint'].strip()
+            if self.options['endpoint'].endswith('/'):
+                self.options['endpoint'] = self.options['endpoint'][:-1]
 
-            if not options['endpoint'].lower().startswith('https://'):
+            if not self.options['endpoint'].lower().startswith('https://'):
                 raise ValueError(f"Client created with an invalid endpoint of '{options['endpoint']}'. The endpoint must be a valid HTTPS url.")
 
         if not self.options['apiKey']:
-            raise ValueError("Client created without an 'apiKey'.")
+            print("Client created without an apiKey.")
 
         self._session = requests.Session()
 
     async def complete_prompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
         startTime = time.time()
-        max_input_tokens = 1024
-        if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
-            max_input_tokens = options.max_input_tokens
-        if hasattr(options, 'completion_type') and options.completion_type == 'text':
+        #print('enter complete prompt')
+        max_input_tokens = options.max_input_tokens or 1024
+        if options.completion_type == 'text':
             result = prompt.renderAsText(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated text completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
-            if self.options['logRequests']:
+            if self.options.logRequests:
                 print(Colorize.title('PROMPT:'))
                 print(Colorize.output(result.output))
 
             request = self.copyOptionsToRequest(CreateCompletionRequest({
-                'model': self.options['model'],
-                'prompt': result['output'],
+                'model': options.model,
+                'prompt': result.output,
             }), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
             response = self.createCompletion(request)
-            if self.options['logRequests']:
+            if self.options.logRequests:
                 print(Colorize.title('RESPONSE:'))
                 print(Colorize.value('statuse', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
-                print(Colorize.output(response.json()))
+                print(Colorize.output(response.message))
 
-            if response.status_code < 300:
-                completion = response.json().get('choices')[0]
-                return {'status': 'success', 'message': {'role': 'assistant', 'content': completion.get('text', '')}}
-            elif response.status_code == 429:
-                if self.options['logRequests']:
-                    print(Colorize.title('HEADERS:'))
-                    print(Colorize.output(response.headers))
-                return {'status': 'rate_limited', 'message': 'The text completion API returned a rate limit error.'}
+            if response.status == 'success':
+                completion = response.message
+                return {'status': 'success', 'message': completion}
             else:
-                return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status_code}: {response.reason}"}
+                return {'status': 'error', 'message': f"The text completion API returned an error status of {response.status}: {response.message}"}
         else:
             result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
             if result.tooLong:
                 return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
             if self.options['logRequests']:
                 print(Colorize.title('CHAT PROMPT:'))
                 print(Colorize.output(result.output))
-            request = self.copyOptionsToRequest(CreateChatCompletionRequest(model=options.model, messages=result.output), options,
-                                                    ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
-            response = self.createChatCompletion(request)
+            #print(f'************* render as messages {result}')
+            request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
+            response = await self.createChatCompletion(request)
             if self.options['logRequests']:
                 print(Colorize.title('CHAT RESPONSE:'))
-                print(Colorize.value('statuse', response.status_code))
+                print(Colorize.value('status', response.status))
                 print(Colorize.value('duration', time.time() - startTime, 'ms'))
-                print(Colorize.output(response.json()))
+                print(Colorize.output(response.text))
 
-            if response.status_code < 300:
-                completion = response.json().get('choices')[0]
-                return {'status': 'success', 'message': completion.get('message', {'role': 'assistant', 'content': ''})}
-            elif response.status_code == 429:
-                if self.options['logRequests']:
-                    print(Colorize.title('HEADERS:'))
-                    print(Colorize.output(response.headers))
-                return {'status': 'rate_limited', 'message': 'The chat completion API returned a rate limit error.'}
+            if response.status == 'success':
+                completion = response.message
+                return {'status': 'success', 'message': completion}
             else:
-                return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status_code}: {response.reason}"}
+                return {'status': 'error', 'message': f"The chat completion API returned an error status of {response.status}: {response.message}"}
 
-    def addRequestHeaders(self, headers: Dict[str, str], options: OpenAIClientOptions):
-        headers['Authorization'] = f"Bearer {options['apiKey']}"
-        if options['organization']:
-            headers['OpenAI-Organization'] = options['organization']
+    def addRequestHeaders(self, headers: Dict[str, str], options: OSClientOptions):
+        headers['Authorization'] = f"Bearer {options.apiKey}"
+        if options.organization:
+            headers['OS-Organization'] = options.organization
 
     def copyOptionsToRequest(self, target: Dict[str, Any], src: Any, fields: list) -> Dict[str, Any]:
         for field in fields:
             if hasattr(src, field) and getattr(src, field) is not None:
                 setattr(target,field, getattr(src,field))
         return target
 
     def createCompletion(self, request: CreateCompletionRequest) -> requests.Response:
-        url = f"{self.options['endpoint'] or self.DefaultEndpoint}/v1/completions"
+        url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/completions"
         return self.post(url, request)
 
     def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
         url = f"{self.options['endpoint'] or self.DefaultEndpoint}/v1/chat/completions"
         return self.post(url, request)
 
-    def post(self, url: str, body: object) -> requests.Response:
+    async def post(self, url: str, body: object) -> requests.Response:
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
-        self.addRequestHeaders(requestHeaders, self.options)
-        jsonbody = asdict(body)
-        keys = list(jsonbody.keys())
-        for key in keys:
-            if jsonbody[key] is None:
-                del jsonbody[key]
-        return self._session.post(url, json=jsonbody, headers=requestHeaders)
-        
+        #print(f'***** OSClient sending {body.messages}')
+        result = ''
+        try:
+            result = ut.ask_LLM(ut.MODEL, body.messages)
+            runon_idx = result.find(client.USER)
+            if runon_idx > 0:
+                result = result[:runon_idx]
+        except Exception as e:
+            print(f'***** OSCLient model returned {result}')
+            return PromptResponse(status='error',message=str(e))
+        return PromptResponse(status='success', message = {'role':'assistant', 'content': result})
```

### Comparing `alphawave-0.2.0/src/alphawave/Response.py` & `alphawave-0.2.1/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/TestClient.py` & `alphawave-0.2.1/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/TestClientTest.py` & `alphawave-0.2.1/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.1/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave/internalTypes.py` & `alphawave-0.2.1/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.1/src/alphawave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.0
+Version: 0.2.1
 Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://github.com/Stevenic/alphawave-py
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.0/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.1/src/alphawave.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 LICENSE
 README.md
 pyproject.toml
 src/alphawave/AlphaWave.py
 src/alphawave/Colorize.py
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
+src/alphawave/LLMClient.py
 src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
 src/alphawave/Response.py
 src/alphawave/TestClient.py
 src/alphawave/TestClientTest.py
 src/alphawave/__init__.py
 src/alphawave/alphawaveTypes.py
 src/alphawave/internalTypes.py
+src/alphawave/jsonParser.py
+src/alphawave/utilityV2.py
 src/alphawave.egg-info/PKG-INFO
 src/alphawave.egg-info/SOURCES.txt
 src/alphawave.egg-info/dependency_links.txt
 src/alphawave.egg-info/requires.txt
 src/alphawave.egg-info/top_level.txt
 src/alphawave_agents/Agent.py
 src/alphawave_agents/AgentCommandSection.py
 src/alphawave_agents/AgentCommandValidator.py
 src/alphawave_agents/AskCommand.py
-src/alphawave_agents/AskCommandTest.py
 src/alphawave_agents/CompleteTaskCommand.py
 src/alphawave_agents/ConfirmAnswerCommand.py
 src/alphawave_agents/FinalAnswerCommand.py
 src/alphawave_agents/MathCommand.py
 src/alphawave_agents/PromptCommand.py
 src/alphawave_agents/SchemaBasedCommand.py
 src/alphawave_agents/SentimentAnalysis.py
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
+tests/testOSClient.py
 tests/testOpenAiClient.py
 tests/testSchema.py
```

### Comparing `alphawave-0.2.0/src/alphawave_agents/Agent.py` & `alphawave-0.2.1/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.1/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.1/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.1/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.1/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,12 +45,12 @@
         )
         super().__init__(schema, title, description)
 
     def execute(self, input: CompleteTaskCommandInput, memory, functions, tokenizer):
         rsp = input.status
         if self.response is not None:
             rsp = self.response
-        return TaskResponse(
+        return asdict(TaskResponse(
             type="TaskResponse",
             status="success",
             message=rsp
-        )
+        ))
```

### Comparing `alphawave-0.2.0/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.1/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.1/src/alphawave_agents/MathCommand.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, Optional
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand
 from alphawave_agents.SchemaBasedCommand import CommandSchema as sbcCommandSchema
 from alphawave_agents.agentTypes import TaskResponse
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 import traceback
 
 @dataclass
 class CommandSchema(sbcCommandSchema):
     schema_type: str
     title: str
     description: str
@@ -44,9 +44,9 @@
         super().__init__(schema, title, description)
 
     def execute(self, input: MathCommandInput, memory: Any, functions: Any, tokenizer: Any) -> Any:
         try:
             return eval(input['code'])
         except Exception as err:
             message = str(err)
-            return TaskResponse('TaskResponse', 'error', message)
+            return asdict(TaskResponse('TaskResponse', 'error', message))
```

### Comparing `alphawave-0.2.0/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.1/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.1/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.1/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.1/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.1/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.0/tests/testOpenAiClient.py` & `alphawave-0.2.1/tests/testOSClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from promptrix.FunctionRegistry import FunctionRegistry 
 from promptrix.Prompt import Prompt
 from promptrix.GPT3Tokenizer import GPT3Tokenizer
 from promptrix.VolatileMemory import VolatileMemory
 from alphawave.alphawaveTypes import PromptCompletionOptions, PromptResponse, PromptResponseValidator, Validation
 from alphawave.DefaultResponseValidator import DefaultResponseValidator
 from alphawave.TestClient import TestClient
-from alphawave.OpenAIClient import OpenAIClient
+from alphawave.OSClient import OSClient
 from alphawave.AlphaWave import AlphaWave
 import os
 from promptrix.SystemMessage import SystemMessage
 from promptrix.ConversationHistory import ConversationHistory
 from promptrix.UserMessage import UserMessage
 from promptrix.AssistantMessage import AssistantMessage
+import alphawave.utilityV2 as ut
 
+ut.MODEL = ut.GUANACO_33B
 
 class TestValidator(PromptResponseValidator):
     def __init__(self, client):
         self.feedback = 'Something is wrong'
         self.repairAttempts = 0
         self.exception = None
         self.clientErrorDuringRepair = False
@@ -45,15 +47,15 @@
             self.returnContent = False
             return { 'type': 'Validation', 'valid': True, 'value': response['message']['content'] }
         else:
             return { 'type': 'Validation', 'valid': True }
 
 class TestAlphaWave(aiounittest.AsyncTestCase):
     def setUp(self):
-        self.client = OpenAIClient(apiKey=os.getenv("OPENAI_API_KEY"))
+        self.client = OSClient()
         #self.client = TestClient('success', { 'role': 'assistant', 'content': 'Hello' })
         self.prompt = Prompt([
             SystemMessage('You are helpful, creative, clever, and very friendly.'),
             ConversationHistory('history', .5),
             UserMessage('{{$input}}', 100)
         ])
 
@@ -64,25 +66,25 @@
         self.tokenizer = GPT3Tokenizer()
         self.validator = DefaultResponseValidator()
 
     def test_constructor(self):
         wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.prompt_options, memory=self.memory, functions=self.functions, tokenizer=self.tokenizer, validator=self.validator, history_variable='history', input_variable='input', max_repair_attempts=5, max_history_messages=20)
         assert_that(wave).is_not_none()
         assert_that(wave.options).is_not_none()
-        assert_that(wave.options.client).is_equal_to(self.client)
-        assert_that(wave.options.prompt).is_equal_to(self.prompt)
-        assert_that(wave.options.prompt_options).is_equal_to(self.prompt_options)
-        assert_that(wave.options.memory).is_equal_to(self.memory)
-        assert_that(wave.options.functions).is_equal_to(self.functions)
-        assert_that(wave.options.tokenizer).is_equal_to(self.tokenizer)
-        assert_that(wave.options.validator).is_equal_to(self.validator)
-        assert_that(wave.options.history_variable).is_equal_to('history')
-        assert_that(wave.options.input_variable).is_equal_to('input')
-        assert_that(wave.options.max_repair_attempts).is_equal_to(5)
-        assert_that(wave.options.max_history_messages).is_equal_to(20)
+        assert_that(wave.options['client']).is_equal_to(self.client)
+        assert_that(wave.options['prompt']).is_equal_to(self.prompt)
+        assert_that(wave.options['prompt_options']).is_equal_to(self.prompt_options)
+        assert_that(wave.options['memory']).is_equal_to(self.memory)
+        assert_that(wave.options['functions']).is_equal_to(self.functions)
+        assert_that(wave.options['tokenizer']).is_equal_to(self.tokenizer)
+        assert_that(wave.options['validator']).is_equal_to(self.validator)
+        assert_that(wave.options['history_variable']).is_equal_to('history')
+        assert_that(wave.options['input_variable']).is_equal_to('input')
+        assert_that(wave.options['max_repair_attempts']).is_equal_to(5)
+        assert_that(wave.options['max_history_messages']).is_equal_to(20)
 
     async def test_basic_prompt_completion(self):
         wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.prompt_options, memory=self.memory, functions=self.functions, tokenizer=self.tokenizer, validator=self.validator)
         
         response = await wave.completePrompt()
         print(response['status'])
         assert_that(response['status']).is_equal_to('success')
@@ -175,15 +177,15 @@
         self.client.response = None
         self.validator.repairAttempts = 1
         response = await wave.completePrompt('Hi')
         assert_that(response['status']).is_equal_to('success')
         assert_that(str(response['message']).startswith("{ 'role': 'assistant', 'content': '' }"))
         self.memory.clear()
         self.memory.set('history', [])
-
+    
     async def test_prompt_completion_with_message_object_response(self):
         wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.prompt_options, memory=self.memory, functions=self.functions, tokenizer=self.tokenizer, validator=self.validator)
         
         self.client.status = 'success'
         self.client.response = { 'role': 'assistant', 'content': { 'foo': 'bar'} }
         self.validator.repairAttempts = 1
         self.validator.returnContent = True
@@ -260,10 +262,10 @@
         response = await wave.completePrompt('Hi')
         assert_that(response['status']).is_equal_to('success')
         assert_that(str(response['message']).startswith("{ 'role': 'assistant', 'content': {"))
         history = self.memory.get('history')
         assert_that(str(history).startswith("[{ 'role': 'user', 'content': 'Hi' },{ 'role': 'assistant', 'content': {"))
         self.memory.clear()
         self.memory.set('history', [])
- 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `alphawave-0.2.0/tests/testSchema.py` & `alphawave-0.2.1/tests/testSchema.py`

 * *Files identical despite different names*

