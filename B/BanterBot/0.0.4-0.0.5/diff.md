# Comparing `tmp/BanterBot-0.0.4.tar.gz` & `tmp/BanterBot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanterBot-0.0.4.tar", last modified: Mon Jun  5 21:51:08 2023, max compression
+gzip compressed data, was "BanterBot-0.0.5.tar", last modified: Wed Jun  7 21:57:46 2023, max compression
```

## Comparing `BanterBot-0.0.4.tar` & `BanterBot-0.0.5.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.947049 BanterBot-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.857545 BanterBot-0.0.4/BanterBot.egg-info/
--rw-rw-rw-   0        0        0     6669 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6669 2023-06-05 21:51:08.947049 BanterBot-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5564 2023-06-05 20:27:33.000000 BanterBot-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.858546 BanterBot-0.0.4/banterbot/
--rw-rw-rw-   0        0        0      740 2023-06-05 20:28:59.000000 BanterBot-0.0.4/banterbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.871547 BanterBot-0.0.4/banterbot/core/
--rw-rw-rw-   0        0        0      251 2023-05-30 22:17:56.000000 BanterBot-0.0.4/banterbot/core/__init__.py
--rw-rw-rw-   0        0        0     8586 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/core/openai_manager.py
--rw-rw-rw-   0        0        0     7671 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/core/speech_to_text.py
--rw-rw-rw-   0        0        0    13493 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/core/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.883047 BanterBot-0.0.4/banterbot/data/
--rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.4/banterbot/data/__init__.py
--rw-rw-rw-   0        0        0     7570 2023-06-04 19:42:55.000000 BanterBot-0.0.4/banterbot/data/azure_neural_voices.py
--rw-rw-rw-   0        0        0      605 2023-06-04 19:49:08.000000 BanterBot-0.0.4/banterbot/data/config.py
--rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.4/banterbot/data/enums.py
--rw-rw-rw-   0        0        0     3347 2023-06-04 19:42:55.000000 BanterBot-0.0.4/banterbot/data/openai_models.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.898048 BanterBot-0.0.4/banterbot/gui/
--rw-rw-rw-   0        0        0      280 2023-06-05 20:28:59.000000 BanterBot-0.0.4/banterbot/gui/__init__.py
--rw-rw-rw-   0        0        0     2626 2023-06-05 20:03:52.000000 BanterBot-0.0.4/banterbot/gui/cli.py
--rw-rw-rw-   0        0        0    11034 2023-06-05 21:44:50.000000 BanterBot-0.0.4/banterbot/gui/interface.py
--rw-rw-rw-   0        0        0     6443 2023-06-05 21:46:26.000000 BanterBot-0.0.4/banterbot/gui/tk_multiplayer_interface.py
--rw-rw-rw-   0        0        0     7487 2023-06-05 21:47:39.000000 BanterBot-0.0.4/banterbot/gui/tk_simple_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.924049 BanterBot-0.0.4/banterbot/utils/
--rw-rw-rw-   0        0        0       67 2023-05-29 12:59:46.000000 BanterBot-0.0.4/banterbot/utils/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-06-04 19:42:56.000000 BanterBot-0.0.4/banterbot/utils/message.py
--rw-rw-rw-   0        0        0     5723 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/utils/nlp.py
--rw-rw-rw-   0        0        0     7631 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/utils/speech_to_text_output.py
--rw-rw-rw-   0        0        0     3887 2023-06-04 19:42:56.000000 BanterBot-0.0.4/banterbot/utils/text_to_speech_output.py
--rw-rw-rw-   0        0        0     2895 2023-06-04 19:42:56.000000 BanterBot-0.0.4/banterbot/utils/thread_queue.py
--rw-rw-rw-   0        0        0     3095 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/utils/word.py
--rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-06-05 21:51:08.949549 BanterBot-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2216 2023-06-04 20:11:00.000000 BanterBot-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.926048 BanterBot-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.929548 BanterBot-0.0.4/tests/core/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/core/__init__.py
--rw-rw-rw-   0        0        0     8816 2023-06-05 21:46:06.000000 BanterBot-0.0.4/tests/core/test_openai_manager.py
--rw-rw-rw-   0        0        0     2659 2023-06-05 21:46:07.000000 BanterBot-0.0.4/tests/core/test_text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.944550 BanterBot-0.0.4/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/test_message.py
--rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/test_nlp.py
--rw-rw-rw-   0        0        0     3085 2023-06-05 21:46:06.000000 BanterBot-0.0.4/tests/utils/test_text_to_speech_output.py
--rw-rw-rw-   0        0        0     1237 2023-06-05 21:46:06.000000 BanterBot-0.0.4/tests/utils/test_text_to_speech_word.py
--rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/test_thread_queue.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.912656 BanterBot-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.816156 BanterBot-0.0.5/BanterBot.egg-info/
+-rw-rw-rw-   0        0        0     6771 2023-06-07 21:57:46.000000 BanterBot-0.0.5/BanterBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1394 2023-06-07 21:57:46.000000 BanterBot-0.0.5/BanterBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 21:57:46.000000 BanterBot-0.0.5/BanterBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-07 21:57:46.000000 BanterBot-0.0.5/BanterBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-06-07 21:57:46.000000 BanterBot-0.0.5/BanterBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 21:57:46.000000 BanterBot-0.0.5/BanterBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6771 2023-06-07 21:57:46.912656 BanterBot-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5636 2023-06-07 21:54:53.000000 BanterBot-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.819656 BanterBot-0.0.5/banterbot/
+-rw-rw-rw-   0        0        0      764 2023-06-07 21:14:18.000000 BanterBot-0.0.5/banterbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.830657 BanterBot-0.0.5/banterbot/api_managers/
+-rw-rw-rw-   0        0        0      275 2023-06-06 18:31:29.000000 BanterBot-0.0.5/banterbot/api_managers/__init__.py
+-rw-rw-rw-   0        0        0     8773 2023-06-07 20:15:55.000000 BanterBot-0.0.5/banterbot/api_managers/openai_manager.py
+-rw-rw-rw-   0        0        0     7673 2023-06-06 18:38:45.000000 BanterBot-0.0.5/banterbot/api_managers/speech_to_text.py
+-rw-rw-rw-   0        0        0    13495 2023-06-06 18:38:45.000000 BanterBot-0.0.5/banterbot/api_managers/text_to_speech.py
+-rw-rw-rw-   0        0        0      605 2023-06-04 19:49:08.000000 BanterBot-0.0.5/banterbot/config.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.844656 BanterBot-0.0.5/banterbot/data/
+-rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.5/banterbot/data/__init__.py
+-rw-rw-rw-   0        0        0     7594 2023-06-07 21:24:03.000000 BanterBot-0.0.5/banterbot/data/azure_neural_voices.py
+-rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.5/banterbot/data/enums.py
+-rw-rw-rw-   0        0        0     3347 2023-06-07 20:17:02.000000 BanterBot-0.0.5/banterbot/data/openai_models.py
+-rw-rw-rw-   0        0        0     1383 2023-06-07 21:06:08.000000 BanterBot-0.0.5/banterbot/data/prompts.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.855156 BanterBot-0.0.5/banterbot/gui/
+-rw-rw-rw-   0        0        0      280 2023-06-05 20:28:59.000000 BanterBot-0.0.5/banterbot/gui/__init__.py
+-rw-rw-rw-   0        0        0     4194 2023-06-07 21:50:18.000000 BanterBot-0.0.5/banterbot/gui/cli.py
+-rw-rw-rw-   0        0        0    12520 2023-06-07 21:15:00.000000 BanterBot-0.0.5/banterbot/gui/interface.py
+-rw-rw-rw-   0        0        0     6588 2023-06-07 21:50:18.000000 BanterBot-0.0.5/banterbot/gui/tk_multiplayer_interface.py
+-rw-rw-rw-   0        0        0     7632 2023-06-07 21:50:18.000000 BanterBot-0.0.5/banterbot/gui/tk_simple_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.867156 BanterBot-0.0.5/banterbot/openai_extensions/
+-rw-rw-rw-   0        0        0      211 2023-06-07 21:13:49.000000 BanterBot-0.0.5/banterbot/openai_extensions/__init__.py
+-rw-rw-rw-   0        0        0     8665 2023-06-07 20:43:49.000000 BanterBot-0.0.5/banterbot/openai_extensions/option_predictor.py
+-rw-rw-rw-   0        0        0     4748 2023-06-07 21:19:41.000000 BanterBot-0.0.5/banterbot/openai_extensions/option_selector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.890656 BanterBot-0.0.5/banterbot/utils/
+-rw-rw-rw-   0        0        0       67 2023-06-06 20:36:53.000000 BanterBot-0.0.5/banterbot/utils/__init__.py
+-rw-rw-rw-   0        0        0     3274 2023-06-07 20:11:35.000000 BanterBot-0.0.5/banterbot/utils/message.py
+-rw-rw-rw-   0        0        0     5725 2023-06-06 18:38:45.000000 BanterBot-0.0.5/banterbot/utils/nlp.py
+-rw-rw-rw-   0        0        0     7633 2023-06-06 18:38:45.000000 BanterBot-0.0.5/banterbot/utils/speech_to_text_output.py
+-rw-rw-rw-   0        0        0     3887 2023-06-04 19:42:56.000000 BanterBot-0.0.5/banterbot/utils/text_to_speech_output.py
+-rw-rw-rw-   0        0        0     2895 2023-06-04 19:42:56.000000 BanterBot-0.0.5/banterbot/utils/thread_queue.py
+-rw-rw-rw-   0        0        0     3097 2023-06-06 18:38:45.000000 BanterBot-0.0.5/banterbot/utils/word.py
+-rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-06-07 21:57:46.914656 BanterBot-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2255 2023-06-07 17:56:36.000000 BanterBot-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.892656 BanterBot-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.896657 BanterBot-0.0.5/tests/core/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.5/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     8818 2023-06-06 18:38:45.000000 BanterBot-0.0.5/tests/core/test_openai_manager.py
+-rw-rw-rw-   0        0        0     2661 2023-06-07 21:50:18.000000 BanterBot-0.0.5/tests/core/test_text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-07 21:57:46.910657 BanterBot-0.0.5/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.5/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.5/tests/utils/test_message.py
+-rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.5/tests/utils/test_nlp.py
+-rw-rw-rw-   0        0        0     3087 2023-06-06 18:38:45.000000 BanterBot-0.0.5/tests/utils/test_text_to_speech_output.py
+-rw-rw-rw-   0        0        0     1239 2023-06-06 18:38:45.000000 BanterBot-0.0.5/tests/utils/test_text_to_speech_word.py
+-rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.5/tests/utils/test_thread_queue.py
```

### Comparing `BanterBot-0.0.4/BanterBot.egg-info/PKG-INFO` & `BanterBot-0.0.5/BanterBot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.4
-Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and Tkinter frontend.
+Version: 0.0.5
+Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions with emotional tone selection. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.4-alpha/BanterBot-0.0.4.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.5-alpha/BanterBot-0.0.5.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -20,21 +20,22 @@
 
 # BanterBot
 
 BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses, Azure Neural Voices for text-to-speech synthesis, and Azure speech-to-text recognition. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
 
 ## Features
 
