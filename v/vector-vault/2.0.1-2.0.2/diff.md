# Comparing `tmp/vector_vault-2.0.1.tar.gz` & `tmp/vector_vault-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-2.0.1.tar", last modified: Tue Jun  6 04:54:51 2023, max compression
+gzip compressed data, was "vector_vault-2.0.2.tar", last modified: Thu Jun  8 04:40:42 2023, max compression
```

## Comparing `vector_vault-2.0.1.tar` & `vector_vault-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-06 04:54:51.190930 vector_vault-2.0.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-06 04:54:51.190635 vector_vault-2.0.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19513 2023-06-05 09:15:29.000000 vector_vault-2.0.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-06 04:54:51.190975 vector_vault-2.0.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-06 04:54:19.000000 vector_vault-2.0.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-06 04:54:51.187549 vector_vault-2.0.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-06 04:54:51.000000 vector_vault-2.0.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-06 04:54:51.190365 vector_vault-2.0.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    14478 2023-06-06 01:07:30.000000 vector_vault-2.0.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-06 04:53:47.000000 vector_vault-2.0.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-2.0.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-2.0.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-06 04:53:41.000000 vector_vault-2.0.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.1/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    30689 2023-06-06 04:53:35.000000 vector_vault-2.0.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.1/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-2.0.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:40:42.931211 vector_vault-2.0.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20851 2023-06-08 04:40:42.931074 vector_vault-2.0.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20126 2023-06-07 13:52:11.000000 vector_vault-2.0.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-08 04:40:42.931249 vector_vault-2.0.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-08 04:40:36.000000 vector_vault-2.0.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:40:42.928079 vector_vault-2.0.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20851 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      452 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-08 04:40:42.000000 vector_vault-2.0.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-08 04:40:42.930788 vector_vault-2.0.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)    13624 2023-06-08 04:36:15.000000 vector_vault-2.0.2/vectorvault/ToolsGPT.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13298 2023-06-08 04:36:35.000000 vector_vault-2.0.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3148 2023-06-08 04:35:18.000000 vector_vault-2.0.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-06-08 04:35:26.000000 vector_vault-2.0.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-06-08 04:35:41.000000 vector_vault-2.0.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-08 04:35:31.000000 vector_vault-2.0.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.2/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    30728 2023-06-08 04:35:55.000000 vector_vault-2.0.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.2/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-2.0.2/vectorvault/wrap.py
```

### Comparing `vector_vault-2.0.1/LICENSE` & `vector_vault-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.1/PKG-INFO` & `vector_vault-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 2.0.1
+Version: 2.0.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -15,21 +15,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
+Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud with under one second response times.
 
-By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
+The `vectorvault` package comes with extensive chat functionality, so that you don't have to think about the details and can make smooth chat applications with ease. Speaking of smooth chat experiences, `vectorvault` also comes with chat streaming built-in. Simply use the `get_chat_stream()` function that works just like the regular `get_chat()` but with streaming. 
 
-Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
+`langchain` is a popular package for building functionality with llms, but when it comes to referencing vector databases, the database retrieval and chat integration can be complicated and difficult. This is one of the reasons we built `vectorvault`. We've integrated all the chat options people like to use with `langchain`, but made them all easier and more straight forward to use. Now with Vector Vault, integrating vector database results into generative chat applications is not only easy, it's the default. You also have total control over every aspect with parameters. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you.
 
