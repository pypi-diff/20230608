# Comparing `tmp/promptengine_catapult-0.0.6.tar.gz` & `tmp/promptengine_catapult-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.0.6.tar", last modified: Thu Jun  8 05:49:24 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.0.7.tar", last modified: Thu Jun  8 05:51:19 2023, max compression
```

## Comparing `promptengine_catapult-0.0.6.tar` & `promptengine_catapult-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:49:24.359155 promptengine_catapult-0.0.6/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.6/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-08 05:49:24.359155 promptengine_catapult-0.0.6/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.6/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:49:24.355155 promptengine_catapult-0.0.6/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-06-04 19:15:11.000000 promptengine_catapult-0.0.6/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.6/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6374 2023-06-06 05:58:50.000000 promptengine_catapult-0.0.6/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      789 2023-06-04 13:28:26.000000 promptengine_catapult-0.0.6/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:49:24.359155 promptengine_catapult-0.0.6/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-08 05:49:24.000000 promptengine_catapult-0.0.6/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-08 05:49:24.000000 promptengine_catapult-0.0.6/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-08 05:49:24.000000 promptengine_catapult-0.0.6/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-06-08 05:49:24.000000 promptengine_catapult-0.0.6/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-08 05:49:24.000000 promptengine_catapult-0.0.6/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-08 05:49:24.359155 promptengine_catapult-0.0.6/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-06-08 05:49:19.000000 promptengine_catapult-0.0.6/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:51:19.923049 promptengine_catapult-0.0.7/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.7/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-08 05:51:19.923049 promptengine_catapult-0.0.7/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.7/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:51:19.923049 promptengine_catapult-0.0.7/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-06-04 19:15:11.000000 promptengine_catapult-0.0.7/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.7/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6390 2023-06-08 05:51:13.000000 promptengine_catapult-0.0.7/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      789 2023-06-04 13:28:26.000000 promptengine_catapult-0.0.7/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-08 05:51:19.923049 promptengine_catapult-0.0.7/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-08 05:51:19.000000 promptengine_catapult-0.0.7/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-08 05:51:19.000000 promptengine_catapult-0.0.7/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-08 05:51:19.000000 promptengine_catapult-0.0.7/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       60 2023-06-08 05:51:19.000000 promptengine_catapult-0.0.7/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-08 05:51:19.000000 promptengine_catapult-0.0.7/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-08 05:51:19.923049 promptengine_catapult-0.0.7/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1467 2023-06-08 05:50:52.000000 promptengine_catapult-0.0.7/setup.py
```

### Comparing `promptengine_catapult-0.0.6/LICENSE` & `promptengine_catapult-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.6/PKG-INFO` & `promptengine_catapult-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.0.6
+Version: 0.0.7
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.6/README.md` & `promptengine_catapult-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.6/promptengine_catapult/config.py` & `promptengine_catapult-0.0.7/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.6/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.0.7/promptengine_catapult/prompt_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,7 +169,8 @@
         transcript = openai.Audio.transcribe("whisper-1", audio_file)
         logging.debug("voice to text conversion successful")
         return transcript["text"]
 
 
 # TO Do:
 # Feedback function
+# redis timeout
```

### Comparing `promptengine_catapult-0.0.6/promptengine_catapult/utils.py` & `promptengine_catapult-0.0.7/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.6/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.0.7/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.0.6
+Version: 0.0.7
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.6/setup.py` & `promptengine_catapult-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```

