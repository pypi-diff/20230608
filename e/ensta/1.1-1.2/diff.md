# Comparing `tmp/ensta-1.1.tar.gz` & `tmp/ensta-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensta-1.1.tar", last modified: Wed Jun  7 15:59:10 2023, max compression
+gzip compressed data, was "ensta-1.2.tar", last modified: Thu Jun  8 07:59:47 2023, max compression
```

## Comparing `ensta-1.1.tar` & `ensta-1.2.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:59:10.874178 ensta-1.1/
--rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3204 2023-06-07 15:59:10.874178 ensta-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2482 2023-06-07 13:14:08.000000 ensta-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 15:59:10.836592 ensta-1.1/ensta/
--rw-rw-rw-   0        0        0    15694 2023-06-07 07:35:55.000000 ensta-1.1/ensta/Guest.py
--rw-rw-rw-   0        0        0    19556 2023-06-07 15:50:54.000000 ensta-1.1/ensta/Host.py
--rw-rw-rw-   0        0        0       60 2023-06-07 07:03:08.000000 ensta-1.1/ensta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:59:10.870871 ensta-1.1/ensta/lib/
--rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-1.1/ensta/lib/Commons.py
--rw-rw-rw-   0        0        0      217 2023-06-05 12:51:10.000000 ensta-1.1/ensta/lib/Exceptions.py
--rw-rw-rw-   0        0        0      197 2023-06-07 07:37:50.000000 ensta-1.1/ensta/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:59:10.857563 ensta-1.1/ensta.egg-info/
--rw-rw-rw-   0        0        0     3204 2023-06-07 15:59:10.000000 ensta-1.1/ensta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-07 15:59:10.000000 ensta-1.1/ensta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:59:10.000000 ensta-1.1/ensta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 15:59:10.000000 ensta-1.1/ensta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-07 15:59:10.000000 ensta-1.1/ensta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-07 15:59:10.876765 ensta-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-06-07 15:59:01.000000 ensta-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.940869 ensta-1.2/
+-rw-rw-rw-   0        0        0     1081 2023-06-06 15:38:39.000000 ensta-1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3368 2023-06-08 07:59:47.940869 ensta-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2646 2023-06-08 05:38:39.000000 ensta-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.861935 ensta-1.2/ensta/
+-rw-rw-rw-   0        0        0    15694 2023-06-07 07:35:55.000000 ensta-1.2/ensta/Guest.py
+-rw-rw-rw-   0        0        0    19079 2023-06-08 07:49:39.000000 ensta-1.2/ensta/Host.py
+-rw-rw-rw-   0        0        0      203 2023-06-08 07:50:42.000000 ensta-1.2/ensta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.911749 ensta-1.2/ensta/data_classes/
+-rw-rw-rw-   0        0        0     1012 2023-06-08 07:22:37.000000 ensta-1.2/ensta/data_classes/Follower.py
+-rw-rw-rw-   0        0        0     1015 2023-06-08 07:47:56.000000 ensta-1.2/ensta/data_classes/Following.py
+-rw-rw-rw-   0        0        0      103 2023-06-08 07:48:06.000000 ensta-1.2/ensta/data_classes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.928180 ensta-1.2/ensta/lib/
+-rw-rw-rw-   0        0        0     1169 2023-06-07 07:34:14.000000 ensta-1.2/ensta/lib/Commons.py
+-rw-rw-rw-   0        0        0      331 2023-06-08 06:52:07.000000 ensta-1.2/ensta/lib/Exceptions.py
+-rw-rw-rw-   0        0        0      223 2023-06-08 07:17:03.000000 ensta-1.2/ensta/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:59:47.893445 ensta-1.2/ensta.egg-info/
+-rw-rw-rw-   0        0        0     3368 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 07:59:47.000000 ensta-1.2/ensta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-08 07:59:47.940869 ensta-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2023-06-08 07:57:10.000000 ensta-1.2/setup.py
```

### Comparing `ensta-1.1/LICENSE.txt` & `ensta-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensta-1.1/PKG-INFO` & `ensta-1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.1
+Version: 1.2
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.1.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.2.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -53,17 +53,19 @@
 host = Host(sessionid)
 result = host.follow_username("username")
 
 print(result)
 ```
 
 ## Session ID
-To get your instagram session id, follow these steps:
+To get your instagram SessionId, run the [**fetch-sessionid.py**](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script.
+
+Alternatively, you can follow these steps if the above method didn't work for you:
 - Open [instagram.com](https://instagram.com) in your browser
-- Open DevTools (Right Click > Inspect)
+- Open DevTools (Ctrl + Shift + I)
 - Go to **Application** tab
 - Expand **Cookies** tab, and click on the first item
 - Here you will find your Instagram User's current sessionid.
 - Copy it and pass it as an argument whenever you are using the [**Host Class**](https://github.com/diezo/ensta#host-mode).
 
 ## Examples
```

