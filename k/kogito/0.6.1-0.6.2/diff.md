# Comparing `tmp/kogito-0.6.1.tar.gz` & `tmp/kogito-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kogito-0.6.1.tar", max compression
+gzip compressed data, was "kogito-0.6.2.tar", max compression
```

## Comparing `kogito-0.6.1.tar` & `kogito-0.6.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11357 2022-07-29 09:05:29.707808 kogito-0.6.1/LICENSE
--rw-r--r--   0        0        0     5058 2023-05-05 10:18:16.890873 kogito-0.6.1/README.md
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.816174 kogito-0.6.1/kogito/__init__.py
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.816532 kogito-0.6.1/kogito/core/__init__.py
--rw-r--r--   0        0        0     4934 2022-07-29 09:05:29.817445 kogito-0.6.1/kogito/core/callbacks.py
--rw-r--r--   0        0        0     6728 2022-10-04 14:17:07.318721 kogito-0.6.1/kogito/core/dataset.py
--rw-r--r--   0        0        0     2055 2022-11-19 17:18:37.281727 kogito-0.6.1/kogito/core/head.py
--rw-r--r--   0        0        0    11915 2023-05-05 09:45:45.099950 kogito-0.6.1/kogito/core/knowledge.py
--rw-r--r--   0        0        0     4400 2022-11-19 17:54:55.647284 kogito-0.6.1/kogito/core/linker.py
--rw-r--r--   0        0        0     4297 2022-07-29 09:05:29.819956 kogito-0.6.1/kogito/core/model.py
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.820047 kogito-0.6.1/kogito/core/processors/__init__.py
--rw-r--r--   0        0        0  8825499 2022-07-29 09:05:29.900729 kogito-0.6.1/kogito/core/processors/data/vocab_glove_100d.npy
--rw-r--r--   0        0        0     5026 2023-05-05 09:45:44.608786 kogito-0.6.1/kogito/core/processors/head.py
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.903291 kogito-0.6.1/kogito/core/processors/models/__init__.py
--rw-r--r--   0        0        0     4319 2022-07-29 09:05:29.904943 kogito-0.6.1/kogito/core/processors/models/bert.py
--rw-r--r--   0        0        0     4477 2022-07-29 09:05:29.906400 kogito-0.6.1/kogito/core/processors/models/distilbert.py
--rw-r--r--   0        0        0     5340 2022-07-29 09:05:29.907930 kogito-0.6.1/kogito/core/processors/models/swem.py
--rw-r--r--   0        0        0     5600 2023-06-07 23:48:30.564321 kogito-0.6.1/kogito/core/processors/models/utils.py
--rw-r--r--   0        0        0     8522 2023-05-05 09:45:44.982119 kogito-0.6.1/kogito/core/processors/relation.py
--rw-r--r--   0        0        0    18434 2023-05-05 09:45:45.746383 kogito-0.6.1/kogito/core/relation.py
--rw-r--r--   0        0        0     6736 2023-05-05 09:45:45.275349 kogito-0.6.1/kogito/core/utils.py
--rw-r--r--   0        0        0     1069 2022-07-29 09:05:29.928015 kogito-0.6.1/kogito/evaluation/LICENSE
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.928144 kogito-0.6.1/kogito/evaluation/__init__.py
--rwxr-xr-x   0        0        0        0 2022-07-29 09:05:29.928254 kogito-0.6.1/kogito/evaluation/bert_score/__init__.py
--rw-r--r--   0        0        0     1192 2022-07-29 09:05:29.935361 kogito-0.6.1/kogito/evaluation/bert_score/bert_score.py
--rw-r--r--   0        0        0     1694 2022-07-29 09:05:29.940448 kogito-0.6.1/kogito/evaluation/bert_score/score.py
--rw-r--r--   0        0        0     8315 2022-07-29 09:05:29.946249 kogito-0.6.1/kogito/evaluation/bert_score/utils.py
--rw-r--r--   0        0        0        6 2022-07-29 09:05:29.950984 kogito-0.6.1/kogito/evaluation/bleu/.gitignore
--rwxr-xr-x   0        0        0     1105 2022-07-29 09:05:29.951225 kogito-0.6.1/kogito/evaluation/bleu/LICENSE
--rwxr-xr-x   0        0        0       21 2022-07-29 09:05:29.956642 kogito-0.6.1/kogito/evaluation/bleu/__init__.py
--rw-r--r--   0        0        0     1265 2022-07-29 09:05:29.957640 kogito-0.6.1/kogito/evaluation/bleu/bleu.py
--rwxr-xr-x   0        0        0     8812 2022-07-29 09:05:29.958040 kogito-0.6.1/kogito/evaluation/bleu/bleu_scorer.py
--rwxr-xr-x   0        0        0       21 2022-07-29 09:05:29.958283 kogito-0.6.1/kogito/evaluation/cider/__init__.py
--rwxr-xr-x   0        0        0     1718 2022-07-29 09:05:29.958879 kogito-0.6.1/kogito/evaluation/cider/cider.py
--rw-r--r--   0        0        0     7771 2022-07-29 09:05:29.959320 kogito-0.6.1/kogito/evaluation/cider/cider_scorer.py
--rwxr-xr-x   0        0        0     1535 2022-07-29 09:05:29.959700 kogito-0.6.1/kogito/evaluation/eval.py
--rwxr-xr-x   0        0        0       21 2022-07-29 09:05:29.959926 kogito-0.6.1/kogito/evaluation/meteor/__init__.py
--rwxr-xr-x   0        0        0      809 2022-07-29 09:05:29.960287 kogito-0.6.1/kogito/evaluation/meteor/meteor.py
--rwxr-xr-x   0        0        0       23 2022-07-29 09:05:29.960644 kogito-0.6.1/kogito/evaluation/rouge/__init__.py
--rwxr-xr-x   0        0        0     3717 2022-07-29 09:05:29.961118 kogito-0.6.1/kogito/evaluation/rouge/rouge.py
--rw-r--r--   0        0        0    10247 2023-05-05 09:47:08.239965 kogito-0.6.1/kogito/inference.py
--rw-r--r--   0        0        0     5144 2022-11-19 17:54:23.886470 kogito-0.6.1/kogito/linkers/deberta.py
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.961921 kogito-0.6.1/kogito/models/__init__.py
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.962016 kogito-0.6.1/kogito/models/bart/__init__.py
--rw-r--r--   0        0        0     8104 2023-05-05 09:45:45.520621 kogito-0.6.1/kogito/models/bart/comet.py
--rw-r--r--   0        0        0     1299 2022-07-29 09:05:29.963101 kogito-0.6.1/kogito/models/bart/config.py
--rw-r--r--   0        0        0    17791 2022-07-29 09:05:29.963594 kogito-0.6.1/kogito/models/bart/utils.py
--rw-r--r--   0        0        0        0 2022-07-29 09:05:29.963714 kogito-0.6.1/kogito/models/gpt2/__init__.py
--rw-r--r--   0        0        0     7695 2023-05-05 09:45:45.583772 kogito-0.6.1/kogito/models/gpt2/comet.py
--rw-r--r--   0        0        0     1117 2022-07-29 09:05:29.965064 kogito-0.6.1/kogito/models/gpt2/utils.py
--rw-r--r--   0        0        0     3331 2023-05-05 09:45:45.407765 kogito-0.6.1/kogito/models/gpt2/zeroshot.py
--rw-r--r--   0        0        0        0 2023-05-05 09:40:07.971015 kogito-0.6.1/kogito/models/gpt3/__init__.py
--rw-r--r--   0        0        0     5171 2023-05-05 09:47:13.417221 kogito-0.6.1/kogito/models/gpt3/zeroshot.py
--rw-r--r--   0        0        0     1162 2023-06-07 23:49:55.340347 kogito-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6598 1970-01-01 00:00:00.000000 kogito-0.6.1/setup.py
--rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 kogito-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-29 09:05:29.707808 kogito-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5058 2023-05-05 10:18:16.890873 kogito-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.816174 kogito-0.6.2/kogito/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.816532 kogito-0.6.2/kogito/core/__init__.py
+-rw-r--r--   0        0        0     4934 2022-07-29 09:05:29.817445 kogito-0.6.2/kogito/core/callbacks.py
+-rw-r--r--   0        0        0     6728 2022-10-04 14:17:07.318721 kogito-0.6.2/kogito/core/dataset.py
+-rw-r--r--   0        0        0     2055 2022-11-19 17:18:37.281727 kogito-0.6.2/kogito/core/head.py
+-rw-r--r--   0        0        0    11915 2023-05-05 09:45:45.099950 kogito-0.6.2/kogito/core/knowledge.py
+-rw-r--r--   0        0        0     4400 2022-11-19 17:54:55.647284 kogito-0.6.2/kogito/core/linker.py
+-rw-r--r--   0        0        0     4297 2022-07-29 09:05:29.819956 kogito-0.6.2/kogito/core/model.py
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.820047 kogito-0.6.2/kogito/core/processors/__init__.py
+-rw-r--r--   0        0        0  8825499 2022-07-29 09:05:29.900729 kogito-0.6.2/kogito/core/processors/data/vocab_glove_100d.npy
+-rw-r--r--   0        0        0     5026 2023-05-05 09:45:44.608786 kogito-0.6.2/kogito/core/processors/head.py
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.903291 kogito-0.6.2/kogito/core/processors/models/__init__.py
+-rw-r--r--   0        0        0     4319 2022-07-29 09:05:29.904943 kogito-0.6.2/kogito/core/processors/models/bert.py
+-rw-r--r--   0        0        0     4477 2022-07-29 09:05:29.906400 kogito-0.6.2/kogito/core/processors/models/distilbert.py
+-rw-r--r--   0        0        0     5340 2022-07-29 09:05:29.907930 kogito-0.6.2/kogito/core/processors/models/swem.py
+-rw-r--r--   0        0        0     5562 2023-06-08 00:18:09.418131 kogito-0.6.2/kogito/core/processors/models/utils.py
+-rw-r--r--   0        0        0     8522 2023-05-05 09:45:44.982119 kogito-0.6.2/kogito/core/processors/relation.py
+-rw-r--r--   0        0        0    18434 2023-05-05 09:45:45.746383 kogito-0.6.2/kogito/core/relation.py
+-rw-r--r--   0        0        0     6736 2023-05-05 09:45:45.275349 kogito-0.6.2/kogito/core/utils.py
+-rw-r--r--   0        0        0     1069 2022-07-29 09:05:29.928015 kogito-0.6.2/kogito/evaluation/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.928144 kogito-0.6.2/kogito/evaluation/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-07-29 09:05:29.928254 kogito-0.6.2/kogito/evaluation/bert_score/__init__.py
+-rw-r--r--   0        0        0     1192 2022-07-29 09:05:29.935361 kogito-0.6.2/kogito/evaluation/bert_score/bert_score.py
+-rw-r--r--   0        0        0     1694 2022-07-29 09:05:29.940448 kogito-0.6.2/kogito/evaluation/bert_score/score.py
+-rw-r--r--   0        0        0     8315 2022-07-29 09:05:29.946249 kogito-0.6.2/kogito/evaluation/bert_score/utils.py
+-rw-r--r--   0        0        0        6 2022-07-29 09:05:29.950984 kogito-0.6.2/kogito/evaluation/bleu/.gitignore
+-rwxr-xr-x   0        0        0     1105 2022-07-29 09:05:29.951225 kogito-0.6.2/kogito/evaluation/bleu/LICENSE
+-rwxr-xr-x   0        0        0       21 2022-07-29 09:05:29.956642 kogito-0.6.2/kogito/evaluation/bleu/__init__.py
+-rw-r--r--   0        0        0     1265 2022-07-29 09:05:29.957640 kogito-0.6.2/kogito/evaluation/bleu/bleu.py
+-rwxr-xr-x   0        0        0     8812 2022-07-29 09:05:29.958040 kogito-0.6.2/kogito/evaluation/bleu/bleu_scorer.py
+-rwxr-xr-x   0        0        0       21 2022-07-29 09:05:29.958283 kogito-0.6.2/kogito/evaluation/cider/__init__.py
+-rwxr-xr-x   0        0        0     1718 2022-07-29 09:05:29.958879 kogito-0.6.2/kogito/evaluation/cider/cider.py
+-rw-r--r--   0        0        0     7771 2022-07-29 09:05:29.959320 kogito-0.6.2/kogito/evaluation/cider/cider_scorer.py
+-rwxr-xr-x   0        0        0     1535 2022-07-29 09:05:29.959700 kogito-0.6.2/kogito/evaluation/eval.py
+-rwxr-xr-x   0        0        0       21 2022-07-29 09:05:29.959926 kogito-0.6.2/kogito/evaluation/meteor/__init__.py
+-rwxr-xr-x   0        0        0      809 2022-07-29 09:05:29.960287 kogito-0.6.2/kogito/evaluation/meteor/meteor.py
+-rwxr-xr-x   0        0        0       23 2022-07-29 09:05:29.960644 kogito-0.6.2/kogito/evaluation/rouge/__init__.py
+-rwxr-xr-x   0        0        0     3717 2022-07-29 09:05:29.961118 kogito-0.6.2/kogito/evaluation/rouge/rouge.py
+-rw-r--r--   0        0        0    10247 2023-05-05 09:47:08.239965 kogito-0.6.2/kogito/inference.py
+-rw-r--r--   0        0        0     5144 2022-11-19 17:54:23.886470 kogito-0.6.2/kogito/linkers/deberta.py
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.961921 kogito-0.6.2/kogito/models/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.962016 kogito-0.6.2/kogito/models/bart/__init__.py
+-rw-r--r--   0        0        0     8104 2023-05-05 09:45:45.520621 kogito-0.6.2/kogito/models/bart/comet.py
+-rw-r--r--   0        0        0     1299 2022-07-29 09:05:29.963101 kogito-0.6.2/kogito/models/bart/config.py
+-rw-r--r--   0        0        0    17791 2022-07-29 09:05:29.963594 kogito-0.6.2/kogito/models/bart/utils.py
+-rw-r--r--   0        0        0        0 2022-07-29 09:05:29.963714 kogito-0.6.2/kogito/models/gpt2/__init__.py
+-rw-r--r--   0        0        0     7695 2023-05-05 09:45:45.583772 kogito-0.6.2/kogito/models/gpt2/comet.py
+-rw-r--r--   0        0        0     1117 2022-07-29 09:05:29.965064 kogito-0.6.2/kogito/models/gpt2/utils.py
+-rw-r--r--   0        0        0     3331 2023-05-05 09:45:45.407765 kogito-0.6.2/kogito/models/gpt2/zeroshot.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:40:07.971015 kogito-0.6.2/kogito/models/gpt3/__init__.py
+-rw-r--r--   0        0        0     5171 2023-05-05 09:47:13.417221 kogito-0.6.2/kogito/models/gpt3/zeroshot.py
+-rw-r--r--   0        0        0     1162 2023-06-08 00:18:23.840327 kogito-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6598 1970-01-01 00:00:00.000000 kogito-0.6.2/setup.py
+-rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 kogito-0.6.2/PKG-INFO
```

### Comparing `kogito-0.6.1/LICENSE` & `kogito-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/README.md` & `kogito-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/callbacks.py` & `kogito-0.6.2/kogito/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/dataset.py` & `kogito-0.6.2/kogito/core/dataset.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/head.py` & `kogito-0.6.2/kogito/core/head.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/knowledge.py` & `kogito-0.6.2/kogito/core/knowledge.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/linker.py` & `kogito-0.6.2/kogito/core/linker.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/model.py` & `kogito-0.6.2/kogito/core/model.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/processors/data/vocab_glove_100d.npy` & `kogito-0.6.2/kogito/core/processors/data/vocab_glove_100d.npy`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/processors/head.py` & `kogito-0.6.2/kogito/core/processors/head.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/processors/models/bert.py` & `kogito-0.6.2/kogito/core/processors/models/bert.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/processors/models/distilbert.py` & `kogito-0.6.2/kogito/core/processors/models/distilbert.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/processors/models/swem.py` & `kogito-0.6.2/kogito/core/processors/models/swem.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/processors/models/utils.py` & `kogito-0.6.2/kogito/core/processors/models/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             train_recall_macro=torchmetrics.Recall(task="multiclass", num_classes=3, average="macro"),
             train_f1_macro=torchmetrics.F1Score(task="multiclass", num_classes=3, average="macro"),
             # (per class)
             train_precision_class=torchmetrics.Precision(task="multiclass", num_classes=3, average="none"),
             train_recall_class=torchmetrics.Recall(task="multiclass", num_classes=3, average="none"),
             train_f1_class=torchmetrics.F1Score(task="multiclass", num_classes=3, average="none"),
             # Validation metrics
-            val_accuracy=torchmetrics.Accuracy(task="multiclass", task="multiclass", num_classes=3),
+            val_accuracy=torchmetrics.Accuracy(task="multiclass", num_classes=3),
             # (weighted)
             val_precision=torchmetrics.Precision(task="multiclass", num_classes=3, average="weighted"),
             val_recall=torchmetrics.Recall(task="multiclass", num_classes=3, average="weighted"),
             val_f1=torchmetrics.F1Score(task="multiclass", num_classes=3, average="weighted"),
             # (micro)
             val_precision_micro=torchmetrics.Precision(task="multiclass", num_classes=3, average="micro"),
             val_recall_micro=torchmetrics.Recall(task="multiclass", num_classes=3, average="micro"),
@@ -59,15 +59,15 @@
             val_recall_macro=torchmetrics.Recall(task="multiclass", num_classes=3, average="macro"),
             val_f1_macro=torchmetrics.F1Score(task="multiclass", num_classes=3, average="macro"),
             # (per class)
             val_precision_class=torchmetrics.Precision(task="multiclass", num_classes=3, average="none"),
             val_recall_class=torchmetrics.Recall(task="multiclass", num_classes=3, average="none"),
             val_f1_class=torchmetrics.F1Score(task="multiclass", num_classes=3, average="none"),
             # Test metrics
-            test_accuracy=torchmetrics.Accuracy(task="multiclass", task="multiclass", num_classes=3),
+            test_accuracy=torchmetrics.Accuracy(task="multiclass", num_classes=3),
             # (weighted)
             test_precision=torchmetrics.Precision(task="multiclass", num_classes=3, average="weighted"),
             test_recall=torchmetrics.Recall(task="multiclass", num_classes=3, average="weighted"),
             test_f1=torchmetrics.F1Score(task="multiclass", num_classes=3, average="weighted"),
             # (micro)
             test_precision_micro=torchmetrics.Precision(task="multiclass", num_classes=3, average="micro"),
             test_recall_micro=torchmetrics.Recall(task="multiclass", num_classes=3, average="micro"),
```

