# Comparing `tmp/languagemodels-0.3.1.tar.gz` & `tmp/languagemodels-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.3.1.tar", last modified: Wed Jun  7 16:59:40 2023, max compression
+gzip compressed data, was "languagemodels-0.3.2.tar", last modified: Thu Jun  8 01:45:08 2023, max compression
```

## Comparing `languagemodels-0.3.1.tar` & `languagemodels-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-07 16:59:40.884523 languagemodels-0.3.1/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8776 2023-06-07 16:59:40.884523 languagemodels-0.3.1/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-07 16:59:40.884523 languagemodels-0.3.1/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10085 2023-06-07 16:39:12.000000 languagemodels-0.3.1/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4415 2023-06-07 13:51:24.000000 languagemodels-0.3.1/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7633 2023-06-07 10:27:54.000000 languagemodels-0.3.1/languagemodels/inference.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-07 16:59:40.884523 languagemodels-0.3.1/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8776 2023-06-07 16:59:40.000000 languagemodels-0.3.1/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-07 16:59:40.000000 languagemodels-0.3.1/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-07 16:59:40.000000 languagemodels-0.3.1/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       53 2023-06-07 16:59:40.000000 languagemodels-0.3.1/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-07 16:59:40.000000 languagemodels-0.3.1/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-07 16:59:40.884523 languagemodels-0.3.1/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      792 2023-06-07 16:59:19.000000 languagemodels-0.3.1/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-08 01:45:08.791806 languagemodels-0.3.2/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8872 2023-06-08 01:45:08.791806 languagemodels-0.3.2/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-08 01:45:08.791806 languagemodels-0.3.2/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10565 2023-06-08 01:43:41.000000 languagemodels-0.3.2/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     4580 2023-06-08 01:33:35.000000 languagemodels-0.3.2/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7860 2023-06-08 01:43:41.000000 languagemodels-0.3.2/languagemodels/inference.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-08 01:45:08.791806 languagemodels-0.3.2/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8872 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      281 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       53 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-08 01:45:08.000000 languagemodels-0.3.2/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-08 01:45:08.791806 languagemodels-0.3.2/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      792 2023-06-08 01:44:57.000000 languagemodels-0.3.2/setup.py
```

### Comparing `languagemodels-0.3.1/PKG-INFO` & `languagemodels-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -150,27 +150,27 @@
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
         Advanced Usage
         --------------
         
