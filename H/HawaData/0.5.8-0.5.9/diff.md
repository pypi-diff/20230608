# Comparing `tmp/HawaData-0.5.8.tar.gz` & `tmp/HawaData-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.8.tar", last modified: Wed May 31 13:02:28 2023, max compression
+gzip compressed data, was "HawaData-0.5.9.tar", last modified: Thu Jun  1 01:32:32 2023, max compression
```

## Comparing `HawaData-0.5.8.tar` & `HawaData-0.5.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.339717 HawaData-0.5.8/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.328223 HawaData-0.5.8/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2612 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2612 2023-05-31 13:02:28.339445 HawaData-0.5.8/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.8/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.329028 HawaData-0.5.8/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.8/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.331800 HawaData-0.5.8/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.8/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.8/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.8/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.8/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.8/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.333933 HawaData-0.5.8/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.8/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.8/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.8/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.8/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.8/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.336569 HawaData-0.5.8/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.8/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.8/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.8/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.8/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.8/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.338083 HawaData-0.5.8/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.8/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    26659 2023-05-31 12:59:00.000000 HawaData-0.5.8/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.8/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-31 13:02:28.339793 HawaData-0.5.8/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.8/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.338788 HawaData-0.5.8/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.8/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.128128 HawaData-0.5.9/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.118232 HawaData-0.5.9/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2638 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-01 01:32:32.000000 HawaData-0.5.9/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2638 2023-06-01 01:32:32.127901 HawaData-0.5.9/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.9/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.118746 HawaData-0.5.9/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.9/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.121218 HawaData-0.5.9/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.9/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.9/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.9/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.9/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.9/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.123071 HawaData-0.5.9/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.9/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.9/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.9/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3065 2023-06-01 01:31:26.000000 HawaData-0.5.9/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.9/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.125006 HawaData-0.5.9/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.9/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.9/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.9/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.9/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.9/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.126881 HawaData-0.5.9/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.9/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    26659 2023-05-31 12:59:00.000000 HawaData-0.5.9/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.9/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-01 01:32:32.128195 HawaData-0.5.9/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.9/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-01 01:32:32.127370 HawaData-0.5.9/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.9/test/test_query.py
```

### Comparing `HawaData-0.5.8/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.9/HawaData.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.8
+Version: 0.5.9
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -90,7 +90,8 @@
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
 - 0.5.6 add dim or field gender compare data to health api
 - 0.5.7 update describe_grade_text
 - 0.5.8 update other report text
+- 0.5.9 add grade periods
```

### Comparing `HawaData-0.5.8/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.9/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/PKG-INFO` & `HawaData-0.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.8
+Version: 0.5.9
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -90,7 +90,8 @@
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
 - 0.5.6 add dim or field gender compare data to health api
 - 0.5.7 update describe_grade_text
 - 0.5.8 update other report text
+- 0.5.9 add grade periods
```

### Comparing `HawaData-0.5.8/README.md` & `HawaData-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/base/db.py` & `HawaData-0.5.9/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/base/init.py` & `HawaData-0.5.9/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/common/data.py` & `HawaData-0.5.9/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/common/query.py` & `HawaData-0.5.9/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/common/utils.py` & `HawaData-0.5.9/hawa/common/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,9 +89,21 @@
         self.is_single_grade = len(self.grades) == 1
 
     @property
     def grade_name(self) -> str:
         return '、'.join([project.grade_simple[i] for i in self.grades]) + '年级'
 
     @property
+    def grade_periods(self):
+        res = set()
+        for g in self.grades:
+            if g <= 6:
+                res.add('小学')
+            elif g <= 9:
+                res.add('初中')
+            else:
+                res.add('高中')
+        return res
+
+    @property
     def grade_name_list(self) -> list[str]:
         return [f"{project.grade_simple[i]}年级" for i in self.grades]
```

### Comparing `HawaData-0.5.8/hawa/config.py` & `HawaData-0.5.9/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/data/klass.py` & `HawaData-0.5.9/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/data/school.py` & `HawaData-0.5.9/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/paper/health.py` & `HawaData-0.5.9/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/hawa/paper/mht.py` & `HawaData-0.5.9/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/setup.py` & `HawaData-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.8/test/test_query.py` & `HawaData-0.5.9/test/test_query.py`

 * *Files identical despite different names*

