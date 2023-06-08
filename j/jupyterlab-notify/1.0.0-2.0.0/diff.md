# Comparing `tmp/jupyterlab_notify-1.0.0.tar.gz` & `tmp/jupyterlab_notify-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyterlab_notify-1.0.0.tar", last modified: Mon Jul 12 22:51:30 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_notify-1.0.0.tar` & `jupyterlab_notify-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/
--rw-r--r--   0 udoff      (501) staff       (20)     1503 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/LICENSE.txt
--rw-r--r--   0 udoff      (501) staff       (20)      446 2021-07-12 22:47:23.000000 jupyterlab_notify-1.0.0/MANIFEST.in
--rw-r--r--   0 udoff      (501) staff       (20)     6782 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)     6077 2021-06-26 13:54:52.000000 jupyterlab_notify-1.0.0/README.md
--rw-r--r--   0 udoff      (501) staff       (20)      200 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/install.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:29.000000 jupyterlab_notify-1.0.0/jupyter-config/
--rw-r--r--   0 udoff      (501) staff       (20)      109 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/jupyter-config/jupyterlab_notify.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/
--rw-r--r--   0 udoff      (501) staff       (20)      524 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/__init__.py
--rw-r--r--   0 udoff      (501) staff       (20)      441 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/_version.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/
--rw-r--r--   0 udoff      (501) staff       (20)    19592 2021-06-24 18:38:54.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/build_log.json
--rw-r--r--   0 udoff      (501) staff       (20)     2289 2021-06-24 18:38:55.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/package.json
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/static/
--rw-r--r--   0 udoff      (501) staff       (20)     4255 2021-06-24 18:38:55.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/static/lib_index_js.d51437c461ac03fb8217.js
--rw-r--r--   0 udoff      (501) staff       (20)     4026 2021-06-24 18:38:55.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/static/lib_index_js.d51437c461ac03fb8217.js.map
--rw-r--r--   0 udoff      (501) staff       (20)    26161 2021-06-24 18:38:55.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/static/remoteEntry.49909e0610d8a39ad5c6.js
--rw-r--r--   0 udoff      (501) staff       (20)    24913 2021-06-24 18:38:55.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/static/remoteEntry.49909e0610d8a39ad5c6.js.map
--rw-r--r--   0 udoff      (501) staff       (20)      118 2021-06-24 18:38:54.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/labextension/static/style.js
--rw-r--r--   0 udoff      (501) staff       (20)     7721 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/jupyterlab_notify/magics.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/
--rw-r--r--   0 udoff      (501) staff       (20)     6782 2021-07-12 22:51:29.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/PKG-INFO
--rw-r--r--   0 udoff      (501) staff       (20)      933 2021-07-12 22:51:29.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/SOURCES.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2021-07-12 22:51:29.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/dependency_links.txt
--rw-r--r--   0 udoff      (501) staff       (20)        1 2021-06-24 17:38:42.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/not-zip-safe
--rw-r--r--   0 udoff      (501) staff       (20)       16 2021-07-12 22:51:29.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/requires.txt
--rw-r--r--   0 udoff      (501) staff       (20)       18 2021-07-12 22:51:29.000000 jupyterlab_notify-1.0.0/jupyterlab_notify.egg-info/top_level.txt
--rw-r--r--   0 udoff      (501) staff       (20)     2367 2021-06-24 17:37:06.000000 jupyterlab_notify-1.0.0/package.json
--rw-r--r--   0 udoff      (501) staff       (20)      550 2021-06-29 11:59:17.000000 jupyterlab_notify-1.0.0/pyproject.toml
--rw-r--r--   0 udoff      (501) staff       (20)       38 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/setup.cfg
--rw-r--r--   0 udoff      (501) staff       (20)     2161 2021-07-12 22:47:29.000000 jupyterlab_notify-1.0.0/setup.py
-drwxr-xr-x   0 udoff      (501) staff       (20)        0 2021-07-12 22:51:30.000000 jupyterlab_notify-1.0.0/src/
--rw-r--r--   0 udoff      (501) staff       (20)     3678 2021-06-26 12:55:52.000000 jupyterlab_notify-1.0.0/src/index.ts
--rw-r--r--   0 udoff      (501) staff       (20)      555 2021-06-24 17:30:27.000000 jupyterlab_notify-1.0.0/tsconfig.json
--rw-r--r--   0 udoff      (501) staff       (20)   147762 2021-06-24 17:31:21.000000 jupyterlab_notify-1.0.0/yarn.lock
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/.gitattributes
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/install.json
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/package.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/tsconfig.json
+-rw-r--r--   0        0        0   186845 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/yarn.lock
+-rw-r--r--   0        0        0    51816 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/docs/notify-screenshot.png
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyter-config/jupyterlab_notify.json
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyter-config/nb-config/jupyterlab_notify.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyter-config/server-config/jupyterlab_notify.json
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/_version.py
+-rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/magics.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/labextension/package.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/labextension/static/568.e6579444d64100ce4ab5.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/labextension/static/747.a8203475eacf622d6015.js
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/labextension/static/remoteEntry.6c782a2e0710537488f0.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/jupyterlab_notify/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/notebooks/Notify.ipynb
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/style/index.js
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/README.md
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 jupyterlab_notify-2.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jupyterlab_notify-1.0.0/LICENSE.txt` & `jupyterlab_notify-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_notify-1.0.0/PKG-INFO` & `jupyterlab_notify-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,9 @@
-Metadata-Version: 2.1
-Name: jupyterlab_notify
-Version: 1.0.0
-Summary: JupyterLab extension to notify cell completion
-Home-page: https://github.com/deshaw/jupyterlab-notify
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # jupyterlab-notify
 
