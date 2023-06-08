# Comparing `tmp/faKy-2.0.1.tar.gz` & `tmp/faKy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-2.0.1.tar", last modified: Tue Jun  6 14:11:05 2023, max compression
+gzip compressed data, was "faKy-2.1.0.tar", last modified: Thu Jun  8 11:37:34 2023, max compression
```

## Comparing `faKy-2.0.1.tar` & `faKy-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.711001 faKy-2.0.1/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:11:05.710632 faKy-2.0.1/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4273 2023-06-06 13:52:24.000000 faKy-2.0.1/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.701789 faKy-2.0.1/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-2.0.1/faKy/__init__.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.707563 faKy-2.0.1/faKy/en_core_web_md-2.3.1/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/MANIFEST.in
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/PKG-INFO
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.709637 faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/setup.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8158 2023-06-06 14:10:42.000000 faKy-2.0.1/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.703735 faKy-2.0.1/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 14:11:05.711122 faKy-2.0.1/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      759 2023-06-06 14:11:00.000000 faKy-2.0.1/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-08 11:37:34.250161 faKy-2.1.0/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     5647 2023-06-08 11:37:34.249908 faKy-2.1.0/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     5291 2023-06-08 10:36:03.000000 faKy-2.1.0/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-08 11:37:34.242549 faKy-2.1.0/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      860 2023-06-08 11:14:56.000000 faKy-2.1.0/faKy/__init__.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-08 11:37:34.247796 faKy-2.1.0/faKy/en_core_web_md-2.3.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/MANIFEST.in
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/PKG-INFO
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-08 11:37:34.248902 faKy-2.1.0/faKy/en_core_web_md-2.3.1/en_core_web_md/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-08 11:19:04.000000 faKy-2.1.0/faKy/en_core_web_md-2.3.1/setup.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8291 2023-06-08 11:19:54.000000 faKy-2.1.0/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-08 11:37:34.244753 faKy-2.1.0/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     5647 2023-06-08 11:37:34.000000 faKy-2.1.0/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-08 11:37:34.000000 faKy-2.1.0/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-08 11:37:34.000000 faKy-2.1.0/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      109 2023-06-08 11:37:34.000000 faKy-2.1.0/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-08 11:37:34.000000 faKy-2.1.0/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-08 11:37:34.250280 faKy-2.1.0/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      878 2023-06-08 11:35:51.000000 faKy-2.1.0/setup.py
```

### Comparing `faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json` & `faKy-2.1.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-2.0.1/faKy/en_core_web_md-2.3.1/meta.json` & `faKy-2.1.0/faKy/en_core_web_md-2.3.1/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-2.0.1/faKy/en_core_web_md-2.3.1/setup.py` & `faKy-2.1.0/faKy/en_core_web_md-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `faKy-2.0.1/faKy/faKy.py` & `faKy-2.1.0/faKy/faKy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import spacy
-
-try:
-    nlp = spacy.load('en_core_web_md')
-except OSError:
-    print("Model not found. Please make sure 'en_core_web_md' is installed.")
-
 import pandas as pd 
 import numpy as np
 import sys
 import gzip
 from spacy.tokens import Doc
 from spacy_readability import Readability
 import nltk
 from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
 
-
+'''
+This exception handling block verifies that the spaCy language model is installed.
+If it is not installed, it downloads the model.
+'''
+try:
+    nlp = spacy.load('en_core_web_md')
+except OSError:
+    print('Downloading language model for the spaCy POS tagger\n'
+        "(don't worry, this will only happen once)")
+    from spacy.cli import download
+    download('en_core_web_md')
+    nlp = spacy.load('en_core_web_md')
 
 nltk.download('vader_lexicon')
 
 
 '''
- The function readability_computation computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. 
- It returns the original document object. 
- It is added to the spaCy pipeline using nlp.add_pipe with last=True.
+Under the hood functin needed for process_readability.
+The function readability_computation computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. 
+It returns the original document object. 
+It is added to the spaCy pipeline using nlp.add_pipe with last=True.
 '''
 def readability_computation(doc):
     read = Readability()
     flesch_kincaid_reading_ease = doc._.flesch_kincaid_reading_ease
     return doc
 nlp.add_pipe(readability_computation, last=True)
 
@@ -37,14 +43,15 @@
 def process_text_readability(text):
     doc = nlp(text)
     doc = readability_computation(doc)
     flesch_kincaid_reading_ease = doc._.flesch_kincaid_reading_ease
     return flesch_kincaid_reading_ease
 
 '''
+Under the hood function needed for process_text_complexity.
 The first line creates a custom extension attribute called "compressed_size" for spaCy's Doc object. 
 The function compress_doc compresses the serialized form of a spaCy Doc object using gzip, calculates the compressed size,
 and sets the compressed size to the custom "compressed_size" attribute of the Doc object before returning the Doc object.
 '''
 Doc.set_extension('compressed_size', default=None,force=True)
 def compress_doc(doc):
     serialized_doc = doc.to_bytes()
@@ -163,18 +170,14 @@
 '''
 def values_by_label(df, feature, labels, df_label):
     values_label = []
     for label in labels:
         values_label.append(df.loc[df[df_label] == label, feature])
     return values_label
 
-'''
-This function takes a list of numerical values as input and returns its mode, mean, standard deviation, and median as a tuple. 
-The mode is calculated using the statistics module, while the mean, standard deviation, and median are calculated using numpy.
-'''
 
 '''
 The dunn_table function takes a DataFrame of Dunn's test results and creates a new DataFrame where each row represents a group and each column represents a pairwise comparison with another group. 
 The new DataFrame contains two sub-columns: value which holds the p-value for each comparison, 
 and reject which holds a Boolean indicating whether the null hypothesis (that the two groups have the same distribution) should be rejected at a significance level of 0.05. 
 The function then returns this new DataFrame.
 '''
@@ -183,8 +186,9 @@
     for i in dunn_results.index:
         for j in dunn_results.columns:
             p_value = dunn_results.loc[i, j]
             reject_h0 = p_value < 0.05 
             reject_h0_table.loc[i, (j, 'value')] = p_value
             reject_h0_table.loc[i, (j, 'reject')] = reject_h0
     reject_h0_table.columns.names = ['group', 'metric']
-    return reject_h0_table
+    return reject_h0_table
+
```

### Comparing `faKy-2.0.1/setup.py` & `faKy-2.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='2.0.1',
-    description='Your library description',
+    version='2.1.0',
+    description='faKy is a Python library for text analysis. It provides functions for readability, complexity, sentiment, and statistical analysis in the scope of fake news detection.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
         'numpy==1.24.2',
-        'spacy==2.3.9',
         'pandas==1.3.4',
         'spacy-readability==1.4.1',
         'nltk==3.7',
         'vaderSentiment==3.3.2',
     ],
     extras_require={
         'vader': ['vaderSentiment'],
```

