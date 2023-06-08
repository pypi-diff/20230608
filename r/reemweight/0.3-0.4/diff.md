# Comparing `tmp/reemweight-0.3.tar.gz` & `tmp/reemweight-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reemweight-0.3.tar", last modified: Thu Jun  8 12:33:59 2023, max compression
+gzip compressed data, was "reemweight-0.4.tar", last modified: Thu Jun  8 12:46:05 2023, max compression
```

## Comparing `reemweight-0.3.tar` & `reemweight-0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 12:33:59.994493 reemweight-0.3/
--rw-rw-rw-   0        0        0     1063 2023-03-22 13:24:02.000000 reemweight-0.3/LICENCE.txt
--rw-rw-rw-   0        0        0      676 2023-06-08 12:33:59.994493 reemweight-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-03-22 13:20:49.000000 reemweight-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 12:33:59.978828 reemweight-0.3/reemweight/
--rw-rw-rw-   0        0        0      117 2023-06-08 12:27:17.000000 reemweight-0.3/reemweight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:33:59.978828 reemweight-0.3/reemweight.egg-info/
--rw-rw-rw-   0        0        0      676 2023-06-08 12:33:59.000000 reemweight-0.3/reemweight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-06-08 12:33:59.000000 reemweight-0.3/reemweight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 12:33:59.000000 reemweight-0.3/reemweight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-08 12:33:59.000000 reemweight-0.3/reemweight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 12:33:59.996497 reemweight-0.3/setup.cfg
--rw-rw-rw-   0        0        0      723 2023-06-08 12:33:20.000000 reemweight-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:05.984548 reemweight-0.4/
+-rw-rw-rw-   0        0        0     1063 2023-03-22 13:24:02.000000 reemweight-0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0      676 2023-06-08 12:46:05.983532 reemweight-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-03-22 13:20:49.000000 reemweight-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:05.966014 reemweight-0.4/reemweight/
+-rw-rw-rw-   0        0        0      117 2023-06-08 12:27:17.000000 reemweight-0.4/reemweight/__init__.py
+-rw-rw-rw-   0        0        0      921 2023-06-08 12:33:25.000000 reemweight-0.4/reemweight/data_examiner.py
+-rw-rw-rw-   0        0        0     7911 2023-06-08 12:33:28.000000 reemweight-0.4/reemweight/linear.py
+-rw-rw-rw-   0        0        0     9945 2023-06-08 12:33:30.000000 reemweight-0.4/reemweight/nonLinear.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:46:05.981354 reemweight-0.4/reemweight.egg-info/
+-rw-rw-rw-   0        0        0      676 2023-06-08 12:46:05.000000 reemweight-0.4/reemweight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-08 12:46:05.000000 reemweight-0.4/reemweight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:46:05.000000 reemweight-0.4/reemweight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 12:46:05.000000 reemweight-0.4/reemweight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 12:46:05.984548 reemweight-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      723 2023-06-08 12:45:56.000000 reemweight-0.4/setup.py
```

### Comparing `reemweight-0.3/LICENCE.txt` & `reemweight-0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `reemweight-0.3/PKG-INFO` & `reemweight-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reemweight
-Version: 0.3
+Version: 0.4
 Summary: <The Python package is designed to assist with the initialization of weights in a neural network sequential model. The package uses machine learning algorithms (MLAs) to initialize the weights, which can lead to improved model performance. Additionally, the package provides a means to compare the results of this weight strategy with other weight initialization strategies.>
 Author: Reem Almoshbb
 Author-email: rsalmoshbb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENCE.txt
```

### Comparing `reemweight-0.3/reemweight.egg-info/PKG-INFO` & `reemweight-0.4/reemweight.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reemweight
-Version: 0.3
+Version: 0.4
 Summary: <The Python package is designed to assist with the initialization of weights in a neural network sequential model. The package uses machine learning algorithms (MLAs) to initialize the weights, which can lead to improved model performance. Additionally, the package provides a means to compare the results of this weight strategy with other weight initialization strategies.>
 Author: Reem Almoshbb
 Author-email: rsalmoshbb@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENCE.txt
```

### Comparing `reemweight-0.3/setup.py` & `reemweight-0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
  name='reemweight', 
- version='0.3',
+ version='0.4',
  author="Reem Almoshbb",
  author_email="rsalmoshbb@gmail.com",
  description="<The Python package is designed to assist with the initialization of weights in a neural network sequential model. The package uses machine learning algorithms (MLAs) to initialize the weights, which can lead to improved model performance. Additionally, the package provides a means to compare the results of this weight strategy with other weight initialization strategies.>",
  packages=setuptools.find_packages(),
  classifiers=[
  "Programming Language :: Python :: 3",
  "License :: OSI Approved :: MIT License",
```

