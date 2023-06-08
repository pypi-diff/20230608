# Comparing `tmp/vector_vault-2.0.3.tar.gz` & `tmp/vector_vault-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.3.tar", last modified: Thu Jun  8 04:46:48 2023, max compression
+gzip compressed data, was "vector_vault-2.0.4.tar", last modified: Thu Jun  8 04:55:05 2023, max compression
```

## Comparing `vector_vault-2.0.3.tar` & `vector_vault-2.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:46:48.712514 vector_vault-2.0.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:46:48.712387 vector_vault-2.0.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20080 2023-06-08 04:45:19.000000 vector_vault-2.0.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-08 04:46:48.712549 vector_vault-2.0.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-08 04:46:37.000000 vector_vault-2.0.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:46:48.708952 vector_vault-2.0.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      452 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-08 04:46:48.000000 vector_vault-2.0.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:46:48.712106 vector_vault-2.0.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)    13625 2023-06-08 04:46:25.000000 vector_vault-2.0.3/vectorvault/ToolsGPT.py
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-08 04:35:31.000000 vector_vault-2.0.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.3/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30728 2023-06-08 04:35:55.000000 vector_vault-2.0.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:55:05.426277 vector_vault-2.0.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:55:05.426146 vector_vault-2.0.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20080 2023-06-08 04:45:19.000000 vector_vault-2.0.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-08 04:55:05.426319 vector_vault-2.0.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-08 04:54:41.000000 vector_vault-2.0.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:55:05.422977 vector_vault-2.0.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20805 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      453 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-08 04:55:05.000000 vector_vault-2.0.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:55:05.425845 vector_vault-2.0.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      143 2023-06-08 04:54:12.000000 vector_vault-2.0.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-08 04:35:31.000000 vector_vault-2.0.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.4/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13627 2023-06-08 04:54:57.000000 vector_vault-2.0.4/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30728 2023-06-08 04:35:55.000000 vector_vault-2.0.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.4/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.4/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.3/LICENSE` & `vector_vault-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/PKG-INFO` & `vector_vault-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.0.3
+Version: 2.0.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.0.3/README.md` & `vector_vault-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/setup.py` & `vector_vault-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.3",
+    version="2.0.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.4/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.3
+Version: 2.0.4
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-2.0.3/vectorvault/ToolsGPT.py` & `vector_vault-2.0.4/vectorvault/tools_gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         
         4. Match or Make
             Get a match to a list of options, or make a new one if unrelated
             Useful if you aren't sure if the input will match one of your existing list options, and need flexibility of creating a new one
 
 '''
 
-class ToolsGPT:
+class ToolsGPT():
     def __init__(self, verbose=False):
         self.verbose = verbose
         self.llm = AI().llm
 
     def get_rating(self, text: str, concept_to_rate_for: str = 'Quality', model='gpt-3.5-turbo', custom_prompt=False, loop_limit=20) -> int:
         '''
             Get a numeric rating out of 10. Input plain text, and optionally include a concept to rate for
```

### Comparing `vector_vault-2.0.3/vectorvault/ai.py` & `vector_vault-2.0.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/cloudmanager.py` & `vector_vault-2.0.4/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/creds.py` & `vector_vault-2.0.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/download.py` & `vector_vault-2.0.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/itemize.py` & `vector_vault-2.0.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/signup.py` & `vector_vault-2.0.4/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/vault.py` & `vector_vault-2.0.4/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.3/vectorvault/vecreq.py` & `vector_vault-2.0.4/vectorvault/vecreq.py`

 * *Files identical despite different names*