-The `vectorvault` package allows you to interact with your Cloud Vaults using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
+By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a Vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up at [VectorVault.io](https://vectorvault.io)
+
+The `vectorvault` package allows you to interact with your Vault Cloud using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
 
 <br>
 
 Basic Interactions:
 
 `add()` : Prepares data to be added to the Vault, with automatic text splitting and processing for long texts. 
 <br>
@@ -99,40 +101,27 @@
 
 vault.save()
 ```
 
 <br>
 <br>
 
-Now that you have saved some data to the vault, you can add more at anytime, and your vault will automatically handle the adding process. These three lines execute very fast.
-```
-vault.add(more_text_data)
-
-vault.get_vectors()
-
-vault.save()
-```
-
-<br>
-<br>
-
-`vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed.
-`vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
+Now that you have saved some data to the vault, you can add more at anytime. `vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed. `vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
 ```
-vault.add(insanely_large_text_data)
+vault.add(very_large_text)
 vault.get_vectors() 
 vault.save() 
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 <br>
 <br>
 
-# Call Your Vault:
+# Vault Call:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
 Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
@@ -294,25 +283,25 @@
 Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
 `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
 
 Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
 `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
 
 Response is a always a stream
-`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message:
+`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message to show their difference:
 
 ```
 ## get_chat()
-print(vault.get_chat(text, history)
+print(vault.get_chat(text, history))
 
 ## get_chat_stream()
 for word in vault.get_chat_stream(text, history):
         print(word)
 ```
-This will take each word yielded and print it as it comes in. However, that will not look good, so it's best to use the built in print function `print_stream`. 
+This will take each word yielded and print it as it comes in. However, it's best to use the built in print function `print_stream`. 
 ```
 vault.print_stream(vault.get_chat_stream(text, history))
 ```
 <br>
 
 Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
 This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
```

### Comparing `vector_vault-2.0.1/README.md` & `vector_vault-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
+Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud with under one second response times.
 
-By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
+The `vectorvault` package comes with extensive chat functionality, so that you don't have to think about the details and can make smooth chat applications with ease. Speaking of smooth chat experiences, `vectorvault` also comes with chat streaming built-in. Simply use the `get_chat_stream()` function that works just like the regular `get_chat()` but with streaming. 
 
-Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
+`langchain` is a popular package for building functionality with llms, but when it comes to referencing vector databases, the database retrieval and chat integration can be complicated and difficult. This is one of the reasons we built `vectorvault`. We've integrated all the chat options people like to use with `langchain`, but made them all easier and more straight forward to use. Now with Vector Vault, integrating vector database results into generative chat applications is not only easy, it's the default. You also have total control over every aspect with parameters. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you.
 
-The `vectorvault` package allows you to interact with your Cloud Vaults using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
+By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a Vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up at [VectorVault.io](https://vectorvault.io)
+
+The `vectorvault` package allows you to interact with your Vault Cloud using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
 
 <br>
 
 Basic Interactions:
 
 `add()` : Prepares data to be added to the Vault, with automatic text splitting and processing for long texts. 
 <br>
@@ -80,40 +82,27 @@
 
 vault.save()
 ```
 
 <br>
 <br>
 
-Now that you have saved some data to the vault, you can add more at anytime, and your vault will automatically handle the adding process. These three lines execute very fast.
-```
-vault.add(more_text_data)
-
-vault.get_vectors()
-
-vault.save()
-```
-
-<br>
-<br>
-
-`vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed.
-`vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
+Now that you have saved some data to the vault, you can add more at anytime. `vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed. `vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
 ```
-vault.add(insanely_large_text_data)
+vault.add(very_large_text)
 vault.get_vectors() 
 vault.save() 
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 <br>
 <br>
 
-# Call Your Vault:
+# Vault Call:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
 Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
@@ -275,25 +264,25 @@
 Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
 `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
 
 Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
 `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
 
 Response is a always a stream
-`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message:
+`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message to show their difference:
 
 ```
 ## get_chat()
-print(vault.get_chat(text, history)
+print(vault.get_chat(text, history))
 
 ## get_chat_stream()
 for word in vault.get_chat_stream(text, history):
         print(word)
 ```
-This will take each word yielded and print it as it comes in. However, that will not look good, so it's best to use the built in print function `print_stream`. 
+This will take each word yielded and print it as it comes in. However, it's best to use the built in print function `print_stream`. 
 ```
 vault.print_stream(vault.get_chat_stream(text, history))
 ```
 <br>
 
 Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
 This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
```

### Comparing `vector_vault-2.0.1/setup.py` & `vector_vault-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="2.0.1",
+    version="2.0.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-2.0.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.2/vector_vault.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 2.0.1
+Version: 2.0.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -15,21 +15,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
-Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
+Vector Vault is a vector database cloud service built to make generative ai chat quick and easy. It allows you to seamlessly vectorize data and access it from the cloud. It's scalable to both small projects and large applications with millions of users. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector search easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud with under one second response times.
 
-By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
+The `vectorvault` package comes with extensive chat functionality, so that you don't have to think about the details and can make smooth chat applications with ease. Speaking of smooth chat experiences, `vectorvault` also comes with chat streaming built-in. Simply use the `get_chat_stream()` function that works just like the regular `get_chat()` but with streaming. 
 
-Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
+`langchain` is a popular package for building functionality with llms, but when it comes to referencing vector databases, the database retrieval and chat integration can be complicated and difficult. This is one of the reasons we built `vectorvault`. We've integrated all the chat options people like to use with `langchain`, but made them all easier and more straight forward to use. Now with Vector Vault, integrating vector database results into generative chat applications is not only easy, it's the default. You also have total control over every aspect with parameters. If you have been looking for an easy and reliable way to use vector databases with ChatGPT, then Vector Vault is for you.
 
-The `vectorvault` package allows you to interact with your Cloud Vaults using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
+By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a Vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more. You will need an api key in order to access the Vault Cloud. If you don't already have one, you can sign up at [VectorVault.io](https://vectorvault.io)
+
+The `vectorvault` package allows you to interact with your Vault Cloud using its Python-based API. Each vault is a seperate vector database. `vectorvault` includes operations such as creating a vault, deleting a vault, preparing data to add, getting vector embeddings for prepared data using OpenAI's text-embedding-ada-002, saving the data and embeddings to the cloud, referencing cloud vault data via vector search and retrieval, interacting with OpenAI's ChatGPT model to get responses, managing conversation history, and retrieving contextualized responses with reference vault data as context.
 
 <br>
 
 Basic Interactions:
 
 `add()` : Prepares data to be added to the Vault, with automatic text splitting and processing for long texts. 
 <br>
@@ -99,40 +101,27 @@
 
 vault.save()
 ```
 
 <br>
 <br>
 
-Now that you have saved some data to the vault, you can add more at anytime, and your vault will automatically handle the adding process. These three lines execute very fast.
-```
-vault.add(more_text_data)
-
-vault.get_vectors()
-
-vault.save()
-```
-
-<br>
-<br>
-
-`vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed.
-`vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
+Now that you have saved some data to the vault, you can add more at anytime. `vault.add()` is very versitile. You can add any length of text, even a full book...and it will be all automatically split and processed. `vault.get_vectors()` is also extremely flexible, because you can `vault.add()` as much as you want, then when you're done, process all the vectors at once with a `vault.get_vectors()` call - Which internally batches vector embeddings with OpenAI's text-embeddings-ada-002, and comes with auto rate-limiting and concurrent requests for maximum processing speed. 
 ```
-vault.add(insanely_large_text_data)
+vault.add(very_large_text)
 vault.get_vectors() 
 vault.save() 
 ```
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 <br>
 <br>
 
-# Call Your Vault:
+# Vault Call:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
 You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
 Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
@@ -294,25 +283,25 @@
 Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
 `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
 
 Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
 `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
 
 Response is a always a stream
-`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message:
+`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message to show their difference:
 
 ```
 ## get_chat()
-print(vault.get_chat(text, history)
+print(vault.get_chat(text, history))
 
 ## get_chat_stream()
 for word in vault.get_chat_stream(text, history):
         print(word)
 ```
-This will take each word yielded and print it as it comes in. However, that will not look good, so it's best to use the built in print function `print_stream`. 
+This will take each word yielded and print it as it comes in. However, it's best to use the built in print function `print_stream`. 
 ```
 vault.print_stream(vault.get_chat_stream(text, history))
 ```
 <br>
 
 Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
 This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
```

### Comparing `vector_vault-2.0.1/vectorvault/__init__.py` & `vector_vault-2.0.2/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.1/vectorvault/ai.py` & `vector_vault-2.0.2/vectorvault/ai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-# VECTOR VAULT CONFIDENTIAL
-# __________________
-# 
-#  All Rights Reserved.
-# 
-# NOTICE:  All information contained herein is, and remains
-# the property of Vector Vault and its suppliers,
-# if any.  The intellectual and technical concepts contained
-# herein are proprietary to Vector Vault
-# and its suppliers and may be covered by U.S. and Foreign Patents,
-# patents in process, and are protected by trade secret or copyright law.
-# Dissemination of this information or reproduction of this material
-# is strictly forbidden unless prior written permission is obtained
-# from Vector Vault.
-
 import openai
 import tiktoken
 
 class AI:
     def __init__(self) -> None:
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
-    def llm(self, user_input, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
+    def llm(self, user_input: str = None, history: str = None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
+        '''
+            If you pass in a custom_prompt with content already fully filled in, and no user_input, it will process your custom_prompt only without changing       
+        '''
         prompt_template = custom_prompt if custom_prompt else """{content}""" 
-        intokes = self.get_tokens(user_input)
-        histokes = self.get_tokens(history) if history else 0
-        if intokes + histokes > max_tokens:
-            tokes_left = max_tokens - intokes - histokes
-            if tokes_left < 0: # way too much input
-                char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
-                user_input = user_input[char_to_remove:] # get in front of it, chop at max
+        if user_input:
+            intokes = self.get_tokens(user_input)
+            histokes = self.get_tokens(history) if history else 0
+            if intokes + histokes > max_tokens:
+                tokes_left = max_tokens - intokes - histokes
+                if tokes_left < 0: # way too much input
+                    char_to_remove = (tokes_left * -1) * 5 # make positive and remove that amount
+                    user_input = user_input[char_to_remove:] # get in front of it, chop at max
+                if history:
+                    intokes = self.get_tokens(user_input)
+                    tokes_left = max_tokens - intokes
+                    chars_left = int(tokes_left * 4)
+                    history = history[-chars_left:]
+                else: # no history. If it was overlimit, then it was taken care of above
+                    pass
             if history:
-                intokes = self.get_tokens(user_input)
-                tokes_left = max_tokens - intokes
-                chars_left = int(tokes_left * 4)
-                history = history[-chars_left:]
-            else: # no history. If it was overlimit, then it was taken care of above
-                pass
-        if history:
-            prompt = prompt_template.format(content=user_input)
-            response = openai.ChatCompletion.create(
-                model=model,
-                messages=[
-                    {"role": "system", "content": f"Chat history: {history}"},
-                    {"role": "user", "content": f"{prompt}"}]
-            )
-            return response['choices'][0]['message']['content']
-        else:
-            # 'model' is the name of the model to use
-            # 'messages' is a list of message objects that mimics a conversation.
-            # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
-            prompt = prompt_template.format(content=user_input)
-            response = openai.ChatCompletion.create(
-                model=model,
-                messages=[{"role": "user", "content": f"{prompt}"}]
-            )
-            return response['choices'][0]['message']['content']
-                        
+                prompt = prompt_template.format(content=user_input)
+                response = openai.ChatCompletion.create(
+                    model=model,
+                    messages=[
+                        {"role": "system", "content": f"Chat history: {history}"},
+                        {"role": "user", "content": f"{prompt}"}]
+                )
+                return response['choices'][0]['message']['content']
+            else:
+                # 'model' is the name of the model to use
+                # 'messages' is a list of message objects that mimics a conversation.
+                # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
+                prompt = prompt_template.format(content=user_input)
+                response = openai.ChatCompletion.create(
+                    model=model,
+                    messages=[{"role": "user", "content": f"{prompt}"}]
+                )
+                return response['choices'][0]['message']['content']
+        else: # make no changes, and return response to passed in custom_prompt
+            if custom_prompt:
+                response = openai.ChatCompletion.create(
+                    model=model,
+                    messages=[{"role": "user", "content": f"{custom_prompt}"}]
+                )
+                return response['choices'][0]['message']['content']
+            else:
+                raise 'Error: Need custom_prompt if no user_input'
+            
                     
-    # This function returns a ChatGPT completion based contextual input
     def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         prompt_template = custom_prompt if custom_prompt else """
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
@@ -112,15 +109,15 @@
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
         )
         return response['choices'][0]['message']['content']
 
-    # This function returns a ChatGPT completion based on a provided input.
+
     def llm_stream(self, user_input, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         prompt_template = custom_prompt if custom_prompt else """{content}""" 
         intokes = self.get_tokens(user_input)
         histokes = self.get_tokens(history) if history else 0
         if intokes + histokes > max_tokens:
             tokes_left = max_tokens - intokes - histokes
             if tokes_left < 0: # way too much input
@@ -145,34 +142,29 @@
                 choices = message.get('choices', [])
                 if choices:
                     delta = choices[0].get('delta', {})
                     if 'content' in delta:
                         content = delta['content']
                         yield content
         else:
-            # 'model' is the name of the model to use
-            # 'messages' is a list of message objects that mimics a conversation.
-            # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
             prompt = prompt_template.format(content=user_input)
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[{"role": "user", "content": f"{prompt}"}],
                 stream=True
             )
-        # The API responds with a 'choices' array containing the 'message' object.
             for message in response:
                 choices = message.get('choices', [])
                 if choices:
                     delta = choices[0].get('delta', {})
                     if 'content' in delta:
                         content = delta['content']
                         yield content
                         
                     
-    # This function returns a ChatGPT completion based contextual input
     def llm_w_context_stream(self, user_input, context, history=None, model='gpt-3.5-turbo', max_tokens=4000, custom_prompt=False):
         prompt_template = custom_prompt if custom_prompt else """
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Chat History (if any): {history}
 
@@ -212,24 +204,22 @@
                 if double_check > max_tokens:
                     overby = double_check - max_tokens
                     char_to_take_away = overby * 5
                     context_length = len(context)
                     remove_from_context = int(context_length - char_to_take_away)
                     context = context[-remove_from_context:] 
 
-        # Format the prompt
         prompt = prompt_template.format(context=context, history=history, question=user_input)
         user_input = history + user_input
         response = openai.ChatCompletion.create(
             model=model,
             messages=[
                 {"role": "user", "content": f"{prompt}"}],
             stream=True
         )
-    # The API responds with a 'choices' array containing the 'message' object.
         for message in response:
             choices = message.get('choices', [])
             if choices:
                 delta = choices[0].get('delta', {})
                 if 'content' in delta:
                     content = delta['content']
                     yield content
@@ -238,44 +228,42 @@
     def summarize(self, user_input, model='gpt-3.5-turbo', custom_prompt=False):   
         prompt_template = custom_prompt if custom_prompt else """Summarize the following: {content}"""
         prompt = prompt_template.format(content=user_input)
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"{prompt}"}]
         )
-        # The API responds with a 'choices' array containing the 'message' object.
         return response['choices'][0]['message']['content']
 
     def summarize_stream(self, user_input, model='gpt-3.5-turbo', custom_prompt=False):   
         prompt_template = custom_prompt if custom_prompt else """Summarize the following: {content}"""
         prompt = prompt_template.format(content=user_input)
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"{prompt}"}],
             stream = True
         )
