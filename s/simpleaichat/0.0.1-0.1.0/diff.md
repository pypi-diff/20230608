# Comparing `tmp/simpleaichat-0.0.1.tar.gz` & `tmp/simpleaichat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaichat-0.0.1.tar", last modified: Wed Jun  7 01:34:03 2023, max compression
+gzip compressed data, was "simpleaichat-0.1.0.tar", last modified: Thu Jun  8 04:36:40 2023, max compression
```

## Comparing `simpleaichat-0.0.1.tar` & `simpleaichat-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-07 01:34:03.116209 simpleaichat-0.0.1/
--rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.0.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    14236 2023-06-07 01:34:03.115970 simpleaichat-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)    13799 2023-06-07 01:09:20.000000 simpleaichat-0.0.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-06-07 01:34:03.116295 simpleaichat-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      938 2023-06-05 04:57:13.000000 simpleaichat-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-07 01:34:03.114333 simpleaichat-0.0.1/simpleaichat/
--rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.0.1/simpleaichat/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    11166 2023-06-05 04:45:17.000000 simpleaichat-0.0.1/simpleaichat/chatgpt.py
--rw-r--r--   0 root         (0) staff       (20)      503 2023-06-05 04:45:20.000000 simpleaichat-0.0.1/simpleaichat/cli.py
--rw-r--r--   0 root         (0) staff       (20)     3052 2023-06-03 05:30:50.000000 simpleaichat-0.0.1/simpleaichat/models.py
--rw-r--r--   0 root         (0) staff       (20)    12134 2023-06-07 01:24:40.000000 simpleaichat-0.0.1/simpleaichat/simpleaichat.py
--rw-r--r--   0 root         (0) staff       (20)     2364 2023-06-03 03:44:43.000000 simpleaichat-0.0.1/simpleaichat/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-07 01:34:03.115625 simpleaichat-0.0.1/simpleaichat.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    14236 2023-06-07 01:34:02.000000 simpleaichat-0.0.1/simpleaichat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      387 2023-06-07 01:34:02.000000 simpleaichat-0.0.1/simpleaichat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-06-07 01:34:02.000000 simpleaichat-0.0.1/simpleaichat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       67 2023-06-07 01:34:02.000000 simpleaichat-0.0.1/simpleaichat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       89 2023-06-07 01:34:02.000000 simpleaichat-0.0.1/simpleaichat.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       13 2023-06-07 01:34:02.000000 simpleaichat-0.0.1/simpleaichat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-08 04:36:40.310901 simpleaichat-0.1.0/
+-rw-r--r--   0 root         (0) staff       (20)     1066 2023-02-18 01:00:20.000000 simpleaichat-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    15879 2023-06-08 04:36:40.310665 simpleaichat-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)    15442 2023-06-08 04:07:08.000000 simpleaichat-0.1.0/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-06-08 04:36:40.310978 simpleaichat-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      938 2023-06-08 04:35:58.000000 simpleaichat-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-08 04:36:40.308759 simpleaichat-0.1.0/simpleaichat/
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-06-05 04:46:22.000000 simpleaichat-0.1.0/simpleaichat/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    11175 2023-06-08 02:34:09.000000 simpleaichat-0.1.0/simpleaichat/chatgpt.py
+-rw-r--r--   0 root         (0) staff       (20)      549 2023-06-08 03:28:41.000000 simpleaichat-0.1.0/simpleaichat/cli.py
+-rw-r--r--   0 root         (0) staff       (20)     3052 2023-06-03 05:30:50.000000 simpleaichat-0.1.0/simpleaichat/models.py
+-rw-r--r--   0 root         (0) staff       (20)    12175 2023-06-08 01:27:02.000000 simpleaichat-0.1.0/simpleaichat/simpleaichat.py
+-rw-r--r--   0 root         (0) staff       (20)     2364 2023-06-03 03:44:43.000000 simpleaichat-0.1.0/simpleaichat/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-08 04:36:40.310307 simpleaichat-0.1.0/simpleaichat.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    15879 2023-06-08 04:36:39.000000 simpleaichat-0.1.0/simpleaichat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      387 2023-06-08 04:36:40.000000 simpleaichat-0.1.0/simpleaichat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-08 04:36:39.000000 simpleaichat-0.1.0/simpleaichat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       67 2023-06-08 04:36:39.000000 simpleaichat-0.1.0/simpleaichat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       89 2023-06-08 04:36:40.000000 simpleaichat-0.1.0/simpleaichat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       13 2023-06-08 04:36:40.000000 simpleaichat-0.1.0/simpleaichat.egg-info/top_level.txt
```

### Comparing `simpleaichat-0.0.1/LICENSE` & `simpleaichat-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.0.1/PKG-INFO` & `simpleaichat-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleaichat
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
 Home-page: https://github.com/minimaxir/simpleaichat
 Author: Max Woolf
 Author-email: max@minimaxir.com
 License: MIT
 Keywords: chatgpt,openai,text generation,ai
 Platform: UNKNOWN
@@ -30,17 +30,17 @@
 - Chat streaming responses and the ability to use tools.
 - Async support, including for streaming and tools.
 - Ablity to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
