# Comparing `tmp/Authomatic-1.0.0.tar.gz` & `tmp/Authomatic-1.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Authomatic-1.0.0.tar", last modified: Wed Nov 27 16:10:12 2019, max compression
+gzip compressed data, was "Authomatic-1.2.0.dev0.tar", last modified: Thu Jun  8 17:43:06 2023, max compression
```

## Comparing `Authomatic-1.0.0.tar` & `Authomatic-1.2.0.dev0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2019-11-27 16:08:02.000000 Authomatic-1.0.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2019-11-27 16:10:12.000000 Authomatic-1.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      175 2019-11-27 16:08:02.000000 Authomatic-1.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1101 2019-11-27 16:08:02.000000 Authomatic-1.0.0/config-template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5419 2019-11-27 16:10:12.000000 Authomatic-1.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3175 2019-11-27 16:08:02.000000 Authomatic-1.0.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/javascript/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7950 2019-11-27 16:08:02.000000 Authomatic-1.0.0/javascript/authomatic.map
--rw-rw-r--   0 travis    (2000) travis    (2000)    16582 2019-11-27 16:08:02.000000 Authomatic-1.0.0/javascript/authomatic.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2019-11-27 16:08:02.000000 Authomatic-1.0.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2019-11-27 16:08:02.000000 Authomatic-1.0.0/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7860 2019-11-27 16:09:33.000000 Authomatic-1.0.0/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2019-11-27 16:08:02.000000 Authomatic-1.0.0/RELEASE.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/authomatic/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/authomatic/providers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3445 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/providers/gaeopenid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57968 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/providers/oauth2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17262 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/providers/openid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/providers/persona.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38857 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/providers/oauth1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30309 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/providers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/authomatic/extras/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1293 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/extras/flask.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/authomatic/extras/gae/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5233 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/extras/gae/openid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7151 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/extras/gae/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/extras/interfaces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/extras/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53267 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6561 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/adapters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29751 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/six.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1224 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2019-11-27 16:08:02.000000 Authomatic-1.0.0/authomatic/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-27 16:10:12.000000 Authomatic-1.0.0/Authomatic.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2019-11-27 16:10:11.000000 Authomatic-1.0.0/Authomatic.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      788 2019-11-27 16:10:11.000000 Authomatic-1.0.0/Authomatic.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-27 16:10:11.000000 Authomatic-1.0.0/Authomatic.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5419 2019-11-27 16:10:11.000000 Authomatic-1.0.0/Authomatic.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2019-11-27 16:10:11.000000 Authomatic-1.0.0/Authomatic.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/Authomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-08 17:43:06.000000 Authomatic-1.2.0.dev0/Authomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 17:43:06.000000 Authomatic-1.2.0.dev0/Authomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:43:06.000000 Authomatic-1.2.0.dev0/Authomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 17:43:06.000000 Authomatic-1.2.0.dev0/Authomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 17:43:06.000000 Authomatic-1.2.0.dev0/Authomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/authomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53269 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/authomatic/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/extras/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/authomatic/extras/gae/
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/extras/gae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/extras/gae/openid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/extras/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/authomatic/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    30309 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/providers/gaeopenid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/providers/oauth1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61564 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/providers/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/providers/openid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/providers/persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29751 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/authomatic/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/config-template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:06.046193 Authomatic-1.2.0.dev0/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/javascript/authomatic.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/javascript/authomatic.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-08 17:43:06.050193 Authomatic-1.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 17:41:37.000000 Authomatic-1.2.0.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Authomatic-1.0.0/setup.cfg` & `Authomatic-1.2.0.dev0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.0
+version = 1.2.0.dev0
 name = Authomatic
 description = Authorization / authentication client library for Python web applications
 long_description = file: README.rst
 author = Peter Hudec
 author_email = peterhudec@peterhudec.com
 maintainer = Authomatic Project Community
 maintainer_email = authomaticproject@protonmail.com
```

### Comparing `Authomatic-1.0.0/config-template.py` & `Authomatic-1.2.0.dev0/config-template.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/PKG-INFO` & `Authomatic-1.2.0.dev0/Authomatic.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,20 @@
 Metadata-Version: 2.1
 Name: Authomatic
