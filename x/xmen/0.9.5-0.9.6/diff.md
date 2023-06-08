# Comparing `tmp/xmen-0.9.5.tar.gz` & `tmp/xmen-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmen-0.9.5.tar", max compression
+gzip compressed data, was "xmen-0.9.6.tar", max compression
```

## Comparing `xmen-0.9.5.tar` & `xmen-0.9.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.5/LICENSE
--rw-r--r--   0        0        0     9422 2023-05-24 13:46:51.648440 xmen-0.9.5/README.md
--rw-r--r--   0        0        0     1061 2023-05-24 13:46:51.811443 xmen-0.9.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.5/xmen/__init__.py
--rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.5/xmen/analysis.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.5/xmen/cli/__init__.py
--rw-r--r--   0        0        0     7713 2023-05-16 20:37:32.742833 xmen-0.9.5/xmen/cli/cli.py
--rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.5/xmen/cli/dict.py
--rw-r--r--   0        0        0     1868 2023-05-24 13:46:51.862444 xmen-0.9.5/xmen/cli/index.py
--rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.5/xmen/cli/utils.py
--rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.5/xmen/confhelper.py
--rw-r--r--   0        0        0      438 2023-05-24 13:46:51.901445 xmen-0.9.5/xmen/data/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-24 13:46:51.921446 xmen-0.9.5/xmen/data/abbrevations.py
--rw-r--r--   0        0        0     4208 2023-05-16 20:37:32.693831 xmen-0.9.5/xmen/data/dataloaders.py
--rw-r--r--   0        0        0      698 2023-05-24 13:46:51.965447 xmen-0.9.5/xmen/data/filter.py
--rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.5/xmen/data/indexed_dataset.py
--rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.5/xmen/data/integrations.py
--rw-r--r--   0        0        0     1308 2023-05-24 13:46:51.969447 xmen-0.9.5/xmen/data/merge_concepts.py
--rw-r--r--   0        0        0     2386 2023-05-24 13:46:51.983447 xmen-0.9.5/xmen/data/retired_cuis.py
--rw-r--r--   0        0        0     2497 2023-05-24 13:46:52.000447 xmen-0.9.5/xmen/data/sampling.py
--rw-r--r--   0        0        0     2093 2023-05-24 13:46:52.039448 xmen-0.9.5/xmen/data/semantic_groups.py
--rw-r--r--   0        0        0     2577 2023-05-24 13:46:52.043448 xmen-0.9.5/xmen/data/semantic_types.py
--rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.5/xmen/data/util.py
--rw-r--r--   0        0        0    15490 2023-05-16 20:37:32.795835 xmen-0.9.5/xmen/evaluation.py
--rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.5/xmen/ext/neleval/annotation.py
--rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.5/xmen/ext/neleval/configs.py
--rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.5/xmen/ext/neleval/document.py
--rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.5/xmen/ext/neleval/evaluate.py
--rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.5/xmen/ext/neleval/prepare.py
--rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.5/xmen/ext/sapbert/LICENSE
--rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.5/xmen/ext/sapbert/README.md
--rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.5/xmen/ext/sapbert/requirements.txt
--rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.5/xmen/ext/sapbert/src/__init__.py
--rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.5/xmen/ext/sapbert/src/data_loader.py
--rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.5/xmen/ext/sapbert/src/metric_learning.py
--rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.5/xmen/ext/sapbert/src/model_wrapper.py
--rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.5/xmen/ext/sapbert/train/.gitignore
--rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.5/xmen/ext/sapbert/train/pretrain.sh
--rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.5/xmen/ext/sapbert/train/train.py
--rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.5/xmen/ext/sapbert/train/xling_train.sh
--rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.5/xmen/ext/scispacy/umls_utils.py
--rw-r--r--   0        0        0     6328 2023-05-24 13:46:52.063449 xmen-0.9.5/xmen/kb.py
--rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.5/xmen/linkers/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.5/xmen/linkers/ensemble.py
--rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.5/xmen/linkers/faiss_indexer.py
--rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.5/xmen/linkers/sap_bert_linker.py
--rw-r--r--   0        0        0     9442 2023-05-24 13:46:52.069449 xmen-0.9.5/xmen/linkers/tf_idf_ngram_linker.py
--rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.5/xmen/linkers/util.py
--rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.5/xmen/log.py
--rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.5/xmen/reranking/__init__.py
--rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.5/xmen/reranking/cross_encoder.py
--rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.5/xmen/reranking/list_wise.py
--rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.5/xmen/reranking/multiple_choice_util.py
--rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.5/xmen/reranking/ranking_util.py
--rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.5/xmen/reranking/rule_based.py
--rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.5/xmen/reranking/scored_cross_encoder.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.5/xmen/resources/.gitkeep
--rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.5/xmen/resources/Readme.md
--rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.5/xmen/resources/SemGroups-v03.txt
--rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.5/xmen/resources/SemGroups.txt
--rw-r--r--   0        0        0    10168 2023-05-16 20:37:32.742833 xmen-0.9.5/xmen/umls.py
--rw-r--r--   0        0        0    10805 1970-01-01 00:00:00.000000 xmen-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.6/LICENSE
+-rw-r--r--   0        0        0     9296 2023-06-07 14:10:12.256707 xmen-0.9.6/README.md
+-rw-r--r--   0        0        0     1061 2023-06-07 14:10:12.568713 xmen-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.6/xmen/__init__.py
+-rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.6/xmen/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.6/xmen/cli/__init__.py
+-rw-r--r--   0        0        0     7705 2023-06-07 14:10:12.598714 xmen-0.9.6/xmen/cli/cli.py
+-rw-r--r--   0        0        0     2730 2023-06-07 14:10:12.635715 xmen-0.9.6/xmen/cli/dict.py
+-rw-r--r--   0        0        0     2025 2023-06-07 14:10:12.647715 xmen-0.9.6/xmen/cli/index.py
+-rw-r--r--   0        0        0     6382 2023-06-07 14:10:12.669715 xmen-0.9.6/xmen/cli/utils.py
+-rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.6/xmen/confhelper.py
+-rw-r--r--   0        0        0      438 2023-05-24 13:46:51.901445 xmen-0.9.6/xmen/data/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-24 13:46:51.921446 xmen-0.9.6/xmen/data/abbrevations.py
+-rw-r--r--   0        0        0     4208 2023-05-16 20:37:32.693831 xmen-0.9.6/xmen/data/dataloaders.py
+-rw-r--r--   0        0        0      698 2023-05-24 13:46:51.965447 xmen-0.9.6/xmen/data/filter.py
+-rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.6/xmen/data/indexed_dataset.py
+-rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.6/xmen/data/integrations.py
+-rw-r--r--   0        0        0     1308 2023-05-24 13:46:51.969447 xmen-0.9.6/xmen/data/merge_concepts.py
+-rw-r--r--   0        0        0     2386 2023-05-24 13:46:51.983447 xmen-0.9.6/xmen/data/retired_cuis.py
+-rw-r--r--   0        0        0     2497 2023-05-24 13:46:52.000447 xmen-0.9.6/xmen/data/sampling.py
+-rw-r--r--   0        0        0     2093 2023-05-24 13:46:52.039448 xmen-0.9.6/xmen/data/semantic_groups.py
+-rw-r--r--   0        0        0     2577 2023-05-24 13:46:52.043448 xmen-0.9.6/xmen/data/semantic_types.py
+-rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.6/xmen/data/util.py
+-rw-r--r--   0        0        0    15495 2023-06-07 14:10:12.715716 xmen-0.9.6/xmen/evaluation.py
+-rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.6/xmen/ext/neleval/annotation.py
+-rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.6/xmen/ext/neleval/configs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.6/xmen/ext/neleval/document.py
+-rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.6/xmen/ext/neleval/evaluate.py
+-rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.6/xmen/ext/neleval/prepare.py
+-rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.6/xmen/ext/sapbert/LICENSE
+-rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.6/xmen/ext/sapbert/README.md
+-rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.6/xmen/ext/sapbert/requirements.txt
+-rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.6/xmen/ext/sapbert/src/__init__.py
+-rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.6/xmen/ext/sapbert/src/data_loader.py
+-rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.6/xmen/ext/sapbert/src/metric_learning.py
+-rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.6/xmen/ext/sapbert/src/model_wrapper.py
+-rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.6/xmen/ext/sapbert/train/.gitignore
+-rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.6/xmen/ext/sapbert/train/pretrain.sh
+-rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.6/xmen/ext/sapbert/train/train.py
+-rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.6/xmen/ext/sapbert/train/xling_train.sh
+-rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.6/xmen/ext/scispacy/umls_utils.py
+-rw-r--r--   0        0        0     6328 2023-05-24 13:46:52.063449 xmen-0.9.6/xmen/kb.py
+-rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.6/xmen/linkers/__init__.py
+-rw-r--r--   0        0        0     6220 2023-06-07 14:10:12.732716 xmen-0.9.6/xmen/linkers/ensemble.py
+-rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.6/xmen/linkers/faiss_indexer.py
+-rw-r--r--   0        0        0     9722 2023-06-07 14:10:12.746717 xmen-0.9.6/xmen/linkers/sap_bert_linker.py
+-rw-r--r--   0        0        0     9442 2023-05-24 13:46:52.069449 xmen-0.9.6/xmen/linkers/tf_idf_ngram_linker.py
+-rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.6/xmen/linkers/util.py
+-rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.6/xmen/log.py
+-rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.6/xmen/reranking/__init__.py
+-rw-r--r--   0        0        0    20918 2023-06-07 14:10:12.760717 xmen-0.9.6/xmen/reranking/cross_encoder.py
+-rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.6/xmen/reranking/list_wise.py
+-rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.6/xmen/reranking/multiple_choice_util.py
+-rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.6/xmen/reranking/ranking_util.py
+-rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.6/xmen/reranking/rule_based.py
+-rw-r--r--   0        0        0    14470 2023-06-07 14:10:12.815718 xmen-0.9.6/xmen/reranking/scored_cross_encoder.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.6/xmen/resources/.gitkeep
+-rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.6/xmen/resources/Readme.md
+-rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.6/xmen/resources/SemGroups-v03.txt
+-rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.6/xmen/resources/SemGroups.txt
+-rw-r--r--   0        0        0    10168 2023-05-16 20:37:32.742833 xmen-0.9.6/xmen/umls.py
+-rw-r--r--   0        0        0    10679 1970-01-01 00:00:00.000000 xmen-0.9.6/PKG-INFO
```

### Comparing `xmen-0.9.5/LICENSE` & `xmen-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/README.md` & `xmen-0.9.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 `pip install xmen`
 
 ### Development
 
 We use [Poetry](https://python-poetry.org/) for building, testing and dependency management (see [pyproject.toml](pyproject.toml)).
 
+## 🚀 Getting Started
+
+A very simple pipeline highlighting the main components of xMEN can be found in [notebooks/Getting_Started.ipynb](notebooks/Getting_Started.ipynb)
+
 ## 📂 Data Loading
 
 Usually, BigBIO-compatible datasets can just be loaded from the Hugging Face Hub:
 
 ```
 from datasets import load_dataset
 dataset = load_dataset("distemist", "distemist_linking_bigbio_kb")
@@ -140,16 +144,15 @@
 Based on the implementation from [scispaCy](https://github.com/allenai/scispacy).
 
 YAML file:
 
 ```
 linker:
   candidate_generation:
-    ngram:
-      k: 100
+    ngram: ~
 ```
 
 Run `xmen index my_config.yaml --ngram` or `xmen index my_config.yaml --all` to create the index.
 
 To use the linker at runtime, pass the index folder as an argument:
 
 ```
@@ -167,34 +170,32 @@
 
 YAML file:
 
 ```
 linker:
   candidate_generation:
     sapbert:
-      embedding_model_name: cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR
-      k: 1000
+      model_name: cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR
 ```
 
 Run `xmen index my_config.yaml --sapbert` or `xmen index my_config.yaml --all` to create the [FAISS](https://github.com/facebookresearch/faiss) index.
 
-To use the linker at runtime, pass the `embedding_model_name` (usually the same as was used for creating the index)  and index folder as an argument. To make predictions on a batch of documents, you have to pass a batch size, as the SapBERT linker runs on the GPU by default:
+To use the linker at runtime, pass the index folder as an argument. To make predictions on a batch of documents, you have to pass a batch size, as the SapBERT linker runs on the GPU by default:
 
 ```
 from xmen.linkers import SapBERTLinker
 
 sapbert_linker = SapBERTLinker(
-    embedding_model_name = "cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR", # Name of SapBERT model
     index_base_path = "/path/to/my/index/sapbert",
     k = 1000
 )
 predictions = sapbert_linker.predict_batch(dataset, batch_size=128)
 ```
 
-If you have loaded a yaml-config as a dictionary, you may also just pass it as kwargs:
+If you have loaded a yaml-config as a dictionary-like object, you may also just pass it as kwargs:
 
 ```
 sapbert_linker = SapBERTLinker(**config)
 ```
 
 By default, SapBERT assumes a CUDA device is available. If you want to disable cuda, pass `cuda=False` to the constructor.
 
@@ -237,33 +238,39 @@
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 from xmen.kb import load_kb
 
 # Load a KB from a pre-computed dictionary (jsonl) to obtain synonyms for concept encoding
 kb = load_kb('path/to/my/dictionary.jsonl')
 
-candidates = linker.predict_batch(dataset) # obtain prediction from candidate generator (see above)
+# Obtain prediction from candidate generator (see above)
+candidates = linker.predict_batch(dataset)
 
 cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb)
 ```
 
 Then you can use this dataset to train a supervised reranking model:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 
-cross_encoder_model = 'bert-base-multilingual-cased' # any BERT model, potentially language specific
-n_epochs = 10 # number of epochs to train
-output_dir = './checkpoints/' # Path to temp dir for writing model checkpoints
+# Number of epochs to train
+n_epochs = 10
 
-train_args = CrossEncoderTrainingArgs(cross_encoder_model, n_epochs)
+# Any BERT model, potentially language-specific
+cross_encoder_model = 'bert-base-multilingual-cased'
+
+args = CrossEncoderTrainingArgs(n_epochs, cross_encoder_model)
 
 rr = CrossEncoderReranker()
-rr.fit(cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset, output_dir=output_dir, training_args=train_args)
 
+# Fit the model
+rr.fit(args, cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset)
+
+# Predict on test set
 prediction = rr.rerank_batch(candidates['test'], cross_enc_ds['test'])
 ```
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
```

### Comparing `xmen-0.9.5/pyproject.toml` & `xmen-0.9.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmen"
-version = "0.9.5"
+version = "0.9.6"
 description = "An extensible toolkit for Cross-lingual (x) Medical Entity Normalization."
 license = "Apache-2.0"
 authors = ["Florian Borchert <florian.borchert@hpi.de>"]
 readme = "README.md"
 repository = "https://github.com/hpi-dhc/xmen"
 
 [tool.poetry.scripts]
```

### Comparing `xmen-0.9.5/xmen/analysis.py` & `xmen-0.9.6/xmen/analysis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/cli/cli.py` & `xmen-0.9.6/xmen/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,35 +132,35 @@
     if os.path.exists(dict):
         logger.info(f"Dictionary found in {dict}. Attempting to build indices.")
 
         is_ngram_selected = ngram or all
         required_key = "linker.candidate_generation.ngram"
         write_path = output / "index" / "ngrams"
         if is_ngram_selected and has_correct_keys(cfg, required_key) and can_write(write_path, overwrite):
-            logger.info("Building N-Gram indices.")
+            logger.info("Building N-Gram index.")
             build_ngram(cfg, output, dict)
         else:
-            logger.info("Skipping N-Gram indices.")
+            logger.info("Skipping N-Gram index.")
 
         is_sapbert_selected = sapbert or all
         required_key = "linker.candidate_generation.sapbert"
         write_path = output / "index" / "sapbert"
         if is_sapbert_selected and has_correct_keys(cfg, required_key) and can_write(write_path, overwrite):
             # check for GPUs
             if torch.cuda.is_available():
                 logger.info(f"CUDA is available. Running on GPU with ID {gpu_id}. To select another, use --gpu-id.")
             else:
                 gpu_id = -1
                 logger.warning(
                     "CUDA is not available on this system. Running on CPU. This can take considerably longer."
                 )
-            logger.info("Building SapBERT indices.")
+            logger.info("Building SapBERT index.")
             build_sapbert(cfg, output, dict, gpu_id)
         else:
-            logger.info("Skipping SapBERT indices.")
+            logger.info("Skipping SapBERT index.")
 
     else:
         logger.info(
             f"Dictionary {dict} does not exist. Build one with command --dict or provide the right path to one with "
             "--dict-dir flag."
         )
```

### Comparing `xmen-0.9.5/xmen/cli/dict.py` & `xmen-0.9.6/xmen/cli/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             cfg.dict.umls.meta_path,
             cfg.dict.umls.get("lang", []),
             sabs=cfg.dict.umls.get("sabs", []),
             sources=cfg.dict.umls.get("sources", []),
             semantic_groups=cfg.dict.umls.get("semantic_groups", None),
             semantic_types=cfg.dict.umls.get("semantic_types", None),
             non_suppressed_only=cfg.dict.umls.get("non_suppressed_only", False),
-            semantic_group_file_version=cfg.dict.umls.get("semantic_group_file_version", False),
+            semantic_group_file_version=cfg.dict.umls.get("semantic_group_file_version", "v03"),
         )
     elif "custom" in cfg.dict:
         return get_custom_concepts(cfg, custom_path)
 
 
 def get_custom_concepts(cfg, path) -> dict:
     """
```

### Comparing `xmen-0.9.5/xmen/cli/index.py` & `xmen-0.9.6/xmen/cli/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,16 +36,21 @@
     # ensure the index folder exists
     work_dir.parent.mkdir(exist_ok=True, parents=True)
     # SapBERT indices
     term_dict = create_flat_term_dict([dict_dir])
     logger.info(f"Number of aliases: {len(term_dict)}.")
     logger.info(f"Number of concepts: {len(term_dict.cui.unique())}.")
 
+    sapbert_cfg = cfg.linker.candidate_generation.sapbert
+    model_name = SapBERTLinker.CROSS_LINGUAL  # default model
+    if sapbert_cfg and "model_name" in sapbert_cfg:
+        model_name = sapbert_cfg.model_name
+
     cuda = False if gpu_id == -1 else True
     with torch.cuda.device(gpu_id):
         SapBERTLinker.write_index(
             work_dir / "index" / "sapbert",
             term_dict=term_dict,
             cuda=cuda,
             subtract_mean=False,
-            embedding_model_name=cfg.linker.candidate_generation.sapbert.embedding_model_name,
+            model_name=model_name,
         )
```

### Comparing `xmen-0.9.5/xmen/cli/utils.py` & `xmen-0.9.6/xmen/cli/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         else:
             is_warnable = os.path.exists(path) and os.listdir(path)
             warning = f"There are already some files in {path}. This command may overwrite them."
 
         if is_warnable:
             logger.warn(warning)
             logger.info(
-                f"To instruct the command to overwrite all coinciding files by default, swith the flag --overwrite."
+                f"To instruct the command to overwrite all coinciding files by default, switch the flag --overwrite."
                 f"You can also provide a different path to write the files with --output. \n"
                 f"What would you like to do this time? Input yes [y] to overwrite it, no [n] to skip the file."
             )
             overwrite = input("[y/n]")
         else:
             overwrite = "y"
```

### Comparing `xmen-0.9.5/xmen/confhelper.py` & `xmen-0.9.6/xmen/confhelper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/abbrevations.py` & `xmen-0.9.6/xmen/data/abbrevations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/dataloaders.py` & `xmen-0.9.6/xmen/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/filter.py` & `xmen-0.9.6/xmen/data/filter.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/indexed_dataset.py` & `xmen-0.9.6/xmen/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/integrations.py` & `xmen-0.9.6/xmen/data/integrations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/merge_concepts.py` & `xmen-0.9.6/xmen/data/merge_concepts.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/retired_cuis.py` & `xmen-0.9.6/xmen/data/retired_cuis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/sampling.py` & `xmen-0.9.6/xmen/data/sampling.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/semantic_groups.py` & `xmen-0.9.6/xmen/data/semantic_groups.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/semantic_types.py` & `xmen-0.9.6/xmen/data/semantic_types.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/data/util.py` & `xmen-0.9.6/xmen/data/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/evaluation.py` & `xmen-0.9.6/xmen/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 "pred_text": pred_text,
                 "gt_start": gt_s,
                 "gt_end": gt_e,
                 "gt_text": gt_text,
                 "entity_match_type": e_match_type,
                 "gold_concept": gt_concept,
                 "gold_type": gt_type,
-                "pred_index": idx,
+                "pred_index": int(idx),
                 "pred_index_score": pred_c[idx].get("score", None) if idx >= 0 else None,
                 "pred_top": pred_c[0]["db_id"] if len(pred_c) > 0 else None,
                 "pred_top_score": pred_c[0].get("score", None) if len(pred_c) > 0 else None,
             }
 
         if not pred_c and gt_c:
             assert len(gt_c) == 1
```

### Comparing `xmen-0.9.5/xmen/ext/neleval/annotation.py` & `xmen-0.9.6/xmen/ext/neleval/annotation.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/neleval/configs.py` & `xmen-0.9.6/xmen/ext/neleval/configs.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/neleval/document.py` & `xmen-0.9.6/xmen/ext/neleval/document.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/neleval/evaluate.py` & `xmen-0.9.6/xmen/ext/neleval/evaluate.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/neleval/prepare.py` & `xmen-0.9.6/xmen/ext/neleval/prepare.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/LICENSE` & `xmen-0.9.6/xmen/ext/sapbert/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/README.md` & `xmen-0.9.6/xmen/ext/sapbert/README.md`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/src/data_loader.py` & `xmen-0.9.6/xmen/ext/sapbert/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/src/metric_learning.py` & `xmen-0.9.6/xmen/ext/sapbert/src/metric_learning.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/src/model_wrapper.py` & `xmen-0.9.6/xmen/ext/sapbert/src/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/train/.gitignore` & `xmen-0.9.6/xmen/ext/sapbert/train/.gitignore`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/train/train.py` & `xmen-0.9.6/xmen/ext/sapbert/train/train.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/sapbert/train/xling_train.sh` & `xmen-0.9.6/xmen/ext/sapbert/train/xling_train.sh`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/ext/scispacy/umls_utils.py` & `xmen-0.9.6/xmen/ext/scispacy/umls_utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/kb.py` & `xmen-0.9.6/xmen/kb.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/linkers/__init__.py` & `xmen-0.9.6/xmen/linkers/__init__.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/linkers/ensemble.py` & `xmen-0.9.6/xmen/linkers/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         - weight: a float representing the weight to give to this linker during combination (default is 1.0)
         """
         self.linkers_fn[name] = linker_fn
         self.linkers_k[name] = k
         self.linker_thresholds[name] = threshold
         self.linker_weigths[name] = weight
 
