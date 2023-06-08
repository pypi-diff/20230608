# Comparing `tmp/smawe_tools-0.2.6.tar.gz` & `tmp/smawe_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smawe_tools-0.2.6.tar", last modified: Sun May 28 10:29:16 2023, max compression
+gzip compressed data, was "smawe_tools-0.3.0.tar", last modified: Thu Jun  8 12:46:32 2023, max compression
```

## Comparing `smawe_tools-0.2.6.tar` & `smawe_tools-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.507922 smawe_tools-0.2.6/
--rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     5955 2023-05-28 10:29:16.506919 smawe_tools-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     5478 2023-05-27 14:13:31.000000 smawe_tools-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 10:29:16.507922 smawe_tools-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1019 2023-04-04 10:22:33.000000 smawe_tools-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.488070 smawe_tools-0.2.6/smawe_tools/
--rw-rw-rw-   0        0        0      194 2023-05-27 14:06:38.000000 smawe_tools-0.2.6/smawe_tools/__init__.py
--rw-rw-rw-   0        0        0       76 2023-05-28 10:27:58.000000 smawe_tools-0.2.6/smawe_tools/__version__.py
--rw-rw-rw-   0        0        0     6799 2023-05-28 10:27:58.000000 smawe_tools-0.2.6/smawe_tools/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.496749 smawe_tools-0.2.6/smawe_tools/exception/
--rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.2.6/smawe_tools/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.500027 smawe_tools-0.2.6/smawe_tools/net/
--rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.2.6/smawe_tools/net/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-04-04 10:22:33.000000 smawe_tools-0.2.6/smawe_tools/net/network_tool.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.502919 smawe_tools-0.2.6/smawe_tools/retrying/
--rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.2.6/smawe_tools/retrying/__init__.py
--rw-rw-rw-   0        0        0     2889 2023-04-09 10:10:02.000000 smawe_tools-0.2.6/smawe_tools/retrying/retry.py
--rw-rw-rw-   0        0        0      670 2023-04-18 02:48:31.000000 smawe_tools-0.2.6/smawe_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.503922 smawe_tools-0.2.6/smawe_tools/struct/
--rw-rw-rw-   0        0        0      946 2023-04-06 10:03:49.000000 smawe_tools-0.2.6/smawe_tools/struct/__init__.py
--rw-rw-rw-   0        0        0     2842 2023-04-19 07:48:57.000000 smawe_tools-0.2.6/smawe_tools/tool.py
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.495750 smawe_tools-0.2.6/smawe_tools.egg-info/
--rw-rw-rw-   0        0        0     5955 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-28 10:29:16.000000 smawe_tools-0.2.6/smawe_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 10:29:16.505922 smawe_tools-0.2.6/tests/
--rw-rw-rw-   0        0        0     1512 2023-05-28 10:19:26.000000 smawe_tools-0.2.6/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.798761 smawe_tools-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6568 2023-06-08 12:46:32.797758 smawe_tools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6091 2023-06-08 12:45:40.000000 smawe_tools-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 12:46:32.798761 smawe_tools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1019 2023-04-04 10:22:33.000000 smawe_tools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.778761 smawe_tools-0.3.0/smawe_tools/
+-rw-rw-rw-   0        0        0      194 2023-06-03 07:46:52.000000 smawe_tools-0.3.0/smawe_tools/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-06-08 12:45:40.000000 smawe_tools-0.3.0/smawe_tools/__version__.py
+-rw-rw-rw-   0        0        0      394 2023-06-08 12:35:51.000000 smawe_tools-0.3.0/smawe_tools/algorithm.py
+-rw-rw-rw-   0        0        0     6799 2023-05-28 10:27:58.000000 smawe_tools-0.3.0/smawe_tools/config.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.788757 smawe_tools-0.3.0/smawe_tools/exception/
+-rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.0/smawe_tools/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.791757 smawe_tools-0.3.0/smawe_tools/net/
+-rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.0/smawe_tools/net/__init__.py
+-rw-rw-rw-   0        0        0     2905 2023-04-04 10:22:33.000000 smawe_tools-0.3.0/smawe_tools/net/network_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.793758 smawe_tools-0.3.0/smawe_tools/retrying/
+-rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.0/smawe_tools/retrying/__init__.py
+-rw-rw-rw-   0        0        0     2889 2023-06-03 07:46:52.000000 smawe_tools-0.3.0/smawe_tools/retrying/retry.py
+-rw-rw-rw-   0        0        0      670 2023-04-18 02:48:31.000000 smawe_tools-0.3.0/smawe_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.795758 smawe_tools-0.3.0/smawe_tools/struct/
+-rw-rw-rw-   0        0        0      946 2023-04-06 10:03:49.000000 smawe_tools-0.3.0/smawe_tools/struct/__init__.py
+-rw-rw-rw-   0        0        0     2842 2023-04-19 07:48:57.000000 smawe_tools-0.3.0/smawe_tools/tool.py
+-rw-rw-rw-   0        0        0     1627 2023-06-08 12:35:51.000000 smawe_tools-0.3.0/smawe_tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.784758 smawe_tools-0.3.0/smawe_tools.egg-info/
+-rw-rw-rw-   0        0        0     6568 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.796762 smawe_tools-0.3.0/tests/
+-rw-rw-rw-   0        0        0       79 2023-06-08 12:39:15.000000 smawe_tools-0.3.0/tests/test.py
```

### Comparing `smawe_tools-0.2.6/LICENSE` & `smawe_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/PKG-INFO` & `smawe_tools-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: smawe_tools
-Version: 0.2.6
-Summary: small tool
-Author: Samwe
-Author-email: 1281722462@qq.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.5.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### ***本文档是由作者本人编写，难免会出现一些小问题，例如打错字等，发现后会及时改正***
 
 ---
 
 ### **核心函数**
 以下函数都可以从smawe_tools包中进行导入  
 例如: from smawe_tools import retry  
