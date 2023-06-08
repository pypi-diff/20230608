# Comparing `tmp/langdash-1.0.0a1.tar.gz` & `tmp/langdash-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.0.0a1.tar", last modified: Wed Jun  7 03:27:37 2023, max compression
+gzip compressed data, was "langdash-1.0.1a1.tar", last modified: Thu Jun  8 05:13:08 2023, max compression
```

## Comparing `langdash-1.0.0a1.tar` & `langdash-1.0.1a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.303313 langdash-1.0.0a1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.0.0a1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.0.0a1/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     2510 2023-06-07 03:27:37.303313 langdash-1.0.0a1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1601 2023-06-07 03:10:35.000000 langdash-1.0.0a1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       63 2023-06-07 03:02:15.000000 langdash-1.0.0a1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    21883 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.0.0a1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      779 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.303313 langdash-1.0.0a1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.0.0a1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/models/_bpe.py
--rw-rw-r--   0 user      (1000) user      (1000)     6343 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7973 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6920 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2577 2023-06-06 03:06:05.000000 langdash-1.0.0a1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.0.0a1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1117 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2787 2023-06-07 02:26:23.000000 langdash-1.0.0a1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-07 03:27:37.299313 langdash-1.0.0a1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     2510 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-07 03:27:37.000000 langdash-1.0.0a1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-07 03:27:37.303313 langdash-1.0.0a1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.0.0a1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.0.1a1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.0.1a1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-08 05:13:08.089345 langdash-1.0.1a1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1804 2023-06-08 05:12:48.000000 langdash-1.0.1a1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       64 2023-06-08 05:11:44.000000 langdash-1.0.1a1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21883 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.085345 langdash-1.0.1a1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.0.1a1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6224 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      779 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7006 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.0.1a1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1886 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/models/_bpe.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6418 2023-06-07 19:42:20.000000 langdash-1.0.1a1/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7973 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      989 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6920 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2577 2023-06-06 03:06:05.000000 langdash-1.0.1a1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.0.1a1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1117 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      947 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2787 2023-06-07 02:26:23.000000 langdash-1.0.1a1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-08 05:13:08.089345 langdash-1.0.1a1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     2713 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1239 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      167 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-08 05:13:08.000000 langdash-1.0.1a1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-08 05:13:08.089345 langdash-1.0.1a1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1560 2023-06-07 02:26:23.000000 langdash-1.0.1a1/setup.py
```

### Comparing `langdash-1.0.0a1/LICENSE.txt` & `langdash-1.0.1a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/PKG-INFO` & `langdash-1.0.1a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.0.0a1
+Version: 1.0.1a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,16 @@
 Provides-Extra: llama_cpp
 Provides-Extra: transformers
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
+[**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
+
 A simple library for interfacing with language models.
 
 **Currently in alpha!**
 
 Features:
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
@@ -56,14 +58,15 @@
 **Note:** If running from source, initialize the git submodules in the `langdash/extern` folder to compile foreign backends.
     
 ## Usage
 
 Examples:
 
   * [Text generation](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/text-generation.md)
+  * [Generating TV shows](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/generating-tv-shows.md)
   * [Embedding search](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/embedding-search.md)
 
 See [examples folder](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/examples) for full examples.
 
 ## License
 
 Apache 2.0
```

### Comparing `langdash-1.0.0a1/README.md` & `langdash-1.0.1a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # langdash
 
+[**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
+
 A simple library for interfacing with language models.
 
 **Currently in alpha!**
 
 Features:
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
@@ -32,14 +34,15 @@
 **Note:** If running from source, initialize the git submodules in the `langdash/extern` folder to compile foreign backends.
     
 ## Usage
 
 Examples:
 
   * [Text generation](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/text-generation.md)
+  * [Generating TV shows](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/generating-tv-shows.md)
   * [Embedding search](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/embedding-search.md)
 
 See [examples folder](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/examples) for full examples.
 
 ## License
 
 Apache 2.0
```

### Comparing `langdash-1.0.0a1/langdash/chains.py` & `langdash-1.0.1a1/langdash/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/classify/token_qa.py` & `langdash-1.0.1a1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/core.py` & `langdash-1.0.1a1/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/infer.py` & `langdash-1.0.1a1/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/llm.py` & `langdash-1.0.1a1/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/llm_session.py` & `langdash-1.0.1a1/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/models/_bpe.py` & `langdash-1.0.1a1/langdash/models/_bpe.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/models/llama_cpp.py` & `langdash-1.0.1a1/langdash/models/llama_cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   Session for llama.cpp model.
   """
 
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
 
     def load_model(llm: LlamaCppModel):
-      return LlamaWrapper(model_path=llm._model_path)
+      return LlamaWrapper(model_path=llm._model_path, **llm._model_kwargs)
 
     self._llama = self._ld._get_model_internal(self._llm, load_model)
     self._eos_token = Llama.token_eos()
     self._bos_token = Llama.token_bos()
 
     self._logits = None
     self._state = None
@@ -198,12 +198,13 @@
 class LlamaCppModel(LLM[LlamaCppSession]):
   """
   llama.cpp model.
   """
 
   Session = LlamaCppSession
 
-  def __init__(self, model_path: str):
+  def __init__(self, model_path: str, **model_kwargs):
     self._model_path = model_path
+    self._model_kwargs = model_kwargs
 
   def session(self, **kwargs):
     return LlamaCppSession(self, **kwargs)
```

### Comparing `langdash-1.0.0a1/langdash/models/mock.py` & `langdash-1.0.1a1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/models/rwkv_cpp.py` & `langdash-1.0.1a1/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/models/sentence_transformers.py` & `langdash-1.0.1a1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/models/transformers.py` & `langdash-1.0.1a1/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/response.py` & `langdash-1.0.1a1/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/sampling.py` & `langdash-1.0.1a1/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/search/embedding_search.py` & `langdash-1.0.1a1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/search/engine.py` & `langdash-1.0.1a1/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash/search/multichoice_search.py` & `langdash-1.0.1a1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/langdash.egg-info/PKG-INFO` & `langdash-1.0.1a1/langdash.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.0.0a1
+Version: 1.0.1a1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,16 @@
 Provides-Extra: llama_cpp
 Provides-Extra: transformers
 Provides-Extra: sentence_transformers
 License-File: LICENSE.txt
 
 # langdash
 
+[**Announcement post**](https://mysymphony.jp.net/a/langdash-announcement/)
+
 A simple library for interfacing with language models.
 
 **Currently in alpha!**
 
 Features:
   
   * Support for text generation, text classification (through prompting) and vector-based document searching.
@@ -56,14 +58,15 @@
 **Note:** If running from source, initialize the git submodules in the `langdash/extern` folder to compile foreign backends.
     
 ## Usage
 
 Examples:
 
   * [Text generation](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/text-generation.md)
+  * [Generating TV shows](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/generating-tv-shows.md)
   * [Embedding search](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/docs/examples/embedding-search.md)
 
 See [examples folder](https://git.mysymphony.jp.net/nana/langdash/src/branch/master/examples) for full examples.
 
 ## License
 
 Apache 2.0
```

### Comparing `langdash-1.0.0a1/langdash.egg-info/SOURCES.txt` & `langdash-1.0.1a1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.0.0a1/setup.py` & `langdash-1.0.1a1/setup.py`

 * *Files identical despite different names*

