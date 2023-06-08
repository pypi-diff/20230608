# Comparing `tmp/acapela_downloader_py-0.0.1.tar.gz` & `tmp/acapela_downloader_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\janaa\source\repos\Acapella-Downloader-Python\dist\.tmp-o_oinhym\acapela_downloader_py-0.0.1.tar", last modified: Thu Jun  8 13:18:10 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.0.3.tar", last modified: Thu Jun  8 13:56:23 2023, max compression
```

## Comparing `acapela_downloader_py-0.0.1.tar` & `acapela_downloader_py-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:10.480587 acapela_downloader_py-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-08 13:16:54.000000 acapela_downloader_py-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      844 2023-06-08 13:18:10.480587 acapela_downloader_py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-06-08 13:16:54.000000 acapela_downloader_py-0.0.1/README.md
--rw-rw-rw-   0        0        0      352 2023-06-08 13:04:54.000000 acapela_downloader_py-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 13:18:10.480587 acapela_downloader_py-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:10.466624 acapela_downloader_py-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:10.469107 acapela_downloader_py-0.0.1/src/acapela_downloader_memer/
--rw-rw-rw-   0        0        0        0 2023-06-08 13:02:08.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_memer/__init__,py.py
--rw-rw-rw-   0        0        0      436 2023-06-08 13:09:04.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_memer/acapela.py
--rw-rw-rw-   0        0        0     1772 2023-06-08 12:59:52.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_memer/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 13:18:10.480090 acapela_downloader_py-0.0.1/src/acapela_downloader_py.egg-info/
--rw-rw-rw-   0        0        0      844 2023-06-08 13:18:10.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-06-08 13:18:10.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 13:18:10.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-08 13:18:10.000000 acapela_downloader_py-0.0.1/src/acapela_downloader_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:23.991738 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 13:56:23.000000 acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-08 13:56:09.000000 acapela_downloader_py-0.0.3/src/utils.py
```

### Comparing `acapela_downloader_py-0.0.1/LICENSE` & `acapela_downloader_py-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `acapela_downloader_py-0.0.1/PKG-INFO` & `acapela_downloader_py-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
-Name: acapela_downloader_py
-Version: 0.0.1
-Summary: Acapela pwned but in Python.
-Author: JWKK
-Project-URL: Homepage, https://memerdev.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Acapela Downloader but in Python
-Translated over to Python from C#: https://github.com/weespin/WillFromAfarDownloader
-
-# How to use
-It's pretty damn easy, just import the generate_audio function from the package and fill out the necessary arguments.
-
-``` python
-from acapela import generate_audio
-generate_audio("Great Test", "enu_willhappy_22k_ns.bvcu", "output.mp3")
-```
-
-## Other Stuff
-
-If you find any code from StupidTown in my package feel free to make a pull request.
+Metadata-Version: 2.1
+Name: acapela_downloader_py
+Version: 0.0.3
+Summary: Acapela pwned but in Python.
+Author: JWKK
+Project-URL: Homepage, https://memerdev.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Acapela Downloader but in Python
+Translated over to Python from C#: https://github.com/weespin/WillFromAfarDownloader
+
+# How to use
+It's pretty damn easy, just import the generate_audio function from the package and fill out the necessary arguments.
+
+``` python
+from acapela import generate_audio
+generate_audio("Great Test", "enu_willhappy_22k_ns.bvcu", "output.mp3")
+```
+
+## Other Stuff
+
+If you find any code from StupidTown in my package feel free to make a pull request.
```