@@ -141,14 +126,36 @@
     ...     print(2)
     ...     print(a, b)
     ...     raise ValueError()
     ...
     >>> test(1, 2) #发生IndexError就进行重试
 
 ---
+此包提供了一个smawe_tools.utils模块, 用于将日志记录发送到QQ邮箱  
+简单使用如下:  
+```python
+import logging
+from smawe_tools.utils import ErrorLogger
+
+error_logger = ErrorLogger(
+    from_addr="xxxx@qq.com",
+    to_addrs=["xyzxxxx@qq.com", "abcdefg@qq.com"],
+    subject="python test",
+    password="xxxxxxxxx",
+    handler_level=logging.INFO,
+    logger_level=logging.INFO
+)
+
+# 这里已经将日志记录发送到QQ邮箱了
+error_logger.info("test message")
+# 然后你的QQ邮箱会收到这样类似的消息
+# test.py <module> INFO: (45)test message...
+```
+
+---
 此包还提供了一个对配置进行读取和保存的子模块smawe_tools.config  
 简单使用如下:  
 ```python
 from smawe_tools.config import Config
 
 config = Config()
 # 切换节，设置选项和值
@@ -170,12 +177,12 @@
 # 获取配置中的值
 print(config.get("s1", "k1"))
 print(config.get("s1", "kk1", fallback="vv2"))
 # 获取默认节中的值, 将其转为布尔值
 print(config.get_boolean("s1", "accept"))
 
 # 将其它值转为布尔值
-config.boolean_states = {"access": "agree"}
+config.boolean_states = {"access": True}
 
 config.set("s1", "can", "access")
 print(config.switch_to_section("s1").get_boolean("can"))
 ```
```

### Comparing `smawe_tools-0.2.6/setup.py` & `smawe_tools-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools/config.py` & `smawe_tools-0.3.0/smawe_tools/config.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools/net/network_tool.py` & `smawe_tools-0.3.0/smawe_tools/net/network_tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools/retrying/retry.py` & `smawe_tools-0.3.0/smawe_tools/retrying/retry.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools/settings.py` & `smawe_tools-0.3.0/smawe_tools/settings.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools/struct/__init__.py` & `smawe_tools-0.3.0/smawe_tools/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools/tool.py` & `smawe_tools-0.3.0/smawe_tools/tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.2.6/smawe_tools.egg-info/PKG-INFO` & `smawe_tools-0.3.0/smawe_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smawe-tools
-Version: 0.2.6
+Version: 0.3.0
 Summary: small tool
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -141,14 +141,36 @@
     ...     print(2)
     ...     print(a, b)
     ...     raise ValueError()
     ...
     >>> test(1, 2) #发生IndexError就进行重试
 
 ---
+此包提供了一个smawe_tools.utils模块, 用于将日志记录发送到QQ邮箱  
+简单使用如下:  
+```python
+import logging
+from smawe_tools.utils import ErrorLogger
+
+error_logger = ErrorLogger(
+    from_addr="xxxx@qq.com",
+    to_addrs=["xyzxxxx@qq.com", "abcdefg@qq.com"],
+    subject="python test",
+    password="xxxxxxxxx",
+    handler_level=logging.INFO,
+    logger_level=logging.INFO
+)
+
+# 这里已经将日志记录发送到QQ邮箱了
+error_logger.info("test message")
+# 然后你的QQ邮箱会收到这样类似的消息
+# test.py <module> INFO: (45)test message...
+```
+
+---
 此包还提供了一个对配置进行读取和保存的子模块smawe_tools.config  
 简单使用如下:  
 ```python
 from smawe_tools.config import Config
 
 config = Config()
 # 切换节，设置选项和值
@@ -170,12 +192,12 @@
 # 获取配置中的值
 print(config.get("s1", "k1"))
 print(config.get("s1", "kk1", fallback="vv2"))
 # 获取默认节中的值, 将其转为布尔值
 print(config.get_boolean("s1", "accept"))
 
 # 将其它值转为布尔值
-config.boolean_states = {"access": "agree"}
+config.boolean_states = {"access": True}
 
 config.set("s1", "can", "access")
 print(config.switch_to_section("s1").get_boolean("can"))
 ```
```

### Comparing `smawe_tools-0.2.6/smawe_tools.egg-info/SOURCES.txt` & `smawe_tools-0.3.0/smawe_tools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 setup.py
 smawe_tools/__init__.py
 smawe_tools/__version__.py
+smawe_tools/algorithm.py
 smawe_tools/config.py
 smawe_tools/settings.py
 smawe_tools/tool.py
+smawe_tools/utils.py
 smawe_tools.egg-info/PKG-INFO
 smawe_tools.egg-info/SOURCES.txt
 smawe_tools.egg-info/dependency_links.txt
 smawe_tools.egg-info/requires.txt
 smawe_tools.egg-info/top_level.txt
 smawe_tools/exception/__init__.py
 smawe_tools/net/__init__.py
```

