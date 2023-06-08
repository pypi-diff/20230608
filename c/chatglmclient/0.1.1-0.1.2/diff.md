# Comparing `tmp/chatglmclient-0.1.1.tar.gz` & `tmp/chatglmclient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglmclient-0.1.1.tar", last modified: Thu Jun  8 02:18:01 2023, max compression
+gzip compressed data, was "chatglmclient-0.1.2.tar", last modified: Thu Jun  8 03:08:33 2023, max compression
```

## Comparing `chatglmclient-0.1.1.tar` & `chatglmclient-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.824455 chatglmclient-0.1.1/
--rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 chatglmclient-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1380 2023-06-08 02:18:01.824455 chatglmclient-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-06-08 02:17:00.000000 chatglmclient-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.816450 chatglmclient-0.1.1/chatglmclient/
--rw-rw-rw-   0        0        0      106 2023-06-08 01:45:15.000000 chatglmclient-0.1.1/chatglmclient/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-06-08 02:08:09.000000 chatglmclient-0.1.1/chatglmclient/chatglm_client.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.820453 chatglmclient-0.1.1/chatglmclient/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 chatglmclient-0.1.1/chatglmclient/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.821453 chatglmclient-0.1.1/chatglmclient/tests/feature/
--rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 chatglmclient-0.1.1/chatglmclient/tests/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.822454 chatglmclient-0.1.1/chatglmclient/tests/script/
--rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 chatglmclient-0.1.1/chatglmclient/tests/script/__init__.py
--rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 chatglmclient-0.1.1/chatglmclient/tests/test_base.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.823456 chatglmclient-0.1.1/chatglmclient/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 chatglmclient-0.1.1/chatglmclient/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1039 2023-06-08 02:08:09.000000 chatglmclient-0.1.1/chatglmclient/tests/unit/client_test.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:18:01.818452 chatglmclient-0.1.1/chatglmclient.egg-info/
--rw-rw-rw-   0        0        0     1380 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-08 02:18:01.000000 chatglmclient-0.1.1/chatglmclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 02:18:01.824455 chatglmclient-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      799 2023-06-08 02:17:00.000000 chatglmclient-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.135473 chatglmclient-0.1.2/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 chatglmclient-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1410 2023-06-08 03:08:33.135473 chatglmclient-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      931 2023-06-08 02:19:32.000000 chatglmclient-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.127472 chatglmclient-0.1.2/chatglmclient/
+-rw-rw-rw-   0        0        0      106 2023-06-08 01:45:15.000000 chatglmclient-0.1.2/chatglmclient/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-06-08 02:08:09.000000 chatglmclient-0.1.2/chatglmclient/chatglm_client.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.131458 chatglmclient-0.1.2/chatglmclient/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 chatglmclient-0.1.2/chatglmclient/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.132471 chatglmclient-0.1.2/chatglmclient/tests/feature/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 chatglmclient-0.1.2/chatglmclient/tests/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.132471 chatglmclient-0.1.2/chatglmclient/tests/script/
+-rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 chatglmclient-0.1.2/chatglmclient/tests/script/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 chatglmclient-0.1.2/chatglmclient/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.134458 chatglmclient-0.1.2/chatglmclient/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 chatglmclient-0.1.2/chatglmclient/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     1039 2023-06-08 02:08:09.000000 chatglmclient-0.1.2/chatglmclient/tests/unit/client_test.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:08:33.130457 chatglmclient-0.1.2/chatglmclient.egg-info/
+-rw-rw-rw-   0        0        0     1410 2023-06-08 03:08:33.000000 chatglmclient-0.1.2/chatglmclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-06-08 03:08:33.000000 chatglmclient-0.1.2/chatglmclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 03:08:33.000000 chatglmclient-0.1.2/chatglmclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-08 03:08:33.000000 chatglmclient-0.1.2/chatglmclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 03:08:33.135473 chatglmclient-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-06-08 03:08:10.000000 chatglmclient-0.1.2/setup.py
```

### Comparing `chatglmclient-0.1.1/LICENSE` & `chatglmclient-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglmclient-0.1.1/PKG-INFO` & `chatglmclient-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: chatglmclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: chat glm client for api
-Home-page: https://github.com/jinghewang/
+Home-page: https://gitee.com/jiwei-data/python-chatglm-client.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -35,16 +35,16 @@
 
 按照提示，输入pypi的用户名、密码，就可以成功了。若中途提示有些库没有安装，则使用pip安装一下，需要用到twine库。
 
 ### 使用
 
 #### 安装或更新
 
-pip3 install chatglmclient
-pip3 install --upgrade chatglmclient
+pip3 install chatglmclient  
+pip3 install --upgrade chatglmclient    
 
 #### 代码使用
 
 ```python
 from chatglmclient.chatglm_client import ChatGLMClient
 
 client = ChatGLMClient(params={'api_host': "http://192.168.1.111:5000"})
```

### Comparing `chatglmclient-0.1.1/README.md` & `chatglmclient-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 按照提示，输入pypi的用户名、密码，就可以成功了。若中途提示有些库没有安装，则使用pip安装一下，需要用到twine库。
 
 ### 使用
 
 #### 安装或更新
 
-pip3 install chatglmclient
-pip3 install --upgrade chatglmclient
+pip3 install chatglmclient  
+pip3 install --upgrade chatglmclient    
 
 #### 代码使用
 
 ```python
 from chatglmclient.chatglm_client import ChatGLMClient
 
 client = ChatGLMClient(params={'api_host': "http://192.168.1.111:5000"})
```

### Comparing `chatglmclient-0.1.1/chatglmclient/chatglm_client.py` & `chatglmclient-0.1.2/chatglmclient/chatglm_client.py`

 * *Files identical despite different names*

### Comparing `chatglmclient-0.1.1/chatglmclient/tests/unit/client_test.py` & `chatglmclient-0.1.2/chatglmclient/tests/unit/client_test.py`

 * *Files identical despite different names*

### Comparing `chatglmclient-0.1.1/chatglmclient.egg-info/PKG-INFO` & `chatglmclient-0.1.2/chatglmclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: chatglmclient
-Version: 0.1.1
+Version: 0.1.2
 Summary: chat glm client for api
-Home-page: https://github.com/jinghewang/
+Home-page: https://gitee.com/jiwei-data/python-chatglm-client.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -35,16 +35,16 @@
 
 按照提示，输入pypi的用户名、密码，就可以成功了。若中途提示有些库没有安装，则使用pip安装一下，需要用到twine库。
 
 ### 使用
 
 #### 安装或更新
 
-pip3 install chatglmclient
-pip3 install --upgrade chatglmclient
+pip3 install chatglmclient  
+pip3 install --upgrade chatglmclient    
 
 #### 代码使用
 
 ```python
 from chatglmclient.chatglm_client import ChatGLMClient
 
 client = ChatGLMClient(params={'api_host': "http://192.168.1.111:5000"})
```

### Comparing `chatglmclient-0.1.1/setup.py` & `chatglmclient-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatglmclient',
-    version='0.1.1',
+    version='0.1.2',
     description="chat glm client for api",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='jinghewang',
     author_email='jinghewang@163.com',
     license='MIT License',
-    url='https://github.com/jinghewang/',
+    url='https://gitee.com/jiwei-data/python-chatglm-client.git',
     packages=find_packages(),
     excluded_packages=['tests'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