-* Employs OpenAI models for generating context-sensitive responses
-* Utilizes Azure Neural Voices for high-quality text-to-speech synthesis
-* Supports a variety of output formats, voices, and speaking styles
-* Enables real-time monitoring of the chatbot's responses
-* Features asynchronous speech-to-text microphone input
-* Provides an abstract base class for crafting frontends for the BanterBot application
-* Includes a tkinter-based frontend implementation
+* Utilizes OpenAI models to generate context-aware responses
+* Leverages Azure Neural Voices for premium text-to-speech synthesis
+* Offers a wide range of output formats, voices, and speaking styles
+* Allows real-time monitoring of the chatbot's responses
+* Supports asynchronous speech-to-text microphone input
+* Includes an abstract base class for creating custom frontends for the BanterBot application
+* Features a tkinter-based frontend implementation
+* Automatically selects an appropriate emotion or tone based on the conversation context
 
 ## Requirements
 
 Three environment variables are required for full functionality:
 
 * `OPENAI_API_KEY`: A valid OpenAI API key
 * `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for text-to-speech and speech-to-text functionality
@@ -87,55 +88,48 @@
 
 ## Usage
 
 ### Launch with Command Line
 
 Start BanterBot by running the `banterbot` command in your terminal.
 
-Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+- Add the `-g` flag to enable GPT-4 for enhanced conversation quality. Please note that GPT-4 API access is required, and using GPT-4 is more costly and slower than the default GPT-3.5-Turbo.
 
-Add the `-s` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-s "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."`).
+- Use the `-p` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-p "You are Grendel the Quiz Troll, a charismatic troll who loves hosting quiz shows."`).
 
-Add the `-m` flag to activate the multiplayer interface.
+- Include the `-m` flag to activate the multiplayer interface.
+
+- Apply the `-e` flag to enable emotional tone evaluation before the bot generates its responses.
+
+- To select a Microsoft Azure Cognitive Services text-to-speech voice, use the `-v` flag followed by one of the available voice options (e.g., `-v jenny`).
+
+- Select a Microsoft Azure Cognitive Services text-to-speech voice style by using the `-s` flag followed by one of the available style options (e.g., `-s friendly`).
 
 ### Launch with a Python script
 
 To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
 
 ```python