-    def predict_batch(self, dataset, batch_size, top_k=None, reuse_preds=None):
+    def predict_batch(self, dataset, batch_size=1, top_k=None, reuse_preds=None):
         """
         Runs the ensemble on a dataset in batches.
 
         Args:
         - dataset: a dataset of documents to run entity linking on
         - batch_size: an integer representing the batch size to use
         - top_k: an optional integer representing the number of top entities to keep per document
```

### Comparing `xmen-0.9.5/xmen/linkers/faiss_indexer.py` & `xmen-0.9.6/xmen/linkers/faiss_indexer.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/linkers/sap_bert_linker.py` & `xmen-0.9.6/xmen/linkers/sap_bert_linker.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 
 from xmen.linkers.faiss_indexer import DenseFlatIndexer, DenseHNSWFlatIndexer
 
 from xmen.log import logger
 
 from scipy.spatial.distance import cosine
 
-_SAP_BERT_XLMR = "cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR"
-_SAP_BERT_EN = "cambridgeltl/SapBERT-from-PubMedBERT-fulltext"
-
 _EMBED_DIM = 768
 
 
 class SapBERTLinker(EntityLinker):
     """
     A class that performs entity linking using the SapBERT model.
 
@@ -28,22 +25,23 @@
     - index_base_path (Union[Path, str]): Path to the directory where the index files are located.
     - kb_name (str): The name of the knowledge base to use.
     - cuda (bool): Whether to use the GPU for inference or not.
     - gpu_batch_size (int): Batch size for inference on GPU.
     - k (int): The number of closest neighbors to retrieve from the index.
     - threshold (float): A threshold value for filtering out candidate entities based on their similarity score.
     - filter_types (bool): Whether to filter out candidate entities based on their semantic type.