-Version: 1.0.0
+Version: 1.2.0.dev0
 Summary: Authorization / authentication client library for Python web applications
-Home-page: UNKNOWN
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/authomatic/authomatic/issues
 Project-URL: Documentation, http://authomatic.github.io/authomatic
 Project-URL: Source Code, https://github.com/authomatic/authomatic/
-Description: .. |gae| replace:: Google App Engine
-        .. _gae: https://developers.google.com/appengine/
-        
-        .. |webapp2| replace:: Webapp2
-        .. _webapp2: http://webapp-improved.appspot.com/
-        
-        .. |oauth2| replace:: OAuth 2.0
-        .. _oauth2: http://oauth.net/2/
-        
-        .. |oauth1| replace:: OAuth 1.0a
-        .. _oauth1: http://oauth.net/core/1.0a/
-        
-        .. |openid| replace:: OpenID
-        .. _openid: http://openid.net/
-        
-        .. |pyopenid| replace:: python-openid
-        .. _pyopenid: http://pypi.python.org/pypi/python-openid/
-        
-        ==========
-        Authomatic
-        ==========
-        
-        .. image:: https://travis-ci.org/authomatic/authomatic.svg?branch=master
-            :target: https://travis-ci.org/authomatic/authomatic
-        
-        **Authomatic**
-        is a **framework agnostic** library
-        for **Python** web applications
-        with a **minimalistic** but **powerful** interface
-        which simplifies **authentication** of users
-        by third party providers like **Facebook** or **Twitter**
-        through standards like **OAuth** and **OpenID**.
-        
-        For more info visit the project page at http://authomatic.github.io/authomatic.
-        
-        Maintainers
-        ===========
-        
-        **Authomatic** was migrated from a private project of Peter Hudec to a community-managed project.
-        Many thanks to Peter Hudec for all his hard work for creating and maintaining **authomatic**!
-        We are now a small team of volunteers, not paid for the work here.
-        Any help is appreciated!
-        
-        
-        Features
-        ========
-        
-        * Loosely coupled.
-        * Tiny but powerful interface.
-        * The |pyopenid|_ library is the only **optional** dependency.
-        * **Framework agnostic** thanks to adapters.
-          Out of the box support for **Django**, **Flask**, **Pyramid** and **Webapp2**.
-        * Ready to accommodate future authorization/authentication protocols.
-        * Makes provider API callls a breeze.
-        * Asynchronous requests.
-        * JavaScript library as a bonus.
-        * Out of the box support for:
-        
-          * |oauth1|_ providers: **Bitbucket**, **Flickr**, **Meetup**, **Plurk**,
-            **Twitter**, **Tumblr**, **UbuntuOne**, **Vimeo**, **Xero**, **Xing** and **Yahoo**.
-          * |oauth2|_ providers: **Amazon**, **Behance**, **Bitly**, **Cosm**,
-            **DeviantART**, **Eventbrite**, **Facebook**, **Foursquare**,
-            **GitHub**, **Google**, **LinkedIn**, **PayPal**, **Reddit**,
-            **Viadeo**, **VK**, **WindowsLive**, **Yammer** and **Yandex**.
-          * |pyopenid|_ and |gae|_ based |openid|_.
-        
-        License
-        =======
-        
-        The package is licensed under
-        `MIT license <http://en.wikipedia.org/wiki/MIT_License>`__.
-        
-        Requirements
-        ============
-        
-        Requires **Python 2.7** and newer.
-        **Python 3.x** support added in **Authomatic 0.0.11** thanks to Emmanuel Leblond <https://github.com/touilleMan>`__.
-        
-        Live Demo
-        =========
-        
-        There is a |gae| based live demo app running at
-        http://authomatic-example.appspot.com which makes use of most of the features.
-        
-        Contribute
-        ==========
-        
-        Contributions of any kind are very welcome.
-        If you want to contribute, please read the
-        `Development Guide <http://authomatic.github.io/authomatic/development.html>`__
-        first. The project is hosted on
-        `GitHub <https://github.com/authomatic/authomatic>`__.
-        
-        Usage
-        =====
-        
-        Read the exhaustive documentation at http://authomatic.github.io/authomatic.
-        
-        Changelog
-        =========
-        
-        The `Changelog is part of the documentation <https://authomatic.github.io/authomatic/changelog.html>`_.
-        
 Keywords: oauth2,oauth,openid,access delegation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -127,7 +22,111 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: OpenID
