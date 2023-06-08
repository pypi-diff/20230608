# Comparing `tmp/deskaone_sdk_scrypt_2023-1.2.0.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.2.0.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.2.1.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.2.0.tar` & `deskaone_sdk_scrypt_2023-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-06-08 01:35:50.858532 deskaone_sdk_scrypt_2023-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.2.0/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-06-08 01:35:57.863534 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    38076 2023-06-08 01:35:11.326682 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3577 2023-06-02 10:50:19.635539 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.2.0/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-08 10:07:35.271875 deskaone_sdk_scrypt_2023-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.2.1/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-08 10:07:38.896052 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    38129 2023-06-08 10:05:25.727107 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3577 2023-06-02 10:50:19.635539 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.2.1/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.2.1/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,18 +153,21 @@
     def __init__(self, Authorization: str) -> None:
         self.BASE_URL   = 'https://proxy.webshare.io/api/v2/'
         self.HEADERS    = dict(Authorization = Authorization)
         self.Session    = requests.Session()
     
     @property
     def __proxy__(self) -> list:
-        URL     = self.BASE_URL + 'proxy/list/?mode=direct&page=1&page_size=1000'
-        Result  = self.Session.get(URL, headers=self.HEADERS).json()
-        #json.dump(Result, open('webshare.json', 'w'), indent=4)
-        return Result.get('results')
+        PO = list()
+        for I in range(1, 11):
+            URL     = self.BASE_URL + f'proxy/list/?mode=direct&page={I}&page_size=100'
+            Result  = self.Session.get(URL, headers=self.HEADERS).json()
+            for P in Result.get('results'):
+                PO.append(P)
+        return PO
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             for Proxy in self.__proxy__:
                 USERNAME        = Proxy.get('username')
                 PASSWORD        = Proxy.get('password')
                 IP              = Proxy.get('proxy_address')
@@ -698,15 +701,15 @@
                 
                 if IpPort in self.ProxyError(Add=False): ProxyErrorGO = True
                 if IpPort in self.ProxyDetect(Add=False): ProxyDetectGO = True
                 Typer.Print(f'{Color.RED}=> {Color.WHITE}Generate New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Count {Color.GREEN}{Count}', Refresh=True)
                 if ProxyDetectGO is False and ProxyErrorGO is False:
                     if kwargs.get('IpPort') != PROXY.get("IpPort"):
                         S1 = requests.Session()
-                        RESULT  = S1.post(f'{kwargs.get("URL_API")}/Proxy', data=json.dumps(dict(DATA = dict(IpPort = IpPort, Proxies = Proxies))), timeout=15)
+                        RESULT  = S1.post(f'{kwargs.get("URL_API")}/Proxy', data=json.dumps(dict(DATA = dict(IpPort = IpPort, Proxies = Proxies))), timeout=30)
                         SPLIT   = str(RESULT.text).split('|')
                         self._CR = Crypto.AES()
                         self._CR.setKey_from_Hex(SPLIT[3][:int(SPLIT[1])])
                         self._CR.setIv_from_Hex(SPLIT[3][int(SPLIT[1]):int(SPLIT[1]) + int(SPLIT[0])])
                         self._CR.setData_FromHex(SPLIT[3][int(SPLIT[1]) + int(SPLIT[0]):])
                         Result  = self._CR.decrypt_to_dict()
                         if Result.get('STATUS') is True:
```

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.2.1/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/setup.py` & `deskaone_sdk_scrypt_2023-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.2.0/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