-from banterbot import TKInterface, get_voice_by_name, get_model_by_name
+from banterbot import TKSimpleInterface, get_voice_by_name, get_model_by_name
 
 model = get_model_by_name("gpt-3.5-turbo")
-voice = get_voice_by_name("Aria")
+voice = get_voice_by_name("Davis")
 
-style = "chat"
+style = "excited"
 # Optional system prompt to set up a custom character prior to initializing BanterBot.
 system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
 
-# The four arguments `model`, `voice`, `style`, and `system` are optional.
-interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system)
+# The four arguments `model`, `voice`, `style`, `system`, and `tone` are optional.
+# Setting `tone` to True enables voice tones and emotions.
+interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system, tone=True)
 interface.run()
 ```
 
-For multiplayer, you can modify the above code slightly:
-
-```python
-from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name
-
-model = get_model_by_name("gpt-3.5-turbo")
-voice = get_voice_by_name("Aria")
-style = "chat"
-
-# Optional system prompt to set up a custom character prior to initializing BanterBot.
-system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
+For multiplayer, you can swap out TKSimpleInterface in the above code with TKMultiplayerInterface.
 
-# The four arguments `model`, `voice`, `style`, and `system` are optional.
-interface = TKMultiplayerInterface(model=model, voice=voice, style=style, system=system)
-interface.run()
-```
 
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
```

### Comparing `BanterBot-0.0.4/BanterBot.egg-info/SOURCES.txt` & `BanterBot-0.0.5/BanterBot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 BanterBot.egg-info/PKG-INFO
 BanterBot.egg-info/SOURCES.txt
 BanterBot.egg-info/dependency_links.txt
 BanterBot.egg-info/entry_points.txt
 BanterBot.egg-info/requires.txt
 BanterBot.egg-info/top_level.txt
 banterbot/__init__.py
-banterbot/core/__init__.py
-banterbot/core/openai_manager.py
-banterbot/core/speech_to_text.py
-banterbot/core/text_to_speech.py
+banterbot/config.py
+banterbot/api_managers/__init__.py
+banterbot/api_managers/openai_manager.py
+banterbot/api_managers/speech_to_text.py
+banterbot/api_managers/text_to_speech.py
 banterbot/data/__init__.py
 banterbot/data/azure_neural_voices.py
-banterbot/data/config.py
 banterbot/data/enums.py
 banterbot/data/openai_models.py
+banterbot/data/prompts.py
 banterbot/gui/__init__.py
 banterbot/gui/cli.py
 banterbot/gui/interface.py
 banterbot/gui/tk_multiplayer_interface.py
 banterbot/gui/tk_simple_interface.py
+banterbot/openai_extensions/__init__.py
+banterbot/openai_extensions/option_predictor.py
+banterbot/openai_extensions/option_selector.py
 banterbot/utils/__init__.py
 banterbot/utils/message.py
 banterbot/utils/nlp.py
 banterbot/utils/speech_to_text_output.py
 banterbot/utils/text_to_speech_output.py
 banterbot/utils/thread_queue.py
 banterbot/utils/word.py
```

### Comparing `BanterBot-0.0.4/PKG-INFO` & `BanterBot-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.4
-Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and Tkinter frontend.
+Version: 0.0.5
+Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions with emotional tone selection. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.4-alpha/BanterBot-0.0.4.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.5-alpha/BanterBot-0.0.5.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -20,21 +20,22 @@
 
 # BanterBot
 
 BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses, Azure Neural Voices for text-to-speech synthesis, and Azure speech-to-text recognition. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
 
 ## Features
 
-* Employs OpenAI models for generating context-sensitive responses
-* Utilizes Azure Neural Voices for high-quality text-to-speech synthesis
-* Supports a variety of output formats, voices, and speaking styles
-* Enables real-time monitoring of the chatbot's responses
-* Features asynchronous speech-to-text microphone input
-* Provides an abstract base class for crafting frontends for the BanterBot application
-* Includes a tkinter-based frontend implementation
+* Utilizes OpenAI models to generate context-aware responses
+* Leverages Azure Neural Voices for premium text-to-speech synthesis
+* Offers a wide range of output formats, voices, and speaking styles
+* Allows real-time monitoring of the chatbot's responses
+* Supports asynchronous speech-to-text microphone input
+* Includes an abstract base class for creating custom frontends for the BanterBot application
+* Features a tkinter-based frontend implementation
+* Automatically selects an appropriate emotion or tone based on the conversation context
 
 ## Requirements
 
 Three environment variables are required for full functionality:
 
 * `OPENAI_API_KEY`: A valid OpenAI API key
 * `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for text-to-speech and speech-to-text functionality
@@ -87,55 +88,48 @@
 
 ## Usage
 
 ### Launch with Command Line
 
 Start BanterBot by running the `banterbot` command in your terminal.
 
-Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+- Add the `-g` flag to enable GPT-4 for enhanced conversation quality. Please note that GPT-4 API access is required, and using GPT-4 is more costly and slower than the default GPT-3.5-Turbo.
 
-Add the `-s` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-s "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."`).
+- Use the `-p` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-p "You are Grendel the Quiz Troll, a charismatic troll who loves hosting quiz shows."`).
 
-Add the `-m` flag to activate the multiplayer interface.
+- Include the `-m` flag to activate the multiplayer interface.
+
+- Apply the `-e` flag to enable emotional tone evaluation before the bot generates its responses.
+
+- To select a Microsoft Azure Cognitive Services text-to-speech voice, use the `-v` flag followed by one of the available voice options (e.g., `-v jenny`).
+
+- Select a Microsoft Azure Cognitive Services text-to-speech voice style by using the `-s` flag followed by one of the available style options (e.g., `-s friendly`).
 
 ### Launch with a Python script
 
 To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
 
 ```python
