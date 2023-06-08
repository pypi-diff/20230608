# Comparing `tmp/frame_semantic_transformer-0.8.2.tar.gz` & `tmp/frame_semantic_transformer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frame_semantic_transformer-0.8.2.tar", max compression
+gzip compressed data, was "frame_semantic_transformer-0.9.0.tar", max compression
```

## Comparing `frame_semantic_transformer-0.8.2.tar` & `frame_semantic_transformer-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1069 2023-04-15 11:31:48.764542 frame_semantic_transformer-0.8.2/LICENSE
--rw-r--r--   0        0        0     6650 2023-04-15 11:31:48.764542 frame_semantic_transformer-0.8.2/README.md
--rw-r--r--   0        0        0     8667 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/FrameSemanticTransformer.py
--rw-r--r--   0        0        0      606 2023-04-15 11:31:49.472555 frame_semantic_transformer-0.8.2/frame_semantic_transformer/__init__.py
--rw-r--r--   0        0        0      223 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/constants.py
--rw-r--r--   0        0        0     4969 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/LoaderDataCache.py
--rw-r--r--   0        0        0     3652 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/TaskSampleDataset.py
--rw-r--r--   0        0        0     1203 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DataAugmentation.py
--rw-r--r--   0        0        0     2148 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py
--rw-r--r--   0        0        0     1946 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py
--rw-r--r--   0        0        0      465 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/LowercaseAugmentation.py
--rw-r--r--   0        0        0     1061 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py
--rw-r--r--   0        0        0     1842 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py
--rw-r--r--   0        0        0     2144 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py
--rw-r--r--   0        0        0     1433 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py
--rw-r--r--   0        0        0      809 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py
--rw-r--r--   0        0        0      932 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/__init__.py
--rw-r--r--   0        0        0      552 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/chain_augmentations.py
--rw-r--r--   0        0        0      267 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/__init__.py
--rw-r--r--   0        0        0      572 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py
--rw-r--r--   0        0        0     1789 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py
--rw-r--r--   0        0        0     4141 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py
--rw-r--r--   0        0        0     4518 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/data_utils.py
--rw-r--r--   0        0        0     1335 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/frame_types.py
--rw-r--r--   0        0        0     2699 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py
--rw-r--r--   0        0        0     5659 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py
--rw-r--r--   0        0        0      209 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/__init__.py
--rw-r--r--   0        0        0      174 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/ensure_framenet_downloaded.py
--rw-r--r--   0        0        0      279 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/ensure_wordnet_downloaded.py
--rw-r--r--   0        0        0     1235 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py
--rw-r--r--   0        0        0     2582 2023-04-15 11:31:48.772543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/loader.py
--rw-r--r--   0        0        0     1661 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py
--rw-r--r--   0        0        0     6404 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py
--rw-r--r--   0        0        0      209 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/__init__.py
--rw-r--r--   0        0        0      603 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py
--rw-r--r--   0        0        0     1296 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py
--rw-r--r--   0        0        0     2479 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py
--rw-r--r--   0        0        0     2356 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py
--rw-r--r--   0        0        0     1107 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationSample.py
--rw-r--r--   0        0        0     2202 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationTask.py
--rw-r--r--   0        0        0      610 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/Task.py
--rw-r--r--   0        0        0      952 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TaskSample.py
--rw-r--r--   0        0        0     2766 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py
--rw-r--r--   0        0        0      634 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py
--rw-r--r--   0        0        0      685 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/__init__.py
--rw-r--r--   0        0        0     2118 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks_from_annotated_sentences.py
--rw-r--r--   0        0        0     3443 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/predict.py
--rw-r--r--   0        0        0     1038 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/evaluate.py
--rw-r--r--   0        0        0     1195 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/train.py
--rw-r--r--   0        0        0     3400 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/ModelRecorder.py
--rw-r--r--   0        0        0     1773 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingDataModule.py
--rw-r--r--   0        0        0     8397 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingModelWrapper.py
--rw-r--r--   0        0        0      186 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/__init__.py
--rw-r--r--   0        0        0     4714 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_batch.py
--rw-r--r--   0        0        0     1454 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_best_val_models.py
--rw-r--r--   0        0        0     3388 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_model.py
--rw-r--r--   0        0        0     1925 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/find_best_val_model_paths.py
--rw-r--r--   0        0        0     5400 2023-04-15 11:31:48.776543 frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/train.py
--rw-r--r--   0        0        0      982 2023-04-15 11:31:49.472555 frame_semantic_transformer-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     7655 1970-01-01 00:00:00.000000 frame_semantic_transformer-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-08 17:49:50.195558 frame_semantic_transformer-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7332 2023-06-08 17:49:50.195558 frame_semantic_transformer-0.9.0/README.md
+-rw-r--r--   0        0        0    10777 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/FrameSemanticTransformer.py
+-rw-r--r--   0        0        0      606 2023-06-08 17:49:50.951557 frame_semantic_transformer-0.9.0/frame_semantic_transformer/__init__.py
+-rw-r--r--   0        0        0      223 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/constants.py
+-rw-r--r--   0        0        0     4969 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/LoaderDataCache.py
+-rw-r--r--   0        0        0     3652 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/TaskSampleDataset.py
+-rw-r--r--   0        0        0     1203 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/DataAugmentation.py
+-rw-r--r--   0        0        0     2148 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py
+-rw-r--r--   0        0        0     1946 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py
+-rw-r--r--   0        0        0      465 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/LowercaseAugmentation.py
+-rw-r--r--   0        0        0     1061 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py
+-rw-r--r--   0        0        0     1842 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py
+-rw-r--r--   0        0        0     2144 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py
+-rw-r--r--   0        0        0     1433 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py
+-rw-r--r--   0        0        0      809 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py
+-rw-r--r--   0        0        0      932 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/__init__.py
+-rw-r--r--   0        0        0      552 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/chain_augmentations.py
+-rw-r--r--   0        0        0      267 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/__init__.py
+-rw-r--r--   0        0        0      572 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py
+-rw-r--r--   0        0        0     1789 2023-06-08 17:49:50.203558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py
+-rw-r--r--   0        0        0     4141 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py
+-rw-r--r--   0        0        0     4518 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/data_utils.py
+-rw-r--r--   0        0        0     1335 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/frame_types.py
+-rw-r--r--   0        0        0     2699 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py
+-rw-r--r--   0        0        0     5659 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py
+-rw-r--r--   0        0        0      209 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/ensure_framenet_downloaded.py
+-rw-r--r--   0        0        0      279 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/ensure_wordnet_downloaded.py
+-rw-r--r--   0        0        0     1235 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py
+-rw-r--r--   0        0        0     2582 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/loader.py
+-rw-r--r--   0        0        0     1661 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py
+-rw-r--r--   0        0        0     6404 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py
+-rw-r--r--   0        0        0      209 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py
+-rw-r--r--   0        0        0     1296 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py
+-rw-r--r--   0        0        0     2479 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py
+-rw-r--r--   0        0        0     2356 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py
+-rw-r--r--   0        0        0     1107 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/FrameClassificationSample.py
+-rw-r--r--   0        0        0     2202 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/FrameClassificationTask.py
+-rw-r--r--   0        0        0      610 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/Task.py
+-rw-r--r--   0        0        0      952 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/TaskSample.py
+-rw-r--r--   0        0        0     2766 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py
+-rw-r--r--   0        0        0      634 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py
+-rw-r--r--   0        0        0      685 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/__init__.py
+-rw-r--r--   0        0        0     2118 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks_from_annotated_sentences.py
+-rw-r--r--   0        0        0     3443 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/predict.py
+-rw-r--r--   0        0        0     1038 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/scripts/evaluate.py
+-rw-r--r--   0        0        0     1195 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/scripts/train.py
+-rw-r--r--   0        0        0     3400 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/ModelRecorder.py
+-rw-r--r--   0        0        0     1773 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/TrainingDataModule.py
+-rw-r--r--   0        0        0     8397 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/TrainingModelWrapper.py
+-rw-r--r--   0        0        0      186 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/__init__.py
+-rw-r--r--   0        0        0     4714 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/evaluate_batch.py
+-rw-r--r--   0        0        0     1454 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/evaluate_best_val_models.py
+-rw-r--r--   0        0        0     3388 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/evaluate_model.py
+-rw-r--r--   0        0        0     1925 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/find_best_val_model_paths.py
+-rw-r--r--   0        0        0     5400 2023-06-08 17:49:50.207558 frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/train.py
+-rw-r--r--   0        0        0     1000 2023-06-08 17:49:50.951557 frame_semantic_transformer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8337 1970-01-01 00:00:00.000000 frame_semantic_transformer-0.9.0/PKG-INFO
```

### Comparing `frame_semantic_transformer-0.8.2/LICENSE` & `frame_semantic_transformer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/README.md` & `frame_semantic_transformer-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,27 @@
 result = frame_transformer.detect_frames_bulk([
     "I'm getting quite hungry, but I can wait a bit longer.",
     "The chef gave the food to the customer.",
     "The hallway smelt of boiled cabbage and old rag mats.",
 ])
 ```
 
+**Note**: It's not recommended to pass more than a single sentence per string to `detect_frames()` or `detect_frames_bulk()`. If you have a paragraph of text to process, it's best to split the paragraph into a list of sentences and pass the sentences as a list to `detect_frames_bulk()`. Only single sentences per string were used during training, so it's not clear how the model will handle multiple sentences in the same string.
+
+```python
+# ❌ Bad, don't do this
+frame_transformer.detect_frames("Fuzzy Wuzzy was a bear. Fuzzy Wuzzy had no hair.")
+
+# 👍 Do this instead
+frame_transformer.detect_frames_bulk([
+  "Fuzzy Wuzzy was a bear.",
+  "Fuzzy Wuzzy had no hair.",
+])
+```
+
 ### Running on GPU vs CPU
 
 By default, `FrameSemanticTransformer` will attempt to use a GPU if one is available. If you'd like to explictly set whether to run on GPU vs CPU, you can pass the `use_gpu` param.
 
 ```python
 # force the model to run on the CPU
 frame_transformer = FrameSemanticTransformer(use_gpu=False)
