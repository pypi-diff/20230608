# Comparing `tmp/PrSpiders-0.5.2.4.tar.gz` & `tmp/PrSpiders-0.5.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.4.tar", last modified: Fri Jun  2 02:53:07 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.2.5.tar", last modified: Thu Jun  8 09:10:06 2023, max compression
```

## Comparing `PrSpiders-0.5.2.4.tar` & `PrSpiders-0.5.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 02:53:07.105864 PrSpiders-0.5.2.4/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0     5497 2023-06-02 02:53:07.043852 PrSpiders-0.5.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 02:53:03.791852 PrSpiders-0.5.2.4/PrSpider/
--rw-rw-rw-   0        0        0    11246 2023-06-02 02:52:44.000000 PrSpiders-0.5.2.4/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.4/PrSpider/__init__.py
--rw-rw-rw-   0        0        0     2799 2023-05-29 06:44:50.000000 PrSpiders-0.5.2.4/PrSpider/log.py
--rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.4/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3260 2023-05-25 07:23:26.000000 PrSpiders-0.5.2.4/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4554 2023-06-02 01:23:50.000000 PrSpiders-0.5.2.4/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.4/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-06-02 02:53:04.689852 PrSpiders-0.5.2.4/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5497 2023-06-02 02:53:01.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-02 02:53:02.000000 PrSpiders-0.5.2.4/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5136 2023-05-25 03:36:57.000000 PrSpiders-0.5.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 02:53:04.886855 PrSpiders-0.5.2.4/pkg/
--rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.4/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 02:53:05.601858 PrSpiders-0.5.2.4/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.4/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.4/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.4/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.4/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-06-02 02:53:06.952852 PrSpiders-0.5.2.4/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.4/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.4/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4217 2023-06-01 06:51:18.000000 PrSpiders-0.5.2.4/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.4/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-06-02 02:53:07.105864 PrSpiders-0.5.2.4/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-02 02:52:53.000000 PrSpiders-0.5.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:10:06.386547 PrSpiders-0.5.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5497 2023-06-08 09:10:06.384552 PrSpiders-0.5.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 09:10:06.092551 PrSpiders-0.5.2.5/PrSpider/
+-rw-rw-rw-   0        0        0    11365 2023-06-08 09:08:15.000000 PrSpiders-0.5.2.5/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.5/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0     2799 2023-05-29 06:44:50.000000 PrSpiders-0.5.2.5/PrSpider/log.py
+-rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.5/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3260 2023-05-25 07:23:26.000000 PrSpiders-0.5.2.5/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4861 2023-06-08 09:08:06.000000 PrSpiders-0.5.2.5/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.5/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:10:06.189561 PrSpiders-0.5.2.5/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5497 2023-06-08 09:10:05.000000 PrSpiders-0.5.2.5/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-06-08 09:10:05.000000 PrSpiders-0.5.2.5/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:10:05.000000 PrSpiders-0.5.2.5/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-08 09:10:05.000000 PrSpiders-0.5.2.5/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-08 09:10:05.000000 PrSpiders-0.5.2.5/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-08 09:10:05.000000 PrSpiders-0.5.2.5/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5136 2023-05-25 03:36:57.000000 PrSpiders-0.5.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:10:06.217547 PrSpiders-0.5.2.5/pkg/
+-rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.5/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:10:06.287548 PrSpiders-0.5.2.5/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.5/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.5/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.5/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.5/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:10:06.365546 PrSpiders-0.5.2.5/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.5/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.5/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4217 2023-06-01 06:51:18.000000 PrSpiders-0.5.2.5/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.5/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-06-08 09:10:06.386547 PrSpiders-0.5.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-08 09:06:16.000000 PrSpiders-0.5.2.5/setup.py
```

### Comparing `PrSpiders-0.5.2.4/LICENSE.txt` & `PrSpiders-0.5.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/PKG-INFO` & `PrSpiders-0.5.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.4
+Version: 0.5.2.5
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.4/PrSpider/PrSpiders.py` & `PrSpiders-0.5.2.5/PrSpider/PrSpiders.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     request_num: Optional[int] = 0  # 请求数
     retry_num: Optional[int] = 0  # 重试数
     success_num: Optional[int] = 0  # 成功请求数
     false_num: Optional[int] = 0  # 失败请求数
     start_urls: Optional[list] = None  # 默认请求起始url
     executor: Optional[object] = None  # 线程池处理器
     retry: Optional[bool] = True  # 重试开关，默认开启
