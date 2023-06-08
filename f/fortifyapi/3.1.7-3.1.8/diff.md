# Comparing `tmp/fortifyapi-3.1.7.tar.gz` & `tmp/fortifyapi-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortifyapi-3.1.7.tar", last modified: Wed May 10 23:13:26 2023, max compression
+gzip compressed data, was "fortifyapi-3.1.8.tar", last modified: Thu Jun  8 02:34:03 2023, max compression
```

## Comparing `fortifyapi-3.1.7.tar` & `fortifyapi-3.1.8.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 23:13:26.684493 fortifyapi-3.1.7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 23:13:26.684493 fortifyapi-3.1.7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 23:13:26.680493 fortifyapi-3.1.7/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/docs/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/docs/couscous.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 23:13:26.680493 fortifyapi-3.1.7/fortifyapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39846 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/fortify.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/fortifyapi/template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 23:13:26.684493 fortifyapi-3.1.7/fortifyapi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 23:13:26.000000 fortifyapi-3.1.7/fortifyapi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-10 23:13:26.000000 fortifyapi-3.1.7/fortifyapi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 23:13:26.000000 fortifyapi-3.1.7/fortifyapi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-10 23:13:26.000000 fortifyapi-3.1.7/fortifyapi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-05-10 23:13:26.000000 fortifyapi-3.1.7/fortifyapi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 23:13:26.000000 fortifyapi-3.1.7/fortifyapi.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-10 23:13:26.684493 fortifyapi-3.1.7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-05-10 23:13:20.000000 fortifyapi-3.1.7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3347 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.895080 fortifyapi-3.1.8/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/docs/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/docs/couscous.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.895080 fortifyapi-3.1.8/fortifyapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40384 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/fortify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/fortifyapi/template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.895080 fortifyapi-3.1.8/fortifyapi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3347 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-08 02:34:03.000000 fortifyapi-3.1.8/fortifyapi.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-08 02:34:03.899080 fortifyapi-3.1.8/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1963 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_artifacts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_bugtracker.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_issues.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_jobs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_pool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3918 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_projects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      442 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_reports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1024 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_rulepack.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2994 2023-06-08 02:33:57.000000 fortifyapi-3.1.8/tests/test_versions.py
```

### Comparing `fortifyapi-3.1.7/LICENSE.txt` & `fortifyapi-3.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/PKG-INFO` & `fortifyapi-3.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.7
+Version: 3.1.8
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.8
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.7
-Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
-        .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
-        .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
-        
-        Fortify API
-        ***********
-        
-        Fortify API is a Python RESTFul API client module for Fortify's `Software Security Center <https://www.microfocus.com/en-us/products/software-security-assurance-sdlc/overview/>`_
-        
-        Quick Start
-        ~~~~~~~~~~~
-        
-        Several quick start options are available:
-        
-        - Build locally: ``pip install wheel setuptools && python setup.py build`` 
-        - Install with pip (recommended): ``pip install fortifyapi``
-        - `Download the latest release <https://pypi.org/project/fortifyapi/>`__.
-        
-        Example
-        ~~~~~~~
-        
-        .. code:: python
-        
-           from os import environ
-           from locale import LC_ALL, setlocale
-           from fortifyapi.fortify import FortifyApi
-            
-           # Set encoding
-           environ["PYTHONIOENCODING"] = "utf-8"
-           myLocale = setlocale(category=LC_ALL, locale="en_GB.UTF-8")
-            
-           # Set vars for connection
-           url = 'https://some-fortify-host/ssc'
-           user = 'Fortify SSC User'
-           password = 'Fortify SSC Password'
-           description = 'fortifyapi test client'
-            
-           # Authenticate and retrieve token
-           def token():
-               api = FortifyApi(host=url, username=user, password=password, verify_ssl=False)
-               response = api.get_token(description=description)
-               return response.data['data']['token']
-            
-           # Re-use token in all requests
-           def api():
-               api = FortifyApi(host=url, token=token(), verify_ssl=False)
-               return api
-            
-           # List ID, Project/application Version
-           def list():
-               response = api().get_all_project_versions()
-               data = response.data['data']
-               for version in data:
-                   print("{0:8} {1:30} {2:30}".format(version['id'], version['project']['name'], version['name']).encode(
-                       'utf-8', errors='ignore').decode())
-            
-           if __name__ == '__main__':
-                list()
-        
-        Bugs and Feature Requests
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Found something that doesn't seem right or have a feature request? Please open a new issue.
-        
-        Copyright and License
-        ~~~~~~~~~~~~~~~~~~~~~
-        .. image:: https://img.shields.io/github/license/fortifyadmin/fortifyapi.svg?style=flat-square
-        
-        
 Keywords: fortify,api,security,software,microfocus,ssc,sast
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires: requests
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+.. image:: https://img.shields.io/pypi/v/fortifyapi.svg
+.. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
+.. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
+
+Fortify API
+***********
+
+Fortify API is a Python RESTFul API client module for Fortify's `Software Security Center <https://www.microfocus.com/en-us/products/software-security-assurance-sdlc/overview/>`_
+
+Quick Start
+~~~~~~~~~~~
+
+Several quick start options are available:
+
+- Build locally: ``pip install wheel setuptools && python setup.py build`` 
+- Install with pip (recommended): ``pip install fortifyapi``
+- `Download the latest release <https://pypi.org/project/fortifyapi/>`__.
+
+Example
+~~~~~~~
+
+.. code:: python
+
+   from os import environ
+   from locale import LC_ALL, setlocale
+   from fortifyapi.fortify import FortifyApi
+    
+   # Set encoding
+   environ["PYTHONIOENCODING"] = "utf-8"
+   myLocale = setlocale(category=LC_ALL, locale="en_GB.UTF-8")
+    
+   # Set vars for connection
+   url = 'https://some-fortify-host/ssc'
+   user = 'Fortify SSC User'
+   password = 'Fortify SSC Password'
+   description = 'fortifyapi test client'
+    
+   # Authenticate and retrieve token
+   def token():
+       api = FortifyApi(host=url, username=user, password=password, verify_ssl=False)
+       response = api.get_token(description=description)
+       return response.data['data']['token']
+    
+   # Re-use token in all requests
+   def api():
+       api = FortifyApi(host=url, token=token(), verify_ssl=False)
+       return api
+    
+   # List ID, Project/application Version
+   def list():
+       response = api().get_all_project_versions()
+       data = response.data['data']
+       for version in data:
+           print("{0:8} {1:30} {2:30}".format(version['id'], version['project']['name'], version['name']).encode(
+               'utf-8', errors='ignore').decode())
+    
+   if __name__ == '__main__':
+        list()
+
+Bugs and Feature Requests
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Found something that doesn't seem right or have a feature request? Please open a new issue.
+
+Copyright and License
+~~~~~~~~~~~~~~~~~~~~~
+.. image:: https://img.shields.io/github/license/fortifyadmin/fortifyapi.svg?style=flat-square
+
```

### Comparing `fortifyapi-3.1.7/README.rst` & `fortifyapi-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/docs/README.md` & `fortifyapi-3.1.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/fortifyapi/api.py` & `fortifyapi-3.1.8/fortifyapi/api.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/fortifyapi/client.py` & `fortifyapi-3.1.8/fortifyapi/client.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/fortifyapi/fortify.py` & `fortifyapi-3.1.8/fortifyapi/fortify.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,14 +641,30 @@
             "type": token_type,
             "terminalDate": expire_date
         }
 
         url = "/api/v1/tokens"
         return self._request('POST', url, json=data)
 
