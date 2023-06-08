# Comparing `tmp/pyxk-0.6.2.tar.gz` & `tmp/pyxk-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.2.tar", last modified: Wed Jun  7 02:35:28 2023, max compression
+gzip compressed data, was "pyxk-0.6.3.tar", last modified: Thu Jun  8 05:57:56 2023, max compression
```

## Comparing `pyxk-0.6.2.tar` & `pyxk-0.6.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.6.2/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-07 02:35:28.709720 pyxk-0.6.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.6.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.699720 pyxk-0.6.2/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      502 2023-06-06 03:59:16.000000 pyxk-0.6.2/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.2/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    19536 2023-06-06 06:59:38.000000 pyxk-0.6.2/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      510 2023-06-06 06:55:14.000000 pyxk-0.6.2/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.2/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3226 2023-06-07 02:28:36.000000 pyxk-0.6.2/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4873 2023-06-07 02:30:15.000000 pyxk-0.6.2/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.2/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.2/pyxk/m3u8/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4690 2023-06-07 02:27:20.000000 pyxk-0.6.2/pyxk/m3u8/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2946 2023-06-07 02:27:51.000000 pyxk-0.6.2/pyxk/m3u8/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    12424 2023-06-07 02:25:09.000000 pyxk-0.6.2/pyxk/m3u8/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.709720 pyxk-0.6.2/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.2/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-25 11:04:02.000000 pyxk-0.6.2/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.2/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    16522 2023-06-07 02:31:20.000000 pyxk-0.6.2/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    18885 2023-06-07 02:31:53.000000 pyxk-0.6.2/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-07 02:35:28.699720 pyxk-0.6.2/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      357 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-07 02:35:28.000000 pyxk-0.6.2/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-07 02:35:28.709720 pyxk-0.6.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      919 2023-06-07 02:35:16.000000 pyxk-0.6.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-08 05:57:56.655691 pyxk-0.6.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1530 2023-06-08 05:36:28.000000 pyxk-0.6.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.645691 pyxk-0.6.3/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       80 2023-06-08 05:49:20.000000 pyxk-0.6.3/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.645691 pyxk-0.6.3/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-06 06:59:00.000000 pyxk-0.6.3/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    19667 2023-06-08 05:44:28.000000 pyxk-0.6.3/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      510 2023-06-06 06:55:14.000000 pyxk-0.6.3/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-06-06 06:43:24.000000 pyxk-0.6.3/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3401 2023-06-08 05:42:28.000000 pyxk-0.6.3/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4873 2023-06-07 02:30:14.000000 pyxk-0.6.3/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       56 2023-06-06 07:01:26.000000 pyxk-0.6.3/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3354 2023-06-06 05:01:50.000000 pyxk-0.6.3/pyxk/m3u8/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4690 2023-06-07 02:27:20.000000 pyxk-0.6.3/pyxk/m3u8/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2946 2023-06-07 02:27:50.000000 pyxk-0.6.3/pyxk/m3u8/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    12434 2023-06-08 05:49:20.000000 pyxk-0.6.3/pyxk/m3u8/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.655691 pyxk-0.6.3/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-06-06 04:23:26.000000 pyxk-0.6.3/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7476 2023-06-08 05:49:20.000000 pyxk-0.6.3/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3493 2023-06-06 04:26:26.000000 pyxk-0.6.3/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    16522 2023-06-07 02:31:20.000000 pyxk-0.6.3/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    18885 2023-06-07 02:31:52.000000 pyxk-0.6.3/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 05:57:56.645691 pyxk-0.6.3/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1882 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      577 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       62 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-08 05:57:56.000000 pyxk-0.6.3/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-08 05:57:56.655691 pyxk-0.6.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      898 2023-06-08 05:37:28.000000 pyxk-0.6.3/setup.py
```

### Comparing `pyxk-0.6.2/LICENSE` & `pyxk-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/aclient/client.py` & `pyxk-0.6.3/pyxk/aclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,23 +452,24 @@
     root: Optional[Any] = None,
     base_url: Optional[str] = None,
     _expr: Optional[str] = None,
     huge_tree: Optional[bool] = None,
     errors: str = "strict",
     **kwargs
 ):
+    """Response.xpath"""
     text = await self.text(encoding=encoding, errors=errors)
     selector = _selector.Selector(
         text=text,
         type=type,
         _expr=_expr,
         namespaces=namespaces,
-        root=root,
+        root=root or _selector._NOT_SET,
         base_url=base_url,
-        huge_tree=_selector.LXML_SUPPORTS_HUGE_TREE if huge_tree is None else huge_tree,
+        huge_tree=huge_tree or _selector.LXML_SUPPORTS_HUGE_TREE,
     )
     return selector.xpath(query=query, **kwargs)
 
 async def css(
     self,
     query: str,
     namespaces: Optional[Mapping[str, str]] = None,
@@ -476,23 +477,24 @@
     type: Optional[str] = None,
     root: Optional[Any] = None,
     base_url: Optional[str] = None,
     _expr: Optional[str] = None,
     huge_tree: Optional[bool] = None,
     errors: str = "strict"
 ):
