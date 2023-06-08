# Comparing `tmp/zhipuai-1.0.1.tar.gz` & `tmp/zhipuai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zhipuai-1.0.1.tar", last modified: Wed May 24 11:25:36 2023, max compression
+gzip compressed data, was "zhipuai-1.0.2.tar", last modified: Thu Jun  8 12:15:13 2023, max compression
```

## Comparing `zhipuai-1.0.1.tar` & `zhipuai-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.823009 zhipuai-1.0.1/
--rw-r--r--   0 haowangai   (501) staff       (20)      525 2023-05-24 11:25:36.822786 zhipuai-1.0.1/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.1/README.md
--rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-05-24 11:25:36.823086 zhipuai-1.0.1/setup.cfg
--rw-r--r--   0 haowangai   (501) staff       (20)      881 2023-05-24 11:13:26.000000 zhipuai-1.0.1/setup.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.820129 zhipuai-1.0.1/tests/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-04-26 12:22:24.000000 zhipuai-1.0.1/tests/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1797 2023-05-24 11:24:35.000000 zhipuai-1.0.1/tests/test.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.820712 zhipuai-1.0.1/zhipuai/
--rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1968 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/api_resource.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.822492 zhipuai-1.0.1/zhipuai/utils/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)      131 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/api_util.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1758 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/http_client.py
--rw-r--r--   0 haowangai   (501) staff       (20)      543 2023-05-24 11:11:12.000000 zhipuai-1.0.1/zhipuai/utils/jwt_token.py
--rw-r--r--   0 haowangai   (501) staff       (20)     4471 2023-04-26 12:22:24.000000 zhipuai-1.0.1/zhipuai/utils/sse_client.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-05-24 11:25:36.821489 zhipuai-1.0.1/zhipuai.egg-info/
--rw-r--r--   0 haowangai   (501) staff       (20)      525 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)      384 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/SOURCES.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/dependency_links.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       13 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/requires.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       14 2023-05-24 11:25:36.000000 zhipuai-1.0.1/zhipuai.egg-info/top_level.txt
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-08 12:15:13.457563 zhipuai-1.0.2/
+-rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-08 12:15:13.457358 zhipuai-1.0.2/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.2/README.md
+-rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-08 12:15:13.457602 zhipuai-1.0.2/setup.cfg
+-rw-r--r--   0 haowangai   (501) staff       (20)      899 2023-06-08 12:14:57.000000 zhipuai-1.0.2/setup.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-08 12:15:13.454464 zhipuai-1.0.2/zhipuai/
+-rw-r--r--   0 haowangai   (501) staff       (20)      221 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/__init__.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-08 12:15:13.455717 zhipuai-1.0.2/zhipuai/examples/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/examples/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1466 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/examples/chatglm6b_example.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1427 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/examples/model_api_example.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-08 12:15:13.456498 zhipuai-1.0.2/zhipuai/model_api/
+-rw-r--r--   0 haowangai   (501) staff       (20)      102 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/model_api/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1858 2023-06-08 12:11:32.000000 zhipuai-1.0.2/zhipuai/model_api/api.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      246 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/model_api/chatglm_params.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      271 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/model_api/params.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-08 12:15:13.457081 zhipuai-1.0.2/zhipuai/utils/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-05 13:56:33.000000 zhipuai-1.0.2/zhipuai/utils/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1252 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/utils/http_client.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      700 2023-06-08 03:38:31.000000 zhipuai-1.0.2/zhipuai/utils/jwt_token.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     4531 2023-06-08 10:53:33.000000 zhipuai-1.0.2/zhipuai/utils/sse_client.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-08 12:15:13.455246 zhipuai-1.0.2/zhipuai.egg-info/
+-rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-08 12:15:13.000000 zhipuai-1.0.2/zhipuai.egg-info/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)      526 2023-06-08 12:15:13.000000 zhipuai-1.0.2/zhipuai.egg-info/SOURCES.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-06-08 12:15:13.000000 zhipuai-1.0.2/zhipuai.egg-info/dependency_links.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)       36 2023-06-08 12:15:13.000000 zhipuai-1.0.2/zhipuai.egg-info/requires.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        8 2023-06-08 12:15:13.000000 zhipuai-1.0.2/zhipuai.egg-info/top_level.txt
```

### Comparing `zhipuai-1.0.1/setup.py` & `zhipuai-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     readme = readme_file.read()
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="zhipuai",
-    version="v1.0.1",
+    version="v1.0.2",
     description="A SDK library for accessing big model apis from ZhipuAI",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Zhipu AI",
     url="https://open.bigmodel.cn/",
-    packages=find_packages(),
+    packages=find_packages(exclude=['tests']),
     include_package_data=True,
     install_requires=requirements,
     python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-)
+)
```

### Comparing `zhipuai-1.0.1/zhipuai/api_resource.py` & `zhipuai-1.0.2/zhipuai/model_api/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 # -*- coding:utf-8 -*-
 import json
 import os.path
 
 import zhipuai
 from zhipuai.utils import jwt_token
-from zhipuai.utils.api_util import InvokeType
 from zhipuai.utils.http_client import get, post, stream
 from zhipuai.utils.sse_client import SSEClient
 
 
-class APIResource:
+class InvokeType:
+    SYNC = "invoke"
+    ASYNC = "async-invoke"
+    SSE = "sse-invoke"
+
+
+class ModelAPI:
     @classmethod
     def invoke(cls, **kwargs):
         url = cls._build_api_url(kwargs, InvokeType.SYNC)