+    def set_assign_user(self, version_id, issue_id, user, revision=0):
+        data = {
+                "type": "AUDIT_ISSUE",
+                "values": {
+                    "issues": [
+                        {
+                            "id": issue_id,
+                            "revision": revision
+                        }
+                    ],
+                    "user": user
+                }
+        }
+        url = f'/api/v1/projectVersions/{version_id}/issues/action'
+        return self._request('POST', url, json=data)
+
     def get_all_rulepacks(self):
         """
         List all rules on an SSC instance
         :return:
         """
         url = "/api/v1/coreRulepacks"
         return self._request('GET', url)
```

### Comparing `fortifyapi-3.1.7/fortifyapi/query.py` & `fortifyapi-3.1.8/fortifyapi/query.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/fortifyapi/template.py` & `fortifyapi-3.1.8/fortifyapi/template.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.7/fortifyapi.egg-info/PKG-INFO` & `fortifyapi-3.1.8/fortifyapi.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.7
+Version: 3.1.8
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.8
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.7
-Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
-        .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
-        .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
-        
-        Fortify API
-        ***********
-        
-        Fortify API is a Python RESTFul API client module for Fortify's `Software Security Center <https://www.microfocus.com/en-us/products/software-security-assurance-sdlc/overview/>`_
-        
-        Quick Start
-        ~~~~~~~~~~~
-        
-        Several quick start options are available:
-        
-        - Build locally: ``pip install wheel setuptools && python setup.py build`` 
-        - Install with pip (recommended): ``pip install fortifyapi``
-        - `Download the latest release <https://pypi.org/project/fortifyapi/>`__.
-        
-        Example
-        ~~~~~~~
-        
-        .. code:: python
-        
-           from os import environ
-           from locale import LC_ALL, setlocale
-           from fortifyapi.fortify import FortifyApi
-            
-           # Set encoding
-           environ["PYTHONIOENCODING"] = "utf-8"
-           myLocale = setlocale(category=LC_ALL, locale="en_GB.UTF-8")
-            
-           # Set vars for connection
-           url = 'https://some-fortify-host/ssc'
-           user = 'Fortify SSC User'
-           password = 'Fortify SSC Password'
-           description = 'fortifyapi test client'
-            
-           # Authenticate and retrieve token
-           def token():
-               api = FortifyApi(host=url, username=user, password=password, verify_ssl=False)
-               response = api.get_token(description=description)
-               return response.data['data']['token']
-            
-           # Re-use token in all requests
-           def api():
-               api = FortifyApi(host=url, token=token(), verify_ssl=False)
-               return api
-            
-           # List ID, Project/application Version
-           def list():
-               response = api().get_all_project_versions()
-               data = response.data['data']
-               for version in data:
-                   print("{0:8} {1:30} {2:30}".format(version['id'], version['project']['name'], version['name']).encode(
-                       'utf-8', errors='ignore').decode())
-            
-           if __name__ == '__main__':
-                list()
-        
-        Bugs and Feature Requests
-        ~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Found something that doesn't seem right or have a feature request? Please open a new issue.
-        
-        Copyright and License
-        ~~~~~~~~~~~~~~~~~~~~~
-        .. image:: https://img.shields.io/github/license/fortifyadmin/fortifyapi.svg?style=flat-square
-        
-        
 Keywords: fortify,api,security,software,microfocus,ssc,sast
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires: requests
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+.. image:: https://img.shields.io/pypi/v/fortifyapi.svg
+.. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
+.. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
+
+Fortify API
+***********
+
+Fortify API is a Python RESTFul API client module for Fortify's `Software Security Center <https://www.microfocus.com/en-us/products/software-security-assurance-sdlc/overview/>`_
+
+Quick Start
+~~~~~~~~~~~
+
+Several quick start options are available:
+
+- Build locally: ``pip install wheel setuptools && python setup.py build`` 
+- Install with pip (recommended): ``pip install fortifyapi``
+- `Download the latest release <https://pypi.org/project/fortifyapi/>`__.
+
+Example
+~~~~~~~
+
+.. code:: python
+
+   from os import environ
+   from locale import LC_ALL, setlocale
+   from fortifyapi.fortify import FortifyApi
+    
+   # Set encoding
+   environ["PYTHONIOENCODING"] = "utf-8"
+   myLocale = setlocale(category=LC_ALL, locale="en_GB.UTF-8")
+    
+   # Set vars for connection
+   url = 'https://some-fortify-host/ssc'
+   user = 'Fortify SSC User'
+   password = 'Fortify SSC Password'
+   description = 'fortifyapi test client'
+    
+   # Authenticate and retrieve token
+   def token():
+       api = FortifyApi(host=url, username=user, password=password, verify_ssl=False)
+       response = api.get_token(description=description)
+       return response.data['data']['token']
+    
+   # Re-use token in all requests
+   def api():
+       api = FortifyApi(host=url, token=token(), verify_ssl=False)
+       return api
+    
+   # List ID, Project/application Version
+   def list():
+       response = api().get_all_project_versions()
+       data = response.data['data']
+       for version in data:
+           print("{0:8} {1:30} {2:30}".format(version['id'], version['project']['name'], version['name']).encode(
+               'utf-8', errors='ignore').decode())
+    
+   if __name__ == '__main__':
+        list()
+
+Bugs and Feature Requests
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Found something that doesn't seem right or have a feature request? Please open a new issue.
+
+Copyright and License
+~~~~~~~~~~~~~~~~~~~~~
+.. image:: https://img.shields.io/github/license/fortifyadmin/fortifyapi.svg?style=flat-square
+
```

### Comparing `fortifyapi-3.1.7/setup.py` & `fortifyapi-3.1.8/setup.py`

 * *Files identical despite different names*