+    """Response.css"""
     text = await self.text(encoding=encoding, errors=errors)
     selector = _selector.Selector(
         text=text,
         type=type,
         _expr=_expr,
         namespaces=namespaces,
-        root=root,
+        root=root or _selector._NOT_SET,
         base_url=base_url,
-        huge_tree=_selector.LXML_SUPPORTS_HUGE_TREE if huge_tree is None else huge_tree,
+        huge_tree=huge_tree or _selector.LXML_SUPPORTS_HUGE_TREE,
     )
     return selector.css(query=query)
 
 async def re(
     self,
     regex: Union[str, Pattern[str]],
     replace_entities: bool = True,
@@ -501,36 +503,39 @@
     type: Optional[str] = None,
     root: Optional[Any] = None,
     base_url: Optional[str] = None,
     _expr: Optional[str] = None,
     huge_tree: Optional[bool] = None,
     errors: str = "strict",
 ):
+    """Response.re"""
     text = await self.text(encoding=encoding, errors=errors)
     selector = _selector.Selector(
         text=text,
         type=type,
         _expr=_expr,
         namespaces=namespaces,
-        root=root,
+        root=root or _selector._NOT_SET,
         base_url=base_url,
-        huge_tree=_selector.LXML_SUPPORTS_HUGE_TREE if huge_tree is None else huge_tree,
+        huge_tree=huge_tree or _selector.LXML_SUPPORTS_HUGE_TREE,
     )
     return selector.re(regex=regex, replace_entities=replace_entities)
 
 def urljoin(self, _url):
+    """Response.urljoin"""
     if isinstance(_url, str):
         _url = _yarl.URL(_url)
     elif not isinstance(_url, _yarl.URL):
         return _url
     if _url.is_absolute():
         return _url
     return self.url.join(_url)
 
 async def apparent_encoding(self):
+    """Response.apparent_encoding"""
     byte = await self.read()
     return chardet(byte)["encoding"]
 
 def add_method_to_response(response):
     """为异步response添加实例方法"""
     response.re = MethodType(re, response)
     response.css = MethodType(css, response)
```

### Comparing `pyxk-0.6.2/pyxk/aes/_fmtdata.py` & `pyxk-0.6.3/pyxk/aes/_fmtdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """AES加解密 数据初始化"""
+from typing import Union, Optional
 from pyxk.utils import LazyLoader
 
 AES = LazyLoader("AES", globals(), "Crypto.Cipher.AES")
 
 
 # 目前支持的模式
 MODES = {
@@ -18,15 +19,22 @@
     "GCM": 11,
     "OCB": 12
 }
 
 
 class FormatData:
     """AES数据初始化"""
-    def __init__(self, key, iv=None, mode="CBC", encode="UTF-8", **kwargs):
+    def __init__(
+        self,
+        key: Union[str, bytes],
+        iv: Optional[Union[str, bytes]] = None,
+        mode: Union[int, str] = "CBC",
+        encode: Optional[str] = "UTF-8",
+        **kwargs
+    ):
         """AES数据初始化 init
 
         :param key: 秘钥
         :param iv: 偏移量(部分加密模式不需要偏移量)
         :param mode: 加解密模式
         :param encode: 编码
         :param kwargs: **kwargs
```

### Comparing `pyxk-0.6.2/pyxk/aes/cryptor.py` & `pyxk-0.6.3/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/m3u8/enter_point.py` & `pyxk-0.6.3/pyxk/m3u8/enter_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/m3u8/m3u8download.py` & `pyxk-0.6.3/pyxk/m3u8/m3u8download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.3/pyxk/m3u8/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/m3u8/main.py` & `pyxk-0.6.3/pyxk/m3u8/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         if not self._reserve and self._temp_file:
             import shutil
             if os.path.isdir(self._temp_file):
                 shutil.rmtree(self._temp_file)
             
     def get_m3u8_content(
         self, url: Optional[str], *, is_m3u8key: bool = False
-    ) -> Union[str, bytes]:
+    ) -> Optional[Union[str, bytes]]:
         """获取m3u8内容
 
         :param url: url
         :param is_m3u8key: m3u8 key(type: bool)
         :return: str, bytes
         """
         if not(url and isinstance(url, str)):
```

### Comparing `pyxk-0.6.2/pyxk/requests/api.py` & `pyxk-0.6.3/pyxk/requests/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,16 +351,16 @@
     transient=False,
     output=None,
     restore=False,
     thread_num=None,
     user_agent=None,
     show_status=False
 ):
+    session = Session(user_agent=user_agent)
     try:
-        session = Session(user_agent=user_agent)
         response = session.downloader(
             method=method,
             url=url,
             params=params,
             data=data,
             headers=headers,
             cookies=cookies,
```

### Comparing `pyxk-0.6.2/pyxk/requests/entry_point.py` & `pyxk-0.6.3/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/requests/sessions.py` & `pyxk-0.6.3/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk/utils.py` & `pyxk-0.6.3/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.2/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.3/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

