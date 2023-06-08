# Comparing `tmp/gameyamlspiderandgenerator-1.5.4.tar.gz` & `tmp/gameyamlspiderandgenerator-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.5.4.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.5.5.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.5.4.tar` & `gameyamlspiderandgenerator-1.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.4/LICENSE
--rwxr-xr-x   0        0        0     1350 2023-05-22 00:40:10.043310 gameyamlspiderandgenerator-1.5.4/README.md
--rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1912 2023-05-22 02:18:45.372264 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     1476 2023-05-22 02:04:55.203167 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/openai.py
--rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3121 2023-05-22 00:40:10.068295 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7008 2023-05-22 02:16:18.462795 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     8006 2023-05-22 00:40:10.090094 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2138 2023-05-22 02:19:44.858160 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2682 2023-05-22 01:42:34.275139 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      719 2023-05-22 02:25:20.115256 gameyamlspiderandgenerator-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.5/LICENSE
+-rwxr-xr-x   0        0        0     1350 2023-05-22 00:40:10.043310 gameyamlspiderandgenerator-1.5.5/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1912 2023-06-07 14:28:50.774672 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      674 2023-06-05 12:09:09.231664 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     1476 2023-05-22 02:04:55.203167 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-07 14:30:32.807398 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7008 2023-06-07 14:12:02.952532 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7926 2023-06-07 14:12:05.775288 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2138 2023-05-22 02:19:44.858160 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-05 12:09:09.321318 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      719 2023-06-05 12:11:33.226209 gameyamlspiderandgenerator-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.5/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.5.4/LICENSE` & `gameyamlspiderandgenerator-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/README.md` & `gameyamlspiderandgenerator-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/exception.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 
 
 class ReadOrWriteConfigFailed(Exception):
     def __init__(self):
         super().__init__("Failed to read or write config")
 
 
-class CommunicateWithServerFailed(Exception):
-    def __init__(self, info: int | str = ""):
-        super().__init__(
-            f"Failed to communicate with server, {('status code: ' + str(info)) if isinstance(info, int) else info}"
-        )
+class InvalidTargetResourceError(Exception):
+    def __init__(self, code: int):
+        super().__init__(f"The target resource is no longer valid.status code: {int}")
 
 
 class ResponseNotInitialized(Exception):
     def __init__(self, url: str):
         super().__init__(f"Response not initialized, url: {url}")
 
 
 class InvalidResponse(Exception):
     def __init__(self, url: str):
-        super().__init__(f"Invalid response, url: {url}")
+        super().__init__(f"Invalid response, url: {url}")
```

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/openai.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/openai.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/hook/validate.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import abc
 import re
 from typing import List
+
+from ..util.fgi_yaml import YamlData
 from ..util.thread import ThreadWithReturnValue
 
 
 class BasePlugin(abc.ABC):
     """插件基类"""
 
     _VERIFY_PATTERN: re.Pattern
@@ -18,15 +20,16 @@
             url: URL
 
         Returns:
             是否符合要求
         """
         return bool(cls._VERIFY_PATTERN.match(url))
 
-    def __load_hook__(self,data: dict):
+    @staticmethod
+    def __load_hook__(data: dict):
         """
         加载钩子
 
         Args:
             data: 钩子数据
         """
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
@@ -145,14 +148,14 @@
         获取游戏截图
 
         Returns:
             游戏截图
         """
 
     @abc.abstractmethod
-    def to_yaml(self) -> str:
+    def to_yaml(self) -> YamlData:
         """
         转换为 YAML
 
         Returns:
             YAML
         """
```

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return s.replace("![]", "![img]")
 
     def __init__(self, link: str) -> None:
         self.id = self.get_steam_id(link)
         fn_list = [ThreadWithReturnValue(target=get_json,
                                          args=(f"https://store.steampowered.com/api/appdetails?appids={self.id}&cc=us"
                                                f"&l=english",)),
-                   ThreadWithReturnValue(target=get_text, args=(link, ))]
+                   ThreadWithReturnValue(target=get_text, args=(link,))]
         for i in fn_list:
             i.start()
         self.data, self.data_html = (ii.join() for ii in fn_list)
         self.soup = BeautifulSoup(self.data_html, "html.parser")
         self.name = self.get_name()
         temp1 = self.soup.body.find_all("a", {"class": "app_tag"})
         self.tag = [re.sub(r"[\n\t\r]*", "", temp1[i].text) for i in range(len(temp1))]
@@ -154,32 +154,26 @@
             self.remove_query(i["path_full"])
             for i in self.data[str(self.id)]["data"]["screenshots"]
         ]
 
     def get_video(self):
         is_nsfw = self.get_if_nsfw()
         video_webm = [
-            self.remove_query(i["webm"]["max"])
+            self.remove_query(i["webm"]["max"]).replace("http", "https")
             for i in self.data[str(self.id)]["data"]["movies"]
         ]
         video_mp4 = [
-            self.remove_query(i["mp4"]["max"])
+            self.remove_query(i["mp4"]["max"]).replace("http", "https")
             for i in self.data[str(self.id)]["data"]["movies"]
         ]
         return [
             {
-                "type": "video",
-                "src": [
-                    {
-                        "mime": "video/webm",
-                        "sensitive": is_nsfw,
-                        "uri": video_webm[i],
-                    },
-                    {"mime": "video/mp4", "sensitive": is_nsfw, "uri": video_mp4[i]},
-                ]
+                "video": [{"mime": "video/webm", "sensitive": is_nsfw, "uri": video_webm[i], },
+                          {"mime": "video/mp4", "sensitive": is_nsfw, "uri": video_mp4[i]},
+                          ]
                 if is_nsfw
                 else [
                     {"mime": "video/webm", "uri": video_webm[i]},
                     {"mime": "video/mp4", "uri": video_mp4[i]},
                 ],
             }
             for i in range(len(video_webm))
```

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.5.5/gameyamlspiderandgenerator/util/spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import requests
 from requests import JSONDecodeError
 
 from ..exception import (
-    CommunicateWithServerFailed,
+    InvalidTargetResourceError,
     InvalidResponse,
 )
 from ..util.config import config
 
 
 class GetResponse:
     """
@@ -33,21 +33,18 @@
         self.args = {
             "proxies": config["proxy"],
             "allow_redirects": allow_redirects,
             **kwargs,
         }
 
     def __enter__(self):
-        try:
-            self.response = requests.get(self.url, **self.args)
-            if self.response.status_code != 200:
-                raise CommunicateWithServerFailed(self.response.status_code)
-            return self
-        except Exception as e:
-            raise CommunicateWithServerFailed(str(e)[:100]) from None
+        self.response = requests.get(self.url, **self.args)
+        if self.response.status_code != 200:
+            raise InvalidTargetResourceError(self.response.status_code)
+        return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.response.close()
 
     @property
     def json(self):
         """
```

### Comparing `gameyamlspiderandgenerator-1.5.4/pyproject.toml` & `gameyamlspiderandgenerator-1.5.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.5.4"
+version = "1.5.5"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.5.4/PKG-INFO` & `gameyamlspiderandgenerator-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.5.4
+Version: 1.5.5
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