-from banterbot import TKInterface, get_voice_by_name, get_model_by_name
+from banterbot import TKSimpleInterface, get_voice_by_name, get_model_by_name
 
 model = get_model_by_name("gpt-3.5-turbo")
-voice = get_voice_by_name("Aria")
+voice = get_voice_by_name("Davis")
 
-style = "chat"
+style = "excited"
 # Optional system prompt to set up a custom character prior to initializing BanterBot.
 system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
 
-# The four arguments `model`, `voice`, `style`, and `system` are optional.
-interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system)
+# The four arguments `model`, `voice`, `style`, `system`, and `tone` are optional.
+# Setting `tone` to True enables voice tones and emotions.
+interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system, tone=True)
 interface.run()
 ```
 
-For multiplayer, you can modify the above code slightly:
-
-```python
-from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name
-
-model = get_model_by_name("gpt-3.5-turbo")
-voice = get_voice_by_name("Aria")
-style = "chat"
-
-# Optional system prompt to set up a custom character prior to initializing BanterBot.
-system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
+For multiplayer, you can swap out TKSimpleInterface in the above code with TKMultiplayerInterface.
 
-# The four arguments `model`, `voice`, `style`, and `system` are optional.
-interface = TKMultiplayerInterface(model=model, voice=voice, style=style, system=system)
-interface.run()
-```
 
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
```

### Comparing `BanterBot-0.0.4/README.md` & `BanterBot-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # BanterBot
 
 BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses, Azure Neural Voices for text-to-speech synthesis, and Azure speech-to-text recognition. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
 
 ## Features
 
-* Employs OpenAI models for generating context-sensitive responses
-* Utilizes Azure Neural Voices for high-quality text-to-speech synthesis
-* Supports a variety of output formats, voices, and speaking styles
-* Enables real-time monitoring of the chatbot's responses
-* Features asynchronous speech-to-text microphone input
-* Provides an abstract base class for crafting frontends for the BanterBot application
-* Includes a tkinter-based frontend implementation
+* Utilizes OpenAI models to generate context-aware responses
+* Leverages Azure Neural Voices for premium text-to-speech synthesis
+* Offers a wide range of output formats, voices, and speaking styles
+* Allows real-time monitoring of the chatbot's responses
+* Supports asynchronous speech-to-text microphone input
+* Includes an abstract base class for creating custom frontends for the BanterBot application
+* Features a tkinter-based frontend implementation
+* Automatically selects an appropriate emotion or tone based on the conversation context
 
 ## Requirements
 
 Three environment variables are required for full functionality:
 
 * `OPENAI_API_KEY`: A valid OpenAI API key
 * `AZURE_SPEECH_KEY`: A valid Azure Cognitive Services Speech API key for text-to-speech and speech-to-text functionality
@@ -67,55 +68,48 @@
 
 ## Usage
 
 ### Launch with Command Line
 
 Start BanterBot by running the `banterbot` command in your terminal.
 
-Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+- Add the `-g` flag to enable GPT-4 for enhanced conversation quality. Please note that GPT-4 API access is required, and using GPT-4 is more costly and slower than the default GPT-3.5-Turbo.
 
-Add the `-s` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-s "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."`).
+- Use the `-p` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-p "You are Grendel the Quiz Troll, a charismatic troll who loves hosting quiz shows."`).
 
-Add the `-m` flag to activate the multiplayer interface.
+- Include the `-m` flag to activate the multiplayer interface.
+
+- Apply the `-e` flag to enable emotional tone evaluation before the bot generates its responses.
+
+- To select a Microsoft Azure Cognitive Services text-to-speech voice, use the `-v` flag followed by one of the available voice options (e.g., `-v jenny`).
+
+- Select a Microsoft Azure Cognitive Services text-to-speech voice style by using the `-s` flag followed by one of the available style options (e.g., `-s friendly`).
 
 ### Launch with a Python script
 
 To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
 
 ```python
-from banterbot import TKInterface, get_voice_by_name, get_model_by_name
+from banterbot import TKSimpleInterface, get_voice_by_name, get_model_by_name
 
 model = get_model_by_name("gpt-3.5-turbo")
-voice = get_voice_by_name("Aria")
+voice = get_voice_by_name("Davis")
 
-style = "chat"
+style = "excited"
 # Optional system prompt to set up a custom character prior to initializing BanterBot.
 system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
 
-# The four arguments `model`, `voice`, `style`, and `system` are optional.
-interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system)
+# The four arguments `model`, `voice`, `style`, `system`, and `tone` are optional.
+# Setting `tone` to True enables voice tones and emotions.
+interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system, tone=True)
 interface.run()
 ```
 
-For multiplayer, you can modify the above code slightly:
-
-```python
-from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name
-
-model = get_model_by_name("gpt-3.5-turbo")
-voice = get_voice_by_name("Aria")
-style = "chat"
-
-# Optional system prompt to set up a custom character prior to initializing BanterBot.
-system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
+For multiplayer, you can swap out TKSimpleInterface in the above code with TKMultiplayerInterface.
 
-# The four arguments `model`, `voice`, `style`, and `system` are optional.
-interface = TKMultiplayerInterface(model=model, voice=voice, style=style, system=system)
-interface.run()
-```
 
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
```

### Comparing `BanterBot-0.0.4/banterbot/__init__.py` & `BanterBot-0.0.5/banterbot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from banterbot.core.openai_manager import OpenAIManager
-from banterbot.core.speech_to_text import SpeechToText
-from banterbot.core.text_to_speech import TextToSpeech
+from banterbot.api_managers.openai_manager import OpenAIManager
+from banterbot.api_managers.speech_to_text import SpeechToText
+from banterbot.api_managers.text_to_speech import TextToSpeech
 from banterbot.data.azure_neural_voices import get_voice_by_name
 from banterbot.data.openai_models import get_model_by_name
 from banterbot.gui.interface import Interface
 from banterbot.gui.tk_multiplayer_interface import TKMultiplayerInterface
 from banterbot.gui.tk_simple_interface import TKSimpleInterface
 from banterbot.utils.nlp import NLP