-    - embedding_model_name (str): Name of the embedding model to use.
-    - consider_n_grams (list): A list of integers representing the number of grams to consider when generating candidate entities.
+    - model_name (str): Name of the embedding model to use.
     - remove_duplicates (bool): Whether to remove duplicate candidate entities or not.
     - expand_abbreviations (bool): Whether to expand abbreviations or not.
     - approximate (bool): Whether to use the hierarchical index for faster inference or not.
-    - unique_aliases_only (bool): Whether to use only unique aliases of entities for linking or not.
     """
 
+    CROSS_LINGUAL = "cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR"
+    ENGLISH = "cambridgeltl/SapBERT-from-PubMedBERT-fulltext"
+
     # Global state
     instance = None
     model_wrapper = None
     candidate_dense_embeds = None
     term_dict = None
 
     # Ignore caching when using dataset.map
@@ -59,27 +57,27 @@
         SapBERTLinker.candidate_dense_embeds = None
         SapBERTLinker.term_dict = None
 
     @staticmethod
     def write_index(
         index_base_path: Union[str, Path],
         term_dict: dict,
-        embedding_model_name: str = _SAP_BERT_XLMR,
+        model_name: str = CROSS_LINGUAL,
         cuda: bool = True,
         subtract_mean=True,
         batch_size=2048 * 6,
         write_flat=False,
     ):
         """
         Write index files to disk.
 
         Args:
         - index_base_path (Union[str, Path]): Path to the directory where the index files will be written.
         - term_dict (dict): A dictionary containing the terms to include in the index.