-- Creating a coding assistant without any unnecessary accompanying output
-- Allowing simpleaichat to make selections for inline ChatGPT usage guidelines.
-- Async interface for conducting many chats in the time it takes to receive one AI message.
+- Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
+- Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
+- Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
 
 ## Installation
 
 simpleaichat can be installed [from PyPI](https://pypi.org/project/simpleaichat/):
 
 ```sh
 pip3 install simpleaichat
@@ -52,15 +52,15 @@
 
 ```py3
 from simpleaichat import AIChat
 
 AIChat(api_key="sk-...")
 ```
 
-And with that, you'll be thrust directly into a chat!
+And with that, you'll be thrust directly into an interactive chat!
 
 ![](docs/helloworld.png)
 
 This AI chat will mimic the behavior of OpenAI's webapp, but on your local computer!
 
 You can also pass the API key by storing it in an `.env` file with a `OPEN_AI_KEY` field in the working directory (recommended), or by setting the environment variable of `OPEN_AI_KEY` directly to the API key.
 
@@ -97,15 +97,15 @@
 ## Building AI-based Apps
 
 The trick with working with new chat-based apps that wasn't readily available with earlier iterations of GPT-3 is the addition of the system prompt: a different class of prompt that guides the AI behavior throughout the entire conversation. In fact, the chat demos above are actually using [system prompt tricks](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#interactive-chat) behind the scenes! OpenAI has also released an official guide for [system prompt best practices](https://platform.openai.com/docs/guides/gpt-best-practices) to building AI apps.
 
 For developers, you can instantiate a programmatic instance of `AIChat` by explicitly specifying a system prompt, or by disabling the console.
 
 ```py3
-ai = AIChat(system="You are a helpful assistant")
+ai = AIChat(system="You are a helpful assistant.")
 ai = AIChat(console=False)  # same as above
 ```
 
 You can then feed the new `ai` class with user input, and it will return and save the response from ChatGPT:
 
 ```py3
 response = ai("What is the capital of California?")
@@ -197,75 +197,77 @@
 {"titre": "Un tableau d'entiers.", "tableau": [-1, 0, 1]}
 ```
 
 ### Tools
 
 One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As defined from the ReAct paper, tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
 
-Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing.
+Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and tools you specify can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing. Each generation returns a dictionary with the `response` and the `tool` function used, which can be used to set up workflows akin to [LangChain](https://github.com/hwchase17/langchain)-style Agents, e.g. recursively feed input to the model until it determines it does not need to use any more tools.
 
 You will need to specify functions with docstrings which provide hints for the AI to select them:
 
 ```py3
-from simpleaichat.utils import wikipedia_search, wikipedia_lookup
+from simpleaichat.utils import wikipedia_search, wikipedia_search_lookup
 
+# This uses the Wikipedia Search API.
+# Results from it are nondeterministic, your mileage will vary.
 def search(query):
     """Search the internet."""
     wiki_matches = wikipedia_search(query, n=3)
-    return {"context": "\n---\n".join(wiki_matches), "titles": wiki_matches}
+    return {"context": ", ".join(wiki_matches), "titles": wiki_matches}
 
 def lookup(query):
     """Lookup more information about a topic."""
     page = wikipedia_search_lookup(query, sentences=3)
-    return {"context": page, "titles": query}
+    return page
 
 params = {"temperature": 0.0, "max_tokens": 100}
 ai = AIChat(params=params, console=False)
 
-ai("What is a good tourist attraction in California?", tools=[search, lookup])
+ai("San Francisco tourist attractions", tools=[search, lookup])
 ```
 
 ```txt
-{'context': 'Tourist attraction\n---\nBuena Park, California\n---\nLombard Street (San Francisco)',
- 'titles': ['Tourist attraction',
-  'Buena Park, California',
+{'context': "Fisherman's Wharf, San Francisco, Tourist attractions in the United States, Lombard Street (San Francisco)",
+ 'titles': ["Fisherman's Wharf, San Francisco",
+  'Tourist attractions in the United States',
   'Lombard Street (San Francisco)'],
  'tool': 'search',
- 'response': "There are many great tourist attractions in California, but two popular ones are Buena Park, which is home to several theme parks such as Knott's Berry Farm and Disneyland, and Lombard Street in San Francisco, which is known for its steep, winding road and beautiful views of the city."}
+ 'response': "There are many popular tourist attractions in San Francisco, including Fisherman's Wharf and Lombard Street. Fisherman's Wharf is a bustling waterfront area known for its seafood restaurants, souvenir shops, and sea lion sightings. Lombard Street, on the other hand, is a famous winding street with eight hairpin turns that attract visitors from all over the world. Both of these attractions are must-sees for anyone visiting San Francisco."}
 ```
 
 ```py3
 ai("Lombard Street?", tools=[search, lookup])
 ```
 
 ```
 {'context': 'Lombard Street is an east–west street in San Francisco, California that is famous for a steep, one-block section with eight hairpin turns. Stretching from The Presidio east to The Embarcadero (with a gap on Telegraph Hill), most of the street\'s western segment is a major thoroughfare designated as part of U.S. Route 101. The famous one-block section, claimed to be "the crookedest street in the world", is located along the eastern segment in the Russian Hill neighborhood.',
- 'titles': 'Lombard Street?',
  'tool': 'lookup',
- 'response': 'Yes, Lombard Street is a famous tourist attraction in San Francisco, California. It is known for its steep, one-block section with eight hairpin turns, which is claimed to be "the crookedest street in the world". The street is located in the Russian Hill neighborhood and is a popular spot for tourists to take photos and enjoy the beautiful views of the city.'}
+ 'response': 'Lombard Street is a famous street in San Francisco, California known for its steep, one-block section with eight hairpin turns. It stretches from The Presidio to The Embarcadero, with a gap on Telegraph Hill. The western segment of the street is a major thoroughfare designated as part of U.S. Route 101, while the famous one-block section, claimed to be "the crookedest street in the world", is located along the eastern segment in the Russian Hill'}
 ```
 
 ```py3
 ai("Thanks for your help!", tools=[search, lookup])
 ```
 
 ```txt
-{'response': "You're welcome! If you have any more questions, feel free to ask.",
+{'response': "You're welcome! If you have any more questions or need further assistance, feel free to ask.",
  'tool': None}
 ```
 
 ## Miscellaneous Notes
 
-- Like [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) before it, the primary motivation behind releasing simpleaichat is to both democratize access to ChatGPT even more without extolling complexity as a virtue, and also offer more transparency for non-engineers into how Chat AI-based apps work under the hood given the disproportionate amount of media misinformation about their capabilities. This is inspired by real-world experience from [my work with BuzzFeed](https://tech.buzzfeed.com/the-right-tools-for-the-job-c05de96e949e) in the domain, where after spending a long time working with the popular LangChain, a more-simple implementation was both much easier to maintain and resulted in much better generations. I began focusing development on simpleaichat after reading a [Hacker News thread](https://news.ycombinator.com/item?id=35820931) filled with many similar complaints, indicating value for an easier-to-use interface for modern AI tricks.
+- Like [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) before it, the primary motivation behind releasing simpleaichat is to both democratize access to ChatGPT even more and also offer more transparency for non-engineers into how Chat AI-based apps work under the hood given the disproportionate amount of media misinformation about their capabilities. This is inspired by real-world experience from [my work with BuzzFeed](https://tech.buzzfeed.com/the-right-tools-for-the-job-c05de96e949e) in the domain, where after spending a long time working with the popular [LangChain](https://github.com/hwchase17/langchain), a more-simple implementation was both much easier to maintain and resulted in much better generations. I began focusing development on simpleaichat after reading a [Hacker News thread](https://news.ycombinator.com/item?id=35820931) filled with many similar complaints, indicating value for an easier-to-use interface for modern AI tricks.
   - simpleaichat very intentionally avoids coupling features with common use cases where possible (e.g. Tools) in order to avoid software lock-in due to the difficulty implementing anything not explicitly mentioned in the project's documentation. The philosophy behind simpleaichat is to provide good demos, and let the user's creativity and business needs take priority instead of having to fit a round peg into a square hole like with LangChain.
-  - simpleaichat makes it easier to interface with Chat AIs, but it does not attempt to solve common technical and ethical problems inherent to large language models trained on the internet, including prompt injection and unintended plagiarism. The user should exercise good judgment when implementing simpleaichat. Use cases of simpleaichat which go against OpenAI's usage policy (including jailbreaking) will not be endorsed.
-  - simpleaichat does not use the "Agent" logical metaphor for its actions. If needed be, you can emulate the Agent workflow with a `while` loop without much additional code, plus with the additional benefit of much more flexibility such as debugging.
+  - simpleaichat makes it easier to interface with Chat AIs, but it does not attempt to solve common technical and ethical problems inherent to large language models trained on the internet, including prompt injection and unintended plagiarism. The user should exercise good judgment when implementing simpleaichat. Use cases of simpleaichat which go against OpenAI's [usage policies](https://openai.com/policies/usage-policies) (including jailbreaking) will not be endorsed.
+  - simpleaichat intentionally does not use the "Agent" logical metaphor for tool workflows because it's become an AI hype buzzword heavily divorced from its origins. If needed be, you can emulate the Agent workflow with a `while` loop without much additional code, plus with the additional benefit of much more flexibility such as debugging.
 - The session manager implements some sensible security defaults, such as using UUIDs as session ids by default, storing authentication information in a way to minimize unintentional leakage, and type enforcement via Pydantic. Your end-user application should still be aware of potential security issues, however.
 - Although OpenAI's documentation says that system prompts are less effective than a user prompt constructed in a similar manner, in my experience it still does perform better for maintaining rules/a persona.
 - Many examples of popular prompts use more conversational prompts, while the example prompts here use more consise and imperative prompts. This aspect of prompt engineering is still evolving, but in my experience commands do better with ChatGPT and with greater token efficieny. That's also why simpleaichat allows users to specify system prompts (and explicitly highlights what the default use) instead of relying on historical best practices.
+- Token counts for async is not supported as OpenAI doesn't return token counts when streaming responses. In general, there may be some desync in token counts and usage for various use cases; I'm working on categorizing them.
 - Outside of the explicit examples, none of this README uses AI-generated text. The introduction code example is just a joke, but it was too good of a real-world use case!
 
 ## Roadmap
 
 - PaLM Chat (Bard) and Anthropic Claude support
 - More fun/feature-filled CLI chat app based on Textual
 - Simple example of using simpleaichat in a webapp
```

### Comparing `simpleaichat-0.0.1/README.md` & `simpleaichat-0.1.0/simpleaichat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: simpleaichat
+Version: 0.1.0
+Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
+Home-page: https://github.com/minimaxir/simpleaichat
+Author: Max Woolf
+Author-email: max@minimaxir.com
+License: MIT
+Keywords: chatgpt,openai,text generation,ai
+Platform: UNKNOWN
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # simpleaichat
 
 ```py3
 from simpleaichat import AIChat
 
 ai = AIChat(system="Write a fancy GitHub README based on the user-provided project name.")
 ai("simpleaichat")
@@ -16,17 +30,17 @@
 - Chat streaming responses and the ability to use tools.
 - Async support, including for streaming and tools.
 - Ablity to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
-- Creating a coding assistant without any unnecessary accompanying output
-- Allowing simpleaichat to make selections for inline ChatGPT usage guidelines.
-- Async interface for conducting many chats in the time it takes to receive one AI message.
+- Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
+- Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
+- Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
 
 ## Installation
 
 simpleaichat can be installed [from PyPI](https://pypi.org/project/simpleaichat/):
 
 ```sh
 pip3 install simpleaichat
@@ -38,15 +52,15 @@
 
 ```py3
 from simpleaichat import AIChat
 
 AIChat(api_key="sk-...")
 ```
 
-And with that, you'll be thrust directly into a chat!
+And with that, you'll be thrust directly into an interactive chat!
 
 ![](docs/helloworld.png)
 
 This AI chat will mimic the behavior of OpenAI's webapp, but on your local computer!
 
 You can also pass the API key by storing it in an `.env` file with a `OPEN_AI_KEY` field in the working directory (recommended), or by setting the environment variable of `OPEN_AI_KEY` directly to the API key.
 
@@ -83,15 +97,15 @@
 ## Building AI-based Apps
 
 The trick with working with new chat-based apps that wasn't readily available with earlier iterations of GPT-3 is the addition of the system prompt: a different class of prompt that guides the AI behavior throughout the entire conversation. In fact, the chat demos above are actually using [system prompt tricks](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#interactive-chat) behind the scenes! OpenAI has also released an official guide for [system prompt best practices](https://platform.openai.com/docs/guides/gpt-best-practices) to building AI apps.
 
 For developers, you can instantiate a programmatic instance of `AIChat` by explicitly specifying a system prompt, or by disabling the console.
 
 ```py3
-ai = AIChat(system="You are a helpful assistant")
+ai = AIChat(system="You are a helpful assistant.")
 ai = AIChat(console=False)  # same as above
 ```
 
 You can then feed the new `ai` class with user input, and it will return and save the response from ChatGPT:
 
 ```py3
 response = ai("What is the capital of California?")
@@ -183,75 +197,77 @@
 {"titre": "Un tableau d'entiers.", "tableau": [-1, 0, 1]}
 ```
 
 ### Tools
 
 One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As defined from the ReAct paper, tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
 
-Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing.
+Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and tools you specify can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing. Each generation returns a dictionary with the `response` and the `tool` function used, which can be used to set up workflows akin to [LangChain](https://github.com/hwchase17/langchain)-style Agents, e.g. recursively feed input to the model until it determines it does not need to use any more tools.
 
 You will need to specify functions with docstrings which provide hints for the AI to select them:
 
 ```py3
-from simpleaichat.utils import wikipedia_search, wikipedia_lookup
+from simpleaichat.utils import wikipedia_search, wikipedia_search_lookup
 
+# This uses the Wikipedia Search API.
+# Results from it are nondeterministic, your mileage will vary.
 def search(query):
     """Search the internet."""
     wiki_matches = wikipedia_search(query, n=3)
-    return {"context": "\n---\n".join(wiki_matches), "titles": wiki_matches}
+    return {"context": ", ".join(wiki_matches), "titles": wiki_matches}
 
 def lookup(query):
     """Lookup more information about a topic."""
     page = wikipedia_search_lookup(query, sentences=3)
-    return {"context": page, "titles": query}
+    return page
 
 params = {"temperature": 0.0, "max_tokens": 100}
 ai = AIChat(params=params, console=False)
 
-ai("What is a good tourist attraction in California?", tools=[search, lookup])
+ai("San Francisco tourist attractions", tools=[search, lookup])
 ```
 
 ```txt
-{'context': 'Tourist attraction\n---\nBuena Park, California\n---\nLombard Street (San Francisco)',
- 'titles': ['Tourist attraction',
-  'Buena Park, California',
+{'context': "Fisherman's Wharf, San Francisco, Tourist attractions in the United States, Lombard Street (San Francisco)",
+ 'titles': ["Fisherman's Wharf, San Francisco",
+  'Tourist attractions in the United States',
   'Lombard Street (San Francisco)'],
  'tool': 'search',
- 'response': "There are many great tourist attractions in California, but two popular ones are Buena Park, which is home to several theme parks such as Knott's Berry Farm and Disneyland, and Lombard Street in San Francisco, which is known for its steep, winding road and beautiful views of the city."}
+ 'response': "There are many popular tourist attractions in San Francisco, including Fisherman's Wharf and Lombard Street. Fisherman's Wharf is a bustling waterfront area known for its seafood restaurants, souvenir shops, and sea lion sightings. Lombard Street, on the other hand, is a famous winding street with eight hairpin turns that attract visitors from all over the world. Both of these attractions are must-sees for anyone visiting San Francisco."}
 ```
 
 ```py3
 ai("Lombard Street?", tools=[search, lookup])
 ```
 
 ```
 {'context': 'Lombard Street is an east–west street in San Francisco, California that is famous for a steep, one-block section with eight hairpin turns. Stretching from The Presidio east to The Embarcadero (with a gap on Telegraph Hill), most of the street\'s western segment is a major thoroughfare designated as part of U.S. Route 101. The famous one-block section, claimed to be "the crookedest street in the world", is located along the eastern segment in the Russian Hill neighborhood.',
- 'titles': 'Lombard Street?',
  'tool': 'lookup',
- 'response': 'Yes, Lombard Street is a famous tourist attraction in San Francisco, California. It is known for its steep, one-block section with eight hairpin turns, which is claimed to be "the crookedest street in the world". The street is located in the Russian Hill neighborhood and is a popular spot for tourists to take photos and enjoy the beautiful views of the city.'}
+ 'response': 'Lombard Street is a famous street in San Francisco, California known for its steep, one-block section with eight hairpin turns. It stretches from The Presidio to The Embarcadero, with a gap on Telegraph Hill. The western segment of the street is a major thoroughfare designated as part of U.S. Route 101, while the famous one-block section, claimed to be "the crookedest street in the world", is located along the eastern segment in the Russian Hill'}
 ```
 
 ```py3
 ai("Thanks for your help!", tools=[search, lookup])
 ```
 
 ```txt
-{'response': "You're welcome! If you have any more questions, feel free to ask.",
+{'response': "You're welcome! If you have any more questions or need further assistance, feel free to ask.",
  'tool': None}
 ```
 
 ## Miscellaneous Notes
 
-- Like [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) before it, the primary motivation behind releasing simpleaichat is to both democratize access to ChatGPT even more without extolling complexity as a virtue, and also offer more transparency for non-engineers into how Chat AI-based apps work under the hood given the disproportionate amount of media misinformation about their capabilities. This is inspired by real-world experience from [my work with BuzzFeed](https://tech.buzzfeed.com/the-right-tools-for-the-job-c05de96e949e) in the domain, where after spending a long time working with the popular LangChain, a more-simple implementation was both much easier to maintain and resulted in much better generations. I began focusing development on simpleaichat after reading a [Hacker News thread](https://news.ycombinator.com/item?id=35820931) filled with many similar complaints, indicating value for an easier-to-use interface for modern AI tricks.
+- Like [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) before it, the primary motivation behind releasing simpleaichat is to both democratize access to ChatGPT even more and also offer more transparency for non-engineers into how Chat AI-based apps work under the hood given the disproportionate amount of media misinformation about their capabilities. This is inspired by real-world experience from [my work with BuzzFeed](https://tech.buzzfeed.com/the-right-tools-for-the-job-c05de96e949e) in the domain, where after spending a long time working with the popular [LangChain](https://github.com/hwchase17/langchain), a more-simple implementation was both much easier to maintain and resulted in much better generations. I began focusing development on simpleaichat after reading a [Hacker News thread](https://news.ycombinator.com/item?id=35820931) filled with many similar complaints, indicating value for an easier-to-use interface for modern AI tricks.
   - simpleaichat very intentionally avoids coupling features with common use cases where possible (e.g. Tools) in order to avoid software lock-in due to the difficulty implementing anything not explicitly mentioned in the project's documentation. The philosophy behind simpleaichat is to provide good demos, and let the user's creativity and business needs take priority instead of having to fit a round peg into a square hole like with LangChain.
-  - simpleaichat makes it easier to interface with Chat AIs, but it does not attempt to solve common technical and ethical problems inherent to large language models trained on the internet, including prompt injection and unintended plagiarism. The user should exercise good judgment when implementing simpleaichat. Use cases of simpleaichat which go against OpenAI's usage policy (including jailbreaking) will not be endorsed.
-  - simpleaichat does not use the "Agent" logical metaphor for its actions. If needed be, you can emulate the Agent workflow with a `while` loop without much additional code, plus with the additional benefit of much more flexibility such as debugging.
+  - simpleaichat makes it easier to interface with Chat AIs, but it does not attempt to solve common technical and ethical problems inherent to large language models trained on the internet, including prompt injection and unintended plagiarism. The user should exercise good judgment when implementing simpleaichat. Use cases of simpleaichat which go against OpenAI's [usage policies](https://openai.com/policies/usage-policies) (including jailbreaking) will not be endorsed.
+  - simpleaichat intentionally does not use the "Agent" logical metaphor for tool workflows because it's become an AI hype buzzword heavily divorced from its origins. If needed be, you can emulate the Agent workflow with a `while` loop without much additional code, plus with the additional benefit of much more flexibility such as debugging.
 - The session manager implements some sensible security defaults, such as using UUIDs as session ids by default, storing authentication information in a way to minimize unintentional leakage, and type enforcement via Pydantic. Your end-user application should still be aware of potential security issues, however.
 - Although OpenAI's documentation says that system prompts are less effective than a user prompt constructed in a similar manner, in my experience it still does perform better for maintaining rules/a persona.
 - Many examples of popular prompts use more conversational prompts, while the example prompts here use more consise and imperative prompts. This aspect of prompt engineering is still evolving, but in my experience commands do better with ChatGPT and with greater token efficieny. That's also why simpleaichat allows users to specify system prompts (and explicitly highlights what the default use) instead of relying on historical best practices.
+- Token counts for async is not supported as OpenAI doesn't return token counts when streaming responses. In general, there may be some desync in token counts and usage for various use cases; I'm working on categorizing them.
 - Outside of the explicit examples, none of this README uses AI-generated text. The introduction code example is just a joke, but it was too good of a real-world use case!
 
 ## Roadmap
 
 - PaLM Chat (Bard) and Anthropic Claude support
 - More fun/feature-filled CLI chat app based on Textual
 - Simple example of using simpleaichat in a webapp
@@ -262,7 +278,9 @@
 Max Woolf ([@minimaxir](https://minimaxir.com))
 
 _Max's open-source projects are supported by his [Patreon](https://www.patreon.com/minimaxir) and [GitHub Sponsors](https://github.com/sponsors/minimaxir). If you found this project helpful, any monetary contributions to the Patreon are appreciated and will be put to good creative use._
 
 ## License
 
 MIT
+
+
```

### Comparing `simpleaichat-0.0.1/setup.py` & `simpleaichat-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="simpleaichat",
     packages=["simpleaichat"],  # this must be the same as the name above
-    version="0.0.1",
+    version="0.1.0",
     description="A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Max Woolf",
     author_email="max@minimaxir.com",
     url="https://github.com/minimaxir/simpleaichat",
     keywords=["chatgpt", "openai", "text generation", "ai"],
```

### Comparing `simpleaichat-0.0.1/simpleaichat/chatgpt.py` & `simpleaichat-0.1.0/simpleaichat/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from httpx import Client, AsyncClient
 from typing import List, Dict, Union, Set, Any
 import orjson
 
 from .models import ChatMessage, ChatSession
 
 tool_prompt = """From the list of tools below:
-- Reply ONLY with the number of the tool appropriate in response to the user's message.
+- Reply ONLY with the number of the tool appropriate in response to the user's last message.
 - If no tool is appropriate, ONLY reply with \"0\".
 
 {tools}"""
 
 
 class ChatGPTSession(ChatSession):
     api_url: HttpUrl = "https://api.openai.com/v1/chat/completions"
@@ -131,15 +131,15 @@
         params: Dict[str, Any] = None,
     ) -> Dict[str, Any]:
 
         # call 1: select tool and populate context
         tools_list = "\n".join(f"{i+1}: {f.__doc__}" for i, f in enumerate(tools))
         tool_prompt_format = tool_prompt.format(tools=tools_list)
 
-        logit_bias_weight = 20
+        logit_bias_weight = 100
         logit_bias = {str(k): logit_bias_weight for k in range(15, 15 + len(tools) + 1)}
 
         tool_idx = int(
             self.gen(
                 prompt,
                 client=client,
                 system=tool_prompt_format,
@@ -147,14 +147,15 @@
                 params={
                     "temperature": 0.0,
                     "max_tokens": 1,
                     "logit_bias": logit_bias,
                 },
             )
         )
+
         # if no tool is selected, do a standard generation instead.
         if tool_idx == 0:
             return {
                 "response": self.gen(
                     prompt,
                     client=client,
                     system=system,
@@ -274,15 +275,15 @@
         params: Dict[str, Any] = None,
     ) -> Dict[str, Any]:
 
         # call 1: select tool and populate context
         tools_list = "\n".join(f"{i+1}: {f.__doc__}" for i, f in enumerate(tools))
         tool_prompt_format = tool_prompt.format(tools=tools_list)
 
-        logit_bias_weight = 20
+        logit_bias_weight = 100
         logit_bias = {str(k): logit_bias_weight for k in range(15, 15 + len(tools) + 1)}
 
         tool_idx = int(
             await self.gen_async(
                 prompt,
                 client=client,
                 system=tool_prompt_format,
@@ -290,14 +291,15 @@
                 params={
                     "temperature": 0.0,
                     "max_tokens": 1,
                     "logit_bias": logit_bias,
                 },
             )
         )
+
         # if no tool is selected, do a standard generation instead.
         if tool_idx == 0:
             return {
                 "response": await self.gen_async(
                     prompt,
                     client=client,
                     system=system,
```

### Comparing `simpleaichat-0.0.1/simpleaichat/models.py` & `simpleaichat-0.1.0/simpleaichat/models.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.0.1/simpleaichat/simpleaichat.py` & `simpleaichat-0.1.0/simpleaichat/simpleaichat.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,17 @@
 
     def reset_session(self, id: Union[str, UUID] = None) -> None:
         sess = self.get_session(id)
         sess.messages = []
 
     def delete_session(self, id: Union[str, UUID] = None) -> None:
         sess = self.get_session(id)
-        if sess.id == self.default_session.id:
-            self.default_session = None
+        if self.default_session:
+            if sess.id == self.default_session.id:
+                self.default_session = None
         del self.sessions[sess.id]
         del sess
 
     def __call__(
         self,
         prompt: str,
         id: Union[str, UUID] = None,
```

### Comparing `simpleaichat-0.0.1/simpleaichat/utils.py` & `simpleaichat-0.1.0/simpleaichat/utils.py`

 * *Files identical despite different names*

### Comparing `simpleaichat-0.0.1/simpleaichat.egg-info/PKG-INFO` & `simpleaichat-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: simpleaichat
-Version: 0.0.1
-Summary: A Python package for easily interfacing with chat apps, with robust features and minimal code complexity.
-Home-page: https://github.com/minimaxir/simpleaichat
-Author: Max Woolf
-Author-email: max@minimaxir.com
-License: MIT
-Keywords: chatgpt,openai,text generation,ai
-Platform: UNKNOWN
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # simpleaichat
 
 ```py3
 from simpleaichat import AIChat
 
 ai = AIChat(system="Write a fancy GitHub README based on the user-provided project name.")
 ai("simpleaichat")
@@ -30,17 +16,17 @@
 - Chat streaming responses and the ability to use tools.
 - Async support, including for streaming and tools.
 - Ablity to create more complex yet clear workflows if needed, such as Agents. (Demo soon!)
 - Coming soon: more chat model support (PaLM, Claude)!
 
 Here's some fun, hackable examples on how simpleaichat works:
 
-- Creating a coding assistant without any unnecessary accompanying output
-- Allowing simpleaichat to make selections for inline ChatGPT usage guidelines.
-- Async interface for conducting many chats in the time it takes to receive one AI message.
+- Creating a [Python coding assistant](examples/notebooks/simpleaichat_coding.ipynb) without any unnecessary accompanying output, allowing 5x faster generation at 1/3rd the cost. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_coding.ipynb))
+- Allowing simpleaichat to [provide inline tips](examples/notebooks/chatgpt_inline_tips.ipynb) following ChatGPT usage guidelines. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/chatgpt_inline_tips.ipynb))
+- Async interface for [conducting many chats](examples/notebooks/simpleaichat_async.ipynb) in the time it takes to receive one AI message. ([Colab](https://colab.research.google.com/github/minimaxir/simpleaichat/blob/main/examples/notebooks/simpleaichat_async.ipynb))
 
 ## Installation
 
 simpleaichat can be installed [from PyPI](https://pypi.org/project/simpleaichat/):
 
 ```sh
 pip3 install simpleaichat
@@ -52,15 +38,15 @@
 
 ```py3
 from simpleaichat import AIChat
 
 AIChat(api_key="sk-...")
 ```
 
-And with that, you'll be thrust directly into a chat!
+And with that, you'll be thrust directly into an interactive chat!
 
 ![](docs/helloworld.png)
 
 This AI chat will mimic the behavior of OpenAI's webapp, but on your local computer!
 
 You can also pass the API key by storing it in an `.env` file with a `OPEN_AI_KEY` field in the working directory (recommended), or by setting the environment variable of `OPEN_AI_KEY` directly to the API key.
 
@@ -97,15 +83,15 @@
 ## Building AI-based Apps
 
 The trick with working with new chat-based apps that wasn't readily available with earlier iterations of GPT-3 is the addition of the system prompt: a different class of prompt that guides the AI behavior throughout the entire conversation. In fact, the chat demos above are actually using [system prompt tricks](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#interactive-chat) behind the scenes! OpenAI has also released an official guide for [system prompt best practices](https://platform.openai.com/docs/guides/gpt-best-practices) to building AI apps.
 
 For developers, you can instantiate a programmatic instance of `AIChat` by explicitly specifying a system prompt, or by disabling the console.
 
 ```py3
-ai = AIChat(system="You are a helpful assistant")
+ai = AIChat(system="You are a helpful assistant.")
 ai = AIChat(console=False)  # same as above
 ```
 
 You can then feed the new `ai` class with user input, and it will return and save the response from ChatGPT:
 
 ```py3
 response = ai("What is the capital of California?")
@@ -197,75 +183,77 @@
 {"titre": "Un tableau d'entiers.", "tableau": [-1, 0, 1]}
 ```
 
 ### Tools
 
 One of the most recent aspects of interacting with ChatGPT is the ability for the model to use "tools." As defined from the ReAct paper, tools allow the model to decide when to use custom functions, which can extend beyond just the chat AI itself, for example retrieving recent information from the internet not present in the chat AI's training data. This workflow is analogous to ChatGPT Plugins.
 
-Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing.
+Parsing the model output to invoke tools typically requires a number of shennanigans, but simpleaichat uses [a neat trick](https://github.com/minimaxir/simpleaichat/blob/main/PROMPTS.md#tools) to make it fast and reliable! Additionally, the specified tools return a `context` for ChatGPT to draw from for its final response, and tools you specify can return a dictionary which you can also populate with arbitrary metadata for debugging and postprocessing. Each generation returns a dictionary with the `response` and the `tool` function used, which can be used to set up workflows akin to [LangChain](https://github.com/hwchase17/langchain)-style Agents, e.g. recursively feed input to the model until it determines it does not need to use any more tools.
 
 You will need to specify functions with docstrings which provide hints for the AI to select them:
 
 ```py3
-from simpleaichat.utils import wikipedia_search, wikipedia_lookup
+from simpleaichat.utils import wikipedia_search, wikipedia_search_lookup
 
+# This uses the Wikipedia Search API.
+# Results from it are nondeterministic, your mileage will vary.
 def search(query):
     """Search the internet."""
     wiki_matches = wikipedia_search(query, n=3)
-    return {"context": "\n---\n".join(wiki_matches), "titles": wiki_matches}
+    return {"context": ", ".join(wiki_matches), "titles": wiki_matches}
 
 def lookup(query):
     """Lookup more information about a topic."""
     page = wikipedia_search_lookup(query, sentences=3)
-    return {"context": page, "titles": query}
+    return page
 
 params = {"temperature": 0.0, "max_tokens": 100}
 ai = AIChat(params=params, console=False)
 
-ai("What is a good tourist attraction in California?", tools=[search, lookup])
+ai("San Francisco tourist attractions", tools=[search, lookup])
 ```
 
 ```txt
-{'context': 'Tourist attraction\n---\nBuena Park, California\n---\nLombard Street (San Francisco)',
- 'titles': ['Tourist attraction',
-  'Buena Park, California',
+{'context': "Fisherman's Wharf, San Francisco, Tourist attractions in the United States, Lombard Street (San Francisco)",
+ 'titles': ["Fisherman's Wharf, San Francisco",
+  'Tourist attractions in the United States',
   'Lombard Street (San Francisco)'],
  'tool': 'search',
- 'response': "There are many great tourist attractions in California, but two popular ones are Buena Park, which is home to several theme parks such as Knott's Berry Farm and Disneyland, and Lombard Street in San Francisco, which is known for its steep, winding road and beautiful views of the city."}
+ 'response': "There are many popular tourist attractions in San Francisco, including Fisherman's Wharf and Lombard Street. Fisherman's Wharf is a bustling waterfront area known for its seafood restaurants, souvenir shops, and sea lion sightings. Lombard Street, on the other hand, is a famous winding street with eight hairpin turns that attract visitors from all over the world. Both of these attractions are must-sees for anyone visiting San Francisco."}
 ```
 
 ```py3
 ai("Lombard Street?", tools=[search, lookup])
 ```
 
 ```
 {'context': 'Lombard Street is an east–west street in San Francisco, California that is famous for a steep, one-block section with eight hairpin turns. Stretching from The Presidio east to The Embarcadero (with a gap on Telegraph Hill), most of the street\'s western segment is a major thoroughfare designated as part of U.S. Route 101. The famous one-block section, claimed to be "the crookedest street in the world", is located along the eastern segment in the Russian Hill neighborhood.',
- 'titles': 'Lombard Street?',
  'tool': 'lookup',
- 'response': 'Yes, Lombard Street is a famous tourist attraction in San Francisco, California. It is known for its steep, one-block section with eight hairpin turns, which is claimed to be "the crookedest street in the world". The street is located in the Russian Hill neighborhood and is a popular spot for tourists to take photos and enjoy the beautiful views of the city.'}
+ 'response': 'Lombard Street is a famous street in San Francisco, California known for its steep, one-block section with eight hairpin turns. It stretches from The Presidio to The Embarcadero, with a gap on Telegraph Hill. The western segment of the street is a major thoroughfare designated as part of U.S. Route 101, while the famous one-block section, claimed to be "the crookedest street in the world", is located along the eastern segment in the Russian Hill'}
 ```
 
 ```py3
 ai("Thanks for your help!", tools=[search, lookup])
 ```
 
 ```txt
-{'response': "You're welcome! If you have any more questions, feel free to ask.",
+{'response': "You're welcome! If you have any more questions or need further assistance, feel free to ask.",
  'tool': None}
 ```
 
 ## Miscellaneous Notes
 
-- Like [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) before it, the primary motivation behind releasing simpleaichat is to both democratize access to ChatGPT even more without extolling complexity as a virtue, and also offer more transparency for non-engineers into how Chat AI-based apps work under the hood given the disproportionate amount of media misinformation about their capabilities. This is inspired by real-world experience from [my work with BuzzFeed](https://tech.buzzfeed.com/the-right-tools-for-the-job-c05de96e949e) in the domain, where after spending a long time working with the popular LangChain, a more-simple implementation was both much easier to maintain and resulted in much better generations. I began focusing development on simpleaichat after reading a [Hacker News thread](https://news.ycombinator.com/item?id=35820931) filled with many similar complaints, indicating value for an easier-to-use interface for modern AI tricks.
+- Like [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple) before it, the primary motivation behind releasing simpleaichat is to both democratize access to ChatGPT even more and also offer more transparency for non-engineers into how Chat AI-based apps work under the hood given the disproportionate amount of media misinformation about their capabilities. This is inspired by real-world experience from [my work with BuzzFeed](https://tech.buzzfeed.com/the-right-tools-for-the-job-c05de96e949e) in the domain, where after spending a long time working with the popular [LangChain](https://github.com/hwchase17/langchain), a more-simple implementation was both much easier to maintain and resulted in much better generations. I began focusing development on simpleaichat after reading a [Hacker News thread](https://news.ycombinator.com/item?id=35820931) filled with many similar complaints, indicating value for an easier-to-use interface for modern AI tricks.
   - simpleaichat very intentionally avoids coupling features with common use cases where possible (e.g. Tools) in order to avoid software lock-in due to the difficulty implementing anything not explicitly mentioned in the project's documentation. The philosophy behind simpleaichat is to provide good demos, and let the user's creativity and business needs take priority instead of having to fit a round peg into a square hole like with LangChain.
-  - simpleaichat makes it easier to interface with Chat AIs, but it does not attempt to solve common technical and ethical problems inherent to large language models trained on the internet, including prompt injection and unintended plagiarism. The user should exercise good judgment when implementing simpleaichat. Use cases of simpleaichat which go against OpenAI's usage policy (including jailbreaking) will not be endorsed.
-  - simpleaichat does not use the "Agent" logical metaphor for its actions. If needed be, you can emulate the Agent workflow with a `while` loop without much additional code, plus with the additional benefit of much more flexibility such as debugging.
+  - simpleaichat makes it easier to interface with Chat AIs, but it does not attempt to solve common technical and ethical problems inherent to large language models trained on the internet, including prompt injection and unintended plagiarism. The user should exercise good judgment when implementing simpleaichat. Use cases of simpleaichat which go against OpenAI's [usage policies](https://openai.com/policies/usage-policies) (including jailbreaking) will not be endorsed.
+  - simpleaichat intentionally does not use the "Agent" logical metaphor for tool workflows because it's become an AI hype buzzword heavily divorced from its origins. If needed be, you can emulate the Agent workflow with a `while` loop without much additional code, plus with the additional benefit of much more flexibility such as debugging.
 - The session manager implements some sensible security defaults, such as using UUIDs as session ids by default, storing authentication information in a way to minimize unintentional leakage, and type enforcement via Pydantic. Your end-user application should still be aware of potential security issues, however.
 - Although OpenAI's documentation says that system prompts are less effective than a user prompt constructed in a similar manner, in my experience it still does perform better for maintaining rules/a persona.
 - Many examples of popular prompts use more conversational prompts, while the example prompts here use more consise and imperative prompts. This aspect of prompt engineering is still evolving, but in my experience commands do better with ChatGPT and with greater token efficieny. That's also why simpleaichat allows users to specify system prompts (and explicitly highlights what the default use) instead of relying on historical best practices.
+- Token counts for async is not supported as OpenAI doesn't return token counts when streaming responses. In general, there may be some desync in token counts and usage for various use cases; I'm working on categorizing them.
 - Outside of the explicit examples, none of this README uses AI-generated text. The introduction code example is just a joke, but it was too good of a real-world use case!
 
 ## Roadmap
 
 - PaLM Chat (Bard) and Anthropic Claude support
 - More fun/feature-filled CLI chat app based on Textual
 - Simple example of using simpleaichat in a webapp
@@ -276,9 +264,7 @@
 Max Woolf ([@minimaxir](https://minimaxir.com))
 
 _Max's open-source projects are supported by his [Patreon](https://www.patreon.com/minimaxir) and [GitHub Sponsors](https://github.com/sponsors/minimaxir). If you found this project helpful, any monetary contributions to the Patreon are appreciated and will be put to good creative use._
 
 ## License
 
 MIT
-
-
```

