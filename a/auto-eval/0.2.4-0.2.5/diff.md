# Comparing `tmp/auto-eval-0.2.4.tar.gz` & `tmp/auto-eval-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.4.tar", last modified: Tue Jun  6 12:44:37 2023, max compression
+gzip compressed data, was "auto-eval-0.2.5.tar", last modified: Thu Jun  8 12:50:27 2023, max compression
```

## Comparing `auto-eval-0.2.4.tar` & `auto-eval-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.387310 auto-eval-0.2.4/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.4/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16597 2023-06-06 12:44:37.387047 auto-eval-0.2.4/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16171 2023-06-06 12:43:19.000000 auto-eval-0.2.4/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.384640 auto-eval-0.2.4/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16597 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-06 12:44:37.000000 auto-eval-0.2.4/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.385190 auto-eval-0.2.4/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.4/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.4/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.385473 auto-eval-0.2.4/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.4/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.4/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.386346 auto-eval-0.2.4/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.4/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.4/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2026 2023-06-06 12:13:28.000000 auto-eval-0.2.4/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-06 12:44:37.386747 auto-eval-0.2.4/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.4/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3917 2023-06-06 10:59:39.000000 auto-eval-0.2.4/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-06 12:44:37.387380 auto-eval-0.2.4/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-06 12:44:21.000000 auto-eval-0.2.4/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-08 12:50:27.376560 auto-eval-0.2.5/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.5/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-08 12:50:27.376331 auto-eval-0.2.5/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.2.5/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-08 12:50:27.373673 auto-eval-0.2.5/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-08 12:50:27.000000 auto-eval-0.2.5/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-08 12:50:27.000000 auto-eval-0.2.5/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-08 12:50:27.000000 auto-eval-0.2.5/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-08 12:50:27.000000 auto-eval-0.2.5/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-08 12:50:27.000000 auto-eval-0.2.5/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-08 12:50:27.000000 auto-eval-0.2.5/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-08 12:50:27.374081 auto-eval-0.2.5/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.5/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.5/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-08 12:50:27.374506 auto-eval-0.2.5/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.5/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.5/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-08 12:50:27.375284 auto-eval-0.2.5/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.5/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3090 2023-05-19 09:15:03.000000 auto-eval-0.2.5/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2026 2023-06-06 12:13:28.000000 auto-eval-0.2.5/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-08 12:50:27.375890 auto-eval-0.2.5/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.5/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3919 2023-06-08 12:49:44.000000 auto-eval-0.2.5/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-08 12:50:27.376614 auto-eval-0.2.5/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-08 12:50:19.000000 auto-eval-0.2.5/setup.py
```

### Comparing `auto-eval-0.2.4/LICENSE` & `auto-eval-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.4/PKG-INFO` & `auto-eval-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,17 @@
-Metadata-Version: 2.1
-Name: auto-eval
-Version: 0.2.4
-Summary: Using only one line of commmands to evaluate multiple models
-Home-page: https://github.com/muximus3/Auto-Eval
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Auto-Eval
+**[中文文档](README_ZH.md)**
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
-The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
-
-To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
+To further personalize the evaluation prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
 ## How does it work?
 
-Assuming we have a test set, we can predict it with any model and output them to a file in JSON, CSV, or other format. The format of the file is as follows:
+Assuming we have a test set, we can use any model to make predictions and save them in a file format such as JSON, CSV, or other formats. The structure of the output file is as follows:
 
 | prompt | output | model | category |
 | --- | --- | --- | --- |
 | What is 1+1? | 3 | model_a | Arithmetic |
 | What is the capital of France? | Paris | model_a | General Knowledge |
 | What is 1+1? | 2 | model_b | Arithmetic |
 | What is the capital of France? | Paris | model_b | General Knowledge |
@@ -182,15 +169,16 @@
 
 - To view more detailed arguments, Please use the command `auto-eval file -h` after installing this repository or refer to the full documentation below.<br>
 
 - The headers(column names) of the file can be one of the following types: 
     - `{"instruction", "input", "output"}`
     -  `{"prompt", "output"}`
     -  `{"question", "answer"}`
-    -  `{"question", "output"}` <br>
+    -  `{"question", "output"}` 
+    - `{"question", "target"}`<br>
 
     The "question," "prompt," and "instruction" + "input" refer to the original inquiry, such as "Please calculate carefully: 1+1=?" or "Explain landing on the moon like I am five." The  "answer" and "output" represent the predicted answer of the model for a given question. If the format is in an {"instruction", "input"} form, we will concatenate both elements to create a complete question. <br>
 
 
 To get an idea of what eval input file looks like.
 here is an example of test data in JSON format with model's pseudo prediction.<br>
 ```json
@@ -290,8 +278,8 @@
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 `--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [x] Supporting prompts evaluation by output the accuracy of different prompts. 
-- [ ] Configuring a default test set for prompt evaluation.
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.4/README.md` & `auto-eval-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,29 @@
+Metadata-Version: 2.1
+Name: auto-eval
+Version: 0.2.5
+Summary: Using only one line of commmands to evaluate multiple models
+Home-page: https://github.com/muximus3/Auto-Eval
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Auto-Eval
+**[中文文档](README_ZH.md)**
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
-The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
-
-To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
+To further personalize the evaluation prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
 ## How does it work?
 
