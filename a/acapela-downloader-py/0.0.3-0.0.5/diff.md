# Comparing `tmp/acapela_downloader_py-0.0.3.tar.gz` & `tmp/acapela_downloader_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.0.3.tar", last modified: Thu Jun  8 13:56:23 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.0.5.tar", last modified: Thu Jun  8 14:55:49 2023, max compression
```

## Comparing `acapela_downloader_py-0.0.3.tar` & `acapela_downloader_py-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:49.226177 acapela_downloader_py-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 14:55:39.000000 acapela_downloader_py-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 14:55:49.226177 acapela_downloader_py-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 14:55:39.000000 acapela_downloader_py-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 14:55:39.000000 acapela_downloader_py-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:55:49.226177 acapela_downloader_py-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:49.226177 acapela_downloader_py-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 14:55:39.000000 acapela_downloader_py-0.0.5/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:55:49.226177 acapela_downloader_py-0.0.5/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 14:55:49.000000 acapela_downloader_py-0.0.5/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 14:55:49.000000 acapela_downloader_py-0.0.5/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:55:49.000000 acapela_downloader_py-0.0.5/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 14:55:49.000000 acapela_downloader_py-0.0.5/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-08 14:55:39.000000 acapela_downloader_py-0.0.5/src/utils.py
```

### Comparing `acapela_downloader_py-0.0.3/LICENSE` & `acapela_downloader_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.0.3/PKG-INFO` & `acapela_downloader_py-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela_downloader_py
-Version: 0.0.3
+Version: 0.0.5
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.0.5/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.0.3
+Version: 0.0.5
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `acapela_downloader_py-0.0.3/src/utils.py` & `acapela_downloader_py-0.0.5/src/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     })
     if len(nonce_response.json()["nonce"]) > 1:
         cached_nonce = nonce_response.json()["nonce"]
         cached_email = fake_email
 
 
 def get_sound_link(text, voice_id):
-    if cached_email == "" or cached_nonce == "" or last_failed:
+    if cached_email == "" or cached_nonce == "":
         update_nonce_token()
     synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
     synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
     headers = {'Content-type': 'application/x-www-form-urlencoded', 'Content-Length': str(len(synthesizer_request_bytes))}
     synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
     split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
     return split_res[1]
```