-        # The API responds with a 'choices' array containing the 'message' object.
         for message in response:
                 choices = message.get('choices', [])
                 if choices:
                     delta = choices[0].get('delta', {})
                     if 'content' in delta:
                         content = delta['content']
                         yield content
+    
+    def smart_summary(self, text, previous_summary, model='gpt-3.5-turbo', custom_prompt=False):   
+        prompt_template = custom_prompt if custom_prompt else """Given the previous summary: {previous_summary} 
+        Continue from where it leaves off by summarizing the next segment content: {content}"""
+        prompt = prompt_template.format(previous_summary=previous_summary, content=text)
+        response = openai.ChatCompletion.create(
+            model=model,
+            messages=[{"role": "user", "content": f"{prompt}"}]
+        )
+        return response['choices'][0]['message']['content']
+        
 
     def get_tokens(self, string: str, encoding_name: str = "cl100k_base") -> int:
         """Returns the number of tokens in a text string."""
         encoding = tiktoken.get_encoding(encoding_name)
         num_tokens = len(encoding.encode(string))
         return num_tokens
-
-
-# Notes: OpenAI's CEO, Sam Altman, recently testified in congress to compel the government to regulate the creation of cutting edge ai 
-# by forcing anyone seeking to do so to acquire a license first, or pay heavy pentalties. This anti-competitive attack on the 
-# open-source community, and development community at large is not cool.
-# If the claimed ai threats made public Altman hold true, then having the most capable models in the hands of only a few small companies 
-# is the real existential crisis we need to watch out for. Diversity is our only true security, and that comes from an open community.
-# While "Open"AI has gone against it's original mission (to stay open and transparent with data and models) they are however, the
-# most used ai right now. They have a great platform that can support massive load at high quality and no one else in the world has that.
-# Our goals are to support the community at large, therefore we integrate with them exclusively for now.
-# In the future, we will add open models, and competitors, as they become well-adopted, and with the exception that they
-# support the open development community at large.
+
```

### Comparing `vector_vault-2.0.1/vectorvault/cloudmanager.py` & `vector_vault-2.0.2/vectorvault/cloudmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # the property of Vector Vault and its suppliers,
 # if any.  The intellectual and technical concepts contained
 # herein are proprietary to Vector Vault
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
-# from Vector Vault.
+# from Vector Vault. See license for consent.
 
 import tempfile
 import os
 import json
 from .creds import CustomCredentials
 from .vecreq import call_proj
 from .itemize import cloud_name