+    retry_xpath: Optional[str] = None  # 重试开关，默认开启
     pid: Optional[int] = os.getppid()  # 程序进程id
     start_time: Optional[int] = time.time()  # 开始时间
     download_delay: Optional[int] = 0  # 请求下载周期 默认 0s
     download_num: Optional[int] = 5  # 请求下载数量 默认 5/次
     logger: Optional[bool or str] = False  # 日志存储开关，默认关闭；可选（bool|文件名）
     log_level: Optional[str] = 'info'  # 日志等级，默认info
     log_stdout: Optional[bool] = False  # 日志控制台重定向，默认关闭
@@ -36,14 +37,15 @@
         settions.init += 1
         if settions.init <= 1:
             Log(self.log_stdout, self.log_level, self.logger).loggering()
         settions.request_num = self.request_num
         settions.success_num = self.success_num
         settions.false_num = self.false_num
         settions.retry = self.retry
+        settions.retry_xpath = self.retry_xpath
         settions.futures = self.futures
         settions.workers = self.workers
         settions.download_delay = self.download_delay
         settions.executor = ThreadPoolExecutor(settions.workers)
         settions.download_num = self.download_num
         settions.logger = self.logger
         settions.log_stdout = self.log_stdout
```

### Comparing `PrSpiders-0.5.2.4/PrSpider/log.py` & `PrSpiders-0.5.2.5/PrSpider/log.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/PrSpider/pxpath.py` & `PrSpiders-0.5.2.5/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/PrSpider/pyconn.py` & `PrSpiders-0.5.2.5/PrSpider/pyconn.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/PrSpider/requestXpath.py` & `PrSpiders-0.5.2.5/requestXpath/requestXpath.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,105 @@
-import requests
 import time
 import json
+import sys
+import datetime
+import requests
+from requests.exceptions import SSLError
 from requests.models import Response
 from .useragent import get_ua
 from .pxpath import Xpath
-from .log import loguercor
 """
 -------------------------------------------------
    File Name:     prequest
    Description :   Network Requests Class
    Author :        penr
    date:          2023/02/16
 -------------------------------------------------
    Change Activity:
                    2023/02/16:
 -------------------------------------------------
 """
-__author__ = "penr"
+__author__ = 'penr'
+__version__ = 0.1
 
+from loguru import logger
+
+format = "<b><green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green></b><b><level> | {level: ^8} | </level></b><b><i>{message}</i></b>"
+stdout_handler = {
+    "sink": sys.stdout,
+    "colorize": True,
+    "format": format
+}
+logger.configure(handlers=[stdout_handler])
 
 class prequest(Xpath):
     def __init__(self):
         self.response = Response()
-        self.retry_num = 0
+        self.amount = 0
+        self.samount = 0
+        self.famount = 0
         self.start_time = time.time()
 
     @property
     def user_agent(self):
         """
         :return: an User-Agent at random
         """
         return get_ua()
 
     @property
     def header(self):
         """
         :return: basic header
         """
-        return {"user-agent": self.user_agent}
+        return {'user-agent': self.user_agent}
 
-    def get(
-            self,
-            url,
-            headers=None,
-            retry_time=3,
-            method="GET",
-            meta=None,
-            encoding="utf-8",
-            retry_interval=1,
-            timeout=3,
-            settion=None,
-            *args,
-            **kwargs,
-    ):
+    def get(self, url, headers=None, retry_time=3, method='get', encoding='utf-8', retry_interval=1, timeout=3, *args,
+            **kwargs):
         """
         get method
         :param url: target url
         :param header: headers default:
         :param retry_time: retry time default: 3
         :param retry_interval: retry interval default: 1
         :param timeout: network timeout default: 3
         :return:
         """
