# Comparing `tmp/iOSReSignApp-1.5.5.tar.gz` & `tmp/iOSReSignApp-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iOSReSignApp-1.5.5.tar", last modified: Wed Mar  1 15:43:54 2023, max compression
+gzip compressed data, was "iOSReSignApp-1.5.6.tar", last modified: Thu Jun  8 07:09:41 2023, max compression
```

## Comparing `iOSReSignApp-1.5.5.tar` & `iOSReSignApp-1.5.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-03-01 15:43:54.827329 iOSReSignApp-1.5.5/
--rw-r--r--   0 shaowei    (501) staff       (20)     1065 2019-05-17 03:04:35.000000 iOSReSignApp-1.5.5/LICENSE
--rw-r--r--   0 shaowei    (501) staff       (20)     5764 2023-03-01 15:43:54.827144 iOSReSignApp-1.5.5/PKG-INFO
--rw-r--r--   0 shaowei    (501) staff       (20)     4850 2022-02-17 10:04:33.000000 iOSReSignApp-1.5.5/README.md
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-03-01 15:43:54.825106 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/
--rw-r--r--   0 shaowei    (501) staff       (20)     5764 2023-03-01 15:43:54.000000 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/PKG-INFO
--rw-r--r--   0 shaowei    (501) staff       (20)      387 2023-03-01 15:43:54.000000 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/SOURCES.txt
--rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-03-01 15:43:54.000000 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/dependency_links.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       60 2023-03-01 15:43:54.000000 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/entry_points.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       45 2023-03-01 15:43:54.000000 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/requires.txt
--rw-r--r--   0 shaowei    (501) staff       (20)       13 2023-03-01 15:43:54.000000 iOSReSignApp-1.5.5/iOSReSignApp.egg-info/top_level.txt
-drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-03-01 15:43:54.826718 iOSReSignApp-1.5.5/iosresignapp/
--rw-r--r--   0 shaowei    (501) staff       (20)      107 2020-04-17 03:18:40.000000 iOSReSignApp-1.5.5/iosresignapp/__init__.py
--rw-r--r--   0 shaowei    (501) staff       (20)     1930 2023-03-01 15:41:08.000000 iOSReSignApp-1.5.5/iosresignapp/codesign.py
--rw-r--r--   0 shaowei    (501) staff       (20)     2772 2021-06-15 08:15:33.000000 iOSReSignApp-1.5.5/iosresignapp/command.py
--rw-r--r--   0 shaowei    (501) staff       (20)     9922 2023-03-01 15:42:07.000000 iOSReSignApp-1.5.5/iosresignapp/resign.py
--rw-r--r--   0 shaowei    (501) staff       (20)     1613 2020-04-17 03:18:40.000000 iOSReSignApp-1.5.5/iosresignapp/security.py
--rw-r--r--   0 shaowei    (501) staff       (20)      165 2020-04-17 03:18:40.000000 iOSReSignApp-1.5.5/iosresignapp/util.py
--rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-03-01 15:43:54.827397 iOSReSignApp-1.5.5/setup.cfg
--rw-r--r--   0 shaowei    (501) staff       (20)     1543 2023-03-01 15:42:30.000000 iOSReSignApp-1.5.5/setup.py
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-08 07:09:41.799917 iOSReSignApp-1.5.6/
+-rw-r--r--   0 shaowei    (501) staff       (20)     1065 2019-05-17 03:04:35.000000 iOSReSignApp-1.5.6/LICENSE
+-rw-r--r--   0 shaowei    (501) staff       (20)     5764 2023-06-08 07:09:41.799717 iOSReSignApp-1.5.6/PKG-INFO
+-rw-r--r--   0 shaowei    (501) staff       (20)     4850 2022-02-17 10:04:33.000000 iOSReSignApp-1.5.6/README.md
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-08 07:09:41.797258 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/
+-rw-r--r--   0 shaowei    (501) staff       (20)     5764 2023-06-08 07:09:41.000000 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/PKG-INFO
+-rw-r--r--   0 shaowei    (501) staff       (20)      387 2023-06-08 07:09:41.000000 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/SOURCES.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)        1 2023-06-08 07:09:41.000000 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/dependency_links.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       60 2023-06-08 07:09:41.000000 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/entry_points.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       45 2023-06-08 07:09:41.000000 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/requires.txt
+-rw-r--r--   0 shaowei    (501) staff       (20)       13 2023-06-08 07:09:41.000000 iOSReSignApp-1.5.6/iOSReSignApp.egg-info/top_level.txt
+drwxr-xr-x   0 shaowei    (501) staff       (20)        0 2023-06-08 07:09:41.799247 iOSReSignApp-1.5.6/iosresignapp/
+-rw-r--r--   0 shaowei    (501) staff       (20)      107 2020-04-17 03:18:40.000000 iOSReSignApp-1.5.6/iosresignapp/__init__.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     1930 2023-03-01 15:41:08.000000 iOSReSignApp-1.5.6/iosresignapp/codesign.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     2772 2021-06-15 08:15:33.000000 iOSReSignApp-1.5.6/iosresignapp/command.py
+-rw-r--r--   0 shaowei    (501) staff       (20)    10285 2023-06-08 07:05:48.000000 iOSReSignApp-1.5.6/iosresignapp/resign.py
+-rw-r--r--   0 shaowei    (501) staff       (20)     1613 2020-04-17 03:18:40.000000 iOSReSignApp-1.5.6/iosresignapp/security.py
+-rw-r--r--   0 shaowei    (501) staff       (20)      165 2020-04-17 03:18:40.000000 iOSReSignApp-1.5.6/iosresignapp/util.py
+-rw-r--r--   0 shaowei    (501) staff       (20)       38 2023-06-08 07:09:41.799997 iOSReSignApp-1.5.6/setup.cfg
+-rw-r--r--   0 shaowei    (501) staff       (20)     1543 2023-06-08 07:06:56.000000 iOSReSignApp-1.5.6/setup.py
```

### Comparing `iOSReSignApp-1.5.5/LICENSE` & `iOSReSignApp-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iOSReSignApp-1.5.5/PKG-INFO` & `iOSReSignApp-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iOSReSignApp
-Version: 1.5.5
+Version: 1.5.6
 Summary: UNKNOWN
 Home-page: https://github.com/shede333/iOSReSignApp
 Author: shede333
 Author-email: 333wshw@163.com
 License: UNKNOWN
 Keywords: codesign ios resign re-sign re_sign re sign app
 Platform: UNKNOWN
