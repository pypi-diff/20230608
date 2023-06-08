# Comparing `tmp/scrapfly-sdk-0.8.5.tar.gz` & `tmp/scrapfly-sdk-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapfly-sdk-0.8.5.tar", last modified: Fri Feb 24 16:37:33 2023, max compression
+gzip compressed data, was "scrapfly-sdk-0.8.6.tar", last modified: Thu Jun  8 02:08:49 2023, max compression
```

## Comparing `scrapfly-sdk-0.8.5.tar` & `scrapfly-sdk-0.8.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-02-24 16:37:33.165442 scrapfly-sdk-0.8.5/
--rw-r--r--   0 johann    (1000) johann    (1000)     1390 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.5/LICENSE
--rw-r--r--   0 johann    (1000) johann    (1000)     2704 2023-02-24 16:37:33.165442 scrapfly-sdk-0.8.5/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)     1451 2023-02-21 22:10:41.000000 scrapfly-sdk-0.8.5/README.md
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-02-24 16:37:33.162109 scrapfly-sdk-0.8.5/scrapfly/
--rw-r--r--   0 johann    (1000) johann    (1000)     1336 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.5/scrapfly/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)    16613 2022-06-14 19:45:38.000000 scrapfly-sdk-0.8.5/scrapfly/api_response.py
--rw-r--r--   0 johann    (1000) johann    (1000)    15969 2023-02-21 22:13:29.000000 scrapfly-sdk-0.8.5/scrapfly/client.py
--rw-r--r--   0 johann    (1000) johann    (1000)     7750 2022-06-14 23:39:55.000000 scrapfly-sdk-0.8.5/scrapfly/errors.py
--rw-r--r--   0 johann    (1000) johann    (1000)      653 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.5/scrapfly/frozen_dict.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-02-24 16:37:33.162109 scrapfly-sdk-0.8.5/scrapfly/polyfill/
--rw-r--r--   0 johann    (1000) johann    (1000)        0 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.5/scrapfly/polyfill/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)      556 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.5/scrapfly/polyfill/cached_property.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-02-24 16:37:33.162109 scrapfly-sdk-0.8.5/scrapfly/reporter/
--rw-r--r--   0 johann    (1000) johann    (1000)      406 2021-12-18 23:00:36.000000 scrapfly-sdk-0.8.5/scrapfly/reporter/ChainReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      214 2021-12-18 22:59:57.000000 scrapfly-sdk-0.8.5/scrapfly/reporter/NoopReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      944 2021-12-19 00:22:06.000000 scrapfly-sdk-0.8.5/scrapfly/reporter/PrintReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1164 2022-04-30 01:02:19.000000 scrapfly-sdk-0.8.5/scrapfly/reporter/SentryReporter.py
--rw-r--r--   0 johann    (1000) johann    (1000)      792 2021-12-18 22:59:04.000000 scrapfly-sdk-0.8.5/scrapfly/reporter/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)    11339 2023-02-24 16:27:20.000000 scrapfly-sdk-0.8.5/scrapfly/scrape_config.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-02-24 16:37:33.165442 scrapfly-sdk-0.8.5/scrapfly/scrapy/
--rw-r--r--   0 johann    (1000) johann    (1000)      473 2022-05-16 00:35:14.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/__init__.py
--rw-r--r--   0 johann    (1000) johann    (1000)     4924 2022-05-13 14:57:24.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/downloader.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3300 2022-05-16 01:42:35.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/middleware.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1800 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/pipelines.py
--rw-r--r--   0 johann    (1000) johann    (1000)     1293 2022-04-05 19:53:12.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/request.py
--rw-r--r--   0 johann    (1000) johann    (1000)     3133 2022-04-05 19:58:38.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/response.py
--rw-r--r--   0 johann    (1000) johann    (1000)     8774 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.5/scrapfly/scrapy/spider.py
-drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-02-24 16:37:33.165442 scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/
--rw-r--r--   0 johann    (1000) johann    (1000)     2704 2023-02-24 16:37:33.000000 scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/PKG-INFO
--rw-r--r--   0 johann    (1000) johann    (1000)      784 2023-02-24 16:37:33.000000 scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-02-24 16:37:33.000000 scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 johann    (1000) johann    (1000)      390 2023-02-24 16:37:33.000000 scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/requires.txt
--rw-r--r--   0 johann    (1000) johann    (1000)        9 2023-02-24 16:37:33.000000 scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/top_level.txt
--rw-r--r--   0 johann    (1000) johann    (1000)      272 2023-02-24 16:37:33.165442 scrapfly-sdk-0.8.5/setup.cfg
--rw-r--r--   0 johann    (1000) johann    (1000)     3124 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.5/setup.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1390 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/LICENSE
+-rw-r--r--   0 johann    (1000) johann    (1000)     2704 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)     1451 2023-02-21 22:10:41.000000 scrapfly-sdk-0.8.6/README.md
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/
+-rw-r--r--   0 johann    (1000) johann    (1000)     1336 2023-02-24 16:37:40.000000 scrapfly-sdk-0.8.6/scrapfly/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    16613 2022-06-14 19:45:38.000000 scrapfly-sdk-0.8.6/scrapfly/api_response.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    15969 2023-02-21 22:13:29.000000 scrapfly-sdk-0.8.6/scrapfly/client.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     7244 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.6/scrapfly/errors.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      653 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/scrapfly/frozen_dict.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/polyfill/
+-rw-r--r--   0 johann    (1000) johann    (1000)        0 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/scrapfly/polyfill/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      556 2021-12-11 00:47:07.000000 scrapfly-sdk-0.8.6/scrapfly/polyfill/cached_property.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/reporter/
+-rw-r--r--   0 johann    (1000) johann    (1000)      406 2021-12-18 23:00:36.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/ChainReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      214 2021-12-18 22:59:57.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/NoopReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      944 2021-12-19 00:22:06.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/PrintReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1164 2022-04-30 01:02:19.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/SentryReporter.py
+-rw-r--r--   0 johann    (1000) johann    (1000)      792 2021-12-18 22:59:04.000000 scrapfly-sdk-0.8.6/scrapfly/reporter/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)    11339 2023-02-24 16:27:20.000000 scrapfly-sdk-0.8.6/scrapfly/scrape_config.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.813965 scrapfly-sdk-0.8.6/scrapfly/scrapy/
+-rw-r--r--   0 johann    (1000) johann    (1000)      473 2022-05-16 00:35:14.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/__init__.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     4924 2022-05-13 14:57:24.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/downloader.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3163 2023-06-08 02:00:48.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/middleware.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1800 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/pipelines.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     1293 2022-04-05 19:53:12.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/request.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     3133 2022-04-05 19:58:38.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/response.py
+-rw-r--r--   0 johann    (1000) johann    (1000)     8774 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.6/scrapfly/scrapy/spider.py
+drwxr-xr-x   0 johann    (1000) johann    (1000)        0 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/
+-rw-r--r--   0 johann    (1000) johann    (1000)     2704 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 johann    (1000) johann    (1000)      784 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        1 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)      390 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/requires.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)        9 2023-06-08 02:08:49.000000 scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/top_level.txt
+-rw-r--r--   0 johann    (1000) johann    (1000)      272 2023-06-08 02:08:49.817298 scrapfly-sdk-0.8.6/setup.cfg
+-rw-r--r--   0 johann    (1000) johann    (1000)     3124 2023-02-21 22:10:15.000000 scrapfly-sdk-0.8.6/setup.py
```

### Comparing `scrapfly-sdk-0.8.5/LICENSE` & `scrapfly-sdk-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/PKG-INFO` & `scrapfly-sdk-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapfly-sdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Scrapfly SDK for Scrapfly
 Home-page: https://github.com/scrapfly/python-sdk
 Author: Scrapfly
 Author-email: tech@scrapfly.io
 License: BSD
 Project-URL: Company, https://scrapfly.io
 Project-URL: Documentation, https://scrapfly.io/docs
