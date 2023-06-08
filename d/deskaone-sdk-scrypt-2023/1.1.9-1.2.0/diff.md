# Comparing `tmp/deskaone_sdk_scrypt_2023-1.1.9.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.9.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.2.0.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.1.9.tar` & `deskaone_sdk_scrypt_2023-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-06-02 10:56:15.171255 deskaone_sdk_scrypt_2023-1.1.9/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.9/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-06-02 10:56:16.775256 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    34717 2023-05-19 13:16:00.694179 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3577 2023-06-02 10:50:19.635539 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.9/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-08 01:35:50.858532 deskaone_sdk_scrypt_2023-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.2.0/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-08 01:35:57.863534 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    38076 2023-06-08 01:35:11.326682 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3577 2023-06-02 10:50:19.635539 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.2.0/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.2.0/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.1.9"
+version = "1.2.0"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List, Optional, Tuple, Dict
+from .Crypto import Crypto
 import sqlalchemy as db, os
 import requests, json, random, os
 from requests.exceptions import ConnectionError, ConnectTimeout, SSLError, RequestException, HTTPError, ProxyError, Timeout, ReadTimeout, JSONDecodeError, TooManyRedirects, ChunkedEncodingError
 from .Typer import Typer, Color
 #from deskaone_sdk_scrypt_2023 import Typer, Color
 from bs4 import BeautifulSoup
 from sqlalchemy import BOOLEAN, INTEGER, VARCHAR, create_engine, MetaData
@@ -680,14 +681,70 @@
         except:pass
         try:
             if kwargs.get('PremiumProxy') is True or kwargs.get('PremiumProxy') is None:__PremiumProxy__().Main(New)
         except:pass
     
     def __check__(self, *args, **kwargs):
         if kwargs.get('IpPort') is None: raise Error('IpPort Required')
+        if kwargs.get('URL_API') is None: raise Error('URL_API Required')
+        ListProxy, Count = self.ListProxy, 0
+        while True:
+            Count += 1
+            try:
+                ProxyErrorGO = False
+                ProxyDetectGO = False
+                PROXY   = ListProxy[random.randint(0, len(ListProxy) - 1)]
+                IpPort  = PROXY.get("IpPort")
+                Proxies = PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies'))
+                
+                if IpPort in self.ProxyError(Add=False): ProxyErrorGO = True
+                if IpPort in self.ProxyDetect(Add=False): ProxyDetectGO = True
+                Typer.Print(f'{Color.RED}=> {Color.WHITE}Generate New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Count {Color.GREEN}{Count}', Refresh=True)
+                if ProxyDetectGO is False and ProxyErrorGO is False:
+                    if kwargs.get('IpPort') != PROXY.get("IpPort"):
+                        S1 = requests.Session()
+                        RESULT  = S1.post(f'{kwargs.get("URL_API")}/Proxy', data=json.dumps(dict(DATA = dict(IpPort = IpPort, Proxies = Proxies))), timeout=15)
+                        SPLIT   = str(RESULT.text).split('|')
+                        self._CR = Crypto.AES()
+                        self._CR.setKey_from_Hex(SPLIT[3][:int(SPLIT[1])])
+                        self._CR.setIv_from_Hex(SPLIT[3][int(SPLIT[1]):int(SPLIT[1]) + int(SPLIT[0])])
+                        self._CR.setData_FromHex(SPLIT[3][int(SPLIT[1]) + int(SPLIT[0]):])
+                        Result  = self._CR.decrypt_to_dict()
+                        if Result.get('STATUS') is True:
+                            DATA    = Result.get('DATA')
+                            API     = DATA.get('API')
+                            S1.close()
+                            __ProxyBase__.Proxys.SaveProxy().Up(IpPort = IpPort, Values = dict(countryCode = API.get("countryCode"), country = API.get("country")))
+                            return dict(
+                                PROXY   = Proxies,
+                                DATA    = API,
+                                IpPort  = IpPort
+                            )
+                        else:
+                            self.ProxyError(IpPort=IpPort, Add=True)
+                if Count >= len(self.ListProxy):
+                    self.Rescan(self.__Authorization__, self.__New__, *self.__args__, **self.__kwargs__)
+                    Count = 0
+            except ProxyError as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except ConnectTimeout as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except ConnectionError as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except ReadTimeout as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except JSONDecodeError:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except TooManyRedirects as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except Exception as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+    
+    def __check1__(self, *args, **kwargs):
+        if kwargs.get('IpPort') is None: raise Error('IpPort Required')
         ListProxy, Count = self.ListProxy, 0
         while True:
             Count += 1
             try:
                 ProxyErrorGO = False
                 ProxyDetectGO = False
                 PROXY   = ListProxy[random.randint(0, len(ListProxy) - 1)]
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/setup.py` & `deskaone_sdk_scrypt_2023-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.1.9',
+    'version': '1.2.0',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.9/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.1.9
+Version: 1.2.0
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

