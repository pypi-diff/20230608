# Comparing `tmp/vector_vault-2.0.2.tar.gz` & `tmp/vector_vault-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.2.tar", last modified: Thu Jun  8 04:40:42 2023, max compression
+gzip compressed data, was "vector_vault-2.0.3.tar", last modified: Thu Jun  8 04:46:48 2023, max compression
```

## Comparing `vector_vault-2.0.2.tar` & `vector_vault-2.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:40:42.931211 vector_vault-2.0.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20851 2023-06-08 04:40:42.931074 vector_vault-2.0.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20126 2023-06-07 13:52:11.000000 vector_vault-2.0.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-08 04:40:42.931249 vector_vault-2.0.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-08 04:40:36.000000 vector_vault-2.0.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:40:42.928079 vector_vault-2.0.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20851 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      452 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:40:42.930788 vector_vault-2.0.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)    13624 2023-06-08 04:36:15.000000 vector_vault-2.0.2/vectorvault/ToolsGPT.py
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-08 04:35:31.000000 vector_vault-2.0.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.2/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30728 2023-06-08 04:35:55.000000 vector_vault-2.0.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:46:48.712514 vector_vault-2.0.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:46:48.712387 vector_vault-2.0.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20080 2023-06-08 04:45:19.000000 vector_vault-2.0.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-08 04:46:48.712549 vector_vault-2.0.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-08 04:46:37.000000 vector_vault-2.0.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:46:48.708952 vector_vault-2.0.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      452 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:46:48.712106 vector_vault-2.0.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)    13625 2023-06-08 04:46:25.000000 vector_vault-2.0.3/vectorvault/ToolsGPT.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-08 04:35:31.000000 vector_vault-2.0.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.3/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30728 2023-06-08 04:35:55.000000 vector_vault-2.0.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.3/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.2/LICENSE` & `vector_vault-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/PKG-INFO` & `vector_vault-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.0.2
+Version: 2.0.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -50,15 +50,15 @@
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-# Build Your Vault:
+# Access The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
@@ -71,15 +71,15 @@
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
 ```
 The api key will be sent to your email.
 
 <br>
 
-# Use Vector Vault:
+# Build The Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (new vault will be created if name does not exist)
@@ -113,15 +113,15 @@
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 <br>
 <br>
 
-# Vault Call:
+# Use The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
 Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
@@ -177,15 +177,15 @@
 ```
 
 
 <br>
 <br>
 
 # ChatGPT
-## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+## Use ChatGPT with `get_chat()` 
 
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
 </p>
 <br>
 
 Get chat response from OpenAI's ChatGPT.
```

### Comparing `vector_vault-2.0.2/README.md` & `vector_vault-2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-# Build Your Vault:
+# Access The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
@@ -52,15 +52,15 @@
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
 ```
 The api key will be sent to your email.
 
 <br>
 
-# Use Vector Vault:
+# Build The Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (new vault will be created if name does not exist)
@@ -94,15 +94,15 @@
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 <br>
 <br>
 
-# Vault Call:
+# Use The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
 Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
@@ -158,15 +158,15 @@
 ```
 
 
 <br>
 <br>
 
 # ChatGPT
-## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+## Use ChatGPT with `get_chat()` 
 
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
 </p>
 <br>
 
 Get chat response from OpenAI's ChatGPT.
```

### Comparing `vector_vault-2.0.2/setup.py` & `vector_vault-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.2",
+    version="2.0.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.3/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.2
+Version: 2.0.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -50,15 +50,15 @@
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-# Build Your Vault:
+# Access The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
@@ -71,15 +71,15 @@
 
 register(first_name='John', last_name='Smith', email='john@smith.com', password='make_a_password')
 ```
 The api key will be sent to your email.
 
 <br>
 
-# Use Vector Vault:
+# Build The Vault:
 
 Set your openai key as an envorionment variable
 ```
 os.environ['OPENAI_API_KEY'] = 'your_openai_api_key'
 ```
 
 1. Create a Vault instance - (new vault will be created if name does not exist)
@@ -113,15 +113,15 @@
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 <br>
 <br>
 
-# Vault Call:
+# Use The Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
 Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
@@ -177,15 +177,15 @@
 ```
 
 
 <br>
 <br>
 
 # ChatGPT
-## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+## Use ChatGPT with `get_chat()` 
 
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
 </p>
 <br>
 
 Get chat response from OpenAI's ChatGPT.
```

### Comparing `vector_vault-2.0.2/vectorvault/ToolsGPT.py` & `vector_vault-2.0.3/vectorvault/ToolsGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ai import AI
+from .ai import AI
 
 '''
     ToolsGPT is a set of tools special to large language models. 
     Every tool turns subjectivity into objectivity.
     
     Objectivity is needed for code. 
     Subjectivity is the primary human input.
```

### Comparing `vector_vault-2.0.2/vectorvault/__init__.py` & `vector_vault-2.0.3/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/ai.py` & `vector_vault-2.0.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/cloudmanager.py` & `vector_vault-2.0.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/creds.py` & `vector_vault-2.0.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/download.py` & `vector_vault-2.0.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/itemize.py` & `vector_vault-2.0.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/signup.py` & `vector_vault-2.0.3/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/vault.py` & `vector_vault-2.0.3/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.2/vectorvault/vecreq.py` & `vector_vault-2.0.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