+License-File: LICENSE.txt
+
+.. |gae| replace:: Google App Engine
+.. _gae: https://developers.google.com/appengine/
+
+.. |webapp2| replace:: Webapp2
+.. _webapp2: http://webapp-improved.appspot.com/
+
+.. |oauth2| replace:: OAuth 2.0
+.. _oauth2: http://oauth.net/2/
+
+.. |oauth1| replace:: OAuth 1.0a
+.. _oauth1: http://oauth.net/core/1.0a/
+
+.. |openid| replace:: OpenID
+.. _openid: http://openid.net/
+
+.. |pyopenid| replace:: python-openid
+.. _pyopenid: http://pypi.python.org/pypi/python-openid/
+
+==========
+Authomatic
+==========
+
+.. image:: https://travis-ci.org/authomatic/authomatic.svg?branch=master
+    :target: https://travis-ci.org/authomatic/authomatic
+
+**Authomatic**
+is a **framework agnostic** library
+for **Python** web applications
+with a **minimalistic** but **powerful** interface
+which simplifies **authentication** of users
+by third party providers like **Facebook** or **Twitter**
+through standards like **OAuth** and **OpenID**.
+
+For more info visit the project page at http://authomatic.github.io/authomatic.
+
+Maintainers
+===========
+
+**Authomatic** was migrated from a private project of Peter Hudec to a community-managed project.
+Many thanks to Peter Hudec for all his hard work for creating and maintaining **authomatic**!
+We are now a small team of volunteers, not paid for the work here.
+Any help is appreciated!
+
+
+Features
+========
+
+* Loosely coupled.
+* Tiny but powerful interface.
+* The |pyopenid|_ library is the only **optional** dependency.
+* **Framework agnostic** thanks to adapters.
+  Out of the box support for **Django**, **Flask**, **Pyramid** and **Webapp2**.
+* Ready to accommodate future authorization/authentication protocols.
+* Makes provider API calls a breeze.
+* Asynchronous requests.
+* JavaScript library as a bonus.
+* Out of the box support for:
+
+  * |oauth1|_ providers: **Bitbucket**, **Flickr**, **Meetup**, **Plurk**,
+    **Twitter**, **Tumblr**, **UbuntuOne**, **Vimeo**, **Xero**, **Xing** and **Yahoo**.
+  * |oauth2|_ providers: **Amazon**, **Behance**, **Bitly**, **Cosm**,
+    **DeviantART**, **Eventbrite**, **Facebook**, **Foursquare**,
+    **GitHub**, **Google**, **LinkedIn**, **PayPal**, **Reddit**,
+    **Viadeo**, **VK**, **WindowsLive**, **Yammer** and **Yandex**.
+  * |pyopenid|_ and |gae|_ based |openid|_.
+
+License
+=======
+
+The package is licensed under
+`MIT license <http://en.wikipedia.org/wiki/MIT_License>`__.
+
+Requirements
+============
+
+Requires **Python 3.4** or newer.
+**Python 3.x** support added in **Authomatic 0.0.11** thanks to Emmanuel Leblond <https://github.com/touilleMan>`__.
+
+Live Demo
+=========
+
+There is a |gae| based live demo app running at
+http://authomatic-example.appspot.com which makes use of most of the features.
+
+Contribute
+==========
+
+Contributions of any kind are very welcome.
+If you want to contribute, please read the
+`Development Guide <http://authomatic.github.io/authomatic/development.html>`__
+first. The project is hosted on
+`GitHub <https://github.com/authomatic/authomatic>`__.
+
+Usage
+=====
+
+Read the exhaustive documentation at http://authomatic.github.io/authomatic.
+
+Changelog
+=========
+
+The `Changelog is part of the documentation <https://authomatic.github.io/authomatic/changelog.html>`_.
```

### Comparing `Authomatic-1.0.0/README.rst` & `Authomatic-1.2.0.dev0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 * Loosely coupled.
 * Tiny but powerful interface.
 * The |pyopenid|_ library is the only **optional** dependency.
 * **Framework agnostic** thanks to adapters.
   Out of the box support for **Django**, **Flask**, **Pyramid** and **Webapp2**.
 * Ready to accommodate future authorization/authentication protocols.
