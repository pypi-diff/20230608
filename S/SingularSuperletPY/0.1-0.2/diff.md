# Comparing `tmp/SingularSuperletPY-0.1.tar.gz` & `tmp/SingularSuperletPY-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SingularSuperletPY-0.1.tar", last modified: Thu Jun  8 13:34:59 2023, max compression
+gzip compressed data, was "SingularSuperletPY-0.2.tar", last modified: Thu Jun  8 13:46:58 2023, max compression
```

## Comparing `SingularSuperletPY-0.1.tar` & `SingularSuperletPY-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:34:59.085255 SingularSuperletPY-0.1/
--rw-rw-rw-   0        0        0       17 2023-06-08 13:23:54.000000 SingularSuperletPY-0.1/LICENCE.txt
--rw-rw-rw-   0        0        0     1015 2023-06-08 13:34:59.085255 SingularSuperletPY-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2497 2023-06-08 13:33:23.000000 SingularSuperletPY-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 13:34:59.065238 SingularSuperletPY-0.1/SingularSuperletPY/
--rw-rw-rw-   0        0        0        0 2023-06-08 13:04:52.000000 SingularSuperletPY-0.1/SingularSuperletPY/__init__py.py
--rw-rw-rw-   0        0        0     1272 2023-06-08 12:36:49.000000 SingularSuperletPY-0.1/SingularSuperletPY/cwt.py
--rw-rw-rw-   0        0        0      991 2023-06-08 09:40:17.000000 SingularSuperletPY-0.1/SingularSuperletPY/generateData.py
--rw-rw-rw-   0        0        0     3104 2023-06-08 13:02:40.000000 SingularSuperletPY-0.1/SingularSuperletPY/run.py
--rw-rw-rw-   0        0        0     1350 2023-06-08 10:41:16.000000 SingularSuperletPY-0.1/SingularSuperletPY/sst.py
--rw-rw-rw-   0        0        0      859 2023-06-08 10:24:31.000000 SingularSuperletPY-0.1/SingularSuperletPY/waveletHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:34:59.085255 SingularSuperletPY-0.1/SingularSuperletPY.egg-info/
--rw-rw-rw-   0        0        0     1015 2023-06-08 13:34:59.000000 SingularSuperletPY-0.1/SingularSuperletPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-08 13:34:59.000000 SingularSuperletPY-0.1/SingularSuperletPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:34:59.000000 SingularSuperletPY-0.1/SingularSuperletPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 13:34:59.000000 SingularSuperletPY-0.1/SingularSuperletPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-08 13:34:59.000000 SingularSuperletPY-0.1/SingularSuperletPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-08 13:34:59.086762 SingularSuperletPY-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1920 2023-06-08 13:20:20.000000 SingularSuperletPY-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:46:58.491895 SingularSuperletPY-0.2/
+-rw-rw-rw-   0        0        0       17 2023-06-08 13:23:54.000000 SingularSuperletPY-0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0     1015 2023-06-08 13:46:58.491895 SingularSuperletPY-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2497 2023-06-08 13:33:23.000000 SingularSuperletPY-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 13:46:58.481106 SingularSuperletPY-0.2/SingularSuperletPY/
+-rw-rw-rw-   0        0        0      254 2023-06-08 13:43:46.000000 SingularSuperletPY-0.2/SingularSuperletPY/__init__py.py
+-rw-rw-rw-   0        0        0     1272 2023-06-08 12:36:49.000000 SingularSuperletPY-0.2/SingularSuperletPY/cwt.py
+-rw-rw-rw-   0        0        0      991 2023-06-08 09:40:17.000000 SingularSuperletPY-0.2/SingularSuperletPY/generateData.py
+-rw-rw-rw-   0        0        0     3104 2023-06-08 13:02:40.000000 SingularSuperletPY-0.2/SingularSuperletPY/run.py
+-rw-rw-rw-   0        0        0     1350 2023-06-08 10:41:16.000000 SingularSuperletPY-0.2/SingularSuperletPY/sst.py
+-rw-rw-rw-   0        0        0      859 2023-06-08 10:24:31.000000 SingularSuperletPY-0.2/SingularSuperletPY/waveletHelper.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:46:58.490902 SingularSuperletPY-0.2/SingularSuperletPY.egg-info/
+-rw-rw-rw-   0        0        0     1015 2023-06-08 13:46:58.000000 SingularSuperletPY-0.2/SingularSuperletPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-08 13:46:58.000000 SingularSuperletPY-0.2/SingularSuperletPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 13:46:58.000000 SingularSuperletPY-0.2/SingularSuperletPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-08 13:46:58.000000 SingularSuperletPY-0.2/SingularSuperletPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-08 13:46:58.000000 SingularSuperletPY-0.2/SingularSuperletPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-08 13:46:58.492879 SingularSuperletPY-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1920 2023-06-08 13:46:42.000000 SingularSuperletPY-0.2/setup.py
```

### Comparing `SingularSuperletPY-0.1/PKG-INFO` & `SingularSuperletPY-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SingularSuperletPY
-Version: 0.1
+Version: 0.2
 Summary: Python repo for Singular Superlet Transform (SST)
 Home-page: https://https://github.com/KaanKesgin/SingularSuperletPY