```

### Comparing `vector_vault-2.0.1/vectorvault/creds.py` & `vector_vault-2.0.2/vectorvault/creds.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # the property of Vector Vault and its suppliers,
 # if any.  The intellectual and technical concepts contained
 # herein are proprietary to Vector Vault
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
-# from Vector Vault.
+# from Vector Vault. See license for consent.
 
 from google.auth.credentials import Credentials
 import requests
 import datetime
 
 class CustomCredentials(Credentials):
     def __init__(self, user, api):
```

### Comparing `vector_vault-2.0.1/vectorvault/itemize.py` & `vector_vault-2.0.2/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.1/vectorvault/signup.py` & `vector_vault-2.0.2/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-2.0.1/vectorvault/vault.py` & `vector_vault-2.0.2/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # the property of Vector Vault and its suppliers,
 # if any.  The intellectual and technical concepts contained
 # herein are proprietary to Vector Vault
 # and its suppliers and may be covered by U.S. and Foreign Patents,
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
-# from Vector Vault.
+# from Vector Vault. See license for consent.
 
 import numpy as np
 import tempfile
 import os
 import time
 import re
 import openai
@@ -227,15 +227,15 @@
             If your text length lenght is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
 
         if len(text) > 15000 or split == True:
             if self.verbose == True:
                 print('Using the built-in "split_text()" function to get a list of texts') 
-            texts = self.split_text(text, split_size) # returns list of text segments
+            texts = self.split_text(text, min_threshold=split_size) # returns list of text segments
         else:
             texts = [text]
         for text in texts:
             self.add_item(text, meta, name)
 
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
```

### Comparing `vector_vault-2.0.1/vectorvault/vecreq.py` & `vector_vault-2.0.2/vectorvault/vecreq.py`

 * *Files identical despite different names*