-Assuming we have a test set, we can predict it with any model and output them to a file in JSON, CSV, or other format. The format of the file is as follows:
+Assuming we have a test set, we can use any model to make predictions and save them in a file format such as JSON, CSV, or other formats. The structure of the output file is as follows:
 
 | prompt | output | model | category |
 | --- | --- | --- | --- |
 | What is 1+1? | 3 | model_a | Arithmetic |
 | What is the capital of France? | Paris | model_a | General Knowledge |
 | What is 1+1? | 2 | model_b | Arithmetic |
 | What is the capital of France? | Paris | model_b | General Knowledge |
@@ -170,15 +181,16 @@
 
 - To view more detailed arguments, Please use the command `auto-eval file -h` after installing this repository or refer to the full documentation below.<br>
 
 - The headers(column names) of the file can be one of the following types: 
     - `{"instruction", "input", "output"}`
     -  `{"prompt", "output"}`
     -  `{"question", "answer"}`
-    -  `{"question", "output"}` <br>
+    -  `{"question", "output"}` 
+    - `{"question", "target"}`<br>
 
     The "question," "prompt," and "instruction" + "input" refer to the original inquiry, such as "Please calculate carefully: 1+1=?" or "Explain landing on the moon like I am five." The  "answer" and "output" represent the predicted answer of the model for a given question. If the format is in an {"instruction", "input"} form, we will concatenate both elements to create a complete question. <br>
 
 
 To get an idea of what eval input file looks like.
 here is an example of test data in JSON format with model's pseudo prediction.<br>
 ```json
@@ -278,8 +290,8 @@
 `--retry`:  ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to retry once for all failed requests. Failed requests may be due to reasons such as exceeding API request frequency, incorrect answer format parsing, or network failure.
 
 `--score_by`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Used to determine the groups for the groupby `pandas.groupby(by=args.score_by)` to get the summary scores of certain groups.
 
 ## ToDo
 - [ ] Conbining multiple GPT-like models for prediction: routing or simply averaging.
 - [x] Supporting prompts evaluation by output the accuracy of different prompts. 
-- [ ] Configuring a default test set for prompt evaluation.
+- [ ] Configuring a default test set for prompt evaluation.
```

### Comparing `auto-eval-0.2.4/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.2.5/auto_eval.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.4
+Version: 0.2.5
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Auto-Eval
+**[中文文档](README_ZH.md)**
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
-The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
-
-To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
+To further personalize the evaluation prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
 ## How does it work?
 
-Assuming we have a test set, we can predict it with any model and output them to a file in JSON, CSV, or other format. The format of the file is as follows:
+Assuming we have a test set, we can use any model to make predictions and save them in a file format such as JSON, CSV, or other formats. The structure of the output file is as follows:
 
 | prompt | output | model | category |
 | --- | --- | --- | --- |
 | What is 1+1? | 3 | model_a | Arithmetic |
 | What is the capital of France? | Paris | model_a | General Knowledge |
 | What is 1+1? | 2 | model_b | Arithmetic |
 | What is the capital of France? | Paris | model_b | General Knowledge |
@@ -182,15 +181,16 @@
 
 - To view more detailed arguments, Please use the command `auto-eval file -h` after installing this repository or refer to the full documentation below.<br>
 
 - The headers(column names) of the file can be one of the following types: 
     - `{"instruction", "input", "output"}`
     -  `{"prompt", "output"}`
     -  `{"question", "answer"}`
-    -  `{"question", "output"}` <br>
+    -  `{"question", "output"}` 
+    - `{"question", "target"}`<br>
 
     The "question," "prompt," and "instruction" + "input" refer to the original inquiry, such as "Please calculate carefully: 1+1=?" or "Explain landing on the moon like I am five." The  "answer" and "output" represent the predicted answer of the model for a given question. If the format is in an {"instruction", "input"} form, we will concatenate both elements to create a complete question. <br>
 
 
 To get an idea of what eval input file looks like.
 here is an example of test data in JSON format with model's pseudo prediction.<br>
 ```json
```

### Comparing `auto-eval-0.2.4/eval/auto_llms_eval.py` & `auto-eval-0.2.5/eval/auto_llms_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.4/eval/commands/auto_eval.py` & `auto-eval-0.2.5/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.4/eval/prompt_template/prompter.py` & `auto-eval-0.2.5/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.4/eval/prompt_template/prompts.py` & `auto-eval-0.2.5/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.4/eval/utils/data_utils.py` & `auto-eval-0.2.5/eval/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 from typing import Union, List
 
 
 def df_reader(data_path, header: Union[int, None] = 0, usecols: Union[List[Union[str, int]], None] = None ,sep='\t', sheet_name=0) -> pd.DataFrame:
     if data_path.endswith('json'):
         df_data = pd.read_json(data_path)
-    if data_path.endswith('jsonl'):
+    elif data_path.endswith('jsonl'):
         df_data = pd.read_json(data_path, lines=True)
     elif data_path.endswith('xlsx'):
         df_data = pd.read_excel(data_path, header=header, usecols=usecols, sheet_name=sheet_name)
     elif data_path.endswith('.pkl'):
         df_data = pd.read_pickle(data_path)
     elif data_path.endswith('csv'):
         df_data = pd.read_csv(data_path, header=header, usecols=usecols, sep=sep)
```

### Comparing `auto-eval-0.2.4/setup.py` & `auto-eval-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