-
 [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-image]][pypi-url]
 [![Github Actions Status][github-status-image]][github-status-url] [![Binder][binder-image]][binder-url]
 
 JupyterLab extension to notify cell completion
 
 ![notify-extension-in-action](https://github.com/deshaw/jupyterlab-notify/blob/main/docs/notify-screenshot.png?raw=true)
 
@@ -36,14 +14,15 @@
 ### Register magics
 
 ```python
 %load_ext jupyterlab_notify
 ```
 
 ### Notify completion of single cell:
+
 ```python
 %%notify
 import time
 time.sleep(1)
 ```
 
 ### Mail output upon completion (with optional title for successfull execution)
@@ -53,60 +32,66 @@
 time.sleep(1)
 ```
 
 **Note:** Mail requires/assumes that you have an SMTP server running on "localhost" - refer [SMTP doc](https://docs.python.org/3/library/smtplib.html#smtplib.SMTP.connect) for more details.
 In case this assumption does not hold true for you, please open an issue with relevant details.
 
 ### Failure scenarios
+
 ```python
 %%notify -f 'Long-running cell in <foo> notebook failed'
 raise ValueError
 ```
 
 ### Threshold-based notifications (unit in seconds)
+
 ```python
 %notify_all --threshold 1
 time.sleep(1)
 ```
 
 Once enabled, `notify_all` will raise a notification for cells that either exceed the given threshold or raise exception. This ability can also be used to check if/when all cells in a notebook completes execution. For instance,
+
 ```python
 # In first cell
 %notify_all -t 86400 -f 'Notebook execution failed'
 # ...
 # ...
 # In last cell
 %%notify -s 'Notebook execution completed'
 ```
 
 ### Disable notifications
+
 ```python
 %notify_all --disable
 time.sleep(1)
 ```
 
 ### Learn more
+
 ```python
 %%notify?
 ```
 
 ```python
 %notify_all?
 ```
 
 ## Troubleshoot
 
 If you notice that the desktop notifications are not showing up, check the below:
+
 1. Make sure JupyterLab is running in a secure context (i.e. either using HTTPS or localhost)
 2. If you've previously denied notification permissions for the site, update the browser settings accordingly. In Chrome, you can do so by navigating to `Setttings -> Privacy and security -> Site Settings -> Notifications` and updating the permissions against your JupyterLab URL.
 3. Verify that notifications work for your browser. You may need to configure an OS setting first. You can test on [this site](https://web-push-book.gauntface.com/demos/notification-examples/).
 
 ## Requirements
 
-* JupyterLab >= 3.0
+- JupyterLab >= 4.0
 
 ## Install
 
 To install this package with [`pip`](https://pip.pypa.io/en/stable/) run
 
 ```bash
 pip install jupyterlab_notify
@@ -192,33 +177,33 @@
 
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab_notify
 ```
 
-
 ## History
 
 This plugin was contributed back to the community by the [D. E. Shaw group](https://www.deshaw.com/).
 
 <p align="center">
     <a href="https://www.deshaw.com">
        <img src="https://www.deshaw.com/assets/logos/blue_logo_417x125.png" alt="D. E. Shaw Logo" height="75" >
     </a>
 </p>
 
 ## License
 
 This project is released under a [BSD-3-Clause license](https://github.com/deshaw/jupyterlab-notify/blob/master/LICENSE.txt).
 
+We love contributions! Before you can contribute, please sign and submit this [Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla).
+This CLA is in place to protect all users of this project.
+
 "Jupyter" is a trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
 
 [pypi-url]: https://pypi.org/project/jupyterlab-notify
 [pypi-image]: https://img.shields.io/pypi/v/jupyterlab-notify
 [pypi-dm-image]: https://img.shields.io/pypi/dm/jupyterlab-notify
 [github-status-image]: https://github.com/deshaw/jupyterlab-notify/workflows/Build/badge.svg
 [github-status-url]: https://github.com/deshaw/jupyterlab-notify/actions?query=workflow%3ABuild
 [binder-image]: https://mybinder.org/badge_logo.svg
 [binder-url]: https://mybinder.org/v2/gh/deshaw/jupyterlab-notify.git/main?urlpath=lab%2Ftree%2Fnotebooks%2Findex.ipynb
-
-
```

### Comparing `jupyterlab_notify-1.0.0/README.md` & `jupyterlab_notify-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,60 @@
-# jupyterlab-notify
+Metadata-Version: 2.1
+Name: jupyterlab_notify
+Version: 2.0.0
+Summary: JupyterLab extension to notify cell completion
+Project-URL: Homepage, https://github.com/deshaw/jupyterlab-notify
+Project-URL: Bug Tracker, https://github.com/deshaw/jupyterlab-notify/issues
+Project-URL: Repository, https://github.com/deshaw/jupyterlab-notify.git
+License: Copyright 2021 D. E. Shaw & Co., L.P.
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE.txt
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
+Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: jupyter-server<3,>=2.0.1
+Description-Content-Type: text/markdown
 
+# jupyterlab-notify
 
 [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-image]][pypi-url]
 [![Github Actions Status][github-status-image]][github-status-url] [![Binder][binder-image]][binder-url]
 
 JupyterLab extension to notify cell completion
 
 ![notify-extension-in-action](https://github.com/deshaw/jupyterlab-notify/blob/main/docs/notify-screenshot.png?raw=true)
@@ -15,14 +66,15 @@
 ### Register magics
 
 ```python
 %load_ext jupyterlab_notify
 ```
 
 ### Notify completion of single cell:
+
 ```python
 %%notify
 import time
 time.sleep(1)
 ```
 
 ### Mail output upon completion (with optional title for successfull execution)
@@ -32,60 +84,66 @@
 time.sleep(1)
 ```
 
 **Note:** Mail requires/assumes that you have an SMTP server running on "localhost" - refer [SMTP doc](https://docs.python.org/3/library/smtplib.html#smtplib.SMTP.connect) for more details.
 In case this assumption does not hold true for you, please open an issue with relevant details.
 
 ### Failure scenarios
+
 ```python
 %%notify -f 'Long-running cell in <foo> notebook failed'
 raise ValueError
 ```
 
 ### Threshold-based notifications (unit in seconds)
+
 ```python
 %notify_all --threshold 1
 time.sleep(1)
 ```
 
 Once enabled, `notify_all` will raise a notification for cells that either exceed the given threshold or raise exception. This ability can also be used to check if/when all cells in a notebook completes execution. For instance,
+
 ```python
 # In first cell
 %notify_all -t 86400 -f 'Notebook execution failed'
 # ...
 # ...
 # In last cell
 %%notify -s 'Notebook execution completed'
 ```
 
 ### Disable notifications
+
 ```python
 %notify_all --disable
 time.sleep(1)
 ```
 
 ### Learn more
+
 ```python
 %%notify?
 ```
 
 ```python
 %notify_all?
 ```
 
 ## Troubleshoot
 
 If you notice that the desktop notifications are not showing up, check the below:
+
 1. Make sure JupyterLab is running in a secure context (i.e. either using HTTPS or localhost)
 2. If you've previously denied notification permissions for the site, update the browser settings accordingly. In Chrome, you can do so by navigating to `Setttings -> Privacy and security -> Site Settings -> Notifications` and updating the permissions against your JupyterLab URL.
 3. Verify that notifications work for your browser. You may need to configure an OS setting first. You can test on [this site](https://web-push-book.gauntface.com/demos/notification-examples/).
 
 ## Requirements
 
-* JupyterLab >= 3.0
+- JupyterLab >= 4.0
 
 ## Install
 
 To install this package with [`pip`](https://pip.pypa.io/en/stable/) run
 
 ```bash
 pip install jupyterlab_notify
@@ -171,29 +229,31 @@
 
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab_notify
 ```
 
-
 ## History
 
 This plugin was contributed back to the community by the [D. E. Shaw group](https://www.deshaw.com/).
 
 <p align="center">
     <a href="https://www.deshaw.com">
        <img src="https://www.deshaw.com/assets/logos/blue_logo_417x125.png" alt="D. E. Shaw Logo" height="75" >
     </a>
 </p>
 
 ## License
 
 This project is released under a [BSD-3-Clause license](https://github.com/deshaw/jupyterlab-notify/blob/master/LICENSE.txt).
 
+We love contributions! Before you can contribute, please sign and submit this [Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla).
+This CLA is in place to protect all users of this project.
+
 "Jupyter" is a trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
 
 [pypi-url]: https://pypi.org/project/jupyterlab-notify
 [pypi-image]: https://img.shields.io/pypi/v/jupyterlab-notify
 [pypi-dm-image]: https://img.shields.io/pypi/dm/jupyterlab-notify
 [github-status-image]: https://github.com/deshaw/jupyterlab-notify/workflows/Build/badge.svg
 [github-status-url]: https://github.com/deshaw/jupyterlab-notify/actions?query=workflow%3ABuild
```

### Comparing `jupyterlab_notify-1.0.0/jupyterlab_notify/magics.py` & `jupyterlab_notify-2.0.0/jupyterlab_notify/magics.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_notify-1.0.0/src/index.ts` & `jupyterlab_notify-2.0.0/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 /**
  * The default mime type for the extension.
  */
 const MIME_TYPE = 'application/desktop-notify+json';
 const PROCESSED_KEY = 'isProcessed';
 // The below can be used to customize notifications
 const NOTIFICATION_OPTIONS = {
-  icon: '/static/favicons/favicon.ico'
+  icon: '/static/favicons/favicon.ico',
 };
 
 interface INotifyMimeData {
   type: 'INIT' | 'NOTIFY';
   payload: Record<string, unknown>;
   isProcessed: boolean;
   id: string;
@@ -27,15 +27,15 @@
 class OutputWidget extends Widget implements IRenderMime.IRenderer {
   constructor(options: IRenderMime.IRendererOptions) {
     super();
     this._mimeType = options.mimeType;
   }
 
   renderModel(model: IRenderMime.IMimeModel): Promise<void> {
-    const mimeData = (model.data[this._mimeType] as unknown) as INotifyMimeData;
+    const mimeData = model.data[this._mimeType] as unknown as INotifyMimeData;
 
     const payload = mimeData.payload as JSONObject;
 
     // If the PROCESSED_KEY is available - do not take any action
     // This is done so that notifications are not repeated on page refresh
     if (mimeData[PROCESSED_KEY]) {
       return Promise.resolve();
@@ -46,15 +46,15 @@
       (mimeData.type === 'INIT' && Notification.permission === 'default') ||
       Notification.permission !== 'granted'
     ) {
       // We do not have any actions to perform upon acquiring permission and so
       // handle only the errors (if any)
       Notification.requestPermission().catch(err => {
         alert(
-          `Encountered error - ${err} while requesting permissions for notebook notifications`
+          `Encountered error - ${err} while requesting permissions for notebook notifications`,
         );
       });
     }
 
     if (mimeData.type === 'NOTIFY') {
       // Notify only if there's sufficient permissions and this has not been processed previously
       if (Notification.permission === 'granted' && !mimeData[PROCESSED_KEY]) {
@@ -63,19 +63,19 @@
         this.node.innerHTML = `<div id="${mimeData.id}">Missing permissions - update "Notifications" preferences under browser settings to receive notifications</div>`;
       }
     }
 
     if (!mimeData[PROCESSED_KEY]) {
       // Add isProcessed property to each notification message so that we can avoid repeating notifications on page reloads
       const updatedModel: IRenderMime.IMimeModel = JSON.parse(
-        JSON.stringify(model)
+        JSON.stringify(model),
       );
-      const updatedMimeData = (updatedModel.data[
+      const updatedMimeData = updatedModel.data[
         this._mimeType
-      ] as unknown) as INotifyMimeData;
+      ] as unknown as INotifyMimeData;
       updatedMimeData[PROCESSED_KEY] = true;
       // The below model update is done inside a separate function and added to
       // the event queue - this is done so to avoid re-rendering before the
       // initial render is complete.
       //
       // Without the setTimeout, calling model.setData triggers the callbacks
       // registered on model-updates that re-renders the widget and it again tries
@@ -93,23 +93,23 @@
 
 /**
  * A mime renderer factory for desktop-notify data.
  */
 const rendererFactory: IRenderMime.IRendererFactory = {
   safe: true,
   mimeTypes: [MIME_TYPE],
-  createRenderer: options => new OutputWidget(options)
+  createRenderer: options => new OutputWidget(options),
 };
 
 /**
  * Extension definition.
  */
 const extension: IRenderMime.IExtension = {
   id: 'desktop-notify:plugin',
   rendererFactory,
   rank: 0,
-  dataType: 'json'
+  dataType: 'json',
 };
 
 console.log('jupyterlab-notify render activated');
 
 export default extension;
```

### Comparing `jupyterlab_notify-1.0.0/tsconfig.json` & `jupyterlab_notify-2.0.0/tsconfig.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True, 'target': 'ES2018'}"}*

```diff
@@ -12,15 +12,15 @@
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
-        "strictNullChecks": false,
-        "target": "es2017",
+        "strictNullChecks": true,
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

