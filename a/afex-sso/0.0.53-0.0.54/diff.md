# Comparing `tmp/afex-sso-0.0.53.tar.gz` & `tmp/afex-sso-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.53.tar", last modified: Tue Jun  6 17:10:43 2023, max compression
+gzip compressed data, was "afex-sso-0.0.54.tar", last modified: Thu Jun  8 16:41:10 2023, max compression
```

## Comparing `afex-sso-0.0.53.tar` & `afex-sso-0.0.54.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-06 17:10:43.074970 afex-sso-0.0.53/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.53/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     1615 2023-06-06 17:10:43.075078 afex-sso-0.0.53/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1170 2023-05-10 08:31:16.000000 afex-sso-0.0.53/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-06 17:10:43.070223 afex-sso-0.0.53/app/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-06 17:10:43.073561 afex-sso-0.0.53/app/AFEX_SSO/
--rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.53/app/AFEX_SSO/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-06 17:10:43.074008 afex-sso-0.0.53/app/AFEX_SSO/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.53/app/AFEX_SSO/src/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1708 2023-06-06 17:04:46.000000 afex-sso-0.0.53/app/AFEX_SSO/src/sso.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-06 17:10:43.074791 afex-sso-0.0.53/app/afex_sso.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1615 2023-06-06 17:10:43.000000 afex-sso-0.0.53/app/afex_sso.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      308 2023-06-06 17:10:43.000000 afex-sso-0.0.53/app/afex_sso.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-06 17:10:43.000000 afex-sso-0.0.53/app/afex_sso.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       61 2023-06-06 17:10:43.000000 afex-sso-0.0.53/app/afex_sso.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        9 2023-06-06 17:10:43.000000 afex-sso-0.0.53/app/afex_sso.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.53/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)      474 2023-06-06 17:10:43.075421 afex-sso-0.0.53/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      802 2023-06-06 17:09:55.000000 afex-sso-0.0.53/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:41:10.695762 afex-sso-0.0.54/
+-rw-rw-rw-   0        0        0     1069 2023-04-05 13:47:57.000000 afex-sso-0.0.54/LICENSE
+-rw-rw-rw-   0        0        0     2315 2023-06-08 16:41:10.695762 afex-sso-0.0.54/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-06-08 16:38:28.000000 afex-sso-0.0.54/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 16:41:10.311873 afex-sso-0.0.54/app/
+drwxrwxrwx   0        0        0        0 2023-06-08 16:41:10.473560 afex-sso-0.0.54/app/AFEX_SSO/
+-rw-rw-rw-   0        0        0       36 2023-04-05 13:47:57.000000 afex-sso-0.0.54/app/AFEX_SSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:41:10.603339 afex-sso-0.0.54/app/AFEX_SSO/src/
+-rw-rw-rw-   0        0        0        0 2023-04-05 13:47:57.000000 afex-sso-0.0.54/app/AFEX_SSO/src/__init__.py
+-rw-rw-rw-   0        0        0      270 2023-06-07 09:13:59.000000 afex-sso-0.0.54/app/AFEX_SSO/src/get_hash_key.py
+-rw-rw-rw-   0        0        0     2115 2023-06-08 16:12:31.000000 afex-sso-0.0.54/app/AFEX_SSO/src/sso.py
+-rw-rw-rw-   0        0        0     1907 2023-06-07 16:54:05.000000 afex-sso-0.0.54/app/AFEX_SSO/src/views.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:41:10.690358 afex-sso-0.0.54/app/afex_sso.egg-info/
+-rw-rw-rw-   0        0        0     2315 2023-06-08 16:41:09.000000 afex-sso-0.0.54/app/afex_sso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-06-08 16:41:09.000000 afex-sso-0.0.54/app/afex_sso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:41:09.000000 afex-sso-0.0.54/app/afex_sso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-08 16:41:09.000000 afex-sso-0.0.54/app/afex_sso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 16:41:09.000000 afex-sso-0.0.54/app/afex_sso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-05 13:47:57.000000 afex-sso-0.0.54/pyproject.toml
+-rw-rw-rw-   0        0        0      497 2023-06-08 16:41:10.718506 afex-sso-0.0.54/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-06-08 16:17:50.000000 afex-sso-0.0.54/setup.py
```

### Comparing `afex-sso-0.0.53/LICENSE` & `afex-sso-0.0.54/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2023 AFEX NIGERIA
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright (c) 2023 AFEX NIGERIA
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `afex-sso-0.0.53/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.54/app/AFEX_SSO/src/sso.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import time
 import json
 import requests
 from django.conf import settings as app_settings
+from django.utils import timezone
 
 URL = app_settings.SSO_URL
+API_KEY = app_settings.SSO_API_KEY
+SECRET_KEY = app_settings.SSO_SECRET_KEY
 
 
 # settings.configure()
 # os.environ.setdefault("DJANGO_SETTINGS_MODULE", "SSO.settings")
 
 
 class SSO:
@@ -20,35 +23,46 @@
     #     self.hash = sp_hash_key
     #     self.session = session_key
 
     # def __call__(self):
     #     return self.check_credentials(self.api, self.hash, self.session)
 
 
-    def check_credentials(self, sp_api_key, sp_hash_key, session_key):
+    def check_credentials(self, session_key):
         try:
+            HASH_KEY = get_hash_key(
+                api_key=API_KEY,
+                secret_key=SECRET_KEY,
+                idempotency_key=session_key
+            )
             headers = {
-                "api-key": sp_api_key,
-                "hash-key":  sp_hash_key,
+                "api-key": API_KEY,
+                "hash-key":  HASH_KEY,
                 "request-ts": session_key
             }
             response = requests.get(
                 f"{URL}/v1/api/verify_sp/{session_key}", headers=headers)
             data = json.loads(response.text)
             return data
 
         except Exception as e:
             return f"Something went wrong, please confirm the credentials and try again: {e}"
 
-    def sign_out(self, sp_api_key, sp_hash_key, session_key, email: str):
+    def sign_out(self, email: str):
         try:
+            REQUEST_TS = timezone.now()
+            HASH_KEY = get_hash_key(
+                api_key=API_KEY,
+                secret_key=SECRET_KEY,
+                idempotency_key=REQUEST_TS
+            )
             headers = {
-                "api-key": sp_api_key,
-                "hash-key": sp_hash_key,
-                "request-ts": session_key
+                "api-key": API_KEY,
+                "hash-key": HASH_KEY,
+                "request-ts": REQUEST_TS
             }
             data = {
                 "email": email
             }
             response = requests.post(
                 f"{URL}/v1/api/signout", headers=headers, data=data)
             data = json.loads(response.text)
```

### Comparing `afex-sso-0.0.53/setup.py` & `afex-sso-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.53",
+    version="0.0.54",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
```

