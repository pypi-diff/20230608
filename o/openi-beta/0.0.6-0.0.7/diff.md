# Comparing `tmp/openi-beta-0.0.6.tar.gz` & `tmp/openi-beta-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.0.6.tar", last modified: Thu Jun  8 02:47:07 2023, max compression
+gzip compressed data, was "openi-beta-0.0.7.tar", last modified: Thu Jun  8 09:49:37 2023, max compression
```

## Comparing `openi-beta-0.0.6.tar` & `openi-beta-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.346746 openi-beta-0.0.6/
--rw-r--r--   0 jochen10518   (501) staff       (20)     1808 2023-06-08 02:47:07.346615 openi-beta-0.0.6/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1178 2023-06-07 10:31:58.000000 openi-beta-0.0.6/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-08 02:47:07.346792 openi-beta-0.0.6/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      976 2023-06-08 02:25:02.000000 openi-beta-0.0.6/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.343836 openi-beta-0.0.6/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.344597 openi-beta-0.0.6/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-08 01:13:13.000000 openi-beta-0.0.6/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-08 02:31:58.000000 openi-beta-0.0.6/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.345173 openi-beta-0.0.6/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.6/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     9560 2023-06-08 02:44:34.000000 openi-beta-0.0.6/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.345975 openi-beta-0.0.6/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     1808 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      344 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-08 02:47:07.000000 openi-beta-0.0.6/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 02:47:07.346349 openi-beta-0.0.6/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      605 2023-06-01 03:43:28.000000 openi-beta-0.0.6/test/test.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      904 2023-06-01 03:43:28.000000 openi-beta-0.0.6/test/test_thread.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.681008 openi-beta-0.0.7/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2103 2023-06-08 09:49:37.680873 openi-beta-0.0.7/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-08 09:39:38.000000 openi-beta-0.0.7/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-08 09:49:37.681073 openi-beta-0.0.7/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)      976 2023-06-08 09:49:30.000000 openi-beta-0.0.7/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.678171 openi-beta-0.0.7/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.678916 openi-beta-0.0.7/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-08 08:37:15.000000 openi-beta-0.0.7/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-08 08:37:15.000000 openi-beta-0.0.7/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.679490 openi-beta-0.0.7/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-beta-0.0.7/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)     9661 2023-06-08 09:32:01.000000 openi-beta-0.0.7/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-08 09:49:37.680646 openi-beta-0.0.7/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2103 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      311 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-08 09:49:37.000000 openi-beta-0.0.7/src/openi_beta.egg-info/top_level.txt
```

### Comparing `openi-beta-0.0.6/PKG-INFO` & `openi-beta-0.0.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,39 @@
-Metadata-Version: 2.1
-Name: openi-beta
-Version: 0.0.6
-Summary: A test packages for openi pypi
-Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
-Author: chenzh05
-Author-email: chenzh.ds@outlook.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # OpenI PyPi
 
 > PYPI package for 启智AI协作平台。
 
 启智平台提供的Python工具包，使用户能在本地上传数据集。
 
 ## 安装
 
 *适配python3.6及以上版本*
 ```bash
 pip install openi
 ```
 
 ## 使用说明
-
-- 确保您拥有此数据集（项目）的权限，`username`参数为数据集的创建者，即项目所属用户/组织的名称
 - 使用前请在平台个人设置中获取token：[点击跳转token获取界面](https://openi.pcl.ac.cn/user/settings/applications)
-- 当前版本为了方便用户本地上传数据集，建议在本地使用，后续版本将适配隐藏token参数、代码仓配置及云脑任务
+- 当前版本为了解决用户上传数据集的需求，建议在本地使用。后续版本将适配代码仓配置、隐藏token及云脑任务。
 
 ## 本地上传数据集示例
+**dataset.upload_file(file, username, repository, token, cluster = "NPU")** 
+
+*上传本地单个文件到启智平台数据集，支持断点续传*
 
+- `file`        **str, 必填**：文件路径(包含文件名，支持linux与mac路径，也支持windows文件路径如d:\\xxx)
+- `username`    **str, 必填**：上传数据集所属项目owner用户名，可以是用户或组织
+- `repository`  **str, 必填**：数据集所属项目路径，此为仓库地址中的名字，更改过名称的项目需填写仓库地址中的路径
+- `token`       **str, 必填**：用户启智上获取的令牌token，并对该数据集有权限
+- `cluster`     **str, 选填, 默认"NPU"**：可填入GPU或NPU，上传至不同的存储集群
 ```python
 from openi.dataset import upload_file
 
 upload_file(
-    file = "", # 必填，文件路径(包含文件名，支持windows文件路径如d:\\xxx)
-    username = "", # 必填，数据集所属项目owner用户名
-    repository = "", # 必填，数据集所属项目名称
-    token = "", #必填，用户启智上获取的令牌token，并对该项目数据集有权限
-    
-    cluster = "" # 选填，可填入GPU或NPU，不填写后台默认为NPU
+    file = "", 
+    username = "", 
+    repository = "", 
+    token = "", 
+    cluster = ""
     )
 ```
-![alt](./media/4.png)
+![alt](./media/4.png)
```

### Comparing `openi-beta-0.0.6/setup.py` & `openi-beta-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.0.6',
+    version='0.0.7',
     description='A test packages for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.0.6/src/openi/dataset/dataset.py` & `openi-beta-0.0.7/src/openi/dataset/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,16 +38,19 @@
         self.cluster = cluster
         self.app_url = app_url
 
         # preset variables
         # self.max_chunk_size = MAX_CHUNK_SIZE
         if cluster == "NPU":
             self.upload_type = 1
-        else:
+        elif cluster == "GPU":
             self.upload_type = 0
+        else:
+            raise ValueError(
+                f"❌ please enter a valid cluster name, 'GPU' or 'NPU'")
 
         if "\\" in self.filepath:
             self.filename = self.filepath.split("\\")[-1]
         else:
             self.filename = self.filepath.split("/")[-1]
 
         self.size = os.path.getsize(self.filepath)
@@ -218,15 +221,15 @@
         # checking upload status
         self.getChunks()
 
         # upload starts
         if self.uuid != '':
             if self.uploaded:
                 raise ValueError(
-                    f'❌ Upload failed: [{self.filename} - {self.cluster}], already exists in [{self.username}/{self.repo}] , cannot be uploaded again.')
+                    f'❌ Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
             else:
                 print(self.stdOut('continue upload...'))
                 uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
                 continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
                 # re-upload last chunk from checkpoint
                 if uploaded_chunks:
                     last_chunk_index = max(uploaded_chunks)
```