-* Makes provider API callls a breeze.
+* Makes provider API calls a breeze.
 * Asynchronous requests.
 * JavaScript library as a bonus.
 * Out of the box support for:
 
   * |oauth1|_ providers: **Bitbucket**, **Flickr**, **Meetup**, **Plurk**,
     **Twitter**, **Tumblr**, **UbuntuOne**, **Vimeo**, **Xero**, **Xing** and **Yahoo**.
   * |oauth2|_ providers: **Amazon**, **Behance**, **Bitly**, **Cosm**,
@@ -69,15 +69,15 @@
 
 The package is licensed under
 `MIT license <http://en.wikipedia.org/wiki/MIT_License>`__.
 
 Requirements
 ============
 
-Requires **Python 2.7** and newer.
+Requires **Python 3.4** or newer.
 **Python 3.x** support added in **Authomatic 0.0.11** thanks to Emmanuel Leblond <https://github.com/touilleMan>`__.
 
 Live Demo
 =========
 
 There is a |gae| based live demo app running at
 http://authomatic-example.appspot.com which makes use of most of the features.
```

### Comparing `Authomatic-1.0.0/javascript/authomatic.map` & `Authomatic-1.2.0.dev0/javascript/authomatic.map`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/javascript/authomatic.js` & `Authomatic-1.2.0.dev0/javascript/authomatic.js`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/LICENSE.txt` & `Authomatic-1.2.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/CHANGES.rst` & `Authomatic-1.2.0.dev0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ..
-
     DO NOT EDIT HERE!
 
     This FILE IS GENERATED by towncrier https://towncrier.readthedocs.io/en/
 
     DO NOT EDIT HERE!
 
     Create a news fragment in the "news" folder instead.
@@ -21,19 +20,19 @@
     Example:
 
     - "1234.bugfix"
     - for two separate fixes in one PR  "3423-1.bugfix" and "3423-2.bugfix"
 
     Sphinx Syntax is allowed.
 
+
 Changelog
 =========
 
 ..
-
   DO NOT EDIT HERE!
 
   Below towncrier inserts the output before release!
 
 .. towncrier release notes start
 
 1.0.0 (2019-11-27)
```

### Comparing `Authomatic-1.0.0/RELEASE.rst` & `Authomatic-1.2.0.dev0/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/providers/gaeopenid.py` & `Authomatic-1.2.0.dev0/authomatic/providers/gaeopenid.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/providers/oauth2.py` & `Authomatic-1.2.0.dev0/authomatic/providers/oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     DeviantART
     Eventbrite
     Facebook
     Foursquare
     GitHub
     Google
     LinkedIn
+    MicrosoftOnline
     PayPal
     Reddit
     Viadeo
     VK
     WindowsLive
     Yammer
     Yandex
@@ -38,16 +39,16 @@
 from authomatic import providers
 from authomatic.exceptions import CancellationError, FailureError, OAuth2Error
 import authomatic.core as core
 
 
 __all__ = ['OAuth2', 'Amazon', 'Behance', 'Bitly', 'Cosm', 'DeviantART',
            'Eventbrite', 'Facebook', 'Foursquare', 'GitHub', 'Google',
-           'LinkedIn', 'PayPal', 'Reddit', 'Viadeo', 'VK', 'WindowsLive',
-           'Yammer', 'Yandex']
+           'LinkedIn', 'MicrosoftOnline', 'PayPal', 'Reddit', 'Viadeo',
+           'VK', 'WindowsLive', 'Yammer', 'Yandex']
 
 
 class OAuth2(providers.AuthorizationProvider):
     """
     Base class for |oauth2|_ providers.
     """
 
