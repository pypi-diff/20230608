# Comparing `tmp/openi-beta-0.0.5.tar.gz` & `tmp/openi-beta-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.5.tar", last modified: Thu Jun  1 10:10:55 2023, max compression
+gzip compressed data, was "openi-beta-0.0.6.tar", last modified: Thu Jun  8 02:47:07 2023, max compression
```

## Comparing `openi-beta-0.0.5.tar` & `openi-beta-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.171168 openi-beta-0.0.5/
--rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 10:10:55.171020 openi-beta-0.0.5/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      878 2023-06-01 03:43:54.000000 openi-beta-0.0.5/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-01 10:10:55.171211 openi-beta-0.0.5/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      985 2023-06-01 09:26:40.000000 openi-beta-0.0.5/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.168919 openi-beta-0.0.5/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.169447 openi-beta-0.0.5/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-01 10:05:04.000000 openi-beta-0.0.5/src/openi/__init__.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.169738 openi-beta-0.0.5/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.5/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    10607 2023-06-01 10:05:03.000000 openi-beta-0.0.5/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.170564 openi-beta-0.0.5/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     1508 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      321 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       20 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-01 10:10:55.000000 openi-beta-0.0.5/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-01 10:10:55.170830 openi-beta-0.0.5/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      605 2023-06-01 03:43:28.000000 openi-beta-0.0.5/test/test.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      904 2023-06-01 03:43:28.000000 openi-beta-0.0.5/test/test_thread.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.346746 openi-beta-0.0.6/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1808 2023-06-08 02:47:07.346615 openi-beta-0.0.6/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1178 2023-06-07 10:31:58.000000 openi-beta-0.0.6/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-08 02:47:07.346792 openi-beta-0.0.6/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      976 2023-06-08 02:25:02.000000 openi-beta-0.0.6/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.343836 openi-beta-0.0.6/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.344597 openi-beta-0.0.6/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-08 01:13:13.000000 openi-beta-0.0.6/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-08 02:31:58.000000 openi-beta-0.0.6/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.345173 openi-beta-0.0.6/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.6/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     9560 2023-06-08 02:44:34.000000 openi-beta-0.0.6/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.345975 openi-beta-0.0.6/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1808 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      344 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.346349 openi-beta-0.0.6/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      605 2023-06-01 03:43:28.000000 openi-beta-0.0.6/test/test.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      904 2023-06-01 03:43:28.000000 openi-beta-0.0.6/test/test_thread.py
```

### Comparing `openi-beta-0.0.5/PKG-INFO` & `openi-beta-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.5
+Version: 0.0.6
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,39 +12,41 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# This is a test package for OpenI PyPi
+# OpenI PyPi
 
-test package for OpenI 启智AI协作平台.
+> PYPI package for 启智AI协作平台。
 
-# 使用说明
+启智平台提供的Python工具包，使用户能在本地上传数据集。
 
 ## 安装
 
+*适配python3.6及以上版本*
 ```bash
-pip install openi-beta
+pip install openi
 ```
 
-## openi.dataset.upload_file()
+## 使用说明
 