@@ -102,14 +115,15 @@
 ## License
 
 The code contained in this repo is released under a MIT license, however the pretrained models are released under an Apache 2.0 license in accordance with FrameNet training data and HuggingFace's T5 base models.
 
 ## Citation
 
 If you use Frame semantic transformer in your work, please cite the following:
+
 ```bibtex
 @article{chanin2023opensource,
   title={Open-source Frame Semantic Parsing},
   author={Chanin, David},
   journal={arXiv preprint arXiv:2303.12788},
   year={2023}
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/__init__.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 from .FrameSemanticTransformer import (
     FrameSemanticTransformer,
     DetectFramesResult,
     FrameElementResult,
     FrameResult,
 )
```

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/LoaderDataCache.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/LoaderDataCache.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/TaskSampleDataset.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/TaskSampleDataset.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DataAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/DoubleQuotesAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/KeyboardAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/RemoveEndPunctuationAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/SimpleMisspellingAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/StripPunctuationAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/SynonymAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/UppercaseAugmentation.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/__init__.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/chain_augmentations.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/chain_augmentations.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/get_sample_text.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/modify_text_without_changing_length.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/augmentations/modification_helpers/splice_text.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/data_utils.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/frame_types.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/frame_types.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/Framenet17InferenceLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/Framenet17TrainingLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/framenet17/sesame_data_splits.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/loader.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/Propbank34InferenceLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/Propbank34TrainingLoader.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/ensure_propbank_downloaded.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/loaders/propbank34/load_propbank_frames.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/ArgumentsExtractionSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/ArgumentsExtractionTask.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationSample.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/FrameClassificationSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/FrameClassificationTask.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/FrameClassificationTask.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/Task.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/Task.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TaskSample.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/TaskSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/TriggerIdentificationSample.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/TriggerIdentificationTask.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks/__init__.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/data/tasks_from_annotated_sentences.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/data/tasks_from_annotated_sentences.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/predict.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/predict.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/evaluate.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/scripts/evaluate.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/scripts/train.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/scripts/train.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/ModelRecorder.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/ModelRecorder.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingDataModule.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/TrainingDataModule.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/TrainingModelWrapper.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/TrainingModelWrapper.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_batch.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/evaluate_batch.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_best_val_models.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/evaluate_best_val_models.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/evaluate_model.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/find_best_val_model_paths.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/find_best_val_model_paths.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/frame_semantic_transformer/training/train.py` & `frame_semantic_transformer-0.9.0/frame_semantic_transformer/training/train.py`

 * *Files identical despite different names*

### Comparing `frame_semantic_transformer-0.8.2/pyproject.toml` & `frame_semantic_transformer-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frame-semantic-transformer"
-version = "0.8.2"
+version = "0.9.0"
 description = "Frame Semantic Parser based on T5 and FrameNet"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chanind/frame-semantic-transformer"
 authors = ["David Chanin <chanindav@gmail.com>"]
 
 [tool.poetry.dependencies]
