# Comparing `tmp/assemblyai-0.7.0.tar.gz` & `tmp/assemblyai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.7.0.tar", last modified: Wed Jun  7 08:51:49 2023, max compression
+gzip compressed data, was "assemblyai-0.8.0.tar", last modified: Thu Jun  8 09:27:53 2023, max compression
```

## Comparing `assemblyai-0.7.0.tar` & `assemblyai-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.836584 assemblyai-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-07 08:51:35.000000 assemblyai-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-07 08:51:49.836584 assemblyai-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-06-07 08:51:35.000000 assemblyai-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.828584 assemblyai-0.7.0/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22372 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    46689 2023-06-07 08:51:35.000000 assemblyai-0.7.0/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.832584 assemblyai-0.7.0/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 08:51:49.000000 assemblyai-0.7.0/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:51:49.836584 assemblyai-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-07 08:51:35.000000 assemblyai-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.832584 assemblyai-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:49.836584 assemblyai-0.7.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_auto_chapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-07 08:51:35.000000 assemblyai-0.7.0/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.843318 assemblyai-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 09:27:38.000000 assemblyai-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-08 09:27:53.839318 assemblyai-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-06-08 09:27:38.000000 assemblyai-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22797 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48521 2023-06-08 09:27:38.000000 assemblyai-0.8.0/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 09:27:53.000000 assemblyai-0.8.0/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:27:53.843318 assemblyai-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 09:27:38.000000 assemblyai-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:53.839318 assemblyai-0.8.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_auto_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_content_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_entity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-08 09:27:38.000000 assemblyai-0.8.0/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.7.0/LICENSE` & `assemblyai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/PKG-INFO` & `assemblyai-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: assemblyai
-Version: 0.7.0
-Summary: AssemblyAI Python SDK
-Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
-Author: AssemblyAI
-Author-email: engineering.sdk@assemblyai.com
-License: MIT License
-Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
-Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
-Project-URL: Documentation, https://github.com/AssemblyAI/assemblyai-python-sdk/blob/master/README.md
-Project-URL: API Documentation, https://www.assemblyai.com/docs/
-Project-URL: Website, https://assemblyai.com/
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img src="https://github.com/AssemblyAI/assemblyai-python-sdk/blob/master/assemblyai.png?raw=true" width="500"/>
 
 ---
 
 [![CI Passing](https://github.com/AssemblyAI/assemblyai-python-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/AssemblyAI/assemblyai-python-sdk/actions/workflows/test.yml)
 [![GitHub License](https://img.shields.io/github/license/AssemblyAI/assemblyai-python-sdk)](https://github.com/AssemblyAI/assemblyai-python-sdk/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/assemblyai.svg)](https://badge.fury.io/py/assemblyai)
@@ -335,14 +305,118 @@
   summarization=True,
   summary_model=aai.SummarizationModel.catchy,
   summary_type=aai.SummarizationType.headline
 )
 ```
 
 </details>
+<details>
+  <summary>Detect Sensitive Content in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(content_safety=True)
+)
+
+
+# Get the parts of the transcript which were flagged as sensitive
+for result in transcript.content_safety_labels.results:
+  print(result.text)  # sensitive text snippet
+  print(result.timestamp.start)
+  print(result.timestamp.end)
+
+  for label in result.labels:
+    print(label.label)  # content safety category
+    print(label.confidence) # model's confidence that the text is in this category
+    print(label.severity) # severity of the text in relation to the category
+
+# Get the confidence of the most common labels in relation to the entire audio file
+for label, confidence in transcript.content_safety_labels.summary.items():
+  print(f"{confidence * 100}% confident that the audio contains {label}")
+
+# Get the overall severity of the most common labels in relation to the entire audio file
+for label, severity_confidence in transcript.content_safety_labels.severity_score_summary.items():
+  print(f"{severity_confidence.low * 100}% confident that the audio contains low-severity {label}")
+  print(f"{severity_confidence.medium * 100}% confident that the audio contains mid-severity {label}")
+  print(f"{severity_confidence.high * 100}% confident that the audio contains high-severity {label}")
+
+```
+
+[Read more about the content safety categories.](https://www.assemblyai.com/docs/Models/content_moderation#all-labels-supported-by-the-model)
+
+By default, the content safety model will only include labels with a confidence greater than 0.5 (50%). To change this, pass `content_safety_confidence` (as an integer percentage between 25 and 100, inclusive) to the `TranscriptionConfig`:
+
+```python
+config=aai.TranscriptionConfig(
+  content_safety=True,
+  content_safety_confidence=80,  # only include labels with a confidence greater than 80%
+)
+```
+
+</details>
+<details>
+  <summary>Analyze the Sentiment of Sentences in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(sentiment_analysis=True)
+)
+
+for sentiment_result in transcript.sentiment_analysis_results:
+  print(sentiment_result.text)
+  print(sentiment_result.sentiment)  # POSITIVE, NEUTRAL, or NEGATIVE
+  print(sentiment_result.confidence)
+  print(f"Timestamp: {sentiment_result.timestamp.start} - {sentiment_result.timestamp.end}")
+```
+
+If `speaker_labels` is also enabled, then each sentiment analysis result will also include a `speaker` field.
+
+```python
+# ...
+
+config = aai.TranscriptionConfig(sentiment_analysis=True, speaker_labels=True)
+
+# ...
+
+for sentiment_result in transcript.sentiment_analysis_results:
+  print(sentiment_result.speaker)
+```
+
+[Read more about sentiment analysis here.](https://www.assemblyai.com/docs/Models/sentiment_analysis)
+
+</details>
+<details>
+  <summary>Identify Entities in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(entity_detection=True)
+)
+
+for entity in transcript.entities:
+  print(entity.text) # i.e. "Dan Gilbert"
+  print(entity.type) # i.e. EntityType.person
+  print(f"Timestamp: {entity.start} - {entity.end}")
+```
+
+[Read more about entity detection here.](https://www.assemblyai.com/docs/Models/entity_detection)
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
```

### Comparing `assemblyai-0.7.0/README.md` & `assemblyai-0.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: assemblyai
+Version: 0.8.0
+Summary: AssemblyAI Python SDK
+Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
+Author: AssemblyAI
+Author-email: engineering.sdk@assemblyai.com
+License: MIT License
+Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
+Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
+Project-URL: Documentation, https://github.com/AssemblyAI/assemblyai-python-sdk/blob/master/README.md
+Project-URL: API Documentation, https://www.assemblyai.com/docs/
+Project-URL: Website, https://assemblyai.com/
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img src="https://github.com/AssemblyAI/assemblyai-python-sdk/blob/master/assemblyai.png?raw=true" width="500"/>
 
 ---
 
 [![CI Passing](https://github.com/AssemblyAI/assemblyai-python-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/AssemblyAI/assemblyai-python-sdk/actions/workflows/test.yml)
 [![GitHub License](https://img.shields.io/github/license/AssemblyAI/assemblyai-python-sdk)](https://github.com/AssemblyAI/assemblyai-python-sdk/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/assemblyai.svg)](https://badge.fury.io/py/assemblyai)
@@ -305,14 +335,118 @@
   summarization=True,
   summary_model=aai.SummarizationModel.catchy,
   summary_type=aai.SummarizationType.headline
 )
 ```
 
 </details>
+<details>
+  <summary>Detect Sensitive Content in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(content_safety=True)
+)
+
+
+# Get the parts of the transcript which were flagged as sensitive
+for result in transcript.content_safety_labels.results:
+  print(result.text)  # sensitive text snippet
+  print(result.timestamp.start)
+  print(result.timestamp.end)
+
+  for label in result.labels:
+    print(label.label)  # content safety category
+    print(label.confidence) # model's confidence that the text is in this category
+    print(label.severity) # severity of the text in relation to the category
+
+# Get the confidence of the most common labels in relation to the entire audio file
+for label, confidence in transcript.content_safety_labels.summary.items():
+  print(f"{confidence * 100}% confident that the audio contains {label}")
+
+# Get the overall severity of the most common labels in relation to the entire audio file
+for label, severity_confidence in transcript.content_safety_labels.severity_score_summary.items():
+  print(f"{severity_confidence.low * 100}% confident that the audio contains low-severity {label}")
+  print(f"{severity_confidence.medium * 100}% confident that the audio contains mid-severity {label}")
+  print(f"{severity_confidence.high * 100}% confident that the audio contains high-severity {label}")
+
+```
+
+[Read more about the content safety categories.](https://www.assemblyai.com/docs/Models/content_moderation#all-labels-supported-by-the-model)
+
+By default, the content safety model will only include labels with a confidence greater than 0.5 (50%). To change this, pass `content_safety_confidence` (as an integer percentage between 25 and 100, inclusive) to the `TranscriptionConfig`:
+
+```python
+config=aai.TranscriptionConfig(
+  content_safety=True,
+  content_safety_confidence=80,  # only include labels with a confidence greater than 80%
+)
+```
+
+</details>
+<details>
+  <summary>Analyze the Sentiment of Sentences in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(sentiment_analysis=True)
+)
+
+for sentiment_result in transcript.sentiment_analysis_results:
+  print(sentiment_result.text)
+  print(sentiment_result.sentiment)  # POSITIVE, NEUTRAL, or NEGATIVE
+  print(sentiment_result.confidence)
+  print(f"Timestamp: {sentiment_result.timestamp.start} - {sentiment_result.timestamp.end}")
+```
+
+If `speaker_labels` is also enabled, then each sentiment analysis result will also include a `speaker` field.
+
+```python
+# ...
+
+config = aai.TranscriptionConfig(sentiment_analysis=True, speaker_labels=True)
+
+# ...
+
+for sentiment_result in transcript.sentiment_analysis_results:
+  print(sentiment_result.speaker)
+```
+
+[Read more about sentiment analysis here.](https://www.assemblyai.com/docs/Models/sentiment_analysis)
+
+</details>
+<details>
+  <summary>Identify Entities in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(entity_detection=True)
+)
+
+for entity in transcript.entities:
+  print(entity.text) # i.e. "Dan Gilbert"
+  print(entity.type) # i.e. EntityType.person
+  print(f"Timestamp: {entity.start} - {entity.end}")
+```
+
+[Read more about entity detection here.](https://www.assemblyai.com/docs/Models/entity_detection)
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
```

### Comparing `assemblyai-0.7.0/assemblyai/__init__.py` & `assemblyai-0.8.0/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/assemblyai/api.py` & `assemblyai-0.8.0/assemblyai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     response = client.post(
         "/transcript",
         json=request.dict(
             exclude_none=True,
             by_alias=True,
         ),
     )
-
     if response.status_code != httpx.codes.ok:
         raise types.TranscriptError(
             f"failed to transcript url {request.audio_url}: {_get_error_message(response)}"
         )
 
     return types.TranscriptResponse.parse_obj(response.json())
```

### Comparing `assemblyai-0.7.0/assemblyai/client.py` & `assemblyai-0.8.0/assemblyai/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """
         Creates the AssemblyAI client.
 
         Args:
             settings: The settings to use for the client.
         """
 
-        self._settings = settings
+        self._settings = settings.copy()
 
         if not self._settings.api_key:
             raise ValueError(
                 "Please provide an API key via the ASSEMBLYAI_API_KEY environment variable or the global settings."
             )
 
         self._http_client = httpx.Client(
@@ -66,13 +66,13 @@
         Return the default client.
 
         Returns:
             The default client with the default settings
         """
         from . import settings as default_settings
 
-        if cls._default is None:
+        if cls._default is None or cls._default.settings != default_settings:
             with cls._lock:
                 if cls._default is None or cls._default.settings != default_settings:
                     cls._default = cls(settings=default_settings)
 
         return cls._default
```

### Comparing `assemblyai-0.7.0/assemblyai/lemur.py` & `assemblyai-0.8.0/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/assemblyai/transcriber.py` & `assemblyai-0.8.0/assemblyai/transcriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,26 @@
         return self._impl.transcript.summary
 
     @property
     def chapters(self) -> Optional[List[types.Chapter]]:
         return self._impl.transcript.chapters
 
     @property
+    def content_safety_labels(self) -> Optional[types.ContentSafetyResponse]:
+        return self._impl.transcript.content_safety_labels
+
+    @property
+    def sentiment_analysis_results(self) -> Optional[List[types.Sentiment]]:
+        return self._impl.transcript.sentiment_analysis_results
+
+    @property
+    def entities(self) -> Optional[List[types.Entity]]:
+        return self._impl.transcript.entities
+
+    @property
     def status(self) -> types.TranscriptStatus:
         "The current status of the transcript"
 
         return self._impl.transcript.status
 
     @property
     def error(self) -> Optional[str]:
```

### Comparing `assemblyai-0.7.0/assemblyai/types.py` & `assemblyai-0.8.0/assemblyai/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -335,34 +335,37 @@
 
     speaker_labels: Optional[bool]
     "Enable Speaker Diarization."
 
     speakers_expected: Optional[int]
     "The number of speakers you expect to be in your audio file."
 
-    # content_safety: bool = False
-    # "Enable Content Safety Detection."
+    content_safety: Optional[bool]
+    "Enable Content Safety Detection."
+
+    content_safety_confidence: Optional[int]
+    "The minimum confidence level for a content safety label to be produced."
 
     # iab_categories: bool = False
     # "Enable Topic Detection."
 
     custom_spelling: Optional[List[Dict[str, List[str]]]]
     "Customize how words are spelled and formatted using to and from values"
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
-    # sentiment_analysis: bool = False
-    # "Enable Sentiment Analysis."
+    sentiment_analysis: Optional[bool]
+    "Enable Sentiment Analysis."
 
     auto_chapters: Optional[bool]
     "Enable Auto Chapters."
 
-    # entity_detection: bool = False
-    # "Enable Entity Detection."
+    entity_detection: Optional[bool]
+    "Enable Entity Detection."
 
     summarization: Optional[bool]
     "Enable Summarization"
     summary_model: Optional[SummarizationModel]
     "The summarization model to use in case `summarization` is enabled"
     summary_type: Optional[SummarizationType]
     "The summarization type to use in case `summarization` is enabled"
@@ -406,21 +409,22 @@
         filter_profanity: Optional[bool] = None,
         redact_pii: Optional[bool] = None,
         redact_pii_audio: Optional[bool] = None,
         redact_pii_policies: Optional[PIIRedactionPolicy] = None,
         redact_pii_sub: Optional[PIISubstitutionPolicy] = None,
         speaker_labels: Optional[bool] = None,
         speakers_expected: Optional[int] = None,
-        # content_safety: bool = False,
+        content_safety: Optional[bool] = None,
+        content_safety_confidence: Optional[int] = None,
         # iab_categories: bool = False,
         custom_spelling: Optional[Dict[str, Union[str, Sequence[str]]]] = None,
         disfluencies: Optional[bool] = None,
-        # sentiment_analysis: bool = False,
+        sentiment_analysis: Optional[bool] = None,
         auto_chapters: Optional[bool] = None,
-        # entity_detection: bool = False,
+        entity_detection: Optional[bool] = None,
         summarization: Optional[bool] = None,
         summary_model: Optional[SummarizationModel] = None,
         summary_type: Optional[SummarizationType] = None,
         # auto_highlights: bool = False,
         language_detection: Optional[bool] = None,
         raw_transcription_config: Optional[RawTranscriptionConfig] = None,
     ) -> None:
@@ -482,21 +486,21 @@
         self.set_redact_pii(
             redact_pii,
             redact_pii_audio,
             redact_pii_policies,
             redact_pii_sub,
         )
         self.set_speaker_diarization(speaker_labels, speakers_expected)
-        # self.content_safety = content_safety
+        self.set_content_safety(content_safety, content_safety_confidence)
         # self.iab_categories = iab_categories
         self.set_custom_spelling(custom_spelling, override=True)
         self.disfluencies = disfluencies
-        # self.sentiment_analysis = sentiment_analysis
+        self.sentiment_analysis = sentiment_analysis
         self.auto_chapters = auto_chapters
-        # self.entity_detection = entity_detection
+        self.entity_detection = entity_detection
         self.set_summarize(
             summarization,
             summary_model,
             summary_type,
         )
         # self.auto_highlights = auto_highlights
         self.language_detection = language_detection
@@ -640,25 +644,59 @@
 
     @property
     def speakers_expected(self) -> Optional[int]:
         "Returns the number of speakers expected to be in the audio file. Used in combination with the `speaker_labels` parameter."
 
         return self._raw_transcription_config.speakers_expected
 
-    # @property
-    # def content_safety(self) -> bool:
-    #     "Returns the status of the Content Safety feature."
+    @property
+    def content_safety(self) -> Optional[bool]:
+        "Returns the status of the Content Safety feature."
+
+        return self._raw_transcription_config.content_safety
 
-    #     return self._raw_transcription_config.content_safety
+    @property
+    def content_safety_confidence(self) -> Optional[int]:
+        "The minimum confidence level for a content safety label to be produced. Used in combination with the `content_safety` parameter."
 
-    # @content_safety.setter
-    # def content_safety(self, enable: bool) -> None:
-    #     "Enable Content Safety feature."
+        return self._raw_transcription_config.content_safety_confidence
 
-    #     self._raw_transcription_config.content_safety = enable
+    def set_content_safety(
+        self,
+        enable: Optional[bool] = True,
+        content_safety_confidence: Optional[int] = None,
+    ) -> Self:
+        """Enable Content Safety feature.
+
+        Args:
+            `enable`: Whether or not to enable the Content Safety feature.
+            `content_safety_confidence`: The minimum confidence level for a content safety label to be produced.
+
+        Raises:
+            `ValueError`: Raised if `content_safety_confidence` is not between 25 and 100 (inclusive).
+        """
+
+        if not enable:
+            self._raw_transcription_config.content_safety = None
+            self._raw_transcription_config.content_safety_confidence = None
+            return self
+
+        if content_safety_confidence is not None and (
+            content_safety_confidence < 25 or content_safety_confidence > 100
+        ):
+            raise ValueError(
+                "content_safety_confidence must be between 25 and 100 (inclusive)."
+            )
+
+        self._raw_transcription_config.content_safety = enable
+        self._raw_transcription_config.content_safety_confidence = (
+            content_safety_confidence
+        )
+
+        return self
 
     # @property
     # def iab_categories(self) -> bool:
     #     "Returns the status of the Topic Detection feature."
 
     #     return self._raw_transcription_config.iab_categories
 
@@ -691,55 +729,55 @@
     def disfluencies(self, enable: Optional[bool]) -> None:
         "Transcribe filler words, like 'umm', in your media file."
 
         self._raw_transcription_config.disfluencies = enable
 
         return self
 
-    # @property
-    # def sentiment_analysis(self) -> bool:
-    #     "Returns the status of the Sentiment Analysis feature."
+    @property
+    def sentiment_analysis(self) -> Optional[bool]:
+        "Returns the status of the Sentiment Analysis feature."
 
-    #     return self._raw_transcription_config.sentiment_analysis
+        return self._raw_transcription_config.sentiment_analysis
 
-    # @sentiment_analysis.setter
-    # def sentiment_analysis(self, enable: bool) -> None:
-    #     "Enable Sentiment Analysis."
+    @sentiment_analysis.setter
+    def sentiment_analysis(self, enable: Optional[bool]) -> None:
+        "Enable Sentiment Analysis."
 
-    #     self._raw_transcription_config.sentiment_analysis = enable
+        self._raw_transcription_config.sentiment_analysis = enable
 
     @property
     def auto_chapters(self) -> bool:
         "Returns the status of the Auto Chapters feature."
 
         return self._raw_transcription_config.auto_chapters
 
     @auto_chapters.setter
-    def auto_chapters(self, enable: bool) -> None:
+    def auto_chapters(self, enable: Optional[bool]) -> None:
         "Enable Auto Chapters."
 
         # Validate required params are also set
         if self.punctuate == False:
             raise ValueError(
                 "If `auto_chapters` is enabled, then `punctuate` must not be disabled"
             )
 
         self._raw_transcription_config.auto_chapters = enable
 
-    # @property
-    # def entity_detection(self) -> bool:
-    #     "Returns whether Entity Detection feature is enabled or not."
+    @property
+    def entity_detection(self) -> bool:
+        "Returns whether Entity Detection feature is enabled or not."
 
-    #     return self._raw_transcription_config.entity_detection
+        return self._raw_transcription_config.entity_detection
 
-    # @entity_detection.setter
-    # def entity_detection(self, enable: bool) -> None:
-    #     "Enable Entity Detection."
+    @entity_detection.setter
+    def entity_detection(self, enable: Optional[bool]) -> None:
+        "Enable Entity Detection."
 
-    #     self._raw_transcription_config.entity_detection = enable
+        self._raw_transcription_config.entity_detection = enable
 
     @property
     def summarization(self) -> Optional[bool]:
         "Returns whether the Summarization feature is enabled or not."
 
         return self._raw_transcription_config.summarization
 
@@ -1158,15 +1196,15 @@
     status: StatusResult
     results: Optional[List[AutohighlightResult]]
 
 
 class ContentSafetyLabelResult(BaseModel):
     label: ContentSafetyLabel
     confidence: float
-    severity: float
+    severity: Optional[float]
 
 
 class ContentSafetySeverityScore(BaseModel):
     low: float
     medium: float
     high: float
 
@@ -1176,16 +1214,18 @@
     labels: List[ContentSafetyLabelResult]
     timestamp: Timestamp
 
 
 class ContentSafetyResponse(BaseModel):
     status: StatusResult
     results: Optional[List[ContentSafetyResult]]
-    summary: Optional[Dict[str, float]]
-    severity_score_summary: Optional[Dict[str, ContentSafetySeverityScore]]
+    summary: Optional[Dict[ContentSafetyLabel, float]]
+    severity_score_summary: Optional[
+        Dict[ContentSafetyLabel, ContentSafetySeverityScore]
+    ]
 
 
 class IABLabelResult(BaseModel):
     relevance: float
     label: str
 
 
@@ -1199,14 +1239,15 @@
     status: StatusResult
     results: Optional[List[IABResult]]
     summary: Optional[Dict[str, float]]
 
 
 class Sentiment(Word):
     sentiment: SentimentType
+    speaker: Optional[str]
 
 
 class Entity(BaseModel):
     entity_type: EntityType
     text: str
     start: int
     end: int
@@ -1304,34 +1345,37 @@
     "The list of PII Redaction policies to enable."
     redact_pii_sub: Optional[PIISubstitutionPolicy]
     "The replacement logic for detected PII."
 
     speaker_labels: Optional[bool]
     "Enable Speaker Diarization."
 
-    # content_safety: bool = False
-    # "Enable Content Safety Detection."
+    content_safety: Optional[bool]
+    "Enable Content Safety Detection."
+
+    content_safety_confidence: Optional[int]
+    "The minimum confidence level for a content safety label to be produced."
 
     # iab_categories: bool = False
     # "Enable Topic Detection."
 
-    custom_spelling: Optional[List[Dict[str, str]]]
+    custom_spelling: Optional[List[Dict[str, Union[str, List[str]]]]]
     "Customize how words are spelled and formatted using to and from values"
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
-    # sentiment_analysis: bool = False
-    # "Enable Sentiment Analysis."
+    sentiment_analysis: Optional[bool]
+    "Enable Sentiment Analysis."
 
     auto_chapters: Optional[bool]
     "Enable Auto Chapters."
 
-    # entity_detection: bool = False
-    # "Enable Entity Detection."
+    entity_detection: Optional[bool]
+    "Enable Entity Detection."
 
     summarization: Optional[bool]
     "Enable Summarization"
     summary_model: Optional[SummarizationModel]
     "The summarization model to use in case `summarization` is enabled"
     summary_type: Optional[SummarizationType]
     "The summarization type to use in case `summarization` is enabled"
@@ -1397,38 +1441,41 @@
 
     summary: Optional[str]
     "The summarization of the transcript"
 
     # auto_highlights_result: Optional[AutohighlightResponse] = None
     # "The list of results when enabling Automatic Transcript Highlights"
 
-    # content_safety_labels: Optional[ContentSafetyResponse] = None
-    # "The list of results when Content Safety is enabled"
+    content_safety_labels: Optional[ContentSafetyResponse]
+    "The list of results when Content Safety is enabled"
 
     # iab_categories_result: Optional[IABResponse] = None
     # "The list of results when Topic Detection is enabled"
 
     chapters: Optional[List[Chapter]]
-    # "When Auto Chapters is enabled, the list of Auto Chapters results"
-
-    # sentiment_analysis_results: Optional[List[Sentiment]] = None
-    # "When Sentiment Analysis is enabled, the list of Sentiment Analysis results"
+    "When Auto Chapters is enabled, the list of Auto Chapters results"
 
-    # entities: Optional[List[Entity]] = None
-    # "When Entity Detection is enabled, the list of detected Entities"
+    sentiment_analysis_results: Optional[List[Sentiment]]
+    "When Sentiment Analysis is enabled, the list of Sentiment Analysis results"
 
-    # def __init__(self, **data: Any):
-    #     # cleanup the response before creating the object
-    #     if data.get("iab_categories_result") == {}:
-    #         data["iab_categories_result"] = None
+    entities: Optional[List[Entity]]
+    "When Entity Detection is enabled, the list of detected Entities"
 
-    #     if data.get("content_safety_labels") == {}:
-    #         data["content_safety_labels"] = None
+    def __init__(self, **data: Any):
+        # cleanup the response before creating the object
+        # if data.get("iab_categories_result") == {}:
+        #     data["iab_categories_result"] = None
+
+        if data.get("content_safety_labels") == {} or (
+            not data.get("content_safety")
+            and data.get("content_safety_labels", {}).get("status") == "unavailable"
+        ):
+            data["content_safety_labels"] = None
 
-    #     super().__init__(**data)
+        super().__init__(**data)
 
 
 class LemurModel(str, Enum):
     lightning = "lightning"
     default = "default"
```

### Comparing `assemblyai-0.7.0/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.8.0/assemblyai.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.7.0
+Version: 0.8.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -335,14 +335,118 @@
   summarization=True,
   summary_model=aai.SummarizationModel.catchy,
   summary_type=aai.SummarizationType.headline
 )
 ```
 
 </details>
+<details>
+  <summary>Detect Sensitive Content in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(content_safety=True)
+)
+
+
+# Get the parts of the transcript which were flagged as sensitive
+for result in transcript.content_safety_labels.results:
+  print(result.text)  # sensitive text snippet
+  print(result.timestamp.start)
+  print(result.timestamp.end)
+
+  for label in result.labels:
+    print(label.label)  # content safety category
+    print(label.confidence) # model's confidence that the text is in this category
+    print(label.severity) # severity of the text in relation to the category
+
+# Get the confidence of the most common labels in relation to the entire audio file
+for label, confidence in transcript.content_safety_labels.summary.items():
+  print(f"{confidence * 100}% confident that the audio contains {label}")
+
+# Get the overall severity of the most common labels in relation to the entire audio file
+for label, severity_confidence in transcript.content_safety_labels.severity_score_summary.items():
+  print(f"{severity_confidence.low * 100}% confident that the audio contains low-severity {label}")
+  print(f"{severity_confidence.medium * 100}% confident that the audio contains mid-severity {label}")
+  print(f"{severity_confidence.high * 100}% confident that the audio contains high-severity {label}")
+
+```
+
+[Read more about the content safety categories.](https://www.assemblyai.com/docs/Models/content_moderation#all-labels-supported-by-the-model)
+
+By default, the content safety model will only include labels with a confidence greater than 0.5 (50%). To change this, pass `content_safety_confidence` (as an integer percentage between 25 and 100, inclusive) to the `TranscriptionConfig`:
+
+```python
+config=aai.TranscriptionConfig(
+  content_safety=True,
+  content_safety_confidence=80,  # only include labels with a confidence greater than 80%
+)
+```
+
+</details>
+<details>
+  <summary>Analyze the Sentiment of Sentences in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(sentiment_analysis=True)
+)
+
+for sentiment_result in transcript.sentiment_analysis_results:
+  print(sentiment_result.text)
+  print(sentiment_result.sentiment)  # POSITIVE, NEUTRAL, or NEGATIVE
+  print(sentiment_result.confidence)
+  print(f"Timestamp: {sentiment_result.timestamp.start} - {sentiment_result.timestamp.end}")
+```
+
+If `speaker_labels` is also enabled, then each sentiment analysis result will also include a `speaker` field.
+
+```python
+# ...
+
+config = aai.TranscriptionConfig(sentiment_analysis=True, speaker_labels=True)
+
+# ...
+
+for sentiment_result in transcript.sentiment_analysis_results:
+  print(sentiment_result.speaker)
+```
+
+[Read more about sentiment analysis here.](https://www.assemblyai.com/docs/Models/sentiment_analysis)
+
+</details>
+<details>
+  <summary>Identify Entities in a Transcript</summary>
+
+```python
+import assemblyai as aai
+
+transcriber = aai.Transcriber()
+transcript = transcriber.transcribe(
+  "https://example.org/audio.mp3",
+  config=aai.TranscriptionConfig(entity_detection=True)
+)
+
+for entity in transcript.entities:
+  print(entity.text) # i.e. "Dan Gilbert"
+  print(entity.type) # i.e. EntityType.person
+  print(f"Timestamp: {entity.start} - {entity.end}")
+```
+
+[Read more about entity detection here.](https://www.assemblyai.com/docs/Models/entity_detection)
+
+</details>
 
 ---
 
 ## Playgrounds
 
 Visit one of our Playgrounds:
```

### Comparing `assemblyai-0.7.0/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.8.0/assemblyai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,13 +13,17 @@
 assemblyai.egg-info/requires.txt
 assemblyai.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/factories.py
 tests/unit/test_auto_chapters.py
+tests/unit/test_client.py
 tests/unit/test_config.py
+tests/unit/test_content_safety.py
 tests/unit/test_domains.py
+tests/unit/test_entity_detection.py
 tests/unit/test_lemur.py
+tests/unit/test_sentiment_analysis.py
 tests/unit/test_summarization.py
 tests/unit/test_transcriber.py
 tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.7.0/setup.py` & `assemblyai-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.7.0",
+    version="0.8.0",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.7.0/tests/unit/factories.py` & `assemblyai-0.8.0/tests/unit/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """
 Contains factories that are used for mocking certain requests/responses
 from AssemblyAI's API.
 """
 
+from enum import Enum
 from functools import partial
 from typing import Any, Callable, Dict
 
 import factory
 import factory.base
 
 import assemblyai as aai
 from assemblyai import types
 
 
+class TimestampFactory(factory.Factory):
+    class Meta:
+        model = aai.Timestamp
+
+    start = factory.Faker("pyint")
+    end = factory.Faker("pyint")
+
+
 class WordFactory(factory.Factory):
     class Meta:
         model = aai.Word
 
     text = factory.Faker("word")
     start = factory.Faker("pyint")
     end = factory.Faker("pyint")
@@ -230,14 +239,16 @@
         for key, value in stub_dict.items():
             if isinstance(value, factory.base.StubObject):
                 stub_dict[key] = (
                     [convert_dict_from_stub(v) for v in value.__dict__.values()]
                     if stub_is_list(value)
                     else convert_dict_from_stub(value)
                 )
+            elif isinstance(value, Enum):
+                stub_dict[key] = value.value
         return stub_dict
 
     def dict_factory(f, **kwargs):
         stub = f.stub(**kwargs)
         stub_dict = convert_dict_from_stub(stub)
         return stub_dict
```

### Comparing `assemblyai-0.7.0/tests/unit/test_auto_chapters.py` & `assemblyai-0.8.0/tests/unit/test_auto_chapters.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/tests/unit/test_domains.py` & `assemblyai-0.8.0/tests/unit/test_domains.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         "raw",  # access to the underlying raw config
         "set_word_boost",  # word boost setter
         "set_casing_and_formatting",  # punctuation, formatting setter
         "set_redact_pii",  # PII redaction
         "set_summarize",  # summarization
         "set_webhook",  # webhook
         "set_speaker_diarization",  # speaker diarization
+        "set_content_safety",  # content safety
     }
 
     # get all members
     non_raw_members = inspect.getmembers(aai.TranscriptionConfig)
 
     # just retrieve the names
     raw_member_names = set(aai.RawTranscriptionConfig.__fields__.keys())
```

### Comparing `assemblyai-0.7.0/tests/unit/test_lemur.py` & `assemblyai-0.8.0/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/tests/unit/test_summarization.py` & `assemblyai-0.8.0/tests/unit/test_summarization.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/tests/unit/test_transcriber.py` & `assemblyai-0.8.0/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.7.0/tests/unit/test_transcript.py` & `assemblyai-0.8.0/tests/unit/test_transcript.py`

 * *Files identical despite different names*