-        This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face.
+        This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face. For integrating language models in more complex ways, [LangChain](https://github.com/hwchase17/langchain) or [guidance](https://github.com/microsoft/guidance) may be helpful.
         
         ### Large models
         
         The default model used for inference is around 250M parameters. There is a larger model that can be used if you don't mind things working a little more slowly. It can be enabled by setting the `LANGUAGEMODELS_SIZE` environment variable to `large`. This model isn't large by modern standards and should still work quickly in most environments (but not the lowest tier repl.it instance).
         
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
         - CLI Chatbot (see examples/chat.py)
-        - [Streamlit chatbot](https://jncraton-languagemodels-examplesstreamlitchat-g68aa2.streamlit.app/) (see examples/streamlitchat.py)
+        - Streamlit chatbot (see examples/streamlitchat.py)
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search over documents
         - Document question answering
```

### Comparing `languagemodels-0.3.1/languagemodels/__init__.py` & `languagemodels-0.3.2/languagemodels/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -159,14 +159,24 @@
         for m in messages
         if m["role"] in ["assistant", "user"]
     ]
 
     # Suppress all user messages to avoid repeating them
     suppress += [m["content"] for m in messages if m["role"] == "user"]
 
+    system_msgs = [m for m in messages if m["role"] == "system"]
+    assistant_msgs = [m for m in messages if m["role"] == "assistant"]
+    user_msgs = [m for m in messages if m["role"] == "user"]
+
+    # Use only the most recent user and assistant message for context
+    # Keep all system messages
+    # The current model is really tuned on instructions and tends to get
+    # lost if it sees too many questions
+    messages = system_msgs + assistant_msgs[-1:] + user_msgs[-1:]
+
     rolemap = {
         "system": "System",
         "user": "Question",
         "assistant": "Assistant",
     }
 
     messages = [f"{rolemap[m['role']]}: {m['content']}" for m in messages]
```

### Comparing `languagemodels-0.3.1/languagemodels/embeddings.py` & `languagemodels-0.3.2/languagemodels/embeddings.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,27 +46,27 @@
     128
     """
 
     def __init__(self, chunk_size=64, chunk_overlap=8):
         self.chunk_size = chunk_size
         self.chunk_overlap = chunk_overlap
         self.clear()
-        self.tokenizer, self.model = get_model("jncraton/all-MiniLM-L6-v2-ct2-int8")
-        self.chunk_tokenizer, _ = get_model("jncraton/LaMini-Flan-T5-248M-ct2-int8")
 
     def clear(self):
         self.docs = []
         self.embeddings = []
         self.chunks = []
         self.chunk_embeddings = []
 
     def get_embedding(self, doc):
         """Gets embeddings for a document"""
-        tokens = self.tokenizer.encode(doc).ids
-        output = self.model.forward_batch([tokens])
+        tokenizer, model = get_model("embedding")
+
+        tokens = tokenizer.encode(doc).ids
+        output = model.forward_batch([tokens])
         embedding = np.mean(np.array(output.last_hidden_state), axis=1)[0]
         embedding = embedding / np.linalg.norm(embedding)
         return embedding
 
     def store(self, doc):
         """Stores a document along with embeddings
 
@@ -92,22 +92,27 @@
         if doc not in self.docs:
             embedding = self.get_embedding(doc)
             self.embeddings.append(embedding)
             self.docs.append(doc)
             self.store_chunks(doc)
 
     def store_chunks(self, doc):
-        tokens = self.chunk_tokenizer.EncodeAsPieces(doc)
+        # Note that the tokenzier used here is from the generative model
+        # This is used for token counting for the context, not for tokenization
+        # before embedding
+        generative_tokenizer, _ = get_model("instruct")
+
+        tokens = generative_tokenizer.EncodeAsPieces(doc)
 
         end = max(len(tokens) - self.chunk_overlap, 1)
         stride = self.chunk_size - self.chunk_overlap
 
         for i in range(0, end, stride):
             chunk = tokens[i : i + self.chunk_size]
-            text = self.chunk_tokenizer.Decode(chunk)
+            text = generative_tokenizer.Decode(chunk)
             embedding = self.get_embedding(text)
             self.chunk_embeddings.append(embedding)
             self.chunks.append(text)
 
     def get_context(self, query, max_tokens=128):
         """Gets context matching a query
 
@@ -124,16 +129,18 @@
         doc_score_pairs = list(zip(self.chunks, scores))
 
         doc_score_pairs = sorted(doc_score_pairs, key=lambda x: x[1], reverse=True)
 
         chunks = []
         tokens = 0
 
+        generative_tokenizer, _ = get_model("instruct")
+
         for chunk, score in doc_score_pairs:
-            chunk_tokens = len(self.chunk_tokenizer.EncodeAsPieces(chunk))
+            chunk_tokens = len(generative_tokenizer.EncodeAsPieces(chunk))
             if tokens + chunk_tokens <= max_tokens and score > 0.1:
                 chunks.append(chunk)
                 tokens += chunk_tokens
 
         context = "\n\n".join(chunks)
 
         return context
```

### Comparing `languagemodels-0.3.1/languagemodels/inference.py` & `languagemodels-0.3.2/languagemodels/inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def list_tokens(prompt):
     """Generates a list of tokens for a supplied prompt
 
     >>> list_tokens("Hello, world!")
     [('▁Hello', 8774), (',', 6), ('▁world', 296), ('!', 55)]
     """
-    tokenizer, _ = get_model("jncraton/LaMini-Flan-T5-248M-ct2-int8")
+    tokenizer, _ = get_model("instruct")
 
     tokens = tokenizer.EncodeAsPieces(prompt)
     ids = tokenizer.EncodeAsIds(prompt)
 
     return list(zip(tokens, ids))
 
 
@@ -77,15 +77,22 @@
 
     try:
         return resp["choices"][0]["text"]
     except KeyError:
         raise InferenceException(f"OpenAI error: {resp}")
 
 
-def get_model(model_name):
+def get_model(model_type):
+    if model_type == "instruct":
+        model_name = "jncraton/LaMini-Flan-T5-248M-ct2-int8"
+    elif model_type == "embedding":
+        model_name = "jncraton/all-MiniLM-L6-v2-ct2-int8"
+    else:
+        raise InferenceException(f"Invalid model: {model_type}")
+
     if os.environ.get("LANGUAGEMODELS_SIZE") == "small":
         model_name = model_name.replace("base", "small")
         model_name = model_name.replace("248M", "77M")
 
     if os.environ.get("LANGUAGEMODELS_SIZE") == "large":
         model_name = model_name.replace("base", "large")
         model_name = model_name.replace("248M", "783M")
@@ -134,27 +141,28 @@
     """
     if os.environ.get("ts_key") or os.environ.get("ts_server"):
         return generate_ts("flan_t5_xxl_q4", prompt, max_tokens)
 
     if os.environ.get("oa_key"):
         return generate_oa("text-babbage-001", prompt, max_tokens)
 
-    tokenizer, model = get_model("jncraton/LaMini-Flan-T5-248M-ct2-int8")
+    tokenizer, model = get_model("instruct")
 
     suppress = [tokenizer.EncodeAsPieces(s) for s in suppress]
 
     input_tokens = tokenizer.EncodeAsPieces(prompt) + ["</s>"]
     results = model.translate_batch(
         [input_tokens],
         target_prefix=[tokenizer.EncodeAsPieces(prefix)],
         repetition_penalty=repetition_penalty,
         max_decoding_length=max_tokens,
         sampling_temperature=temperature,
         sampling_topk=40,
         suppress_sequences=suppress,
+        beam_size=2,
     )
 
     output_tokens = results[0].hypotheses[0]
 
     return tokenizer.DecodePieces(output_tokens)
```

### Comparing `languagemodels-0.3.1/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.3.2/languagemodels.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.3.1
+Version: 0.3.2
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
@@ -150,27 +150,27 @@
         ```
         
         [Full documentation](https://languagemodels.netlify.app/)
         
         Advanced Usage
         --------------
         
-        This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face.
+        This package is not meant for advanced usage. If you are looking for something more powerful you could explore [transformers](https://huggingface.co/docs/transformers) from Hugging Face. For integrating language models in more complex ways, [LangChain](https://github.com/hwchase17/langchain) or [guidance](https://github.com/microsoft/guidance) may be helpful.
         
         ### Large models
         
         The default model used for inference is around 250M parameters. There is a larger model that can be used if you don't mind things working a little more slowly. It can be enabled by setting the `LANGUAGEMODELS_SIZE` environment variable to `large`. This model isn't large by modern standards and should still work quickly in most environments (but not the lowest tier repl.it instance).
         
         Projects Ideas
         --------------
         
         This package can be used to do the heavy lifting for a number of learning projects:
         
         - CLI Chatbot (see examples/chat.py)
-        - [Streamlit chatbot](https://jncraton-languagemodels-examplesstreamlitchat-g68aa2.streamlit.app/) (see examples/streamlitchat.py)
+        - Streamlit chatbot (see examples/streamlitchat.py)
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search over documents
         - Document question answering
```

### Comparing `languagemodels-0.3.1/setup.py` & `languagemodels-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.3.1",
+    version="0.3.2",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
```

