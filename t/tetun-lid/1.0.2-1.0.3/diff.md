# Comparing `tmp/tetun_lid-1.0.2.tar.gz` & `tmp/tetun_lid-1.0.3.tar.gz`

## Comparing `tetun_lid-1.0.2.tar` & `tetun_lid-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/.DS_Store
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/Pipfile
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/Pipfile.lock
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/tetunlid/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/tetunlid/lid.py
--rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/tetunlid/model/tetun_lid_model.pkl
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/LICENSE
--rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/README.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/.DS_Store
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/Pipfile
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/Pipfile.lock
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/tetunlid/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/tetunlid/lid.py
+-rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/tetunlid/model/tetun_lid_model.pkl
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/LICENSE
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 tetun_lid-1.0.3/PKG-INFO
```

### Comparing `tetun_lid-1.0.2/.DS_Store` & `tetun_lid-1.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.2/Pipfile.lock` & `tetun_lid-1.0.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.2/tetunlid/lid.py` & `tetun_lid-1.0.3/tetunlid/lid.py`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.2/tetunlid/model/tetun_lid_model.pkl` & `tetun_lid-1.0.3/tetunlid/model/tetun_lid_model.pkl`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.2/LICENSE` & `tetun_lid-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.2/README.md` & `tetun_lid-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### Tetun LID
 Tetun Language Identification (Tetun LID) model is a machine learning model that automatically identifies the language of a given text. It was specifically designed to recognize four languages commonly spoken in Timor-Leste: Tetun, Portuguese, English, and Indonesian.
 
 
-Using a combination of cutting-edge algorithms and sophisticated linguistic features, Tetun LID was trained on a large corpus of text data to accurately recognize the characteristic of each language and the linguistic patterns. Its ability to accurately identify multiple languages makes it a valuable tool for anyone working with multilingual text data in Timor-Leste in the natural language processing (NLP) and information retrieval (IR) areas.
+Using a combination of cutting-edge algorithms and sophisticated linguistic features, Tetun LID was trained on a large corpus of textual data to accurately recognize the characteristic of each language and the linguistic patterns. Its ability to accurately identify multiple languages makes it a valuable tool for anyone working with multilingual text data in Timor-Leste in the natural language processing (NLP) and information retrieval (IR) fields.
 
 ### Installation
 
 To install Tetun LID, run the following command in your console:
 
 ```
 pip install tetun-lid
@@ -109,15 +109,15 @@
 ```
 Ha'u ema baibain (Tetun)
 I am quite busy (English)
 Kamu malas sekali (Indonesian)
 Vou sair daqui (Portuguese)
 ```
 
-If you want to see the details of each input, you can use the same function as illustrated above. Here you go:
+If you want to print the details of each input, you can use the same function as illustrated above. Here you go:
 
 ```python
 
 from tetunlid import lid
 
 input_texts = ["Ha'u ema baibain", "I am quite busy",
                "Kamu malas sekali", "Vou sair daqui"]
@@ -181,15 +181,15 @@
 
 The output will be:
 
 ```
 ["Ha'u ema baibain"]
 ```
 
-5. You can also use Tetun LID to predict a text from a file containing various languages or texts extracted from web pages. Here is an example:
+5. You can also use Tetun LID to predict a text from a file containing various languages or texts extracted from the web. Here is an example:
 
 ```python
 from pathlib import Path
 from tetunlid import lid
 
 
 file_path = Path("myfile/example.txt")
@@ -202,13 +202,14 @@
 
 output = [(content, lid.predict_language(content)) for content in contents]
 print(output)
 ```
 
 There are a few more ways to read file contents that you can use to achieve the same output.
 
+For the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-lid) for this project.
 
 ### Additional notes
 
 1. Please follow the instruction carefully and try to understand how it works. All the dependencies need to be installed properly.
 2. If you encountered an `AttributeError: 'list' object has no attribute 'predict_proba'`, you might have some issues while installing the package. Please send me an email, and I will guide you on how to handle the error.
 3. Please make sure that you use the latest version of Tetun LID. To get the latest version, run this command in your console: `pip install --upgrade tetun-lid`.
```

### Comparing `tetun_lid-1.0.2/PKG-INFO` & `tetun_lid-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: tetun_lid
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tetun Language Identification Model
+Project-URL: repository, https://github.com/borulilitimornews/tetun-lid
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ### Tetun LID
 Tetun Language Identification (Tetun LID) model is a machine learning model that automatically identifies the language of a given text. It was specifically designed to recognize four languages commonly spoken in Timor-Leste: Tetun, Portuguese, English, and Indonesian.
 
 
-Using a combination of cutting-edge algorithms and sophisticated linguistic features, Tetun LID was trained on a large corpus of text data to accurately recognize the characteristic of each language and the linguistic patterns. Its ability to accurately identify multiple languages makes it a valuable tool for anyone working with multilingual text data in Timor-Leste in the natural language processing (NLP) and information retrieval (IR) areas.
+Using a combination of cutting-edge algorithms and sophisticated linguistic features, Tetun LID was trained on a large corpus of textual data to accurately recognize the characteristic of each language and the linguistic patterns. Its ability to accurately identify multiple languages makes it a valuable tool for anyone working with multilingual text data in Timor-Leste in the natural language processing (NLP) and information retrieval (IR) fields.
 
 ### Installation
 
 To install Tetun LID, run the following command in your console:
 
 ```
 pip install tetun-lid
@@ -121,15 +122,15 @@
 ```
 Ha'u ema baibain (Tetun)
 I am quite busy (English)
 Kamu malas sekali (Indonesian)
 Vou sair daqui (Portuguese)
 ```
 
-If you want to see the details of each input, you can use the same function as illustrated above. Here you go:
+If you want to print the details of each input, you can use the same function as illustrated above. Here you go:
 
 ```python
 
 from tetunlid import lid
 
 input_texts = ["Ha'u ema baibain", "I am quite busy",
                "Kamu malas sekali", "Vou sair daqui"]
@@ -193,15 +194,15 @@
 
 The output will be:
 
 ```
 ["Ha'u ema baibain"]
 ```
 
-5. You can also use Tetun LID to predict a text from a file containing various languages or texts extracted from web pages. Here is an example:
+5. You can also use Tetun LID to predict a text from a file containing various languages or texts extracted from the web. Here is an example:
 
 ```python
 from pathlib import Path
 from tetunlid import lid
 
 
 file_path = Path("myfile/example.txt")
@@ -214,13 +215,14 @@
 
 output = [(content, lid.predict_language(content)) for content in contents]
 print(output)
 ```
 
 There are a few more ways to read file contents that you can use to achieve the same output.
 
+For the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-lid) for this project.
 
 ### Additional notes
 
 1. Please follow the instruction carefully and try to understand how it works. All the dependencies need to be installed properly.
 2. If you encountered an `AttributeError: 'list' object has no attribute 'predict_proba'`, you might have some issues while installing the package. Please send me an email, and I will guide you on how to handle the error.
 3. Please make sure that you use the latest version of Tetun LID. To get the latest version, run this command in your console: `pip install --upgrade tetun-lid`.
```