@@ -1121,31 +1122,31 @@
     * Dashboard: https://github.com/settings/developers
     * Docs: http://developer.github.com/v3/#authentication
     * API reference: http://developer.github.com/v3/
 
     .. note::
 
         GitHub API
-        `documentation <http://developer.github.com/v3/#user-agent-required>`_
-        says:
 
-            all API requests MUST include a valid ``User-Agent`` header.
+        Users may not have a public email address. In order to obtain the private email address, the
+        `documentation <https://developer.github.com/v3/users/emails/#list-email-addresses-for-a-user>`_
+        specifies to request ``user:email`` scope.
+         This allows the ``access`` function to scrape ``users/email`` API endpoint.
 
-        You can apply a default ``User-Agent`` header for all API calls in
-        the config like this:
+            You can set the ``user:email`` scope like this:
 
         .. code-block:: python
             :emphasize-lines: 6
 
             CONFIG = {
                 'github': {
                     'class_': oauth2.GitHub,
                     'consumer_key': '#####',
                     'consumer_secret': '#####',
-                    'access_headers': {'User-Agent': 'Awesome-Octocat-App'},
+                    'scope': ['user:email']
                 }
             }
 
     Supported :class:`.User` properties:
 
     * email
     * id
@@ -1196,14 +1197,46 @@
 
     @classmethod
     def _x_credentials_parser(cls, credentials, data):
         if data.get('token_type') == 'bearer':
             credentials.token_type = cls.BEARER
         return credentials
 
+    def access(self, url, **kwargs):
+        # https://developer.github.com/v3/#user-agent-required
+        # GitHub requires that all API requests MUST include a valid ``User-Agent`` header.
+        headers = kwargs["headers"] = kwargs.get("headers", {})
+        if not headers.get("User-Agent"):
+            headers["User-Agent"] = self.settings.config[self.name]["consumer_key"]
+
+        def parent_access(url):
+            return super(GitHub, self).access(url, **kwargs)
+
+        response = parent_access(url)
+
+        # additional action to get email is required:
+        # https://developer.github.com/v3/users/emails/
+        if response.status == 200:
+            email_response = parent_access(url + "/emails")
+            if email_response.status == 200:
+                response.data["emails"] = email_response.data
+
+                # find first or primary email
+                primary_email = None
+                for item in email_response.data:
+                    is_primary = item["primary"]
+                    if not primary_email or is_primary:
+                        primary_email = item["email"]
+
+                    if is_primary:
+                        break
+
+                response.data["email"] = primary_email
+        return response
+
 
 class Google(OAuth2):
     """
     Google |oauth2| provider.
 
     * Dashboard: https://console.developers.google.com/project
     * Docs: https://developers.google.com/accounts/docs/OAuth2
@@ -1411,14 +1444,91 @@
             _year = _birthdate.get('year')
             if _day and _month and _year:
                 user.birth_date = datetime.datetime(_year, _month, _day)
 
         return user
 
 
+class MicrosoftOnline(OAuth2):
+    """
+    Microsoft Online |oauth2| provider.
+
+    Supported :class:`.User` properties:
+
+    * email
+    * first_name
+    * id
+    * last_name
+    * location
+    * name
+    * phone
+    * picture
+    * username
+
+    Unsupported :class:`.User` properties:
+
+    * birth_date
+    * city
+    * country
+    * gender
+    * link
+    * locale
+    * nickname
+    * postal_code
+    * timezone
+
+    """
+
+    user_authorization_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/authorize'
+    access_token_url = 'https://login.microsoftonline.com/common/oauth2/v2.0/token'
+    user_info_url = "https://graph.microsoft.com/v1.0/me"
+
+    user_info_scope = ['openid profile']
+
+    supported_user_attributes = core.SupportedUserAttributes(
+        id=True,
+        email=True,
+        first_name=True,
+        last_name=True,
+        location=True,
+        name=True,
+        phone=True,
+        picture=True,
+        username=True,
+    )
+
+    def __init__(self, *args, **kwargs):
+        super(MicrosoftOnline, self).__init__(*args, **kwargs)
+        auth = args[0]
+        provider_name = kwargs.get('provider_name')
+        domain = auth.config.get(provider_name, {}).get('domain')
+        if domain is not None:
+            self.user_authorization_url = MicrosoftOnline.user_authorization_url.replace('/common/', '/%s/' % domain)
+            self.access_token_url = MicrosoftOnline.access_token_url.replace('/common/', '/%s/' % domain)
+
+    @classmethod
+    def _x_credentials_parser(cls, credentials, data):
+        if data.get('token_type') == 'bearer':
+            credentials.token_type = cls.BEARER
+        return credentials
+
+    @staticmethod
+    def _x_user_parser(user, data):
+        user.id = data.get('id')
+        user.name = data.get('displayName', '')
+        user.first_name = data.get('givenName', '')
+        user.last_name = data.get('surname', '')
+        user.email = data.get('mail', '')
+        user.location = data.get('officeLocation', '')
+        user.phone = data.get('mobilePhone', '')
+        user.picture = data.get('picture', '')
+        user.username = data.get('userPrincipalName', '')
+        return user
+
+
 class PayPal(OAuth2):
     """
     PayPal |oauth2| provider.
 
     * Dashboard: https://developer.paypal.com/webapps/developer/applications
     * Docs: https://developer.paypal.com/webapps/developer/docs/integration/direct/make-your-first-call/
     * API reference: https://developer.paypal.com/webapps/developer/docs/api/