### Comparing `kogito-0.6.1/kogito/core/processors/relation.py` & `kogito-0.6.2/kogito/core/processors/relation.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/relation.py` & `kogito-0.6.2/kogito/core/relation.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/core/utils.py` & `kogito-0.6.2/kogito/core/utils.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/LICENSE` & `kogito-0.6.2/kogito/evaluation/LICENSE`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/bert_score/bert_score.py` & `kogito-0.6.2/kogito/evaluation/bert_score/bert_score.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/bert_score/score.py` & `kogito-0.6.2/kogito/evaluation/bert_score/score.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/bert_score/utils.py` & `kogito-0.6.2/kogito/evaluation/bert_score/utils.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/bleu/LICENSE` & `kogito-0.6.2/kogito/evaluation/bleu/LICENSE`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/bleu/bleu.py` & `kogito-0.6.2/kogito/evaluation/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/bleu/bleu_scorer.py` & `kogito-0.6.2/kogito/evaluation/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/cider/cider.py` & `kogito-0.6.2/kogito/evaluation/cider/cider.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/cider/cider_scorer.py` & `kogito-0.6.2/kogito/evaluation/cider/cider_scorer.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/eval.py` & `kogito-0.6.2/kogito/evaluation/eval.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/meteor/meteor.py` & `kogito-0.6.2/kogito/evaluation/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/evaluation/rouge/rouge.py` & `kogito-0.6.2/kogito/evaluation/rouge/rouge.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/inference.py` & `kogito-0.6.2/kogito/inference.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/linkers/deberta.py` & `kogito-0.6.2/kogito/linkers/deberta.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/bart/comet.py` & `kogito-0.6.2/kogito/models/bart/comet.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/bart/config.py` & `kogito-0.6.2/kogito/models/bart/config.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/bart/utils.py` & `kogito-0.6.2/kogito/models/bart/utils.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/gpt2/comet.py` & `kogito-0.6.2/kogito/models/gpt2/comet.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/gpt2/utils.py` & `kogito-0.6.2/kogito/models/gpt2/utils.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/gpt2/zeroshot.py` & `kogito-0.6.2/kogito/models/gpt2/zeroshot.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/kogito/models/gpt3/zeroshot.py` & `kogito-0.6.2/kogito/models/gpt3/zeroshot.py`

 * *Files identical despite different names*