-        data = post(url, cls._generate_token(), kwargs)
+        data = post(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
         return json.loads(data)
 
     @classmethod
     def async_invoke(cls, **kwargs):
         url = cls._build_api_url(kwargs, InvokeType.ASYNC)
-        data = post(url, cls._generate_token(), kwargs)
+        data = post(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
         return json.loads(data)
 
     @classmethod
-    def query_async_invoke_result(cls, task_order_number: str):
-        url = cls._build_api_url(None, InvokeType.ASYNC, task_order_number)
-        data = get(url, cls._generate_token())
+    def query_async_invoke_result(cls, task_id: str):
+        url = cls._build_api_url(None, InvokeType.ASYNC, task_id)
+        data = get(url, cls._generate_token(), zhipuai.api_timeout_seconds)
         return json.loads(data)
 
     @classmethod
     def sse_invoke(cls, **kwargs):
         url = cls._build_api_url(kwargs, InvokeType.SSE)
-        data = stream(url, cls._generate_token(), kwargs)
-        return SSEClient(data)
-
-    @classmethod
-    def sse_risk_invoke(cls, **kwargs):
-        url = cls._build_api_url(kwargs, InvokeType.SSE, InvokeType.RISK)
-        data = stream(url, cls._generate_token(), kwargs)
+        data = stream(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
         return SSEClient(data)
 
     @staticmethod
     def _build_api_url(kwargs, *path):
         if kwargs:
             if "model" not in kwargs:
                 raise Exception("model param missed")
             model = kwargs.pop("model")
         else:
             model = "-"
 
-        return os.path.join(zhipuai.api_base, model, *path)
+        return os.path.join(zhipuai.model_api_url, model, *path)
 
     @staticmethod
     def _generate_token():
         if not zhipuai.api_key:
             raise Exception(
                 "api_key not provided, you could provide it with `shell: export API_KEY=xxx` or `code: zhipuai.api_key=xxx`"
             )
 
-        return jwt_token.generate_token(zhipuai.api_key, zhipuai.api_token_ttl_seconds)
+        return jwt_token.generate_token(zhipuai.api_key)
```

### Comparing `zhipuai-1.0.1/zhipuai/utils/http_client.py` & `zhipuai-1.0.2/zhipuai/utils/http_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,47 @@
 # -*- coding:utf-8 -*-
 import json
 import logging
 
 import requests
-from requests import exceptions
 
 headers = {
     "Accept": "application/json",
     "Content-Type": "application/json; charset=UTF-8",
 }
 
 
-def post(api_url, token, params, timeout=300):
+def post(api_url, token, params, timeout):
     try:
         headers.update({"Authorization": token})
         resp = requests.post(
             url=api_url, data=json.dumps(params), headers=headers, timeout=timeout
         )
         if requests.codes.ok == resp.status_code:
             return resp.text
-    except exceptions.Timeout as e:
-        logging.exception("请求超时", e)
-    except exceptions.ConnectionError as e:
-        logging.exception("请求连接错误", e)
-    except exceptions.HTTPError as e:
-        logging.exception("http请求错误", e)
+    except Exception as e:
+        logging.exception("请求异常", e)
 
 
-def stream(api_url, token, params, timeout=300):
+def stream(api_url, token, params, timeout):
     try:
         resp = requests.post(
             api_url,
             stream=True,
             headers={"Authorization": token},
             json=params,
             timeout=timeout,
         )
         if requests.codes.ok == resp.status_code:
             return resp
-    except exceptions.Timeout as e:
-        logging.exception("请求超时", e)
-    except exceptions.ConnectionError as e:
-        logging.exception("请求连接错误", e)
-    except exceptions.HTTPError as e:
-        logging.exception("http请求错误", e)
+    except Exception as e:
+        logging.exception("请求异常", e)
 
 
-def get(api_url, token):
+def get(api_url, token, timeout):
     try:
         headers.update({"Authorization": token})
-        resp = requests.get(api_url, headers=headers)
+        resp = requests.get(api_url, headers=headers, timeout=timeout)
         if requests.codes.ok == resp.status_code:
             return resp.text
-    except exceptions.ConnectionError as e:
-        logging.exception("请求连接错误", e)
-    except exceptions.HTTPError as e:
-        logging.exception("http请求错误", e)
+    except Exception as e:
+        logging.exception("请求异常", e)
```

### Comparing `zhipuai-1.0.1/zhipuai/utils/sse_client.py` & `zhipuai-1.0.2/zhipuai/utils/sse_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding:utf-8 -*-
 import logging
 
 _FIELD_SEPARATOR = ":"
 
+# Reference claim: https://github.com/mpetazzoni/sseclient
+
 
 class SSEClient(object):
     """Implementation of a SSE client.
     See http://www.w3.org/TR/2009/WD-eventsource-20091029/ for the
     specification.
     """
 
@@ -100,15 +102,15 @@
         """Manually close the event source stream."""
         self._event_source.close()
 
 
 class Event(object):
     """Representation of an event from the event stream."""
 
-    def __init__(self, id=None, event="message", data="", retry=None, meta={}):
+    def __init__(self, id=None, event: str = "", data="", retry=None, meta={}):
         self.id = id
         self.event = event
         self.data = data
         self.retry = retry
         self.meta = meta
 
     def __str__(self):
```