@@ -1963,14 +2073,15 @@
     DeviantART,
     Eventbrite,
     Facebook,
     Foursquare,
     GitHub,
     Google,
     LinkedIn,
+    MicrosoftOnline,
     OAuth2,
     PayPal,
     Reddit,
     Viadeo,
     VK,
     WindowsLive,
     Yammer,
```

### Comparing `Authomatic-1.0.0/authomatic/providers/openid.py` & `Authomatic-1.2.0.dev0/authomatic/providers/openid.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/providers/oauth1.py` & `Authomatic-1.2.0.dev0/authomatic/providers/oauth1.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/providers/__init__.py` & `Authomatic-1.2.0.dev0/authomatic/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/extras/flask.py` & `Authomatic-1.2.0.dev0/authomatic/extras/flask.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,8 +40,9 @@
                     *login_args,
                     **login_kwargs)
                 return f(*args, **kwargs)
             return decorated
         return decorator
 
     def session_saver(self):
-        session.modified = True
+        # FIXME: pylint false positive - see https://github.com/pallets/flask/issues/4020
+        session.modified = True  # pylint: disable=assigning-non-slot
```

### Comparing `Authomatic-1.0.0/authomatic/extras/gae/openid.py` & `Authomatic-1.2.0.dev0/authomatic/extras/gae/openid.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/extras/gae/__init__.py` & `Authomatic-1.2.0.dev0/authomatic/extras/gae/__init__.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/extras/interfaces.py` & `Authomatic-1.2.0.dev0/authomatic/extras/interfaces.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/core.py` & `Authomatic-1.2.0.dev0/authomatic/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -913,15 +913,15 @@
         cfg = config.get(provider_name)
 
         # Get the provider class.
         ProviderClass = resolve_provider_class(cfg.get('class_'))
 
         deserialized = Credentials(config)
 
-        deserialized.provider_id = provider_id
+        deserialized.provider_id = int(split[0])
         deserialized.provider_type = ProviderClass.get_type()
         deserialized.provider_type_id = split[1]
         deserialized.provider_class = ProviderClass
         deserialized.provider_name = provider_name
         deserialized.provider_class = ProviderClass
 
         # Add provider type specific properties.
```

### Comparing `Authomatic-1.0.0/authomatic/adapters.py` & `Authomatic-1.2.0.dev0/authomatic/adapters.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/six.py` & `Authomatic-1.2.0.dev0/authomatic/six.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/authomatic/exceptions.py` & `Authomatic-1.2.0.dev0/authomatic/exceptions.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/Authomatic.egg-info/SOURCES.txt` & `Authomatic-1.2.0.dev0/Authomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Authomatic-1.0.0/Authomatic.egg-info/PKG-INFO` & `Authomatic-1.2.0.dev0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,20 @@
 Metadata-Version: 2.1
 Name: Authomatic