### Comparing `kogito-0.6.1/pyproject.toml` & `kogito-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kogito"
-version = "0.6.1"
+version = "0.6.2"
 description = "A Python NLP Commonsense Knowledge Inference Toolkit"
 authors = ["Mete Ismayil <mahammad.ismayilzada@epfl.ch>", "Antoine Bosselut <antoine.bosselut@epfl.ch>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/epfl-nlp/kogito"
 repository = "https://github.com/epfl-nlp/kogito"
 documentation = "https://github.com/epfl-nlp/kogito"
```

### Comparing `kogito-0.6.1/setup.py` & `kogito-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'spacy>=3.2.3,<4.0.0',
  'torch>=1.10.1,<2.0.0',
  'transformers>=4.15.0,<5.0.0',
  'wandb>=0.12.9,<0.13.0']
 
 setup_kwargs = {
     'name': 'kogito',
-    'version': '0.6.1',
+    'version': '0.6.2',
     'description': 'A Python NLP Commonsense Knowledge Inference Toolkit',
     'long_description': '# kogito\nA Python NLP Commonsense Knowledge Inference Toolkit\n\nSystem Description available here: https://arxiv.org/abs/2211.08451\n\n## Installation\n\n### Installation with pip\n**kogito** can be installed using pip.\n\n```sh\npip install kogito\n```\n\nIt requires a minimum ``python`` version of ``3.8``.\n\n## Setup\n\n### Inference\n**kogito** uses [spacy](https://spacy.io) under the hood for various text processing purposes, so, a [spacy](https://spacy.io) language package has to be installed before running the inference module.\n\n```sh\npython -m spacy download en_core_web_sm\n``` \nBy default, ``CommonsenseInference`` module uses ``en_core_web_sm`` to initialize ``spacy`` pipeline, but a different language pipeline can be specified as well.\n\n### Evaluation\nIf you also would like evaluate knowledge models using `METEOR` score, then you need to download the following ``nltk`` libraries:\n```python\nimport nltk\n\nnltk.download("punkt")\nnltk.download("wordnet")\nnltk.download("omw-1.4")\n```\n\n## Quickstart\n**kogito** provides an easy interface to interact with knowledge inference or commonsense reasoning models such as [COMET](https://arxiv.org/abs/2010.05953) to generate inferences from a text input.\nHere is a sample usage of the library where you can initialize an inference module, a custom commonsense reasoning model, and generate a knowledge graph from text on the fly.\n\n```python\nfrom kogito.models.bart.comet import COMETBART\nfrom kogito.inference import CommonsenseInference\n\n# Load pre-trained model from HuggingFace\nmodel = COMETBART.from_pretrained("mismayil/comet-bart-ai2")\n\n# Initialize inference module with a spacy language pipeline\ncsi = CommonsenseInference(language="en_core_web_sm")\n\n# Run inference\ntext = "PersonX becomes a great basketball player"\nkgraph = csi.infer(text, model)\n\n# Save output knowledge graph to JSON file\nkgraph.to_jsonl("kgraph.json")\n```\n\nHere is an excerpt from the result of the above code sample:\n\n```json\n{"head": "PersonX becomes a great basketball player", "relation": "Causes", "tails": [" PersonX practices every day.", " PersonX plays basketball every day", " PersonX practices every day"]}\n{"head": "basketball", "relation": "ObjectUse", "tails": [" play with friends", " play basketball with", " play basketball"]}\n{"head": "player", "relation": "CapableOf", "tails": [" play game", " win game", " play football"]}\n{"head": "great basketball player", "relation": "HasProperty", "tails": [" good at basketball", " good at sports", " very good"]}\n{"head": "become player", "relation": "isAfter", "tails": [" play game", " become coach", " play with"]}\n```\nThis is just one way to generate commonsense inferences and **kogito** offers much more. For complete documentation, check out the [kogito docs](https://kogito.readthedocs.io).\n\n## Development\n\n### Setup\n**kogito** uses [Poetry](https://python-poetry.org/) to manage its dependencies. \n\nInstall poetry from the official repository first:\n```sh\ncurl -sSL https://install.python-poetry.org | python3 -\n```\n\nThen run the following command to install package dependencies:\n```sh\npoetry install\n```\n\n## Data\nIf you need the ATOMIC2020 data to train your knowledge models, you can download it from AI2:\n\nFor ATOMIC:\n```sh\nwget https://storage.googleapis.com/ai2-mosaic/public/atomic/v1.0/atomic_data.tgz\n```\n\nFor ATOMIC 2020:\n```sh\nwget https://ai2-atomic.s3-us-west-2.amazonaws.com/data/atomic2020_data-feb2021.zip\n```\n\n## Paper\nIf you want to learn more about the library design, models and data used for this toolkit, check out our [paper](https://arxiv.org/abs/2211.08451). The paper can be cited as:\n\n```\n@article{Ismayilzada2022kogito,\n  title={kogito: A Commonsense Knowledge Inference Toolkit},\n  author={Mete Ismayilzada and Antoine Bosselut},\n  journal={ArXiv},\n  volume={abs/2211.08451},\n  year={2022}\n}\n```\n\nIf you work with knowledge models, consider citing the following papers:\n\n```\n@article{Hwang2020COMETATOMIC,\n author = {Jena D. Hwang and Chandra Bhagavatula and Ronan Le Bras and Jeff Da and Keisuke Sakaguchi and Antoine Bosselut and Yejin Choi},\n booktitle = {Proceedings of the 35th AAAI Conference on Artificial Intelligence (AAAI)},\n title = {COMET-ATOMIC 2020: On Symbolic and Neural Commonsense Knowledge Graphs},\n year = {2021}\n}\n\n@inproceedings{Bosselut2019COMETCT,\n author = {Antoine Bosselut and Hannah Rashkin and Maarten Sap and Chaitanya Malaviya and Asli Çelikyilmaz and Yejin Choi},\n booktitle = {Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics (ACL)},\n title = {COMET: Commonsense Transformers for Automatic Knowledge Graph Construction},\n year = {2019}\n}\n```\n\n## Acknowledgements\nSignificant portion of the model training and evaluation code has been adapted from the original [codebase](https://github.com/allenai/comet-atomic-2020) for the paper [(Comet-) Atomic 2020: On Symbolic and Neural Commonsense Knowledge Graphs.](https://www.semanticscholar.org/paper/COMET-ATOMIC-2020%3A-On-Symbolic-and-Neural-Knowledge-Hwang-Bhagavatula/e39503e01ebb108c6773948a24ca798cd444eb62)\n',
     'author': 'Mete Ismayil',
     'author_email': 'mahammad.ismayilzada@epfl.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/epfl-nlp/kogito',
```

### Comparing `kogito-0.6.1/PKG-INFO` & `kogito-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kogito
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python NLP Commonsense Knowledge Inference Toolkit
 Home-page: https://github.com/epfl-nlp/kogito
 License: Apache-2.0
 Keywords: natural language processing,nlp,natural language understanding,commonsense reasoning,commonsense inference,knowledge inference
 Author: Mete Ismayil
 Author-email: mahammad.ismayilzada@epfl.ch
 Requires-Python: >=3.8,<3.11
```

