# Comparing `tmp/BlaApi-1.3.tar.gz` & `tmp/BlaApi-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.3.tar", last modified: Wed May 24 21:54:38 2023, max compression
+gzip compressed data, was "dist\BlaApi-1.4.tar", last modified: Wed Jun  7 22:55:22 2023, max compression
```

## Comparing `BlaApi-1.3.tar` & `BlaApi-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 21:54:38.733148 BlaApi-1.3/
-drwxrwxrwx   0        0        0        0 2023-05-24 21:54:38.723631 BlaApi-1.3/BlaApi/
--rw-rw-rw-   0        0        0        0 2023-04-16 12:18:24.000000 BlaApi-1.3/BlaApi/__init__.py
--rw-rw-rw-   0        0        0     4012 2023-05-24 21:45:48.000000 BlaApi-1.3/BlaApi/client.py
--rw-rw-rw-   0        0        0     3857 2023-05-24 21:48:54.000000 BlaApi-1.3/BlaApi/diary.py
-drwxrwxrwx   0        0        0        0 2023-05-24 21:54:38.731130 BlaApi-1.3/BlaApi.egg-info/
--rw-rw-rw-   0        0        0     6155 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 21:54:38.000000 BlaApi-1.3/BlaApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-04-16 12:18:24.000000 BlaApi-1.3/LICENSE
--rw-rw-rw-   0        0        0     6155 2023-05-24 21:54:38.733148 BlaApi-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5504 2023-05-24 21:49:00.000000 BlaApi-1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 21:54:38.734152 BlaApi-1.3/setup.cfg
--rw-rw-rw-   0        0        0     3712 2023-05-24 21:54:24.000000 BlaApi-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 22:55:22.000000 BlaApi-1.4/
+drwxrwxrwx   0        0        0        0 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi/
+-rw-rw-rw-   0        0        0        0 2023-06-07 22:15:05.000000 BlaApi-1.4/BlaApi/__init__.py
+-rw-rw-rw-   0        0        0     4024 2023-06-07 22:31:28.000000 BlaApi-1.4/BlaApi/client.py
+-rw-rw-rw-   0        0        0     3857 2023-06-07 22:15:05.000000 BlaApi-1.4/BlaApi/diary.py
+drwxrwxrwx   0        0        0        0 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/
+-rw-rw-rw-   0        0        0     6133 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-07 22:15:05.000000 BlaApi-1.4/LICENSE
+-rw-rw-rw-   0        0        0     6133 2023-06-07 22:55:22.000000 BlaApi-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-06-07 22:16:04.000000 BlaApi-1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 22:55:22.000000 BlaApi-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3708 2023-06-07 22:42:26.000000 BlaApi-1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `BlaApi-1.3/BlaApi/client.py` & `BlaApi-1.4/BlaApi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import httpx
 from fake_useragent import UserAgent as ua
 
 class Client:
-    client = httpx.Client() # instanciate 
+    client = httpx.Client(verify=False) # instanciate 
     #! BLA credentials must be passed in as string
     def __init__(self, username: str, password: str):
         # Random UserAgent
         self.headers = {'UserAgent': str(ua().chrome)}
         self.username = username
         self.password = password
         self.token = self.login().get('token')
```

### Comparing `BlaApi-1.3/BlaApi/diary.py` & `BlaApi-1.4/BlaApi/diary.py`

 * *Files identical despite different names*

### Comparing `BlaApi-1.3/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.4/BlaApi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.3
+Version: 1.4
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+License: BSD-4
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # BLA-API-Wrapper.
 
 ## Description
 
-##### A light weight python library to interact with [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
+##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
 
 ### Table of Contents
 
 - [Installation](#Installation)
```

### Comparing `BlaApi-1.3/LICENSE` & `BlaApi-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.3/PKG-INFO` & `BlaApi-1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.3
+Version: 1.4
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+License: BSD-4
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # BLA-API-Wrapper.
 
 ## Description
 
-##### A light weight python library to interact with [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
+##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
 
 ### Table of Contents
 
 - [Installation](#Installation)
```

### Comparing `BlaApi-1.3/README.md` & `BlaApi-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BLA-API-Wrapper.
 
 ## Description
 
-##### A light weight python library to interact with [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
+##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
 
 ### Table of Contents
 
 - [Installation](#Installation)
```

### Comparing `BlaApi-1.3/setup.py` & `BlaApi-1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.3'
+VERSION = '1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
      'httpx', 'fake_useragent',
 ]
 
 # What packages are optional?
@@ -73,15 +73,15 @@
         except OSError:
             pass
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
-        os.system('py -m twine upload dist/*')
+        os.system('twine upload dist/*')
 
         self.status('Pushing git tags…')
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
@@ -103,19 +103,19 @@
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
-    license='MIT',
+    license='BSD-4',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
```