-
         header = self.header
-        self.method = method.upper()
+        method = method.upper()
+        self.method = method
         self.retry_time = retry_time
         self.retry_interval = retry_interval
-        self.meta_ = {"retry_num": self.retry_num}
-        self.meta_.update(meta) if meta else meta
         if headers and isinstance(headers, dict):
-            if headers.get("user-agent") or headers.get("User-Agent"):
-                header = {}
             header.update(headers)
         while True:
             try:
+                self.amount += 1
                 self.response = requests.request(
-                    url=url,
-                    headers=header,
-                    timeout=timeout,
-                    method=self.method,
-                    *args,
-                    **kwargs,
-                )
+                    url=url, headers=header, timeout=timeout, method=method, *args, **kwargs)
                 self.response.encoding = encoding
-                if self.response.ok:
+                if self.response.status_code == 200:
+                    self.samount += 1
+                    logger.info(
+                        f'{method} {self.response.status_code} {self.response.url}')
                     return self
                 else:
-                    raise Exception(f"Crawl False %s" % self.code)
-
+                    logger.error(
+                        f'{method} {self.response.status_code} {self.response.url}')
+                    raise Exception(f'Respider {self.retry_interval}s')
+            except SSLError as e:
+                self.famount += 1
+                logging.error(e)
+                return self
             except Exception as e:
+                self.famount += 1
+                logger.error(e)
                 retry_time -= 1
-                self.retry_num += 1
-                if retry_time < 0 or settion.retry is False:
-                    loguercor.error("<yellow>[Crawl Fasle] %s %s %s</yellow>" % (self.method, url, e))
-                    self.response.status_code = (
-                        410
-                        if not self.response.status_code
-                        else self.response.status_code
-                    )
-                    self.meta_["retry_num"] = self.retry_num
-                    return self
-                else:
-                    loguercor.info(
-                        "<red>[Retry] %s %s %s %ss</red>"
-                        % (url, self.method, e, retry_interval)
-                    )
-
+                if retry_time <= 0:
+                    return None
                 time.sleep(retry_interval)
 
     @property
     def text(self):
         return self.response.text
 
     @property
@@ -126,41 +115,32 @@
         return self.response.history
 
     @property
     def json(self):
         return json.loads(self.response.text)
 
     @property
-    def code(self):
+    def status_code(self):
         return self.response.status_code
 
     @property
     def headers(self):
         return self.response.headers
 
     @property
-    def len(self):
+    def get_len(self):
         return len(self.response.text)
 
     @property
     def tree(self):
         return Xpath(self.response.text)
 
-    def xpath(self, xpath_str, **kwargs):
-        return Xpath(self.response.text).xpath(xpath_str, **kwargs)
-
-    @property
-    def ok(self):
-        return self.response.ok
-
-    @property
-    def meta(self):
-        return self.meta_
-
     def __del__(self):
-        try:
-            self.response.close()
-        except:
-            pass
-
-    def __str__(self) -> str:
-        return f"<Response Code={self.code} Len={self.len}>"
+        self.end_time = time.time()
+        spend_time = self.end_time - self.start_time
+        msg = """
+Requests: %s
+Success Requests: %s
+False Requests: %s
+Requests Time: %s
+        """ % (self.amount, self.samount, self.famount, spend_time)
+        logger.info(msg)
```

### Comparing `PrSpiders-0.5.2.4/PrSpider/useragent.py` & `PrSpiders-0.5.2.5/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.2.5/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2.4
+Version: 0.5.2.5
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `PrSpiders-0.5.2.4/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.2.5/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/README.md` & `PrSpiders-0.5.2.5/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.2.5/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/pkg/prspider/start.py` & `PrSpiders-0.5.2.5/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/requestXpath/__init__.py` & `PrSpiders-0.5.2.5/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/requestXpath/pxpath.py` & `PrSpiders-0.5.2.5/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/requestXpath/useragent.py` & `PrSpiders-0.5.2.5/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2.4/setup.py` & `PrSpiders-0.5.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.2.4"
+__version__ = "0.5.2.5"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