-Version: 1.0.0
+Version: 1.2.0.dev0
 Summary: Authorization / authentication client library for Python web applications
-Home-page: UNKNOWN
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/authomatic/authomatic/issues
 Project-URL: Documentation, http://authomatic.github.io/authomatic
 Project-URL: Source Code, https://github.com/authomatic/authomatic/
-Description: .. |gae| replace:: Google App Engine
-        .. _gae: https://developers.google.com/appengine/
-        
-        .. |webapp2| replace:: Webapp2
-        .. _webapp2: http://webapp-improved.appspot.com/
-        
-        .. |oauth2| replace:: OAuth 2.0
-        .. _oauth2: http://oauth.net/2/
-        
-        .. |oauth1| replace:: OAuth 1.0a
-        .. _oauth1: http://oauth.net/core/1.0a/
-        
-        .. |openid| replace:: OpenID
-        .. _openid: http://openid.net/
-        
-        .. |pyopenid| replace:: python-openid
-        .. _pyopenid: http://pypi.python.org/pypi/python-openid/
-        
-        ==========
-        Authomatic
-        ==========
-        
-        .. image:: https://travis-ci.org/authomatic/authomatic.svg?branch=master
-            :target: https://travis-ci.org/authomatic/authomatic
-        
-        **Authomatic**
-        is a **framework agnostic** library
-        for **Python** web applications
-        with a **minimalistic** but **powerful** interface
-        which simplifies **authentication** of users
-        by third party providers like **Facebook** or **Twitter**
-        through standards like **OAuth** and **OpenID**.
-        
-        For more info visit the project page at http://authomatic.github.io/authomatic.
-        
-        Maintainers
-        ===========
-        
-        **Authomatic** was migrated from a private project of Peter Hudec to a community-managed project.
-        Many thanks to Peter Hudec for all his hard work for creating and maintaining **authomatic**!
-        We are now a small team of volunteers, not paid for the work here.
-        Any help is appreciated!
-        
-        
-        Features
-        ========
-        
-        * Loosely coupled.
-        * Tiny but powerful interface.
-        * The |pyopenid|_ library is the only **optional** dependency.
-        * **Framework agnostic** thanks to adapters.
-          Out of the box support for **Django**, **Flask**, **Pyramid** and **Webapp2**.
-        * Ready to accommodate future authorization/authentication protocols.
-        * Makes provider API callls a breeze.
-        * Asynchronous requests.
-        * JavaScript library as a bonus.
-        * Out of the box support for:
-        
-          * |oauth1|_ providers: **Bitbucket**, **Flickr**, **Meetup**, **Plurk**,
-            **Twitter**, **Tumblr**, **UbuntuOne**, **Vimeo**, **Xero**, **Xing** and **Yahoo**.
-          * |oauth2|_ providers: **Amazon**, **Behance**, **Bitly**, **Cosm**,
-            **DeviantART**, **Eventbrite**, **Facebook**, **Foursquare**,
-            **GitHub**, **Google**, **LinkedIn**, **PayPal**, **Reddit**,
-            **Viadeo**, **VK**, **WindowsLive**, **Yammer** and **Yandex**.
-          * |pyopenid|_ and |gae|_ based |openid|_.
-        
-        License
-        =======
-        
-        The package is licensed under
-        `MIT license <http://en.wikipedia.org/wiki/MIT_License>`__.
-        
-        Requirements
-        ============
-        
-        Requires **Python 2.7** and newer.
-        **Python 3.x** support added in **Authomatic 0.0.11** thanks to Emmanuel Leblond <https://github.com/touilleMan>`__.
-        
-        Live Demo
-        =========
-        
-        There is a |gae| based live demo app running at
-        http://authomatic-example.appspot.com which makes use of most of the features.
-        
-        Contribute
-        ==========
-        
-        Contributions of any kind are very welcome.
-        If you want to contribute, please read the
-        `Development Guide <http://authomatic.github.io/authomatic/development.html>`__
-        first. The project is hosted on
-        `GitHub <https://github.com/authomatic/authomatic>`__.
-        
-        Usage
-        =====
-        
-        Read the exhaustive documentation at http://authomatic.github.io/authomatic.
-        
-        Changelog
-        =========
-        
-        The `Changelog is part of the documentation <https://authomatic.github.io/authomatic/changelog.html>`_.
-        
 Keywords: oauth2,oauth,openid,access delegation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -127,7 +22,111 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: OpenID
