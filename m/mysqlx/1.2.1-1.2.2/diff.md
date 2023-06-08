# Comparing `tmp/mysqlx-1.2.1.tar.gz` & `tmp/mysqlx-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.2.1.tar", last modified: Thu Jun  8 14:33:08 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.2.2.tar", last modified: Thu Jun  8 14:42:41 2023, max compression
```

## Comparing `mysqlx-1.2.1.tar` & `mysqlx-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:33:08.000000 mysqlx-1.2.1/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx/
--rw-rw-rw-   0        0        0     5484 2023-06-08 14:29:56.000000 mysqlx-1.2.1/mysqlx/coder.py
--rw-rw-rw-   0        0        0    10185 2023-06-07 12:34:06.000000 mysqlx-1.2.1/mysqlx/db.py
--rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.2.1/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.2.1/mysqlx/helper.py
--rw-rw-rw-   0        0        0    11033 2023-06-07 14:35:41.000000 mysqlx-1.2.1/mysqlx/orm.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.1/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.1/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      404 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      297 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-08 14:33:08.000000 mysqlx-1.2.1/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-08 14:33:08.000000 mysqlx-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 14:33:08.000000 mysqlx-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-08 14:32:48.000000 mysqlx-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:42:41.000000 mysqlx-1.2.2/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.2.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx/
+-rw-rw-rw-   0        0        0     5484 2023-06-08 14:29:56.000000 mysqlx-1.2.2/mysqlx/coder.py
+-rw-rw-rw-   0        0        0     1425 2023-06-08 14:27:56.000000 mysqlx-1.2.2/mysqlx/coder.tpl
+-rw-rw-rw-   0        0        0    10185 2023-06-07 12:34:06.000000 mysqlx-1.2.2/mysqlx/db.py
+-rw-rw-rw-   0        0        0     3370 2023-06-06 00:29:56.000000 mysqlx-1.2.2/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     5295 2023-06-06 23:27:22.000000 mysqlx-1.2.2/mysqlx/helper.py
+-rw-rw-rw-   0        0        0    11033 2023-06-07 14:35:41.000000 mysqlx-1.2.2/mysqlx/orm.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.2.2/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-06 08:06:39.000000 mysqlx-1.2.2/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      404 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      314 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 14:42:41.000000 mysqlx-1.2.2/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      404 2023-06-08 14:42:41.000000 mysqlx-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2598 2023-06-06 12:09:45.000000 mysqlx-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 14:42:41.000000 mysqlx-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-06-08 14:42:30.000000 mysqlx-1.2.2/setup.py
```

### Comparing `mysqlx-1.2.1/LICENSE` & `mysqlx-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/mysqlx/coder.py` & `mysqlx-1.2.2/mysqlx/coder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/mysqlx/db.py` & `mysqlx-1.2.2/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/mysqlx/dbx.py` & `mysqlx-1.2.2/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/mysqlx/helper.py` & `mysqlx-1.2.2/mysqlx/helper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/mysqlx/orm.py` & `mysqlx-1.2.2/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/README.md` & `mysqlx-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mysqlx-1.2.1/setup.py` & `mysqlx-1.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     packages=find_packages(),
     description="mysqlx is a simple python sql executor for MySQL like iBatis.",
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=3.0.3',
         'mysql-connector-python>=8.0.20',
     ],
-    version='1.2.1',
+    version='1.2.2',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'iBatis', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
-        '': ['*.rst', '*.txt'],
+        '': ['*.rst', '*.txt', '*.tpl'],
     },
     include_package_data=True,
     python_requires='>=3.4.0',
     zip_safe=False
 )
```