```

### Comparing `scrapfly-sdk-0.8.5/README.md` & `scrapfly-sdk-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/__init__.py` & `scrapfly-sdk-0.8.6/scrapfly/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.5'
+__version__ = '0.8.6'
 
 from typing import Tuple
 from .errors import ScrapflyError
 from .errors import ScrapflyAspError
 from .errors import ScrapflyProxyError
 from .errors import ScrapflyScheduleError
 from .errors import ScrapflyScrapeError
```

### Comparing `scrapfly-sdk-0.8.5/scrapfly/api_response.py` & `scrapfly-sdk-0.8.6/scrapfly/api_response.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/client.py` & `scrapfly-sdk-0.8.6/scrapfly/client.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/errors.py` & `scrapfly-sdk-0.8.6/scrapfly/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,14 @@
     RESOURCE_THROTTLE = 'THROTTLE'
     RESOURCE_SCRAPE = 'SCRAPE'
     RESOURCE_ASP = 'ASP'
     RESOURCE_SCHEDULE = 'SCHEDULE'
     RESOURCE_WEBHOOK = 'WEBHOOK'
     RESOURCE_SESSION = 'SESSION'
 
-    RETRYABLE_CODE = [
-        'ERR::SCRAPE::OPERATION_TIMEOUT',
-        'ERR::SCRAPE::TOO_MANY_CONCURRENT_REQUEST',
-        'ERR::PROXY::RESOURCES_SATURATION',
-        'ERR::PROXY::NOT_REACHABLE',
-        'ERR::PROXY::UNAVAILABLE',
-        'ERR::THROTTLE::MAX_CONCURRENT_REQUEST_EXCEEDED',
-        'ERR::THROTTLE::MAX_REQUEST_RATE_EXCEEDED',
-        'ERR::SESSION::CONCURRENT_ACCESS',
-        'ERR::ASP::SHIELD_EXPIRED',
-        'ERR::SCRAPE::NETWORK_ISSUE',
-        'ERR::SCRAPE::DRIVER_TIMEOUT'
-    ]
-
     def __init__(
         self,
         message: str,
         code: str,
         http_status_code: int,
         resource: Optional[str]=None,
         is_retryable: bool = False,
@@ -79,15 +65,14 @@
 
     def __init__(self, request:Request, response:Optional[Response]=None, **kwargs):
         self.request = request
         self.response = response
         super().__init__(**kwargs)
 
     def __str__(self) -> str:
-
         if isinstance(self, UpstreamHttpError):
             text = "%s -- %s " % (self.api_response.scrape_result['status_code'], self.api_response.scrape_result['reason'])
         else:
             text = "%s -- %s " % (self.response.status_code, self.response.reason)
 
             if isinstance(self, (ApiHttpClientError, ApiHttpServerError)):
                 try:
```

### Comparing `scrapfly-sdk-0.8.5/scrapfly/frozen_dict.py` & `scrapfly-sdk-0.8.6/scrapfly/frozen_dict.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/polyfill/cached_property.py` & `scrapfly-sdk-0.8.6/scrapfly/polyfill/cached_property.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/reporter/PrintReporter.py` & `scrapfly-sdk-0.8.6/scrapfly/reporter/PrintReporter.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/reporter/SentryReporter.py` & `scrapfly-sdk-0.8.6/scrapfly/reporter/SentryReporter.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/reporter/__init__.py` & `scrapfly-sdk-0.8.6/scrapfly/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrape_config.py` & `scrapfly-sdk-0.8.6/scrapfly/scrape_config.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrapy/downloader.py` & `scrapfly-sdk-0.8.6/scrapfly/scrapy/downloader.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrapy/middleware.py` & `scrapfly-sdk-0.8.6/scrapfly/scrapy/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from scrapy.spidermiddlewares.referer import RefererMiddleware as ScrapyRefererMidleware
 from twisted.web._newclient import ResponseNeverReceived
 
 from .spider import ScrapflySpider
 from .request import ScrapflyScrapyRequest
 from .response import ScrapflyScrapyResponse
 
-from .. import ScrapflyError, HttpError
+from .. import HttpError, ScrapflyError
 
 
 # spider middleware
 class ScrapflyRefererMiddleware(ScrapyRefererMidleware):
 
     def process_spider_output(self, response, result, spider) -> Iterable:
         if isinstance(response, ScrapflyScrapyResponse) and response.scrape_config.session is not None:
@@ -47,31 +47,27 @@
 
         if request.scrape_config.proxy_pool is None and spider.settings.get('SCRAPFLY_PROXY_POOL'):
             request.scrape_config.proxy_pool = spider.settings.get('SCRAPFLY_PROXY_POOL')
 
         return None
 
     def process_exception(self, request, exception:Union[str, Exception], spider:ScrapflySpider):
-        if isinstance(exception, ResponseNeverReceived):
-            return spider.retry(request, exception, 5)
-
-        if not isinstance(exception, ScrapflyError):
-            raise exception
+        delay = 1
 
-        if isinstance(exception, HttpError):
-            if exception.code in ScrapflyError.RETRYABLE_CODE or exception.http_status_code in [502]:
-                delay = 5
+        if isinstance(exception, ResponseNeverReceived):
+            return spider.retry(request, exception, delay)
 
-                if 'retry-after' in exception.response.headers:
-                    delay = int(exception.response.headers['retry-after'])
+        if isinstance(exception, ScrapflyError):
+            if exception.is_retryable:
+                if isinstance(exception, HttpError) and exception.response is not None:
+                    if 'retry-after' in exception.response.headers:
+                        delay = int(exception.response.headers['retry-after'])
 
                 return spider.retry(request, exception, delay)
 
-        if spider.settings.get('SCRAPFLY_CUSTOM_RETRY_CODE', False) and exception.code in spider.settings.get('SCRAPFLY_CUSTOM_RETRY_CODE'):
-            return spider.retry(request, exception, 5)
-        elif exception.is_retryable is True:
-            return spider.retry(request, exception, 5)
+            if spider.settings.get('SCRAPFLY_CUSTOM_RETRY_CODE', False) and exception.code in spider.settings.get('SCRAPFLY_CUSTOM_RETRY_CODE'):
+                return spider.retry(request, exception, delay)
 
         raise exception
 
     def process_response(self, request: Union[Request, ScrapflyScrapyRequest], response: Union[Response, ScrapflyScrapyResponse], spider: Union[Spider, ScrapflySpider]) -> Union[ScrapflyScrapyResponse, ScrapflyScrapyRequest]:
         return response
```

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrapy/pipelines.py` & `scrapfly-sdk-0.8.6/scrapfly/scrapy/pipelines.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrapy/request.py` & `scrapfly-sdk-0.8.6/scrapfly/scrapy/request.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrapy/response.py` & `scrapfly-sdk-0.8.6/scrapfly/scrapy/response.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly/scrapy/spider.py` & `scrapfly-sdk-0.8.6/scrapfly/scrapy/spider.py`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/PKG-INFO` & `scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapfly-sdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Scrapfly SDK for Scrapfly
 Home-page: https://github.com/scrapfly/python-sdk
 Author: Scrapfly
 Author-email: tech@scrapfly.io
 License: BSD
 Project-URL: Company, https://scrapfly.io
 Project-URL: Documentation, https://scrapfly.io/docs
```

### Comparing `scrapfly-sdk-0.8.5/scrapfly_sdk.egg-info/SOURCES.txt` & `scrapfly-sdk-0.8.6/scrapfly_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapfly-sdk-0.8.5/setup.py` & `scrapfly-sdk-0.8.6/setup.py`

 * *Files identical despite different names*