```

### Comparing `BanterBot-0.0.4/banterbot/core/openai_manager.py` & `BanterBot-0.0.5/banterbot/api_managers/openai_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import time
 from typing import Generator, Iterator, List, Union
 
 import openai
-from banterbot.data.config import RETRY_LIMIT
+
+from banterbot.config import RETRY_LIMIT
 from banterbot.data.enums import EnvVar
 from banterbot.data.openai_models import OpenAIModel
 from banterbot.utils.message import Message
 from banterbot.utils.nlp import NLP
 
 # Set the OpenAI API key
 openai.api_key = os.environ.get(EnvVar.OPENAI_API_KEY.value)
@@ -38,31 +39,33 @@
 
         # Indicates whether the current instance of OpenAIManager is streaming.
         self._streaming = False
 
         # Set the interruption flag to the current time: if interruptions are raised, this will be updated.
         self._interrupt: int = time.perf_counter_ns()
 
-    def prompt(self, messages: List[Message], **kwargs) -> List[str]:
+    def prompt(self, messages: List[Message], split: bool = True, **kwargs) -> Union[List[str], str]:
         """
         Sends messages to the OpenAI ChatCompletion API and retrieves the response as a list of sentences.
 
         Args:
             messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
+            split (bool): Whether the response should be split into sentences.
+
             **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
             and frequency_penalty.
 
         Returns:
-            List[str]: A list of sentences forming the response from the OpenAI API. This can be used to display
-            the generated response to the user or for further processing.
+            Union[List[str], str]: A list of sentences forming the response from the OpenAI API. This can be used to
+            display the generated response to the user or for further processing. If `split` is False, returns a string.
         """
         response = self._request(messages=messages, stream=False, **kwargs)
-        return NLP.segment_sentences(response)
+        return NLP.segment_sentences(response) if split else response
 
     def prompt_stream(self, messages: List[Message], **kwargs) -> Generator[List[str], None, None]:
         """
         Sends messages to the OpenAI API and retrieves the response as a stream of blocks of sentences.
 
         Args:
             messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
@@ -118,15 +121,15 @@
             messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
         Returns:
             int: The total number of tokens in the messages. This is used to ensure that the generated response does not
             exceed the model's maximum token limit.
         """
-        num_tokens = 3
+        num_tokens = 2
 
         for message in messages:
             num_tokens += message.count_tokens(self._model)
 
         return num_tokens
 
     def _request(self, messages: List[Message], stream: bool, **kwargs) -> Union[Iterator, str]:
@@ -145,15 +148,15 @@
         Returns:
             Union[Iterator, str]: The response from the OpenAI API, either as a stream (Iterator) or text (str).
         """
         kwargs["model"] = self._model.name
         kwargs["n"] = 1
         kwargs["stream"] = stream
         kwargs["messages"] = [message() for message in messages]
-        kwargs["max_tokens"] = self._model.max_tokens - self._count_tokens(messages=messages)
+        # kwargs["max_tokens"] = self._model.max_tokens - self._count_tokens(messages=messages)
 
         success = False
         for i in range(RETRY_LIMIT):
             try:
                 response = openai.ChatCompletion.create(**kwargs)
                 success = True
                 break
```

### Comparing `BanterBot-0.0.4/banterbot/core/speech_to_text.py` & `BanterBot-0.0.5/banterbot/api_managers/speech_to_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import threading
 import time
 from typing import Generator, List
 
 import azure.cognitiveservices.speech as speechsdk
+
 from banterbot.data.enums import EnvVar
 from banterbot.utils.speech_to_text_output import SpeechToTextOutput
 from banterbot.utils.word import Word
 
 
 class SpeechToText:
     """
```

### Comparing `BanterBot-0.0.4/banterbot/core/text_to_speech.py` & `BanterBot-0.0.5/banterbot/api_managers/text_to_speech.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import threading
 import time
 from typing import Generator, List, Optional, TypedDict
 
 import azure.cognitiveservices.speech as speechsdk
 from azure.cognitiveservices.speech import SpeechSynthesisOutputFormat
+
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import EnvVar, SpeechProcessingType, WordCategory
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
 from banterbot.utils.word import Word
 
 
 class TimedEvent(TypedDict):
```

### Comparing `BanterBot-0.0.4/banterbot/data/azure_neural_voices.py` & `BanterBot-0.0.5/banterbot/data/azure_neural_voices.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             "unfriendly",
             "whispering",
         ],
     },
 }
 
 # Create instances of AzureNeuralVoice for each voice in the dictionary
-_neural_voices = {name: AzureNeuralVoice(name=name, **voice) for name, voice in _neural_voice_data.items()}
+_neural_voices = {name.lower(): AzureNeuralVoice(name=name, **voice) for name, voice in _neural_voice_data.items()}
 
 
 def get_voice_by_name(name: str) -> AzureNeuralVoice:
     """
     Retrieve an AzureNeuralVoice instance by its name.
 
     Args:
@@ -226,23 +226,23 @@
 
     Returns:
         AzureNeuralVoice: The corresponding AzureNeuralVoice instance.
 
     Raises:
         KeyError: If the specified name is not found in the _neural_voices dictionary.
     """
-    if name not in _neural_voices.keys():
+    if name.lower() not in _neural_voices.keys():
         available_voices = ", ".join(f"`{name}`" for name in _neural_voices.keys())
         error_message = (
             f"BanterBot was unable to load a Microsoft Azure neural voice model with the name `{name}`, available "
             f"voices are: {available_voices}."
         )
         raise KeyError(error_message)
 