### Comparing `ensta-1.1/README.md` & `ensta-1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 host = Host(sessionid)
 result = host.follow_username("username")
 
 print(result)
 ```
 
 ## Session ID
-To get your instagram session id, follow these steps:
+To get your instagram SessionId, run the [**fetch-sessionid.py**](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script.
+
+Alternatively, you can follow these steps if the above method didn't work for you:
 - Open [instagram.com](https://instagram.com) in your browser
-- Open DevTools (Right Click > Inspect)
+- Open DevTools (Ctrl + Shift + I)
 - Go to **Application** tab
 - Expand **Cookies** tab, and click on the first item
 - Here you will find your Instagram User's current sessionid.
 - Copy it and pass it as an argument whenever you are using the [**Host Class**](https://github.com/diezo/ensta#host-mode).
 
 ## Examples
```

### Comparing `ensta-1.1/ensta/Guest.py` & `ensta-1.2/ensta/Guest.py`

 * *Files identical despite different names*

### Comparing `ensta-1.1/ensta/lib/Commons.py` & `ensta-1.2/ensta/lib/Commons.py`

 * *Files identical despite different names*

### Comparing `ensta-1.1/ensta.egg-info/PKG-INFO` & `ensta-1.2/ensta.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ensta
-Version: 1.1
+Version: 1.2
 Summary: Simple & Up-to-date Instagram API
 Home-page: https://github.com/diezo/ensta
-Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.1.tar.gz
+Download-URL: https://github.com/diezo/ensta/archive/refs/tags/v1.2.tar.gz
 Author: Deepak Soni
 Author-email: lonelycube@proton.me
 License: MIT
 Keywords: instagram,web,private,api,scraper,easy,download,upload
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -53,17 +53,19 @@
 host = Host(sessionid)
 result = host.follow_username("username")
 
 print(result)
 ```
 
 ## Session ID
-To get your instagram session id, follow these steps:
+To get your instagram SessionId, run the [**fetch-sessionid.py**](https://github.com/diezo/ensta/blob/master/fetch-sessionid.py) script.
+
+Alternatively, you can follow these steps if the above method didn't work for you:
 - Open [instagram.com](https://instagram.com) in your browser
-- Open DevTools (Right Click > Inspect)
+- Open DevTools (Ctrl + Shift + I)
 - Go to **Application** tab
 - Expand **Cookies** tab, and click on the first item
 - Here you will find your Instagram User's current sessionid.
 - Copy it and pass it as an argument whenever you are using the [**Host Class**](https://github.com/diezo/ensta#host-mode).
 
 ## Examples
```

### Comparing `ensta-1.1/setup.py` & `ensta-1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from distutils.core import setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="ensta",
-    packages=["ensta", "ensta.lib"],
-    version="1.1",
+    packages=["ensta", "ensta.lib", "ensta.data_classes"],
+    version="1.2",
     license="MIT",
     description="Simple & Up-to-date Instagram API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepak Soni",
     author_email="lonelycube@proton.me",
     url="https://github.com/diezo/ensta",
-    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.1.tar.gz",
+    download_url="https://github.com/diezo/ensta/archive/refs/tags/v1.2.tar.gz",
     keywords=["instagram", "web", "private", "api", "scraper", "easy", "download", "upload"],
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
```