-        - embedding_model_name (str): Name of the embedding model to use.
+        - model_name (str): Name of the embedding model to use.
         - cuda (bool): Whether to use the GPU for inference or not.
         - subtract_mean (bool): Whether to subtract the mean from the embeddings or not.
         - batch_size (int): Batch size for embedding generation.
         - write_flat (bool): Whether to write the flat index to disk or not.
         """
         index_base_path = Path(index_base_path)
 
@@ -88,17 +86,17 @@
         out_dict_file = index_base_path / "dict.pickle"
         out_faiss_flat_file = index_base_path / "embed_faiss_flat.pickle"
         out_faiss_hier_file = index_base_path / "embed_faiss_hier.pickle"
 
         term_dict.to_pickle(out_dict_file)
 
         wrapper = Model_Wrapper()
-        wrapper.load_model(embedding_model_name, use_cuda=cuda)
+        wrapper.load_model(model_name, use_cuda=cuda)
 
-        logger.info(f"Computing dictionary embeddings with {embedding_model_name}")
+        logger.info(f"Computing dictionary embeddings with {model_name}")
         candidate_dense_embeds = wrapper.embed_dense(
             term_dict.term.tolist(),
             agg_mode="cls",
             use_cuda=cuda,
             show_progress=True,
             batch_size=batch_size,
         )
@@ -124,29 +122,26 @@
         self,
         index_base_path: Union[Path, str],
         kb_name: str = "UMLS",
         cuda=True,
         gpu_batch_size: int = 16,
         k: int = 10,
         threshold: float = 0.0,
-        filter_types: bool = False,
-        embedding_model_name: str = _SAP_BERT_XLMR,
-        consider_n_grams: list = [],
+        model_name: str = CROSS_LINGUAL,
         remove_duplicates=True,
-        expand_abbreviations=False,
+        expand_abbreviations=True,
         approximate=True,
-        unique_aliases_only=False,
     ):
         index_base_path = Path(index_base_path)
         term_dict_pkl = index_base_path / "dict.pickle"
 
         if SapBERTLinker.instance:
             raise Exception("SapBERTLinker is a singleton")
         SapBERTLinker.model_wrapper = Model_Wrapper()
-        SapBERTLinker.model_wrapper.load_model(embedding_model_name, use_cuda=cuda)
+        SapBERTLinker.model_wrapper.load_model(model_name, use_cuda=cuda)
         self.cuda = cuda
         if approximate:
             logger.info("Loading hierarchical faiss index")
             self.indexer = DenseHNSWFlatIndexer(_EMBED_DIM)
             self.indexer.deserialize_from(str(index_base_path / "embed_faiss_hier.pickle"))
         else:
             logger.info("Loading flat faiss index")
@@ -157,26 +152,22 @@
         #    SapBERTLinker.candidate_dense_embeds = pickle.load(f)
         with open(term_dict_pkl, "rb") as f:
             SapBERTLinker.term_dict = pd.read_pickle(f)
             self.term_dict_idx = SapBERTLinker.term_dict.set_index("cui")
         self.k = k
         self.kb_name = kb_name
         self.threshold = threshold
-        self.filter_types = filter_types
-        self.consider_n_grams = consider_n_grams
-        self.filter_types = filter_types
         self.gpu_batch_size = gpu_batch_size
         self.remove_duplicates = remove_duplicates
         self.expand_abbreviations = expand_abbreviations
-        self.unique_aliases_only = unique_aliases_only
 
         SapBERTLinker.instance = self
         self.valid = True
 
-    def predict_batch(self, dataset, batch_size):
+    def predict_batch(self, dataset, batch_size=1):
         """
         Perform entity linking on a batch of sentences.
 
         Args:
         - dataset (Dataset): A `Dataset` object containing the sentences to link entities in.
         - batch_size (int): The batch size to use for linking.