+License-File: LICENSE.txt
+
+.. |gae| replace:: Google App Engine
+.. _gae: https://developers.google.com/appengine/
+
+.. |webapp2| replace:: Webapp2
+.. _webapp2: http://webapp-improved.appspot.com/
+
+.. |oauth2| replace:: OAuth 2.0
+.. _oauth2: http://oauth.net/2/
+
+.. |oauth1| replace:: OAuth 1.0a
+.. _oauth1: http://oauth.net/core/1.0a/
+
+.. |openid| replace:: OpenID
+.. _openid: http://openid.net/
+
+.. |pyopenid| replace:: python-openid
+.. _pyopenid: http://pypi.python.org/pypi/python-openid/
+
+==========
+Authomatic
+==========
+
+.. image:: https://travis-ci.org/authomatic/authomatic.svg?branch=master
+    :target: https://travis-ci.org/authomatic/authomatic
+
+**Authomatic**
+is a **framework agnostic** library
+for **Python** web applications
+with a **minimalistic** but **powerful** interface
+which simplifies **authentication** of users
+by third party providers like **Facebook** or **Twitter**
+through standards like **OAuth** and **OpenID**.
+
+For more info visit the project page at http://authomatic.github.io/authomatic.
+
+Maintainers
+===========
+
+**Authomatic** was migrated from a private project of Peter Hudec to a community-managed project.
+Many thanks to Peter Hudec for all his hard work for creating and maintaining **authomatic**!
+We are now a small team of volunteers, not paid for the work here.
+Any help is appreciated!
+
+
+Features
+========
+
+* Loosely coupled.
+* Tiny but powerful interface.
+* The |pyopenid|_ library is the only **optional** dependency.
+* **Framework agnostic** thanks to adapters.
+  Out of the box support for **Django**, **Flask**, **Pyramid** and **Webapp2**.
+* Ready to accommodate future authorization/authentication protocols.
+* Makes provider API calls a breeze.
+* Asynchronous requests.
+* JavaScript library as a bonus.
+* Out of the box support for:
+
+  * |oauth1|_ providers: **Bitbucket**, **Flickr**, **Meetup**, **Plurk**,
+    **Twitter**, **Tumblr**, **UbuntuOne**, **Vimeo**, **Xero**, **Xing** and **Yahoo**.
+  * |oauth2|_ providers: **Amazon**, **Behance**, **Bitly**, **Cosm**,
+    **DeviantART**, **Eventbrite**, **Facebook**, **Foursquare**,
+    **GitHub**, **Google**, **LinkedIn**, **PayPal**, **Reddit**,
+    **Viadeo**, **VK**, **WindowsLive**, **Yammer** and **Yandex**.
+  * |pyopenid|_ and |gae|_ based |openid|_.
+
+License
+=======
+
+The package is licensed under
+`MIT license <http://en.wikipedia.org/wiki/MIT_License>`__.
+
+Requirements
+============
+
+Requires **Python 3.4** or newer.
+**Python 3.x** support added in **Authomatic 0.0.11** thanks to Emmanuel Leblond <https://github.com/touilleMan>`__.
+
+Live Demo
+=========
+
+There is a |gae| based live demo app running at
+http://authomatic-example.appspot.com which makes use of most of the features.
+
+Contribute
+==========
+
+Contributions of any kind are very welcome.
+If you want to contribute, please read the
+`Development Guide <http://authomatic.github.io/authomatic/development.html>`__
+first. The project is hosted on
+`GitHub <https://github.com/authomatic/authomatic>`__.
+
+Usage
+=====
+
+Read the exhaustive documentation at http://authomatic.github.io/authomatic.
+
+Changelog
+=========
+
+The `Changelog is part of the documentation <https://authomatic.github.io/authomatic/changelog.html>`_.
```