-> 上传数据集函数
+- 确保您拥有此数据集（项目）的权限，`username`参数为数据集的创建者，即项目所属用户/组织的名称
+- 使用前请在平台个人设置中获取token：[点击跳转token获取界面](https://openi.pcl.ac.cn/user/settings/applications)
+- 当前版本为了方便用户本地上传数据集，建议在本地使用，后续版本将适配隐藏token参数、代码仓配置及云脑任务
 
-安装完成可仿照下列示，运行即可上传数据集
+## 本地上传数据集示例
 
 ```python
 from openi.dataset import upload_file
 
 upload_file(
-    file = "", # 必填，文件路径(包含文件名)
-    username = "", # 必填，数据集所属项目用户名
-    repository = "", # 必填，数据集所属项目名
+    file = "", # 必填，文件路径(包含文件名，支持windows文件路径如d:\\xxx)
+    username = "", # 必填，数据集所属项目owner用户名
+    repository = "", # 必填，数据集所属项目名称
     token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
     
-    cluster = "", # 选填，可填入GPU或NPU，不填写后台默认为NPU
-    app_url = "" #选填, 默认为平台地址，开发测试用
+    cluster = "" # 选填，可填入GPU或NPU，不填写后台默认为NPU
     )
 ```
-![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/7d3365f667974c5a06aaeb390003a3b929fde0d9/media/4.png)
+![alt](./media/4.png)
```

### Comparing `openi-beta-0.0.5/README.md` & `openi-beta-0.0.6/test/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,11 @@
-# This is a test package for OpenI PyPi
-
-test package for OpenI 启智AI协作平台.
-
-# 使用说明
-
-## 安装
-
-```bash
-pip install openi-beta
-```
-
-## openi.dataset.upload_file()
-
-> 上传数据集函数
-
-安装完成可仿照下列示，运行即可上传数据集
-
-```python
 from openi.dataset import upload_file
 
 upload_file(
-    file = "", # 必填，文件路径(包含文件名)
-    username = "", # 必填，数据集所属项目用户名
-    repository = "", # 必填，数据集所属项目名
-    token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
-    
-    cluster = "", # 选填，可填入GPU或NPU，不填写后台默认为NPU
-    app_url = "" #选填, 默认为平台地址，开发测试用
-    )
-```
-![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/7d3365f667974c5a06aaeb390003a3b929fde0d9/media/4.png)
+    file = "./output/car_image.zip", # 必填，文件路径(包含文件名)
+    username = "chenzh", # 必填，数据集所属项目用户名
+    repository = "openi-api-test", # 必填，数据集所属项目名
+    token = "c40d9f40d47078c33b431a3ac5156461ceaef95e", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
+
+    cluster = "GPU", # 选填，可填入GPU或NPU，不填写后台默认为NPU
+    app_url = "http://192.168.207.34/api/v1/" #选填, 默认为平台地址，用户不用填写，开发测试用
+)
```

### Comparing `openi-beta-0.0.5/setup.py` & `openi-beta-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.5',
+    version='0.0.6',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
@@ -22,10 +22,10 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Operating System :: OS Independent',
     ],
-    install_requires=['emoji', 'requests','tqdm'],
+    install_requires=['requests','tqdm'],
     python_requires='>=3.6',
 )
```

### Comparing `openi-beta-0.0.5/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.0.6/src/openi_beta.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.0.5
+Version: 0.0.6
 Summary: A test packages for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,39 +12,41 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# This is a test package for OpenI PyPi
+# OpenI PyPi
 
-test package for OpenI 启智AI协作平台.
+> PYPI package for 启智AI协作平台。
 
-# 使用说明
+启智平台提供的Python工具包，使用户能在本地上传数据集。
 
 ## 安装
 
+*适配python3.6及以上版本*
 ```bash
-pip install openi-beta
+pip install openi
 ```
 
-## openi.dataset.upload_file()
+## 使用说明
 
-> 上传数据集函数
+- 确保您拥有此数据集（项目）的权限，`username`参数为数据集的创建者，即项目所属用户/组织的名称
+- 使用前请在平台个人设置中获取token：[点击跳转token获取界面](https://openi.pcl.ac.cn/user/settings/applications)
+- 当前版本为了方便用户本地上传数据集，建议在本地使用，后续版本将适配隐藏token参数、代码仓配置及云脑任务
 
-安装完成可仿照下列示，运行即可上传数据集
+## 本地上传数据集示例
 
 ```python
 from openi.dataset import upload_file
 
 upload_file(
-    file = "", # 必填，文件路径(包含文件名)
-    username = "", # 必填，数据集所属项目用户名
-    repository = "", # 必填，数据集所属项目名
+    file = "", # 必填，文件路径(包含文件名，支持windows文件路径如d:\\xxx)
+    username = "", # 必填，数据集所属项目owner用户名
+    repository = "", # 必填，数据集所属项目名称
     token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
     
-    cluster = "", # 选填，可填入GPU或NPU，不填写后台默认为NPU
-    app_url = "" #选填, 默认为平台地址，开发测试用
+    cluster = "" # 选填，可填入GPU或NPU，不填写后台默认为NPU
     )
 ```
-![alt](https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi/raw/commit/7d3365f667974c5a06aaeb390003a3b929fde0d9/media/4.png)
+![alt](./media/4.png)
```

### Comparing `openi-beta-0.0.5/test/test_thread.py` & `openi-beta-0.0.6/test/test_thread.py`

 * *Files identical despite different names*