-Download-URL: https://github.com/KaanKesgin/SingularSuperletPY/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/KaanKesgin/SingularSuperletPY/archive/refs/tags/v_02.tar.gz
 Author: Kaan Kesgin
 Author-email: kesginkaan@gmail.com
 License: MIT
 Keywords: time-frequency decomposition,signal processing,wavelet transform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `SingularSuperletPY-0.1/README.md` & `SingularSuperletPY-0.2/README.md`

 * *Files identical despite different names*

### Comparing `SingularSuperletPY-0.1/SingularSuperletPY/cwt.py` & `SingularSuperletPY-0.2/SingularSuperletPY/cwt.py`

 * *Files identical despite different names*

### Comparing `SingularSuperletPY-0.1/SingularSuperletPY/generateData.py` & `SingularSuperletPY-0.2/SingularSuperletPY/generateData.py`

 * *Files identical despite different names*

### Comparing `SingularSuperletPY-0.1/SingularSuperletPY/run.py` & `SingularSuperletPY-0.2/SingularSuperletPY/run.py`

 * *Files identical despite different names*

### Comparing `SingularSuperletPY-0.1/SingularSuperletPY/sst.py` & `SingularSuperletPY-0.2/SingularSuperletPY/sst.py`

 * *Files identical despite different names*

### Comparing `SingularSuperletPY-0.1/SingularSuperletPY/waveletHelper.py` & `SingularSuperletPY-0.2/SingularSuperletPY/waveletHelper.py`

 * *Files identical despite different names*

### Comparing `SingularSuperletPY-0.1/SingularSuperletPY.egg-info/PKG-INFO` & `SingularSuperletPY-0.2/SingularSuperletPY.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SingularSuperletPY
-Version: 0.1
+Version: 0.2
 Summary: Python repo for Singular Superlet Transform (SST)
 Home-page: https://https://github.com/KaanKesgin/SingularSuperletPY
-Download-URL: https://github.com/KaanKesgin/SingularSuperletPY/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/KaanKesgin/SingularSuperletPY/archive/refs/tags/v_02.tar.gz
 Author: Kaan Kesgin
 Author-email: kesginkaan@gmail.com
 License: MIT
 Keywords: time-frequency decomposition,signal processing,wavelet transform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `SingularSuperletPY-0.1/setup.py` & `SingularSuperletPY-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'SingularSuperletPY',      # How you named your package folder
   packages = ['SingularSuperletPY'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Python repo for Singular Superlet Transform (SST)',   # Give a short description about your library
   author = 'Kaan Kesgin',                   # Type in your name
   author_email = 'kesginkaan@gmail.com',      # Type in your E-Mail
   url = 'https://https://github.com/KaanKesgin/SingularSuperletPY',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/KaanKesgin/SingularSuperletPY/archive/refs/tags/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/KaanKesgin/SingularSuperletPY/archive/refs/tags/v_02.tar.gz',    # I explain this later on
   keywords = ['time-frequency decomposition', 'signal processing', 'wavelet transform'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'matplotlib',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