### Comparing `acapela_downloader_py-0.0.1/src/acapela_downloader_memer/utils.py` & `acapela_downloader_py-0.0.3/src/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-import random
-import string
-import re
-from requests import post
-
-NONCE_ENDPOINT = "https://acapelavoices.acapela-group.com/index/getnonce/"
-SYNTHESIZER_ENDPOINT = "https://www.acapela-group.com:8443/Services/Synthesizer"
-cached_nonce = ""
-cached_email = ""
-last_failed = False
-
-
-def update_nonce_token():
-    global NONCE_ENDPOINT
-    global cached_nonce
-    global cached_email
-    global last_failed
-    EMAIL_LENGTH = random.randint(10, 20)
-    fake_email = ""
-    for i in range(EMAIL_LENGTH):
-        fake_email += random.choice(string.ascii_letters)
-    print(fake_email)
-    fake_email += "@gmail.com"
-    nonce_response = post(NONCE_ENDPOINT, json={
-        "googleid": fake_email
-    })
-    if len(nonce_response.json()["nonce"]) > 1:
-        cached_nonce = nonce_response.json()["nonce"]
-        cached_email = fake_email
-    last_failed = False
-    print(cached_nonce + " " + cached_email)
-
-
-def get_sound_link(text, voice_id):
-    if cached_email == "" or cached_nonce == "" or last_failed:
-        update_nonce_token()
-    synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
-    synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
-    headers = {'Content-type': 'application/x-www-form-urlencoded', 'Content-Length': str(len(synthesizer_request_bytes))}
-    synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
-    split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
-    return split_res[1]
-
-
+import random
+import string
+import re
+from requests import post
+
+NONCE_ENDPOINT = "https://acapelavoices.acapela-group.com/index/getnonce/"
+SYNTHESIZER_ENDPOINT = "https://www.acapela-group.com:8443/Services/Synthesizer"
+cached_nonce = ""
+cached_email = ""
+
+
+def update_nonce_token():
+    global NONCE_ENDPOINT
+    global cached_nonce
+    global cached_email
+    global last_failed
+    EMAIL_LENGTH = random.randint(10, 20)
+    fake_email = ""
+    for i in range(EMAIL_LENGTH):
+        fake_email += random.choice(string.ascii_letters)
+    print(fake_email)
+    fake_email += "@gmail.com"
+    nonce_response = post(NONCE_ENDPOINT, json={
+        "googleid": fake_email
+    })
+    if len(nonce_response.json()["nonce"]) > 1:
+        cached_nonce = nonce_response.json()["nonce"]
+        cached_email = fake_email
+
+
+def get_sound_link(text, voice_id):
+    if cached_email == "" or cached_nonce == "" or last_failed:
+        update_nonce_token()
+    synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
+    synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
+    headers = {'Content-type': 'application/x-www-form-urlencoded', 'Content-Length': str(len(synthesizer_request_bytes))}
+    synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
+    split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
+    return split_res[1]
+
+
```

### Comparing `acapela_downloader_py-0.0.1/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.0.3/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1
-Name: acapela-downloader-py
-Version: 0.0.1
-Summary: Acapela pwned but in Python.
-Author: JWKK
-Project-URL: Homepage, https://memerdev.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Acapela Downloader but in Python
-Translated over to Python from C#: https://github.com/weespin/WillFromAfarDownloader
-
-# How to use
-It's pretty damn easy, just import the generate_audio function from the package and fill out the necessary arguments.
-
-``` python
-from acapela import generate_audio
-generate_audio("Great Test", "enu_willhappy_22k_ns.bvcu", "output.mp3")
-```
-
-## Other Stuff
-
-If you find any code from StupidTown in my package feel free to make a pull request.
+Metadata-Version: 2.1
+Name: acapela-downloader-py
+Version: 0.0.3
+Summary: Acapela pwned but in Python.
+Author: JWKK
+Project-URL: Homepage, https://memerdev.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Acapela Downloader but in Python
+Translated over to Python from C#: https://github.com/weespin/WillFromAfarDownloader
+
+# How to use
+It's pretty damn easy, just import the generate_audio function from the package and fill out the necessary arguments.
+
+``` python
+from acapela import generate_audio
+generate_audio("Great Test", "enu_willhappy_22k_ns.bvcu", "output.mp3")
+```
+
+## Other Stuff
+
+If you find any code from StupidTown in my package feel free to make a pull request.
```