```

### Comparing `xmen-0.9.5/xmen/linkers/tf_idf_ngram_linker.py` & `xmen-0.9.6/xmen/linkers/tf_idf_ngram_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/linkers/util.py` & `xmen-0.9.6/xmen/linkers/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/reranking/cross_encoder.py` & `xmen-0.9.6/xmen/reranking/cross_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from xmen.reranking.scored_cross_encoder import ScoredInputExample, ScoredCrossEncoder
 from xmen.reranking.ranking_util import get_flat_candidate_ds
 
 from sentence_transformers.readers import InputExample
 from sentence_transformers.cross_encoder import CrossEncoder
 from torch.utils.data import DataLoader
 
+from transformers.trainer_utils import set_seed
+
 from sentence_transformers.cross_encoder.evaluation import (
     CEBinaryClassificationEvaluator,
 )
 
 from datasets import DatasetDict
 from xmen.data import IndexedDatasetDict, IndexedDataset
 
@@ -193,34 +195,39 @@
     """
 
     def __init__(self, args: dict):
         self.args = args
 
     def __init__(
         self,
-        model_name: str,
         num_train_epochs: int,
+        model_name: str = "bert-base-multilingual-cased",
         fp16: bool = True,
         label_smoothing: bool = False,
         score_regularization: bool = False,
         train_layers: list = None,
         softmax_loss: bool = True,
+        random_seed: int = 42,
     ):
         self.args = {}
         self.args["model_name"] = model_name
         self.args["num_train_epochs"] = num_train_epochs
         self.args["fp16"] = fp16
         self.args["label_smoothing"] = label_smoothing
         self.args["score_regularization"] = score_regularization
         self.args["train_layers"] = train_layers
         self.args["softmax_loss"] = softmax_loss
+        self.args["random_seed"] = random_seed
 
     def __getitem__(self, key):
         return self.args[key]
 
+    def get(self, key, default_val):
+        return self.args.get(key, default_val)
+
 
 class CrossEncoderReranker(Reranker):
     """
     Reranker that uses a cross-encoder to score a set of candidate passages against a query.
     Inherits from the abstract class Reranker.
     """
 
@@ -291,29 +298,31 @@
                 encode_sem_type,
                 masking,
             )
             return IndexedDataset(ds, doc_index)
 
     def fit(
         self,
+        training_args: CrossEncoderTrainingArgs,
         train_dataset,
         val_dataset,
-        output_dir: Union[str, Path],
-        training_args: CrossEncoderTrainingArgs,
+        output_dir: Union[str, Path] = "./output/cross_encoder",
         train_continue=False,
         loss_fct=None,
         callback=None,
         add_special_tokens=True,
         max_length=512,
         eval_callback=None,
+        show_progress_bar=True,
     ):
         """
         Fits the model using the given training and validation datasets.
 
         Args:
+        - training_args: Training Arguments
         - train_dataset (List[InputExample]): The list of InputExample objects representing the training dataset.
         - val_dataset (List[InputExample]): The list of InputExample objects representing the validation dataset.
         - output_dir (Union[str, Path]): The directory where the trained model will be saved.
         - train_continue (bool, optional): If True, the training will be continued from the current state of the model. Defaults to False.
         - softmax_loss (bool, optional): If True, uses CrossEntropyLoss as the loss function. Otherwise, no loss function is used. Defaults to True.
         - loss_fct (optional): The loss function to be used. If None, the function will be automatically set based on the value of softmax_loss. Defaults to None.
         - callback (optional): A callback function to be called at the end of each epoch. Defaults to None.
@@ -324,14 +333,15 @@
         - **training_args: A dictionary containing the training arguments to be passed to the ScoredCrossEncoder model.
 
         Raises:
         - AssertionError: If train_continue is False and the model already exists.
         """
         for k, v in training_args.args.items():
             print(k, ":=", v)
+        set_seed(training_args.get("random_seed", 0))
         if not self.model:
             self.model = ScoredCrossEncoder(training_args["model_name"], num_labels=1, max_length=max_length)
             if add_special_tokens:
                 self.model.tokenizer.add_special_tokens({"additional_special_tokens": ["[START]", "[END]", "[TITLE]"]})
                 self.model.model.resize_token_embeddings(len(self.model.tokenizer))
         else:
             assert train_continue, "Training must be continued if model is set"
@@ -367,14 +377,15 @@
             warmup_steps=100,
             output_path=output_dir,
             callback=callback,
             use_amp=training_args["fp16"],
             label_smoothing=training_args["label_smoothing"],
             score_regularization=training_args["score_regularization"],
             train_layers=training_args["train_layers"],
+            show_progress_bar=show_progress_bar,
         )
 
     def rerank_batch(self, candidates, cross_enc_dataset, show_progress_bar=True, convert_to_numpy=True):
         """
         Re-ranks a batch of candidates using a cross encoder and returns the re-ranked candidates.
 
         Args:
```

### Comparing `xmen-0.9.5/xmen/reranking/list_wise.py` & `xmen-0.9.6/xmen/reranking/list_wise.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/reranking/multiple_choice_util.py` & `xmen-0.9.6/xmen/reranking/multiple_choice_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/reranking/ranking_util.py` & `xmen-0.9.6/xmen/reranking/ranking_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/reranking/rule_based.py` & `xmen-0.9.6/xmen/reranking/rule_based.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/reranking/scored_cross_encoder.py` & `xmen-0.9.6/xmen/reranking/scored_cross_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,17 +141,14 @@
         :param max_grad_norm: Used for gradient normalization.
         :param use_amp: Use Automatic Mixed Precision (AMP). Only for Pytorch >= 1.6.0
         :param callback: Callback function that is invoked after each evaluation.
                 It must accept the following three parameters in this order:
                 `score`, `epoch`, `steps`
         :param show_progress_bar: If True, output a tqdm progress bar
         """
-        print("Using score regularization:", score_regularization)
-        print("Using label smoothing factor:", label_smoothing)
-
         train_dataloader.collate_fn = self.smart_batching_collate_with_scores
 
         if use_amp:
             from torch.cuda.amp import autocast
 
             scaler = torch.cuda.amp.GradScaler()
```

### Comparing `xmen-0.9.5/xmen/resources/SemGroups-v03.txt` & `xmen-0.9.6/xmen/resources/SemGroups-v03.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/resources/SemGroups.txt` & `xmen-0.9.6/xmen/resources/SemGroups.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/xmen/umls.py` & `xmen-0.9.6/xmen/umls.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.5/PKG-INFO` & `xmen-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmen
-Version: 0.9.5
+Version: 0.9.6
 Summary: An extensible toolkit for Cross-lingual (x) Medical Entity Normalization.
 Home-page: https://github.com/hpi-dhc/xmen
 License: Apache-2.0
 Author: Florian Borchert
 Author-email: florian.borchert@hpi.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -46,14 +46,18 @@
 
 `pip install xmen`
 
 ### Development
 
 We use [Poetry](https://python-poetry.org/) for building, testing and dependency management (see [pyproject.toml](pyproject.toml)).
 
+## 🚀 Getting Started
+
+A very simple pipeline highlighting the main components of xMEN can be found in [notebooks/Getting_Started.ipynb](notebooks/Getting_Started.ipynb)
+
 ## 📂 Data Loading
 
 Usually, BigBIO-compatible datasets can just be loaded from the Hugging Face Hub:
 
 ```
 from datasets import load_dataset
 dataset = load_dataset("distemist", "distemist_linking_bigbio_kb")
@@ -173,16 +177,15 @@
 Based on the implementation from [scispaCy](https://github.com/allenai/scispacy).
 
 YAML file:
 
 ```
 linker:
   candidate_generation:
-    ngram:
-      k: 100
+    ngram: ~
 ```
 
 Run `xmen index my_config.yaml --ngram` or `xmen index my_config.yaml --all` to create the index.
 
 To use the linker at runtime, pass the index folder as an argument:
 
 ```
@@ -200,34 +203,32 @@
 
 YAML file:
 
 ```
 linker:
   candidate_generation:
     sapbert:
-      embedding_model_name: cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR
-      k: 1000
+      model_name: cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR
 ```
 
 Run `xmen index my_config.yaml --sapbert` or `xmen index my_config.yaml --all` to create the [FAISS](https://github.com/facebookresearch/faiss) index.
 
-To use the linker at runtime, pass the `embedding_model_name` (usually the same as was used for creating the index)  and index folder as an argument. To make predictions on a batch of documents, you have to pass a batch size, as the SapBERT linker runs on the GPU by default:
+To use the linker at runtime, pass the index folder as an argument. To make predictions on a batch of documents, you have to pass a batch size, as the SapBERT linker runs on the GPU by default:
 
 ```
 from xmen.linkers import SapBERTLinker
 
 sapbert_linker = SapBERTLinker(
-    embedding_model_name = "cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR", # Name of SapBERT model
     index_base_path = "/path/to/my/index/sapbert",
     k = 1000
 )
 predictions = sapbert_linker.predict_batch(dataset, batch_size=128)
 ```
 
-If you have loaded a yaml-config as a dictionary, you may also just pass it as kwargs:
+If you have loaded a yaml-config as a dictionary-like object, you may also just pass it as kwargs:
 
 ```
 sapbert_linker = SapBERTLinker(**config)
 ```
 
 By default, SapBERT assumes a CUDA device is available. If you want to disable cuda, pass `cuda=False` to the constructor.
 
@@ -270,33 +271,39 @@
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 from xmen.kb import load_kb
 
 # Load a KB from a pre-computed dictionary (jsonl) to obtain synonyms for concept encoding
 kb = load_kb('path/to/my/dictionary.jsonl')
 
-candidates = linker.predict_batch(dataset) # obtain prediction from candidate generator (see above)
+# Obtain prediction from candidate generator (see above)
+candidates = linker.predict_batch(dataset)
 
 cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb)
 ```
 
 Then you can use this dataset to train a supervised reranking model:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 
-cross_encoder_model = 'bert-base-multilingual-cased' # any BERT model, potentially language specific
-n_epochs = 10 # number of epochs to train
-output_dir = './checkpoints/' # Path to temp dir for writing model checkpoints
+# Number of epochs to train
+n_epochs = 10
 
-train_args = CrossEncoderTrainingArgs(cross_encoder_model, n_epochs)
+# Any BERT model, potentially language-specific
+cross_encoder_model = 'bert-base-multilingual-cased'
+
+args = CrossEncoderTrainingArgs(n_epochs, cross_encoder_model)
 
 rr = CrossEncoderReranker()
-rr.fit(cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset, output_dir=output_dir, training_args=train_args)
 
+# Fit the model
+rr.fit(args, cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset)
+
+# Predict on test set
 prediction = rr.rerank_batch(candidates['test'], cross_enc_ds['test'])
 ```
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
```

