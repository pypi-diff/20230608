# Comparing `tmp/yplib-0.0.5.tar.gz` & `tmp/yplib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.0.5.tar", last modified: Thu Jun  8 03:15:00 2023, max compression
+gzip compressed data, was "dist\yplib-0.0.7.tar", last modified: Thu Jun  8 03:18:34 2023, max compression
```

## Comparing `yplib-0.0.5.tar` & `yplib-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 03:15:00.792461 yplib-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-08 03:15:00.791885 yplib-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 03:15:00.792740 yplib-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-08 03:14:56.000000 yplib-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:15:00.788529 yplib-0.0.5/yplib/
--rw-rw-rw-   0        0        0     2864 2023-06-08 03:14:40.000000 yplib-0.0.5/yplib/__init__.py
--rw-rw-rw-   0        0        0       43 2023-06-08 00:54:48.000000 yplib-0.0.5/yplib/example.py
-drwxrwxrwx   0        0        0        0 2023-06-08 03:15:00.791246 yplib-0.0.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-08 03:15:00.000000 yplib-0.0.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-08 03:15:00.000000 yplib-0.0.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 03:15:00.000000 yplib-0.0.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 03:15:00.000000 yplib-0.0.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 03:18:34.475913 yplib-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-08 03:18:34.475790 yplib-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 03:18:34.475913 yplib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-08 03:18:24.000000 yplib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:18:34.473039 yplib-0.0.7/yplib/
+-rw-rw-rw-   0        0        0     3155 2023-06-08 03:18:17.000000 yplib-0.0.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-06-08 00:54:48.000000 yplib-0.0.7/yplib/example.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:18:34.475178 yplib-0.0.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 03:18:34.000000 yplib-0.0.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.0.5/LICENSE` & `yplib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.0.5/PKG-INFO` & `yplib-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.0.5
+Version: 0.0.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.0.5/setup.py` & `yplib-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.0.5",
+  version="0.0.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.0.5/yplib/__init__.py` & `yplib-0.0.7/yplib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,22 +56,29 @@
     # 3. 添加Excel工作表
     mySheet = myWorkbook.add_sheet(str(file_name))
     # 4. 写入数据
     # myStyle = xlwt.easyxf('font: name Times New Roman, color-index red, bold on')  # 数据格式
     m = 0
     for one_data in list_data:
         n = 0
-        for one in one_data:
-            # mySheet.write(n, m, one)  # 写入A3，数值等于1
-            if isinstance(one, dict) or isinstance(one, list):
-                s = json.dumps(one)
+        if isinstance(one_data, list):
+            for one in one_data:
+                # mySheet.write(n, m, one)  # 写入A3，数值等于1
+                if isinstance(one, dict) or isinstance(one, list):
+                    s = json.dumps(one)
+                else:
+                    s = str(one)
+                mySheet.write(m, n, s)  # 写入A3，数值等于1
+                n += 1
+        else:
+            if isinstance(one_data, dict):
+                s = json.dumps(one_data)
             else:
-                s = str(one)
+                s = str(one_data)
             mySheet.write(m, n, s)  # 写入A3，数值等于1
-            n += 1
         m += 1
     # 5. 保存
     # myWorkbook.save('5002200.xls')
     myWorkbook.save(file_path + '/' + get_file_name(file_name, '.xls'))
 
 
 # 将 excel 文件读取到 list 中, 单元格中的空格自动过滤掉了
```

### Comparing `yplib-0.0.5/yplib.egg-info/PKG-INFO` & `yplib-0.0.7/yplib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.0.5
+Version: 0.0.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

