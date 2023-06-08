# Comparing `tmp/chatglmclient-0.1.0.tar.gz` & `tmp/chatglmclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglmclient-0.1.0.tar", last modified: Thu Jun  8 02:14:34 2023, max compression
+gzip compressed data, was "chatglmclient-0.1.1.tar", last modified: Thu Jun  8 02:18:01 2023, max compression
```

## Comparing `chatglmclient-0.1.0.tar` & `chatglmclient-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.332199 chatglmclient-0.1.0/
--rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 chatglmclient-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1385 2023-06-08 02:14:34.332199 chatglmclient-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      930 2023-06-08 02:13:51.000000 chatglmclient-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.321193 chatglmclient-0.1.0/chatglmclient/
--rw-rw-rw-   0        0        0      106 2023-06-08 01:45:15.000000 chatglmclient-0.1.0/chatglmclient/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-06-08 02:08:09.000000 chatglmclient-0.1.0/chatglmclient/chatglm_client.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.327190 chatglmclient-0.1.0/chatglmclient/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 chatglmclient-0.1.0/chatglmclient/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.328189 chatglmclient-0.1.0/chatglmclient/tests/feature/
--rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 chatglmclient-0.1.0/chatglmclient/tests/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.329189 chatglmclient-0.1.0/chatglmclient/tests/script/
--rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 chatglmclient-0.1.0/chatglmclient/tests/script/__init__.py
--rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 chatglmclient-0.1.0/chatglmclient/tests/test_base.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.331191 chatglmclient-0.1.0/chatglmclient/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 chatglmclient-0.1.0/chatglmclient/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1039 2023-06-08 02:08:09.000000 chatglmclient-0.1.0/chatglmclient/tests/unit/client_test.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:34.325193 chatglmclient-0.1.0/chatglmclient.egg-info/
--rw-rw-rw-   0        0        0     1385 2023-06-08 02:14:34.000000 chatglmclient-0.1.0/chatglmclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-06-08 02:14:34.000000 chatglmclient-0.1.0/chatglmclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:14:34.000000 chatglmclient-0.1.0/chatglmclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 02:14:34.000000 chatglmclient-0.1.0/chatglmclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 02:14:34.332199 chatglmclient-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      799 2023-06-08 02:09:33.000000 chatglmclient-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.824455 chatglmclient-0.1.1/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 chatglmclient-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1380 2023-06-08 02:18:01.824455 chatglmclient-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      925 2023-06-08 02:17:00.000000 chatglmclient-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.816450 chatglmclient-0.1.1/chatglmclient/
+-rw-rw-rw-   0        0        0      106 2023-06-08 01:45:15.000000 chatglmclient-0.1.1/chatglmclient/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-06-08 02:08:09.000000 chatglmclient-0.1.1/chatglmclient/chatglm_client.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.820453 chatglmclient-0.1.1/chatglmclient/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 chatglmclient-0.1.1/chatglmclient/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.821453 chatglmclient-0.1.1/chatglmclient/tests/feature/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 chatglmclient-0.1.1/chatglmclient/tests/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.822454 chatglmclient-0.1.1/chatglmclient/tests/script/
+-rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 chatglmclient-0.1.1/chatglmclient/tests/script/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 chatglmclient-0.1.1/chatglmclient/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.823456 chatglmclient-0.1.1/chatglmclient/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 chatglmclient-0.1.1/chatglmclient/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     1039 2023-06-08 02:08:09.000000 chatglmclient-0.1.1/chatglmclient/tests/unit/client_test.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.818452 chatglmclient-0.1.1/chatglmclient.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:18:01.824455 chatglmclient-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      799 2023-06-08 02:17:00.000000 chatglmclient-0.1.1/setup.py
```

### Comparing `chatglmclient-0.1.0/LICENSE` & `chatglmclient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglmclient-0.1.0/PKG-INFO` & `chatglmclient-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: chatglmclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: chat glm client for api
 Home-page: https://github.com/jinghewang/
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chatglmclient
 
-集微工具箱，包括各种常用操作，后续不断完善
+ChatGLM Client，对 api 访问进行封装，方便调用
 
 ### 构建
 
 在项目文件夹中运行以下命令
 
 ```shell
 python setup.py sdist bdist_wheel
```

### Comparing `chatglmclient-0.1.0/README.md` & `chatglmclient-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # chatglmclient
 
-集微工具箱，包括各种常用操作，后续不断完善
+ChatGLM Client，对 api 访问进行封装，方便调用
 
 ### 构建
 
 在项目文件夹中运行以下命令
 
 ```shell
 python setup.py sdist bdist_wheel
```

### Comparing `chatglmclient-0.1.0/chatglmclient/chatglm_client.py` & `chatglmclient-0.1.1/chatglmclient/chatglm_client.py`

 * *Files identical despite different names*

### Comparing `chatglmclient-0.1.0/chatglmclient/tests/unit/client_test.py` & `chatglmclient-0.1.1/chatglmclient/tests/unit/client_test.py`

 * *Files identical despite different names*

### Comparing `chatglmclient-0.1.0/chatglmclient.egg-info/PKG-INFO` & `chatglmclient-0.1.1/chatglmclient.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: chatglmclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: chat glm client for api
 Home-page: https://github.com/jinghewang/
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chatglmclient
 
-集微工具箱，包括各种常用操作，后续不断完善
+ChatGLM Client，对 api 访问进行封装，方便调用
 
 ### 构建
 
 在项目文件夹中运行以下命令
 
 ```shell
 python setup.py sdist bdist_wheel
```

### Comparing `chatglmclient-0.1.0/setup.py` & `chatglmclient-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatglmclient',
-    version='0.1.0',
+    version='0.1.1',
     description="chat glm client for api",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='jinghewang',
     author_email='jinghewang@163.com',
     license='MIT License',
```