```

### Comparing `iOSReSignApp-1.5.5/README.md` & `iOSReSignApp-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `iOSReSignApp-1.5.5/iOSReSignApp.egg-info/PKG-INFO` & `iOSReSignApp-1.5.6/iOSReSignApp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iOSReSignApp
-Version: 1.5.5
+Version: 1.5.6
 Summary: UNKNOWN
 Home-page: https://github.com/shede333/iOSReSignApp
 Author: shede333
 Author-email: 333wshw@163.com
 License: UNKNOWN
 Keywords: codesign ios resign re-sign re_sign re sign app
 Platform: UNKNOWN
```

### Comparing `iOSReSignApp-1.5.5/iosresignapp/codesign.py` & `iOSReSignApp-1.5.6/iosresignapp/codesign.py`

 * *Files identical despite different names*

### Comparing `iOSReSignApp-1.5.5/iosresignapp/command.py` & `iOSReSignApp-1.5.6/iosresignapp/command.py`

 * *Files identical despite different names*

### Comparing `iOSReSignApp-1.5.5/iosresignapp/resign.py` & `iOSReSignApp-1.5.6/iosresignapp/resign.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from iosappinfoparser.info_plist import change_app_display_name
 from mobileprovision import MobileProvisionModel
 from mobileprovision import util as mp_util
 
 from . import codesign
 from . import security
 from .util import plog
+from datetime import datetime
 
 
 class ResignException(Exception):
     pass
 
 
 def zip_payload(payload_path, ipa_path):
@@ -102,15 +103,19 @@
     # 处理冲突参数
     if output_ipa_path and re_suffix_name:
         raise ResignException("不能同时设置： output_ipa_path 与 re_suffix_name ")
 
     # 解析mobileprovision文件里的有效信息
     mp_model = parse_mobileprovision(mobileprovision_info)
     if not mp_model.date_is_valid():
-        raise ResignException("mobileprovision 已过期")
+        profile_info = f"{mp_model.name}, {mp_model.app_id_name}, {mp_model.uuid}"
+        time_info = f"create time: {mp_model.creation_timestamp}, "
+        time_info += f"current utc time: {datetime.utcnow().timestamp()}, "
+        time_info += f"expiration time: {mp_model.expiration_timestamp}, "
+        raise ResignException(f"mobileprovision({profile_info}), 已过期: {time_info}")
     # 查找p12文件的签名ID：sha1
     id_model_list = security.security_find_identity()
     valid_sha1_set = set((tmp_model.sha1 for tmp_model in id_model_list if tmp_model.is_valid))
     if not valid_sha1_set:
         raise ResignException("钥匙串里 不存在有效的签名证书sign!")
     if sign:
         invalid_sha1_set = set(
```

### Comparing `iOSReSignApp-1.5.5/iosresignapp/security.py` & `iOSReSignApp-1.5.6/iosresignapp/security.py`

 * *Files identical despite different names*

### Comparing `iOSReSignApp-1.5.5/setup.py` & `iOSReSignApp-1.5.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("README.md").read_text()
 
 print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='iOSReSignApp',  # 包名字
-    version='1.5.5',  # 包版本
+    version='1.5.6',  # 包版本
     author='shede333',  # 作者
     author_email='333wshw@163.com',  # 作者邮箱
     keywords='codesign ios resign re-sign re_sign re sign app',
     description='',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/shede333/iOSReSignApp',  # 包的主页
```