@@ -21,14 +21,15 @@
 pytest = "^5.2"
 black = "^22.3.0"
 mypy = "^0.950"
 flake8 = "^4.0.1"
 syrupy = "^2.0.0"
 pygments = "^2.14.0"
 furo = "^2022.12.7"
+torch = "^1.13.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = [
```

### Comparing `frame_semantic_transformer-0.8.2/PKG-INFO` & `frame_semantic_transformer-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frame-semantic-transformer
-Version: 0.8.2
+Version: 0.9.0
 Summary: Frame Semantic Parser based on T5 and FrameNet
 Home-page: https://github.com/chanind/frame-semantic-transformer
 License: MIT
 Author: David Chanin
 Author-email: chanindav@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -88,14 +88,27 @@
 result = frame_transformer.detect_frames_bulk([
     "I'm getting quite hungry, but I can wait a bit longer.",
     "The chef gave the food to the customer.",
     "The hallway smelt of boiled cabbage and old rag mats.",
 ])
 ```
 
+**Note**: It's not recommended to pass more than a single sentence per string to `detect_frames()` or `detect_frames_bulk()`. If you have a paragraph of text to process, it's best to split the paragraph into a list of sentences and pass the sentences as a list to `detect_frames_bulk()`. Only single sentences per string were used during training, so it's not clear how the model will handle multiple sentences in the same string.
+
+```python
+# ❌ Bad, don't do this
+frame_transformer.detect_frames("Fuzzy Wuzzy was a bear. Fuzzy Wuzzy had no hair.")
+
+# 👍 Do this instead
+frame_transformer.detect_frames_bulk([
+  "Fuzzy Wuzzy was a bear.",
+  "Fuzzy Wuzzy had no hair.",
+])
+```
+
 ### Running on GPU vs CPU
 
 By default, `FrameSemanticTransformer` will attempt to use a GPU if one is available. If you'd like to explictly set whether to run on GPU vs CPU, you can pass the `use_gpu` param.
 
 ```python
 # force the model to run on the CPU
 frame_transformer = FrameSemanticTransformer(use_gpu=False)
@@ -127,14 +140,15 @@
 ## License
 
 The code contained in this repo is released under a MIT license, however the pretrained models are released under an Apache 2.0 license in accordance with FrameNet training data and HuggingFace's T5 base models.
 
 ## Citation
 
 If you use Frame semantic transformer in your work, please cite the following:
+
 ```bibtex
 @article{chanin2023opensource,
   title={Open-source Frame Semantic Parsing},
   author={Chanin, David},
   journal={arXiv preprint arXiv:2303.12788},
   year={2023}
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