-    return _neural_voices[name]
+    return _neural_voices[name.lower()]
 
 
 def get_voices_by_gender(gender: AzureNeuralVoiceGender) -> List[AzureNeuralVoice]:
     """
     Retrieve a list of AzureNeuralVoice instances with the specified gender.
 
     Args:
```

### Comparing `BanterBot-0.0.4/banterbot/data/config.py` & `BanterBot-0.0.5/banterbot/config.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.4/banterbot/data/enums.py` & `BanterBot-0.0.5/banterbot/data/enums.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.4/banterbot/data/openai_models.py` & `BanterBot-0.0.5/banterbot/data/openai_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         """
         self.tokenizer: Encoding = tiktoken.encoding_for_model(self.name)
 
 
 # Define the available OpenAI models
 _openai_models_dict = {
     "gpt-3.5-turbo": {
-        "max_tokens": 4095,
+        "max_tokens": 4097,
         "version": 3,
         "rank": 2,
     },
     "gpt-4": {
         "max_tokens": 8191,
         "version": 4,
         "rank": 1,
```

### Comparing `BanterBot-0.0.4/banterbot/gui/cli.py` & `BanterBot-0.0.5/banterbot/gui/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 
+from banterbot.data.azure_neural_voices import _neural_voices, get_voice_by_name
 from banterbot.data.openai_models import get_model_by_name
 from banterbot.gui.tk_multiplayer_interface import TKMultiplayerInterface
 from banterbot.gui.tk_simple_interface import TKSimpleInterface
 
 
 def run() -> None:
     """
@@ -18,53 +19,101 @@
             "This program initializes a GUI that allows users to interact with a chatbot by entering a name and a "
             "message, and it displays the conversation history in a scrollable text area. Users can send messages by "
             "pressing the `Send` button or the `Enter` key. The chatbot's responses are generated using the specified "
             "OpenAI model and can be played back using the specified Azure Neural Voice. Additionally, users can "
             "toggle speech-to-text input by pressing the `Listen` button."
         ),
         epilog=(
-            "Requires three environment variables for full functionality. "
-            "1) OPENAI_API_KEY: A valid OpenAI API key,\n"
+            "Requires three environment variables for full functionality."
+            "1) OPENAI_API_KEY: A valid OpenAI API key,"
             "2) AZURE_SPEECH_KEY: A valid Azure Cognitive Services Speech API key for text-to-speech and "
-            "speech-to-text functionality,\n"
+            "speech-to-text functionality,"
             "3) AZURE_SPEECH_REGION: The region associated with your Azure Cognitive Services Speech API key."
         ),
     )
 
     parser.add_argument(
-        "-s",
-        "--system",
+        "-p",
+        "--prompt",
         action="store",
         type=str,
-        dest="system",
-        help="Adds a system message to the beginning of the conversation; can help to set the scene.",
+        dest="prompt",
+        help="Adds a system prompt to the beginning of the conversation; can help to set the scene.",
     )
 
     parser.add_argument(
         "-g",
         "--gpt4",
         action="store_true",
         dest="gpt4",
         help="Enable GPT-4; only works if you have GPT-4 API access.",
     )
 
     parser.add_argument(
         "-m",
         "--multiplayer",
         action="store_true",
-        dest="mp",
+        dest="multiplayer",
         help="Enables the pre-release multiplayer interface; multiplayer is not fully implemented and may be buggy.",
     )
 
+    parser.add_argument(
+        "-e",
+        "--emotion",
+        action="store_true",
+        dest="tone",
+        help="Enables emotional tone evaluation prior to the bot's responses.",
+    )
+
+    voices = ", ".join(f"`{voice}`" for voice in _neural_voices.keys())
+    parser.add_argument(
+        "-v",
+        "--voice",
+        action="store",
+        type=str,
+        default="Aria",
+        dest="voice",
+        help=f"Select a Microsoft Azure Cognitive Services text-to-speech voice. Options are: {voices}",
+    )
+
+    universal_styles = [
+        "angry",
+        "cheerful",
+        "excited",
+        "friendly",
+        "hopeful",
+        "sad",
+        "shouting",
+        "terrified",
+        "unfriendly",
+        "whispering",
+    ]
+    universal_styles = ", ".join(f"`{style}`" for style in universal_styles)
+    parser.add_argument(
+        "-s",
+        "--style",
+        action="store",
+        type=str,
+        default="friendly",
+        dest="style",
+        help=(
+            "Select a Microsoft Azure Cognitive Services text-to-speech voice style. Universally available styles "
+            f"across all available voices are: {universal_styles}. Some voices may have more available styles, see "
+            "`/banterbot/data/azure_neural_voices.py` for more information."
+        ),
+    )
     args = parser.parse_args()
 
     kwargs = {
         "model": get_model_by_name("gpt-4") if args.gpt4 else get_model_by_name("gpt-3.5-turbo"),
-        "system": args.system,
+        "voice": get_voice_by_name(args.voice),
+        "style": args.style,
+        "system": args.prompt,
+        "tone": args.tone,
     }
 
-    if args.mp:
+    if args.multiplayer:
         interface = TKMultiplayerInterface(**kwargs)
     else:
         interface = TKSimpleInterface(**kwargs)
 
     interface.run()
```

### Comparing `BanterBot-0.0.4/banterbot/gui/interface.py` & `BanterBot-0.0.5/banterbot/gui/interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 import datetime
 import logging
 import threading
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
-from banterbot.core.openai_manager import OpenAIManager
-from banterbot.core.speech_to_text import SpeechToText
-from banterbot.core.text_to_speech import TextToSpeech
+from banterbot.api_managers.openai_manager import OpenAIManager
+from banterbot.api_managers.speech_to_text import SpeechToText
+from banterbot.api_managers.text_to_speech import TextToSpeech
+from banterbot.config import chat_logs, logging_level
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
-from banterbot.data.config import chat_logs, logging_level
-from banterbot.data.openai_models import OpenAIModel
+from banterbot.data.openai_models import OpenAIModel, get_model_by_name
+from banterbot.data.prompts import ToneSelection
+from banterbot.openai_extensions.option_selector import OptionSelector
 from banterbot.utils.message import Message
 from banterbot.utils.thread_queue import ThreadQueue
 
 logging.basicConfig(format="Interface %(asctime)s - %(message)s", level=logging_level)
 
 
 class Interface(ABC):
     """
     Interface is an abstract base class for creating frontends for the BanterBot application. It provides a high-level
     interface for managing conversation with the bot, including sending messages, receiving responses, and updating the
     conversation area. The interface supports both text and speech-to-text input for user messages.
     """
 
-    def __init__(self, model: OpenAIModel, voice: AzureNeuralVoice, style: str, system: Optional[str] = None) -> None:
+    def __init__(
+        self,
+        model: OpenAIModel,
+        voice: AzureNeuralVoice,
+        style: str,
+        system: Optional[str] = None,
+        tone: bool = False,
+    ) -> None:
         """
         Initialize the BanterBotInterface with the given model, voice, and style.
 
         Args:
             model (OpenAIModel): The OpenAI model to use for generating responses.
             voice (AzureNeuralVoice): The voice to use for text-to-speech synthesis.
             style (str): The speaking style to use for text-to-speech synthesis.
             system (Optional[str]): An initialization prompt that can be used to set the scene.
+            tone (bool): Whether an OptionSelector should evaluate emotional responses between prompts.
         """
         # Initialize OpenAI ChatCompletion, Azure Speech-to-Text, and Azure text-to-speech components
         self._openai_manager = OpenAIManager(model=model)
         self._speech_to_text = SpeechToText()
         self._text_to_speech = TextToSpeech()
 
         # Initialize message handling and conversation attributes
@@ -48,14 +58,23 @@
         self._thread_queue = ThreadQueue()
 
         # Initialize model, voice, and style attributes
         self._model = model
         self._voice = voice
         self._style = style
 
+        # Initialize the OptionSelector for tone selection
+        self._tone = tone
+        self._tone_selector = OptionSelector(
+            model=get_model_by_name("gpt-3.5-turbo"),
+            options=self._voice.styles,
+            system=ToneSelection.SYSTEM.value,
+            prompt=ToneSelection.PROMPT.value.format(self._style),
+        )
+
         # Initialize the system message, if provided
         self._system = system
         if self._system is not None:
             message_instance = Message(role="system", content=system)
             self._messages.append(message_instance)
 
         # Initialize the subclass GUI
@@ -171,21 +190,31 @@
         """
         Get a response from the bot and update the conversation area with the response. This method handles generating
         the bot's response using the OpenAIManager and updating the conversation area with the response text using
         text-to-speech synthesis.
         """
         prefixed = False
         content = []
-        for block in self._openai_manager.prompt_stream(messages=self._messages):
+        style = self._style
+
+        # Prepare the generator for asynchronous yielding of sentence blocks
+        response = self._openai_manager.prompt_stream(messages=self._messages)
+
+        # If the tone is to be evaluated, evaluate it once before yielding the blocks
+        if self._tone:
+            style = self._get_next_tone()
+
+        for block in response:
+
             if not prefixed:
                 self.update_conversation_area("Assistant: ")
                 prefixed = True
 
             sentences = " ".join(block)
-            for word in self._text_to_speech.speak(sentences, voice=self._voice, style=self._style):
+            for word in self._text_to_speech.speak(sentences, voice=self._voice, style=style):
                 self.update_conversation_area(word.word)
                 content.append(word.word)
 
             self.update_conversation_area(" ")
             content.append(" ")
 
         content = "".join(content)
@@ -269,7 +298,18 @@
 
         Args:
             word (str): The word to be added to the conversation area.
         """
         with self._log_lock:
             with open(self._log_path, "a+") as fs:
                 fs.write(word)
+
+    def _get_next_tone(self):
+        """
+        Sends the message history as an input to the tone selector to semi-randomly select a fitting tone for the
+        assistant's next response. If the tone selection fails, returns the default style.
+
+        Returns:
+            str: A voice tone compatible with the active AzureNeuralVoice instance.
+        """
+        tone = self._tone_selector.select(self._messages)
+        return tone if tone is not None else self._style
```

### Comparing `BanterBot-0.0.4/banterbot/gui/tk_multiplayer_interface.py` & `BanterBot-0.0.5/banterbot/gui/tk_multiplayer_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,27 +19,29 @@
     """
 
     def __init__(
         self,
         model: OpenAIModel = get_model_by_name("gpt-3.5-turbo"),
         voice: AzureNeuralVoice = get_voice_by_name("Aria"),
         style: str = "chat",
+        tone: bool = False,
         system: Optional[str] = None,
     ) -> None:
         """
         Initialize the TKMultiplayerInterface class, which inherits from both tkinter.Tk and Interface.
 
         Args:
             model (OpenAIModel, optional): The OpenAI model to be used for generating responses.
             voice (AzureNeuralVoice, optional): The Azure Neural Voice to be used for text-to-speech.
             style (str, optional): The style of the conversation (e.g., "cheerful", "sad", "chat").
             system (Optional[str]): An initialization prompt that can be used to set the scene.
+            tone (bool): Whether an OptionSelector should evaluate emotional responses between prompts.
         """
         tk.Tk.__init__(self)
-        Interface.__init__(self, model=model, voice=voice, style=style, system=system)
+        Interface.__init__(self, model=model, voice=voice, style=style, system=system, tone=tone)
 
         # Bind the `_quit` method to program exit, in order to guarantee the stopping of all running threads.
         self.protocol("WM_DELETE_WINDOW", self._quit)
 
     def update_conversation_area(self, word: str) -> None:
         super().update_conversation_area(word)
         self.conversation_area["state"] = tk.NORMAL
```

### Comparing `BanterBot-0.0.4/banterbot/gui/tk_simple_interface.py` & `BanterBot-0.0.5/banterbot/gui/tk_simple_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 
     def __init__(
         self,
         model: OpenAIModel = get_model_by_name("gpt-3.5-turbo"),
         voice: AzureNeuralVoice = get_voice_by_name("Aria"),
         style: str = "chat",
         system: Optional[str] = None,
+        tone: bool = False,
     ) -> None:
         """
         Initialize the TKSimpleInterface class, which inherits from both tkinter.Tk and Interface.
 
         Args:
             model (OpenAIModel, optional): The OpenAI model to be used for generating responses.
             voice (AzureNeuralVoice, optional): The Azure Neural Voice to be used for text-to-speech.
             style (str, optional): The style of the conversation (e.g., "cheerful", "sad", "chat").
             system (Optional[str]): An initialization prompt that can be used to set the scene.
+            tone (bool): Whether an OptionSelector should evaluate emotional responses between prompts.
         """
         tk.Tk.__init__(self)
-        Interface.__init__(self, model=model, voice=voice, style=style, system=system)
+        Interface.__init__(self, model=model, voice=voice, style=style, system=system, tone=tone)
 
         # Bind the `_quit` method to program exit, in order to guarantee the stopping of all running threads.
         self.protocol("WM_DELETE_WINDOW", self._quit)
 
     def update_conversation_area(self, word: str) -> None:
         """
         Update the conversation area with the given word.
```

### Comparing `BanterBot-0.0.4/banterbot/utils/message.py` & `BanterBot-0.0.5/banterbot/utils/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         num_tokens = 4
         # Count the number of tokens in the role string
         num_tokens += len(model.tokenizer.encode(self.role))
         # Count the number of tokens in the content string
         num_tokens += len(model.tokenizer.encode(self.content))
         # Count the number of tokens in the name string, if a name is provided
         if self.name is not None:
-            num_tokens += len(model.tokenizer.encode(self.name))
+            num_tokens += len(model.tokenizer.encode(self.name)) - 1
 
         return num_tokens
 
     def __call__(self) -> Dict[str, str]:
         """
         Creates and returns a dictionary that is compatible with the OpenAI ChatCompletion API.
```

### Comparing `BanterBot-0.0.4/banterbot/utils/nlp.py` & `BanterBot-0.0.5/banterbot/utils/nlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Tuple
 
 import spacy
+
 from banterbot.data.enums import SpaCyLangModel
 
 
 class NLP:
     """
     A comprehensive toolkit that provides a set of Natural Language Processing utilities. It leverages the capabilities
     of the SpaCy package. The toolkit is designed to automatically download the necessary models if they are not
```

### Comparing `BanterBot-0.0.4/banterbot/utils/speech_to_text_output.py` & `BanterBot-0.0.5/banterbot/utils/speech_to_text_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import json
 from typing import Iterator, List, TypedDict
 
 import azure.cognitiveservices.speech as speechsdk
+
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import SpeechProcessingType, WordCategory
 from banterbot.utils.nlp import NLP
 from banterbot.utils.word import Word
 
 
 class WordJSON(TypedDict):
```

### Comparing `BanterBot-0.0.4/banterbot/utils/text_to_speech_output.py` & `BanterBot-0.0.5/banterbot/utils/text_to_speech_output.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.4/banterbot/utils/thread_queue.py` & `BanterBot-0.0.5/banterbot/utils/thread_queue.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.4/banterbot/utils/word.py` & `BanterBot-0.0.5/banterbot/utils/word.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 from dataclasses import dataclass
 from typing import Optional
 
 import azure.cognitiveservices.speech as speechsdk
+
 from banterbot.data.enums import SpeechProcessingType, WordCategory
 
 
 @dataclass(frozen=True)
 class Word:
     """
     This class encapsulates a word in the output of a text-to-speech synthesis or input from a speech-to-text
```

### Comparing `BanterBot-0.0.4/setup.py` & `BanterBot-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest
 
 from setuptools import find_packages, setup
 
-dependencies = ["openai", "tiktoken", "requests", "azure-cognitiveservices-speech", "spacy"]
+dependencies = ["openai", "tiktoken", "requests", "azure-cognitiveservices-speech", "spacy", "numpy"]
 
 url = "https://github.com/GabrielSCabrera/BanterBot"
 
 description = (
     "BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech "
-    "interactions. Features real-time monitoring and Tkinter frontend."
+    "interactions with emotional tone selection. Features real-time monitoring and Tkinter frontend."
 )
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 # For running tests: python -m unittest discover -s tests
 # For building: python setup.py sdist bdist_wheel
@@ -21,15 +21,15 @@
 
 def run_tests():
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover("tests", pattern="test_*.py")
     return test_suite
 
 
-version = "0.0.4"
+version = "0.0.5"
 setup(
     name="BanterBot",
     packages=find_packages(),
     test_suite="setup.run_tests",
     version=version,
     description=description,
     long_description=long_description,
```

### Comparing `BanterBot-0.0.4/tests/core/test_openai_manager.py` & `BanterBot-0.0.5/tests/core/test_openai_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import os
 import unittest
 from dataclasses import dataclass
 from unittest.mock import patch
 
 import openai
+
 from banterbot.core.openai_manager import OpenAIManager
 from banterbot.data.openai_models import OpenAIModel
 from banterbot.utils.message import Message
 from banterbot.utils.nlp import NLP
 
 
 @dataclass
```

### Comparing `BanterBot-0.0.4/tests/core/test_text_to_speech.py` & `BanterBot-0.0.5/tests/core/test_text_to_speech.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 from unittest.mock import MagicMock, patch
 
 from azure.cognitiveservices.speech import SpeechSynthesisBoundaryType, SpeechSynthesisOutputFormat, SpeechSynthesizer
+
 from banterbot.core.text_to_speech import TextToSpeech
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
 
 
 class TestTextToSpeech(unittest.TestCase):
     def setUp(self):
         self.tts = TextToSpeech()
```

### Comparing `BanterBot-0.0.4/tests/utils/test_message.py` & `BanterBot-0.0.5/tests/utils/test_message.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.4/tests/utils/test_nlp.py` & `BanterBot-0.0.5/tests/utils/test_nlp.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.4/tests/utils/test_text_to_speech_output.py` & `BanterBot-0.0.5/tests/utils/test_text_to_speech_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 appending new words, stopping the output process, and streaming words from the output.
 """
 import datetime
 import unittest
 from typing import List
 
 import azure.cognitiveservices.speech as speechsdk
+
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
 from banterbot.utils.text_to_speech_word import TextToSpeechWord
 
 
 class TextToSpeechOutputTestCase(unittest.TestCase):
     def setUp(self):
         self.output = TextToSpeechOutput("Hello, world!")
```

### Comparing `BanterBot-0.0.4/tests/utils/test_text_to_speech_word.py` & `BanterBot-0.0.5/tests/utils/test_text_to_speech_word.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 as a string representation.
 """
 import datetime
 import unittest
 from dataclasses import dataclass
 
 import azure.cognitiveservices.speech as speechsdk
+
 from banterbot.utils.text_to_speech_word import TextToSpeechWord
 
 
 @dataclass(frozen=True)
 class MockSpeechSynthesisBoundaryType:
     WORD = "word"
     PUNCTUATION = "punctuation"
```

### Comparing `BanterBot-0.0.4/tests/utils/test_thread_queue.py` & `BanterBot-0.0.5/tests/utils/test_thread_queue.py`

 * *Files identical despite different names*

