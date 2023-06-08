# Comparing `tmp/kex-2.0.5.tar.gz` & `tmp/kex-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kex-2.0.5.tar", last modified: Wed Feb 10 14:57:40 2021, max compression
+gzip compressed data, was "kex-2.0.6.tar", last modified: Thu Jun  8 15:50:55 2023, max compression
```

## Comparing `kex-2.0.5.tar` & `kex-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2021-02-10 14:57:40.523260 kex-2.0.5/
--rw-r--r--   0 asahi      (501) staff       (20)     7130 2021-02-10 14:57:40.523482 kex-2.0.5/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     5423 2021-02-10 14:52:20.000000 kex-2.0.5/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2021-02-10 14:57:40.520529 kex-2.0.5/kex/
--rw-r--r--   0 asahi      (501) staff       (20)      516 2021-01-27 21:01:49.000000 kex-2.0.5/kex/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     1336 2021-01-27 20:47:02.000000 kex-2.0.5/kex/_get_algorithm.py
--rw-r--r--   0 asahi      (501) staff       (20)     4452 2021-02-10 14:30:26.000000 kex-2.0.5/kex/_get_dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     7777 2021-01-27 20:44:54.000000 kex-2.0.5/kex/_phrase_constructor.py
--rw-r--r--   0 asahi      (501) staff       (20)     2099 2021-02-10 14:23:02.000000 kex-2.0.5/kex/_stopwords.py
--rw-r--r--   0 asahi      (501) staff       (20)     1280 2021-01-27 17:52:03.000000 kex-2.0.5/kex/baseline.py
--rw-r--r--   0 asahi      (501) staff       (20)    10765 2021-01-27 17:53:44.000000 kex-2.0.5/kex/graph_text_rank.py
--rw-r--r--   0 asahi      (501) staff       (20)     6068 2021-01-27 17:51:32.000000 kex-2.0.5/kex/graph_topic_rank.py
--rw-r--r--   0 asahi      (501) staff       (20)     3532 2020-11-30 17:07:08.000000 kex-2.0.5/kex/graph_tpr.py
--rw-r--r--   0 asahi      (501) staff       (20)     5109 2021-02-02 16:10:35.000000 kex-2.0.5/kex/lda.py
--rw-r--r--   0 asahi      (501) staff       (20)     9057 2021-02-02 16:10:35.000000 kex-2.0.5/kex/lexical_specificity.py
--rw-r--r--   0 asahi      (501) staff       (20)     5710 2021-02-02 16:10:35.000000 kex-2.0.5/kex/tfidf.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2021-02-10 14:57:40.522942 kex-2.0.5/kex.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)     7130 2021-02-10 14:57:40.000000 kex-2.0.5/kex.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      396 2021-02-10 14:57:40.000000 kex-2.0.5/kex.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2021-02-10 14:57:40.000000 kex-2.0.5/kex.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       70 2021-02-10 14:57:40.000000 kex-2.0.5/kex.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        4 2021-02-10 14:57:40.000000 kex-2.0.5/kex.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2021-02-10 14:57:40.524140 kex-2.0.5/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1475 2021-02-10 14:00:13.000000 kex-2.0.5/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-08 15:50:55.023870 kex-2.0.6/
+-rw-r--r--   0 asahi      (501) staff       (20)     1064 2021-01-27 17:09:58.000000 kex-2.0.6/LICENSE.txt
+-rw-r--r--   0 asahi      (501) staff       (20)     7880 2023-06-08 15:50:55.024095 kex-2.0.6/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     7150 2022-02-16 23:02:15.000000 kex-2.0.6/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-08 15:50:55.021161 kex-2.0.6/kex/
+-rw-r--r--   0 asahi      (501) staff       (20)      516 2021-01-27 21:01:49.000000 kex-2.0.6/kex/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1336 2021-01-27 20:47:02.000000 kex-2.0.6/kex/_get_algorithm.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4453 2021-02-13 17:56:28.000000 kex-2.0.6/kex/_get_dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7777 2021-01-27 20:44:54.000000 kex-2.0.6/kex/_phrase_constructor.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2108 2022-02-16 23:02:15.000000 kex-2.0.6/kex/_stopwords.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1280 2021-01-27 17:52:03.000000 kex-2.0.6/kex/baseline.py
+-rw-r--r--   0 asahi      (501) staff       (20)    10765 2021-01-27 17:53:44.000000 kex-2.0.6/kex/graph_text_rank.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6068 2021-01-27 17:51:32.000000 kex-2.0.6/kex/graph_topic_rank.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3532 2020-11-30 17:07:08.000000 kex-2.0.6/kex/graph_tpr.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5110 2021-02-13 17:56:48.000000 kex-2.0.6/kex/lda.py
+-rw-r--r--   0 asahi      (501) staff       (20)     9058 2021-02-13 17:57:05.000000 kex-2.0.6/kex/lexical_specificity.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5711 2021-02-13 17:56:55.000000 kex-2.0.6/kex/tfidf.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-08 15:50:55.023538 kex-2.0.6/kex.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)     7880 2023-06-08 15:50:54.000000 kex-2.0.6/kex.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      408 2023-06-08 15:50:54.000000 kex-2.0.6/kex.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-06-08 15:50:54.000000 kex-2.0.6/kex.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       70 2023-06-08 15:50:54.000000 kex-2.0.6/kex.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        4 2023-06-08 15:50:54.000000 kex-2.0.6/kex.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-06-08 15:50:55.024831 kex-2.0.6/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1475 2022-02-16 23:03:13.000000 kex-2.0.6/setup.py
```

### Comparing `kex-2.0.5/PKG-INFO` & `kex-2.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,144 +1,148 @@
-Metadata-Version: 2.1
-Name: kex
-Version: 2.0.5
-Summary: Light/easy keyword extraction from documents.
-Home-page: https://github.com/asahi417/kex
-Author: Asahi Ushio
-Author-email: asahi1992ushio@gmail.com
-License: MIT
-Download-URL: https://github.com/asahi417/kex/archive/v2.0.5.tar.gz
-Description: # [Kex](https://pypi.org/project/kex/)
-        *Kex* is a python library for unsurpervised keyword extractions, supporting the following features: 
-        - [Easy interface for keyword extraction with a variety of algorithms](https://github.com/asahi417/kex#extract-keywords-with-kex)
-        - [Quick benchmarking over 15 English public datasets](https://github.com/asahi417/kex#benchmark-on-15-public-datasets)
-        - [Custom keyword extractor implementation support](https://github.com/asahi417/kex#implement-custom-extractor-with-kex)
-        
-        ## Get Started
-        Install via pip
-        ```shell script
-        pip install kex
-        ```
-        
-        ## Extract Keywords with Kex
-        Built-in algorithms in *kex* is below:
-        - `FirstN`: heuristic baseline to pick up first n phrases as keywords 
-        - `TF`: scoring by term frequency
-        - `TFIDF`: scoring by TFIDF
-        - `LexSpec`: scoring by [lexical specificity](https://www.aclweb.org/anthology/N15-1059.pdf)
-        - `TextRank`: [Mihalcea et al., 04](https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf)
-        - `SingleRank`: [Wan et al., 08](https://aclanthology.info/pdf/C/C08/C08-1122.pdf)
-        - `TopicalPageRank`: [Liu et al.,10](http://nlp.csai.tsinghua.edu.cn/~lzy/publications/emnlp2010.pdf)
-        - `SingleTPR`: [Sterckx et al.,15](https://core.ac.uk/download/pdf/55828317.pdf)
-        - `TopicRank`: [Bougouin et al.,13](http://www.aclweb.org/anthology/I13-1062)
-        - `PositionRank`: [Florescu et al.,18](http://people.cs.ksu.edu/~ccaragea/papers/acl17.pdf)
-        - `TFIDFRank`: SingleRank + TFIDF based word distribution prior
-        - `LexRank`: SingleRank + lexical specificity based word distribution prior
-        
-        Basic usage:
-        
-        ```python
-        >>> import kex
-        >>> model = kex.SingleRank()  # any algorithm listed above
-        >>> sample = '''
-        We propose a novel unsupervised keyphrase extraction approach that filters candidate keywords using outlier detection.
-        It starts by training word embeddings on the target document to capture semantic regularities among the words. It then
-        uses the minimum covariance determinant estimator to model the distribution of non-keyphrase word vectors, under the
-        assumption that these vectors come from the same distribution, indicative of their irrelevance to the semantics
-        expressed by the dimensions of the learned vector representation. Candidate keyphrases only consist of words that are
-        detected as outliers of this dominant distribution. Empirical results show that our approach outperforms state
-        of-the-art and recent unsupervised keyphrase extraction methods.
-        '''
-        >>> model.get_keywords(sample, n_keywords=2)
-        [{'stemmed': 'non-keyphras word vector',
-          'pos': 'ADJ NOUN NOUN',
-          'raw': ['non-keyphrase word vectors'],
-          'offset': [[47, 49]],
-          'count': 1,
-          'score': 0.06874471825637762,
-          'n_source_tokens': 112},
-         {'stemmed': 'semant regular word',
-          'pos': 'ADJ NOUN NOUN',
-          'raw': ['semantic regularities words'],
-          'offset': [[28, 32]],
-          'count': 1,
-          'score': 0.06001468574146248,
-          'n_source_tokens': 112}]
-        ```
-        
-        ### Compute a statistical prior
-        Algorithms such as `TF`, `TFIDF`, `TFIDFRank`, `LexSpec`, `LexRank`, `TopicalPageRank`, and `SingleTPR` need to compute
-        a prior distribution beforehand by
-        ```python
-        >>> import kex
-        >>> model = kex.SingleTPR()
-        >>> test_sentences = ['documentA', 'documentB', 'documentC']
-        >>> model.train(test_sentences, export_directory='./tmp')
-        ``` 
-        
-        Priors are cached and can be loaded on the fly as 
-        ```python
-        >>> import kex
-        >>> model = kex.SingleTPR()
-        >>> model.load('./tmp')
-        ```
-        
-        ### Supported language
-        Currently algorithms are available only in English, but soon we will relax the constrain to allow other language to be supported.
-        
-        ## Benchmark on 15 Public Datasets
-        Users can fetch 15 public keyword extraction datasets via [`kex.get_benchmark_dataset`](https://github.com/asahi417/kex/blob/master/kex/_get_dataset.py#L41).
-        
-        ```python
-        >>> import kex
-        >>> json_line, language = kex.get_benchmark_dataset('Inspec')
-        >>> json_line[0]
-        {
-            'keywords': ['kind infer', 'type check', 'overload', 'nonstrict pure function program languag', ...],
-            'source': 'A static semantics for Haskell\nThis paper gives a static semantics for Haskell 98, a non-strict ...',
-            'id': '1053.txt'
-        }
-        ```
-         
-        Please take a look an [example script](https://github.com/asahi417/kex/blob/master/examples/benchmark.py) to run a benchmark on those datasets.
-        
-        ## Implement Custom Extractor with Kex
-        We provide an API to run a basic pipeline for preprocessing, by which one can implement a custom keyword extractor.
-        
-        ```python
-        import kex
-        
-        class CustomExtractor:
-            """ Custom keyword extractor example: First N keywords extractor """
-        
-            def __init__(self, maximum_word_number: int = 3):
-                """ First N keywords extractor """
-                self.phrase_constructor = kex.PhraseConstructor(maximum_word_number=maximum_word_number)
-        
-            def get_keywords(self, document: str, n_keywords: int = 10):
-                """ Get keywords
-        
-                 Parameter
-                ------------------
-                document: str
-                n_keywords: int
-        
-                 Return
-                ------------------
-                a list of dictionary consisting of 'stemmed', 'pos', 'raw', 'offset', 'count'.
-                eg) {'stemmed': 'grid comput', 'pos': 'ADJ NOUN', 'raw': ['grid computing'], 'offset': [[11, 12]], 'count': 1}
-                """
-                phrase_instance, stemmed_tokens = self.phrase_constructor.tokenize_and_stem_and_phrase(document)
-                sorted_phrases = sorted(phrase_instance.values(), key=lambda x: x['offset'][0][0])
-                return sorted_phrases[:min(len(sorted_phrases), n_keywords)]
-        ```
-        
-Keywords: keyword-extraction,nlp,information-retrieval
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/kex/blob/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/kex.svg)](https://badge.fury.io/py/kex)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/kex.svg)](https://pypi.python.org/pypi/kex/)
+[![PyPI status](https://img.shields.io/pypi/status/kex.svg)](https://pypi.python.org/pypi/kex/)
+
+
+# KEX
+*Kex* is a python library for unsurpervised keyword extractions, supporting the following features: 
+- [Easy interface for keyword extraction with a variety of algorithms](https://github.com/asahi417/kex#extract-keywords-with-kex)
+- [Quick benchmarking over 15 English public datasets](https://github.com/asahi417/kex#benchmark-on-15-public-datasets)
+- [Custom keyword extractor implementation support](https://github.com/asahi417/kex#implement-custom-extractor-with-kex)
+
+***Our paper got accepted by EMNLP 2021 main conference 🎉*** (camera-ready is [here](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)):  
+In our paper, we conducted an extensive comparison and analysis over existing keyword extraction algorithms and proposed new algorithms `LexRank` and `LexSpec` that
+achieve very competitive baseline with very low complexity. Our proposed algorithms are based on the lexical specificity and we write a short introduction to the 
+lexical specificity [here](./asset/lexical_specificity.md).
+To reproduce all the result in the paper, please follow [these instructions](https://github.com/asahi417/kex/tree/emnlp_2021/examples/result_back_to_the_basic).
+
+## Get Started
+Install via pip
+```shell script
+pip install kex
+```
+
+## Extract Keywords with Kex
+Built-in algorithms in *kex* is below:
+- `FirstN`: heuristic baseline to pick up first n phrases as keywords 
+- `TF`: scoring by term frequency
+- `TFIDF`: scoring by TFIDF
+- `LexSpec`: [Ushio et al., 21](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)
+- `TextRank`: [Mihalcea et al., 04](https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf)
+- `SingleRank`: [Wan et al., 08](https://aclanthology.info/pdf/C/C08/C08-1122.pdf)
+- `TopicalPageRank`: [Liu et al.,10](http://nlp.csai.tsinghua.edu.cn/~lzy/publications/emnlp2010.pdf)
+- `SingleTPR`: [Sterckx et al.,15](https://core.ac.uk/download/pdf/55828317.pdf)
+- `TopicRank`: [Bougouin et al.,13](http://www.aclweb.org/anthology/I13-1062)
+- `PositionRank`: [Florescu et al.,18](http://people.cs.ksu.edu/~ccaragea/papers/acl17.pdf)
+- `TFIDFRank`: SingleRank + TFIDF based word distribution prior
+- `LexRank`: [Ushio et al., 21](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)
+
+Basic usage:
+
+```python
+>>> import kex
+>>> model = kex.SingleRank()  # any algorithm listed above
+>>> sample = '''
+We propose a novel unsupervised keyphrase extraction approach that filters candidate keywords using outlier detection.
+It starts by training word embeddings on the target document to capture semantic regularities among the words. It then
+uses the minimum covariance determinant estimator to model the distribution of non-keyphrase word vectors, under the
+assumption that these vectors come from the same distribution, indicative of their irrelevance to the semantics
+expressed by the dimensions of the learned vector representation. Candidate keyphrases only consist of words that are
+detected as outliers of this dominant distribution. Empirical results show that our approach outperforms state
+of-the-art and recent unsupervised keyphrase extraction methods.
+'''
+>>> model.get_keywords(sample, n_keywords=2)
+[{'stemmed': 'non-keyphras word vector',
+  'pos': 'ADJ NOUN NOUN',
+  'raw': ['non-keyphrase word vectors'],
+  'offset': [[47, 49]],
+  'count': 1,
+  'score': 0.06874471825637762,
+  'n_source_tokens': 112},
+ {'stemmed': 'semant regular word',
+  'pos': 'ADJ NOUN NOUN',
+  'raw': ['semantic regularities words'],
+  'offset': [[28, 32]],
+  'count': 1,
+  'score': 0.06001468574146248,
+  'n_source_tokens': 112}]
+```
+
+### Compute a statistical prior
+Algorithms such as `TF`, `TFIDF`, `TFIDFRank`, `LexSpec`, `LexRank`, `TopicalPageRank`, and `SingleTPR` need to compute
+a prior distribution beforehand by
+```python
+>>> import kex
+>>> model = kex.SingleTPR()
+>>> test_sentences = ['documentA', 'documentB', 'documentC']
+>>> model.train(test_sentences, export_directory='./tmp')
+``` 
+
+Priors are cached and can be loaded on the fly as 
+```python
+>>> import kex
+>>> model = kex.SingleTPR()
+>>> model.load('./tmp')
+```
+
+### Supported language
+Currently algorithms are available only in English, but soon we will relax the constrain to allow other language to be supported.
+
+## Benchmark on 15 Public Datasets
+Users can fetch 15 public keyword extraction datasets via [`kex.get_benchmark_dataset`](https://github.com/asahi417/kex/blob/master/kex/_get_dataset.py#L41).
+
+```python
+>>> import kex
+>>> json_line, language = kex.get_benchmark_dataset('Inspec')
+>>> json_line[0]
+{
+    'keywords': ['kind infer', 'type check', 'overload', 'nonstrict pure function program languag', ...],
+    'source': 'A static semantics for Haskell\nThis paper gives a static semantics for Haskell 98, a non-strict ...',
+    'id': '1053.txt'
+}
+```
+ 
+Please take a look an [example script](https://github.com/asahi417/kex/blob/emnlp_2021/examples/result_back_to_the_basic/benchmark.py) to run a benchmark on those datasets.
+
+## Implement Custom Extractor with Kex
+We provide an API to run a basic pipeline for preprocessing, by which one can implement a custom keyword extractor.
+
+```python
+import kex
+
+class CustomExtractor:
+    """ Custom keyword extractor example: First N keywords extractor """
+
+    def __init__(self, maximum_word_number: int = 3):
+        """ First N keywords extractor """
+        self.phrase_constructor = kex.PhraseConstructor(maximum_word_number=maximum_word_number)
+
+    def get_keywords(self, document: str, n_keywords: int = 10):
+        """ Get keywords
+
+         Parameter
+        ------------------
+        document: str
+        n_keywords: int
+
+         Return
+        ------------------
+        a list of dictionary consisting of 'stemmed', 'pos', 'raw', 'offset', 'count'.
+        eg) {'stemmed': 'grid comput', 'pos': 'ADJ NOUN', 'raw': ['grid computing'], 'offset': [[11, 12]], 'count': 1}
+        """
+        phrase_instance, stemmed_tokens = self.phrase_constructor.tokenize_and_stem_and_phrase(document)
+        sorted_phrases = sorted(phrase_instance.values(), key=lambda x: x['offset'][0][0])
+        return sorted_phrases[:min(len(sorted_phrases), n_keywords)]
+```
+
+## Reference paper
+If you use any of these resources, please cite the following paper:
+```
+@inproceedings{ushio-etal-2021-kex,
+    title={{B}ack to the {B}asics: {A} {Q}uantitative {A}nalysis of {S}tatistical and {G}raph-{B}ased {T}erm {W}eighting {S}chemes for {K}eyword {E}xtraction},
+    author={Ushio, Asahi and Liberatore, Federico and Camacho-Collados, Jose},
+        booktitle={Proceedings of the {EMNLP} 2021 Main Conference},
+    year = {2021},
+    publisher={Association for Computational Linguistics}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kex-2.0.5/README.md` & `kex-2.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,66 @@
-# [Kex](https://pypi.org/project/kex/)
+Metadata-Version: 2.1
+Name: kex
+Version: 2.0.6
+Summary: Light/easy keyword extraction from documents.
+Home-page: https://github.com/asahi417/kex
+Author: Asahi Ushio
+Author-email: asahi1992ushio@gmail.com
+License: MIT
+Download-URL: https://github.com/asahi417/kex/archive/v2.0.6.tar.gz
+Keywords: keyword-extraction,nlp,information-retrieval
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/kex/blob/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/kex.svg)](https://badge.fury.io/py/kex)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/kex.svg)](https://pypi.python.org/pypi/kex/)
+[![PyPI status](https://img.shields.io/pypi/status/kex.svg)](https://pypi.python.org/pypi/kex/)
+
+
+# KEX
 *Kex* is a python library for unsurpervised keyword extractions, supporting the following features: 
 - [Easy interface for keyword extraction with a variety of algorithms](https://github.com/asahi417/kex#extract-keywords-with-kex)
 - [Quick benchmarking over 15 English public datasets](https://github.com/asahi417/kex#benchmark-on-15-public-datasets)
 - [Custom keyword extractor implementation support](https://github.com/asahi417/kex#implement-custom-extractor-with-kex)
 
+***Our paper got accepted by EMNLP 2021 main conference 🎉*** (camera-ready is [here](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)):  
+In our paper, we conducted an extensive comparison and analysis over existing keyword extraction algorithms and proposed new algorithms `LexRank` and `LexSpec` that
+achieve very competitive baseline with very low complexity. Our proposed algorithms are based on the lexical specificity and we write a short introduction to the 
+lexical specificity [here](./asset/lexical_specificity.md).
+To reproduce all the result in the paper, please follow [these instructions](https://github.com/asahi417/kex/tree/emnlp_2021/examples/result_back_to_the_basic).
+
 ## Get Started
 Install via pip
 ```shell script
 pip install kex
 ```
 
 ## Extract Keywords with Kex
 Built-in algorithms in *kex* is below:
 - `FirstN`: heuristic baseline to pick up first n phrases as keywords 
 - `TF`: scoring by term frequency
 - `TFIDF`: scoring by TFIDF
-- `LexSpec`: scoring by [lexical specificity](https://www.aclweb.org/anthology/N15-1059.pdf)
+- `LexSpec`: [Ushio et al., 21](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)
 - `TextRank`: [Mihalcea et al., 04](https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf)
 - `SingleRank`: [Wan et al., 08](https://aclanthology.info/pdf/C/C08/C08-1122.pdf)
 - `TopicalPageRank`: [Liu et al.,10](http://nlp.csai.tsinghua.edu.cn/~lzy/publications/emnlp2010.pdf)
 - `SingleTPR`: [Sterckx et al.,15](https://core.ac.uk/download/pdf/55828317.pdf)
 - `TopicRank`: [Bougouin et al.,13](http://www.aclweb.org/anthology/I13-1062)
 - `PositionRank`: [Florescu et al.,18](http://people.cs.ksu.edu/~ccaragea/papers/acl17.pdf)
 - `TFIDFRank`: SingleRank + TFIDF based word distribution prior
-- `LexRank`: SingleRank + lexical specificity based word distribution prior
+- `LexRank`: [Ushio et al., 21](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)
 
 Basic usage:
 
 ```python
 >>> import kex
 >>> model = kex.SingleRank()  # any algorithm listed above
 >>> sample = '''
@@ -86,15 +119,15 @@
 {
     'keywords': ['kind infer', 'type check', 'overload', 'nonstrict pure function program languag', ...],
     'source': 'A static semantics for Haskell\nThis paper gives a static semantics for Haskell 98, a non-strict ...',
     'id': '1053.txt'
 }
 ```
  
-Please take a look an [example script](https://github.com/asahi417/kex/blob/master/examples/benchmark.py) to run a benchmark on those datasets.
+Please take a look an [example script](https://github.com/asahi417/kex/blob/emnlp_2021/examples/result_back_to_the_basic/benchmark.py) to run a benchmark on those datasets.
 
 ## Implement Custom Extractor with Kex
 We provide an API to run a basic pipeline for preprocessing, by which one can implement a custom keyword extractor.
 
 ```python
 import kex
 
@@ -118,7 +151,21 @@
         a list of dictionary consisting of 'stemmed', 'pos', 'raw', 'offset', 'count'.
         eg) {'stemmed': 'grid comput', 'pos': 'ADJ NOUN', 'raw': ['grid computing'], 'offset': [[11, 12]], 'count': 1}
         """
         phrase_instance, stemmed_tokens = self.phrase_constructor.tokenize_and_stem_and_phrase(document)
         sorted_phrases = sorted(phrase_instance.values(), key=lambda x: x['offset'][0][0])
         return sorted_phrases[:min(len(sorted_phrases), n_keywords)]
 ```
+
+## Reference paper
+If you use any of these resources, please cite the following paper:
+```
+@inproceedings{ushio-etal-2021-kex,
+    title={{B}ack to the {B}asics: {A} {Q}uantitative {A}nalysis of {S}tatistical and {G}raph-{B}ased {T}erm {W}eighting {S}chemes for {K}eyword {E}xtraction},
+    author={Ushio, Asahi and Liberatore, Federico and Camacho-Collados, Jose},
+        booktitle={Proceedings of the {EMNLP} 2021 Main Conference},
+    year = {2021},
+    publisher={Association for Computational Linguistics}
+}
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kex-2.0.5/kex/__init__.py` & `kex-2.0.6/kex/__init__.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/_get_algorithm.py` & `kex-2.0.6/kex/_get_algorithm.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/_get_dataset.py` & `kex-2.0.6/kex/_get_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 from glob import glob
 from ._phrase_constructor import PhraseConstructor
 from nltk.stem.porter import PorterStemmer  # only for English
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
 
-CACHE_DIR = '{}/cache_kex'.format(os.path.expanduser('~'))
+CACHE_DIR = '{}/.cache/kex'.format(os.path.expanduser('~'))
 STEMMER = PorterStemmer()
 VALID_DATASET_LIST = [
     # "110-PT-BN-KP", "cacic", "pak2018", "WikiNews", "wicc"
     "citeulike180", "fao30", "fao780", "Inspec", "kdd", "Krapivin2009", "Nguyen2007", "PubMed", "Schutz2008",
     "SemEval2010", "SemEval2017", "theses100", "wiki20", "www", "500N-KPCrowd-v1.1"
 ]
```

### Comparing `kex-2.0.5/kex/_phrase_constructor.py` & `kex-2.0.6/kex/_phrase_constructor.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/_stopwords.py` & `kex-2.0.6/kex/_stopwords.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import os
 import requests
 import tarfile
 import logging
 from typing import List
 logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
 
-CACHE_DIR = '{}/cache_kex'.format(os.path.expanduser('~'))
+CACHE_DIR = '{}/.cache/kex'.format(os.path.expanduser('~'))
 STOPWORDS_DIR = '{}/stopwords'.format(CACHE_DIR)
 
 
 def download_stopwords_dump():
     os.makedirs(CACHE_DIR, exist_ok=True)
-    url = "https://github.com/asahi417/kex/raw/master/asset/stopwords.tar.gz"
+    url = "https://github.com/asahi417/kex/releases/download/v2.0.5/stopwords.tar.gz"
     filename = '{}/{}'.format(CACHE_DIR, os.path.basename(url))
     logging.info('downloading stopwords dump from `{}` to `{}`'.format(url, CACHE_DIR))
     with open(filename, "wb") as f:
         r = requests.get(url)
         f.write(r.content)
     tar = tarfile.open(filename, "r:gz")
     tar.extractall(CACHE_DIR)
```

### Comparing `kex-2.0.5/kex/baseline.py` & `kex-2.0.6/kex/baseline.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/graph_text_rank.py` & `kex-2.0.6/kex/graph_text_rank.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/graph_topic_rank.py` & `kex-2.0.6/kex/graph_topic_rank.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/graph_tpr.py` & `kex-2.0.6/kex/graph_tpr.py`

 * *Files identical despite different names*

### Comparing `kex-2.0.5/kex/lda.py` & `kex-2.0.6/kex/lda.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import gensim
 from gensim import corpora
 
 from ._phrase_constructor import PhraseConstructor
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
 __all__ = 'LDA'
-CACHE_DIR = '{}/cache_kex/lda'.format(os.path.expanduser('~'))
+CACHE_DIR = '{}/.cache/kex/lda'.format(os.path.expanduser('~'))
 
 
 class LDA:
     """ LDA """
 
     def __init__(self, language: str = 'en'):
         self.__model = None
```

### Comparing `kex-2.0.5/kex/lexical_specificity.py` & `kex-2.0.6/kex/lexical_specificity.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from math import log, factorial, log10
 from collections import Counter
 from itertools import chain
 
 from ._phrase_constructor import PhraseConstructor
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
-CACHE_DIR = '{}/cache_kex/lexspec'.format(os.path.expanduser('~'))
+CACHE_DIR = '{}/.cache/kex/lexspec'.format(os.path.expanduser('~'))
 __all__ = ('LexSpec', 'lexical_specificity', 'TF')
 
 
 def average(_list):
     return sum(_list)/len(_list)
```

### Comparing `kex-2.0.5/kex/tfidf.py` & `kex-2.0.6/kex/tfidf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import gensim
 import numpy as np
 from gensim import corpora
 
 from ._phrase_constructor import PhraseConstructor
 
 logging.basicConfig(format='%(asctime)s %(levelname)-8s %(message)s', level=logging.INFO, datefmt='%Y-%m-%d %H:%M:%S')
-CACHE_DIR = '{}/cache_kex/tfidf'.format(os.path.expanduser('~'))
+CACHE_DIR = '{}/.cache/kex/tfidf'.format(os.path.expanduser('~'))
 __all__ = 'TFIDF'
 
 
 class TFIDF:
     """ TFIDF """
 
     def __init__(self, language: str = 'en'):
```

### Comparing `kex-2.0.5/kex.egg-info/PKG-INFO` & `kex-2.0.6/kex.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,171 @@
 Metadata-Version: 2.1
 Name: kex
-Version: 2.0.5
+Version: 2.0.6
 Summary: Light/easy keyword extraction from documents.
 Home-page: https://github.com/asahi417/kex
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT
-Download-URL: https://github.com/asahi417/kex/archive/v2.0.5.tar.gz
-Description: # [Kex](https://pypi.org/project/kex/)
-        *Kex* is a python library for unsurpervised keyword extractions, supporting the following features: 
-        - [Easy interface for keyword extraction with a variety of algorithms](https://github.com/asahi417/kex#extract-keywords-with-kex)
-        - [Quick benchmarking over 15 English public datasets](https://github.com/asahi417/kex#benchmark-on-15-public-datasets)
-        - [Custom keyword extractor implementation support](https://github.com/asahi417/kex#implement-custom-extractor-with-kex)
-        
-        ## Get Started
-        Install via pip
-        ```shell script
-        pip install kex
-        ```
-        
-        ## Extract Keywords with Kex
-        Built-in algorithms in *kex* is below:
-        - `FirstN`: heuristic baseline to pick up first n phrases as keywords 
-        - `TF`: scoring by term frequency
-        - `TFIDF`: scoring by TFIDF
-        - `LexSpec`: scoring by [lexical specificity](https://www.aclweb.org/anthology/N15-1059.pdf)
-        - `TextRank`: [Mihalcea et al., 04](https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf)
-        - `SingleRank`: [Wan et al., 08](https://aclanthology.info/pdf/C/C08/C08-1122.pdf)
-        - `TopicalPageRank`: [Liu et al.,10](http://nlp.csai.tsinghua.edu.cn/~lzy/publications/emnlp2010.pdf)
-        - `SingleTPR`: [Sterckx et al.,15](https://core.ac.uk/download/pdf/55828317.pdf)
-        - `TopicRank`: [Bougouin et al.,13](http://www.aclweb.org/anthology/I13-1062)
-        - `PositionRank`: [Florescu et al.,18](http://people.cs.ksu.edu/~ccaragea/papers/acl17.pdf)
-        - `TFIDFRank`: SingleRank + TFIDF based word distribution prior
-        - `LexRank`: SingleRank + lexical specificity based word distribution prior
-        
-        Basic usage:
-        
-        ```python
-        >>> import kex
-        >>> model = kex.SingleRank()  # any algorithm listed above
-        >>> sample = '''
-        We propose a novel unsupervised keyphrase extraction approach that filters candidate keywords using outlier detection.
-        It starts by training word embeddings on the target document to capture semantic regularities among the words. It then
-        uses the minimum covariance determinant estimator to model the distribution of non-keyphrase word vectors, under the
-        assumption that these vectors come from the same distribution, indicative of their irrelevance to the semantics
-        expressed by the dimensions of the learned vector representation. Candidate keyphrases only consist of words that are
-        detected as outliers of this dominant distribution. Empirical results show that our approach outperforms state
-        of-the-art and recent unsupervised keyphrase extraction methods.
-        '''
-        >>> model.get_keywords(sample, n_keywords=2)
-        [{'stemmed': 'non-keyphras word vector',
-          'pos': 'ADJ NOUN NOUN',
-          'raw': ['non-keyphrase word vectors'],
-          'offset': [[47, 49]],
-          'count': 1,
-          'score': 0.06874471825637762,
-          'n_source_tokens': 112},
-         {'stemmed': 'semant regular word',
-          'pos': 'ADJ NOUN NOUN',
-          'raw': ['semantic regularities words'],
-          'offset': [[28, 32]],
-          'count': 1,
-          'score': 0.06001468574146248,
-          'n_source_tokens': 112}]
-        ```
-        
-        ### Compute a statistical prior
-        Algorithms such as `TF`, `TFIDF`, `TFIDFRank`, `LexSpec`, `LexRank`, `TopicalPageRank`, and `SingleTPR` need to compute
-        a prior distribution beforehand by
-        ```python
-        >>> import kex
-        >>> model = kex.SingleTPR()
-        >>> test_sentences = ['documentA', 'documentB', 'documentC']
-        >>> model.train(test_sentences, export_directory='./tmp')
-        ``` 
-        
-        Priors are cached and can be loaded on the fly as 
-        ```python
-        >>> import kex
-        >>> model = kex.SingleTPR()
-        >>> model.load('./tmp')
-        ```
-        
-        ### Supported language
-        Currently algorithms are available only in English, but soon we will relax the constrain to allow other language to be supported.
-        
-        ## Benchmark on 15 Public Datasets
-        Users can fetch 15 public keyword extraction datasets via [`kex.get_benchmark_dataset`](https://github.com/asahi417/kex/blob/master/kex/_get_dataset.py#L41).
-        
-        ```python
-        >>> import kex
-        >>> json_line, language = kex.get_benchmark_dataset('Inspec')
-        >>> json_line[0]
-        {
-            'keywords': ['kind infer', 'type check', 'overload', 'nonstrict pure function program languag', ...],
-            'source': 'A static semantics for Haskell\nThis paper gives a static semantics for Haskell 98, a non-strict ...',
-            'id': '1053.txt'
-        }
-        ```
-         
-        Please take a look an [example script](https://github.com/asahi417/kex/blob/master/examples/benchmark.py) to run a benchmark on those datasets.
-        
-        ## Implement Custom Extractor with Kex
-        We provide an API to run a basic pipeline for preprocessing, by which one can implement a custom keyword extractor.
-        
-        ```python
-        import kex
-        
-        class CustomExtractor:
-            """ Custom keyword extractor example: First N keywords extractor """
-        
-            def __init__(self, maximum_word_number: int = 3):
-                """ First N keywords extractor """
-                self.phrase_constructor = kex.PhraseConstructor(maximum_word_number=maximum_word_number)
-        
-            def get_keywords(self, document: str, n_keywords: int = 10):
-                """ Get keywords
-        
-                 Parameter
-                ------------------
-                document: str
-                n_keywords: int
-        
-                 Return
-                ------------------
-                a list of dictionary consisting of 'stemmed', 'pos', 'raw', 'offset', 'count'.
-                eg) {'stemmed': 'grid comput', 'pos': 'ADJ NOUN', 'raw': ['grid computing'], 'offset': [[11, 12]], 'count': 1}
-                """
-                phrase_instance, stemmed_tokens = self.phrase_constructor.tokenize_and_stem_and_phrase(document)
-                sorted_phrases = sorted(phrase_instance.values(), key=lambda x: x['offset'][0][0])
-                return sorted_phrases[:min(len(sorted_phrases), n_keywords)]
-        ```
-        
+Download-URL: https://github.com/asahi417/kex/archive/v2.0.6.tar.gz
 Keywords: keyword-extraction,nlp,information-retrieval
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/kex/blob/master/LICENSE)
+[![PyPI version](https://badge.fury.io/py/kex.svg)](https://badge.fury.io/py/kex)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/kex.svg)](https://pypi.python.org/pypi/kex/)
+[![PyPI status](https://img.shields.io/pypi/status/kex.svg)](https://pypi.python.org/pypi/kex/)
+
+
+# KEX
+*Kex* is a python library for unsurpervised keyword extractions, supporting the following features: 
+- [Easy interface for keyword extraction with a variety of algorithms](https://github.com/asahi417/kex#extract-keywords-with-kex)
+- [Quick benchmarking over 15 English public datasets](https://github.com/asahi417/kex#benchmark-on-15-public-datasets)
+- [Custom keyword extractor implementation support](https://github.com/asahi417/kex#implement-custom-extractor-with-kex)
+
+***Our paper got accepted by EMNLP 2021 main conference 🎉*** (camera-ready is [here](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)):  
+In our paper, we conducted an extensive comparison and analysis over existing keyword extraction algorithms and proposed new algorithms `LexRank` and `LexSpec` that
+achieve very competitive baseline with very low complexity. Our proposed algorithms are based on the lexical specificity and we write a short introduction to the 
+lexical specificity [here](./asset/lexical_specificity.md).
+To reproduce all the result in the paper, please follow [these instructions](https://github.com/asahi417/kex/tree/emnlp_2021/examples/result_back_to_the_basic).
+
+## Get Started
+Install via pip
+```shell script
+pip install kex
+```
+
+## Extract Keywords with Kex
+Built-in algorithms in *kex* is below:
+- `FirstN`: heuristic baseline to pick up first n phrases as keywords 
+- `TF`: scoring by term frequency
+- `TFIDF`: scoring by TFIDF
+- `LexSpec`: [Ushio et al., 21](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)
+- `TextRank`: [Mihalcea et al., 04](https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf)
+- `SingleRank`: [Wan et al., 08](https://aclanthology.info/pdf/C/C08/C08-1122.pdf)
+- `TopicalPageRank`: [Liu et al.,10](http://nlp.csai.tsinghua.edu.cn/~lzy/publications/emnlp2010.pdf)
+- `SingleTPR`: [Sterckx et al.,15](https://core.ac.uk/download/pdf/55828317.pdf)
+- `TopicRank`: [Bougouin et al.,13](http://www.aclweb.org/anthology/I13-1062)
+- `PositionRank`: [Florescu et al.,18](http://people.cs.ksu.edu/~ccaragea/papers/acl17.pdf)
+- `TFIDFRank`: SingleRank + TFIDF based word distribution prior
+- `LexRank`: [Ushio et al., 21](https://github.com/asahi417/kex/blob/master/asset/EMNLP21_Keyword_Extraction_camera.pdf)
+
+Basic usage:
+
+```python
+>>> import kex
+>>> model = kex.SingleRank()  # any algorithm listed above
+>>> sample = '''
+We propose a novel unsupervised keyphrase extraction approach that filters candidate keywords using outlier detection.
+It starts by training word embeddings on the target document to capture semantic regularities among the words. It then
+uses the minimum covariance determinant estimator to model the distribution of non-keyphrase word vectors, under the
+assumption that these vectors come from the same distribution, indicative of their irrelevance to the semantics
+expressed by the dimensions of the learned vector representation. Candidate keyphrases only consist of words that are
+detected as outliers of this dominant distribution. Empirical results show that our approach outperforms state
+of-the-art and recent unsupervised keyphrase extraction methods.
+'''
+>>> model.get_keywords(sample, n_keywords=2)
+[{'stemmed': 'non-keyphras word vector',
+  'pos': 'ADJ NOUN NOUN',
+  'raw': ['non-keyphrase word vectors'],
+  'offset': [[47, 49]],
+  'count': 1,
+  'score': 0.06874471825637762,
+  'n_source_tokens': 112},
+ {'stemmed': 'semant regular word',
+  'pos': 'ADJ NOUN NOUN',
+  'raw': ['semantic regularities words'],
+  'offset': [[28, 32]],
+  'count': 1,
+  'score': 0.06001468574146248,
+  'n_source_tokens': 112}]
+```
+
+### Compute a statistical prior
+Algorithms such as `TF`, `TFIDF`, `TFIDFRank`, `LexSpec`, `LexRank`, `TopicalPageRank`, and `SingleTPR` need to compute
+a prior distribution beforehand by
+```python
+>>> import kex
+>>> model = kex.SingleTPR()
+>>> test_sentences = ['documentA', 'documentB', 'documentC']
+>>> model.train(test_sentences, export_directory='./tmp')
+``` 
+
+Priors are cached and can be loaded on the fly as 
+```python
+>>> import kex
+>>> model = kex.SingleTPR()
+>>> model.load('./tmp')
+```
+
+### Supported language
+Currently algorithms are available only in English, but soon we will relax the constrain to allow other language to be supported.
+
+## Benchmark on 15 Public Datasets
+Users can fetch 15 public keyword extraction datasets via [`kex.get_benchmark_dataset`](https://github.com/asahi417/kex/blob/master/kex/_get_dataset.py#L41).
+
+```python
+>>> import kex
+>>> json_line, language = kex.get_benchmark_dataset('Inspec')
+>>> json_line[0]
+{
+    'keywords': ['kind infer', 'type check', 'overload', 'nonstrict pure function program languag', ...],
+    'source': 'A static semantics for Haskell\nThis paper gives a static semantics for Haskell 98, a non-strict ...',
+    'id': '1053.txt'
+}
+```
+ 
+Please take a look an [example script](https://github.com/asahi417/kex/blob/emnlp_2021/examples/result_back_to_the_basic/benchmark.py) to run a benchmark on those datasets.
+
+## Implement Custom Extractor with Kex
+We provide an API to run a basic pipeline for preprocessing, by which one can implement a custom keyword extractor.
+
+```python
+import kex
+
+class CustomExtractor:
+    """ Custom keyword extractor example: First N keywords extractor """
+
+    def __init__(self, maximum_word_number: int = 3):
+        """ First N keywords extractor """
+        self.phrase_constructor = kex.PhraseConstructor(maximum_word_number=maximum_word_number)
+
+    def get_keywords(self, document: str, n_keywords: int = 10):
+        """ Get keywords
+
+         Parameter
+        ------------------
+        document: str
+        n_keywords: int
+
+         Return
+        ------------------
+        a list of dictionary consisting of 'stemmed', 'pos', 'raw', 'offset', 'count'.
+        eg) {'stemmed': 'grid comput', 'pos': 'ADJ NOUN', 'raw': ['grid computing'], 'offset': [[11, 12]], 'count': 1}
+        """
+        phrase_instance, stemmed_tokens = self.phrase_constructor.tokenize_and_stem_and_phrase(document)
+        sorted_phrases = sorted(phrase_instance.values(), key=lambda x: x['offset'][0][0])
+        return sorted_phrases[:min(len(sorted_phrases), n_keywords)]
+```
+
+## Reference paper
+If you use any of these resources, please cite the following paper:
+```
+@inproceedings{ushio-etal-2021-kex,
+    title={{B}ack to the {B}asics: {A} {Q}uantitative {A}nalysis of {S}tatistical and {G}raph-{B}ased {T}erm {W}eighting {S}chemes for {K}eyword {E}xtraction},
+    author={Ushio, Asahi and Liberatore, Federico and Camacho-Collados, Jose},
+        booktitle={Proceedings of the {EMNLP} 2021 Main Conference},
+    year = {2021},
+    publisher={Association for Computational Linguistics}
+}
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kex-2.0.5/setup.py` & `kex-2.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
-VERSION = '2.0.5'
+VERSION = '2.0.6'
 setup(
     name='kex',
     packages=find_packages(exclude=['examples', 'tests', 'asset', 'benchmark']),
     version=VERSION,
     license='MIT',
     description='Light/easy keyword extraction from documents.',
     url='https://github.com/asahi417/kex',
```

