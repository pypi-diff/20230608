# Comparing `tmp/PromptEHR-0.0.5.tar.gz` & `tmp/PromptEHR-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PromptEHR-0.0.5.tar", last modified: Wed Jan 11 19:35:29 2023, max compression
+gzip compressed data, was "PromptEHR-0.0.6.tar", last modified: Thu Jun  8 05:25:35 2023, max compression
```

## Comparing `PromptEHR-0.0.5.tar` & `PromptEHR-0.0.6.tar`

### file list

```diff
@@ -1,142 +1,156 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1063 2022-05-21 16:44:50.000000 PromptEHR-0.0.5/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3165 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PKG-INFO
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PromptEHR.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3165 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PromptEHR.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4478 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PromptEHR.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PromptEHR.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       75 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PromptEHR.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       18 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/PromptEHR.egg-info/top_level.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2530 2023-01-09 06:53:36.000000 PromptEHR-0.0.5/README.md
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/promptehr/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      143 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8576 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/bart_model.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      787 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/constants.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9431 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    31397 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/dataset.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1686 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/demo_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1968 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/evaluator.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    72762 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/generator.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10485 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/model.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4704 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/modeling_bart.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10409 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/modeling_config.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    28061 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/modeling_promptbart.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    31276 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/promptehr.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20697 2023-01-11 19:34:15.000000 PromptEHR-0.0.5/promptehr/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      266 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/data/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-26 22:43:18.000000 PromptEHR-0.0.5/pytrial/data/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10756 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/data/demo_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/data/drug_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14996 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/data/patient_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7040 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/data/trial_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/data/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      807 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/data/vocab_data.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-06-04 06:34:14.000000 PromptEHR-0.0.5/pytrial/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4722 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/model_utils/bert.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    18920 2022-06-12 05:32:09.000000 PromptEHR-0.0.5/pytrial/model_utils/drug.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10785 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/model_utils/icd.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-28 16:27:50.000000 PromptEHR-0.0.5/pytrial/tasks/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-26 22:43:18.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/causal/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-27 05:55:40.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/causal/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/confidence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-28 01:19:42.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/confidence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1681 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11361 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20846 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/dipole.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13446 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/raim.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10711 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/retain.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13118 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/rnn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15457 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/stagenet.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9858 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/mlp.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/transtab.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7553 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/xgboost.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/site_selection/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-26 22:43:18.000000 PromptEHR-0.0.5/pytrial/tasks/site_selection/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_opt/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-08-31 19:56:11.000000 PromptEHR-0.0.5/pytrial/tasks/trial_opt/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       86 2022-08-31 19:56:11.000000 PromptEHR-0.0.5/pytrial/tasks/trial_opt/shapley.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      124 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    40457 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/hint.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/mlp.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/dataloader.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7926 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/module.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13678 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4734 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6722 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_outcome/xgboost.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/compose.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/deepenroll.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2022-08-31 19:56:11.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-27 05:27:47.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-08-31 19:56:11.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/bm25.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/doc2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/trial2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_search/models/whiten_bert.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2022-05-26 22:43:18.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      109 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9976 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/eva.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9651 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7388 2023-01-11 18:58:48.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/promptehr.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/synteg.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      126 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14713 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/copula_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8085 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/ct_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3867 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9360 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/tvae.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/tasks/trial_simulation/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/pytrial/utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2022-06-06 05:06:05.000000 PromptEHR-0.0.5/pytrial/utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2022-08-31 19:56:11.000000 PromptEHR-0.0.5/pytrial/utils/check.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2022-06-04 17:58:23.000000 PromptEHR-0.0.5/pytrial/utils/mimic_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/utils/parallel.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12713 2022-11-16 21:01:19.000000 PromptEHR-0.0.5/pytrial/utils/tabular_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17980 2022-11-16 21:01:12.000000 PromptEHR-0.0.5/pytrial/utils/trainer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2022-06-23 03:54:07.000000 PromptEHR-0.0.5/pytrial/utils/trial_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-01-11 19:35:29.000000 PromptEHR-0.0.5/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1164 2023-01-11 19:34:41.000000 PromptEHR-0.0.5/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.916034 PromptEHR-0.0.6/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1063 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3180 2023-06-08 05:25:35.916034 PromptEHR-0.0.6/PKG-INFO
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.897034 PromptEHR-0.0.6/PromptEHR.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3180 2023-06-08 05:25:35.000000 PromptEHR-0.0.6/PromptEHR.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5136 2023-06-08 05:25:35.000000 PromptEHR-0.0.6/PromptEHR.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-06-08 05:25:35.000000 PromptEHR-0.0.6/PromptEHR.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       75 2023-06-08 05:25:35.000000 PromptEHR-0.0.6/PromptEHR.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       18 2023-06-08 05:25:35.000000 PromptEHR-0.0.6/PromptEHR.egg-info/top_level.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2530 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/README.md
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.899034 PromptEHR-0.0.6/promptehr/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      143 2023-06-08 05:23:30.000000 PromptEHR-0.0.6/promptehr/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8576 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/bart_model.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      787 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/constants.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9431 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    31397 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/dataset.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1658 2023-06-08 05:01:56.000000 PromptEHR-0.0.6/promptehr/demo_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1968 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/evaluator.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    36318 2023-06-08 04:56:06.000000 PromptEHR-0.0.6/promptehr/generator.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10566 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/model.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4704 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/modeling_bart.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10410 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/modeling_config.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    28208 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/modeling_promptbart.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    31581 2023-06-08 04:46:00.000000 PromptEHR-0.0.6/promptehr/promptehr.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21004 2023-06-08 05:18:18.000000 PromptEHR-0.0.6/promptehr/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.899034 PromptEHR-0.0.6/pytrial/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.900034 PromptEHR-0.0.6/pytrial/data/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/data/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10893 2023-06-08 04:09:26.000000 PromptEHR-0.0.6/pytrial/data/demo_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/data/drug_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15741 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/data/patient_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    22007 2023-06-08 04:09:26.000000 PromptEHR-0.0.6/pytrial/data/site_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13918 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/data/trial_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/data/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/data/vocab_data.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.901034 PromptEHR-0.0.6/pytrial/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/model_utils/bert.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/model_utils/drug.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/model_utils/icd.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.901034 PromptEHR-0.0.6/pytrial/tasks/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.902034 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.902034 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/causal/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/causal/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.902034 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/confidence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/confidence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.903034 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/dipole.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/raim.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/retain.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/rnn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/stagenet.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.904034 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/mlp.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/transtab.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/xgboost.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.905034 PromptEHR-0.0.6/pytrial/tasks/site_selection/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8739 2023-06-08 04:09:26.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    18343 2023-06-08 04:30:44.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/framm.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5941 2023-06-08 04:09:26.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/metrics.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8185 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/pgentropy.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/site_selection/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.907034 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      147 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2335 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2167 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41581 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/hint.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/mlp.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.909034 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7751 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/data_structure.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2934 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/data_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/dataloader.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8303 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/module.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12827 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5784 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8295 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    33283 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/spot.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_outcome/xgboost.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.909034 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.910034 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/compose.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/deepenroll.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.910034 PromptEHR-0.0.6/pytrial/tasks/trial_search/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.912034 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/bm25.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/doc2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/trial2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_search/models/whiten_bert.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.913034 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.914034 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      159 2023-06-08 04:09:26.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/eva.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/knn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/promptehr.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/synteg.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21920 2023-06-08 04:09:26.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/twin.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.915034 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/copula_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/ct_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15310 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/med_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/tvae.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/tasks/trial_simulation/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-06-08 05:25:35.916034 PromptEHR-0.0.6/pytrial/utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/utils/check.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/utils/mimic_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/utils/parallel.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16479 2023-06-08 04:45:25.000000 PromptEHR-0.0.6/pytrial/utils/tabular_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/utils/trainer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-06-08 04:09:15.000000 PromptEHR-0.0.6/pytrial/utils/trial_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-06-08 05:25:35.916034 PromptEHR-0.0.6/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1181 2023-06-08 05:23:55.000000 PromptEHR-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PromptEHR-0.0.5/LICENSE` & `PromptEHR-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/PKG-INFO` & `PromptEHR-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PromptEHR
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sequence patient electronic healthcare record generation with large language models (LLMs) as the neural database.
 Home-page: https://github.com/RyanWangZf/PromptEHR
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
-Keywords: healthcare,EHR,deep learning,AI
+Keywords: synthetic data,healthcare,EHR,deep learning,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PromptEHR-0.0.5/PromptEHR.egg-info/PKG-INFO` & `PromptEHR-0.0.6/PromptEHR.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PromptEHR
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sequence patient electronic healthcare record generation with large language models (LLMs) as the neural database.
 Home-page: https://github.com/RyanWangZf/PromptEHR
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
-Keywords: healthcare,EHR,deep learning,AI
+Keywords: synthetic data,healthcare,EHR,deep learning,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PromptEHR-0.0.5/PromptEHR.egg-info/SOURCES.txt` & `PromptEHR-0.0.6/PromptEHR.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 promptehr/promptehr.py
 promptehr/trainer.py
 pytrial/__init__.py
 pytrial/data/__init__.py
 pytrial/data/demo_data.py
 pytrial/data/drug_data.py
 pytrial/data/patient_data.py
+pytrial/data/site_data.py
 pytrial/data/trial_data.py
 pytrial/data/utils.py
 pytrial/data/vocab_data.py
 pytrial/model_utils/__init__.py
 pytrial/model_utils/bert.py
 pytrial/model_utils/drug.py
 pytrial/model_utils/icd.py
@@ -51,29 +52,40 @@
 pytrial/tasks/indiv_outcome/tabular/base.py
 pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
 pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
 pytrial/tasks/indiv_outcome/tabular/mlp.py
 pytrial/tasks/indiv_outcome/tabular/transtab.py
 pytrial/tasks/indiv_outcome/tabular/xgboost.py
 pytrial/tasks/site_selection/__init__.py
-pytrial/tasks/trial_opt/__init__.py
-pytrial/tasks/trial_opt/shapley.py
+pytrial/tasks/site_selection/base.py
+pytrial/tasks/site_selection/data.py
+pytrial/tasks/site_selection/framm.py
+pytrial/tasks/site_selection/losses.py
+pytrial/tasks/site_selection/metrics.py
+pytrial/tasks/site_selection/pgentropy.py
+pytrial/tasks/site_selection/trainer.py
 pytrial/tasks/trial_outcome/__init__.py
 pytrial/tasks/trial_outcome/base.py
+pytrial/tasks/trial_outcome/data.py
+pytrial/tasks/trial_outcome/evaluation.py
 pytrial/tasks/trial_outcome/hint.py
 pytrial/tasks/trial_outcome/logistic_regression.py
 pytrial/tasks/trial_outcome/mlp.py
+pytrial/tasks/trial_outcome/spot.py
 pytrial/tasks/trial_outcome/xgboost.py
 pytrial/tasks/trial_outcome/model_utils/__init__.py
+pytrial/tasks/trial_outcome/model_utils/data_structure.py
+pytrial/tasks/trial_outcome/model_utils/data_utils.py
 pytrial/tasks/trial_outcome/model_utils/dataloader.py
 pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
 pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
 pytrial/tasks/trial_outcome/model_utils/module.py
 pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
 pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
+pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
 pytrial/tasks/trial_outcome/model_utils/utils.py
 pytrial/tasks/trial_patient_match/__init__.py
 pytrial/tasks/trial_patient_match/data.py
 pytrial/tasks/trial_patient_match/losses.py
 pytrial/tasks/trial_patient_match/trainer.py
 pytrial/tasks/trial_patient_match/models/__init__.py
 pytrial/tasks/trial_patient_match/models/base.py
@@ -93,23 +105,26 @@
 pytrial/tasks/trial_simulation/data.py
 pytrial/tasks/trial_simulation/losses.py
 pytrial/tasks/trial_simulation/trainer.py
 pytrial/tasks/trial_simulation/sequence/__init__.py
 pytrial/tasks/trial_simulation/sequence/base.py
 pytrial/tasks/trial_simulation/sequence/eva.py
 pytrial/tasks/trial_simulation/sequence/evaluation.py
+pytrial/tasks/trial_simulation/sequence/knn.py
 pytrial/tasks/trial_simulation/sequence/promptehr.py
 pytrial/tasks/trial_simulation/sequence/rnn_gan.py
 pytrial/tasks/trial_simulation/sequence/synteg.py
+pytrial/tasks/trial_simulation/sequence/twin.py
 pytrial/tasks/trial_simulation/tabular/__init__.py
 pytrial/tasks/trial_simulation/tabular/base.py
 pytrial/tasks/trial_simulation/tabular/copula_gan.py
 pytrial/tasks/trial_simulation/tabular/ct_gan.py
 pytrial/tasks/trial_simulation/tabular/evaluation.py
 pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
+pytrial/tasks/trial_simulation/tabular/med_gan.py
 pytrial/tasks/trial_simulation/tabular/tvae.py
 pytrial/utils/__init__.py
 pytrial/utils/check.py
 pytrial/utils/mimic_utils.py
 pytrial/utils/parallel.py
 pytrial/utils/tabular_utils.py
 pytrial/utils/trainer.py
```

### Comparing `PromptEHR-0.0.5/README.md` & `PromptEHR-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/bart_model.py` & `PromptEHR-0.0.6/promptehr/bart_model.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/constants.py` & `PromptEHR-0.0.6/promptehr/constants.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/data.py` & `PromptEHR-0.0.6/promptehr/data.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/dataset.py` & `PromptEHR-0.0.6/promptehr/dataset.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/demo_data.py` & `PromptEHR-0.0.6/promptehr/demo_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 
 #     return return_dict
 
 def load_synthetic_data(input_dir='./demo_data/synthetic_ehr', n_sample=None):
     '''
     Load the generated synthetic EHRs by PromptEHR.
     '''
-    if input_dir is None or not os.path.exists(input_dir):
-        if input_dir is None:
-            input_dir = './demo_data/synthetic_ehr'
+    if input_dir is None:
+        input_dir = './demo_data/synthetic_ehr'
+
+    if not os.path.exists(input_dir):
         os.makedirs(input_dir)
         url = constants.SYNTHETIC_DATA_URL
         filename = wget.download(url, out=input_dir)
         print(f'Download synthetic EHRs to {input_dir}.')
     
     with open(os.path.join(input_dir,'data.pkl'), 'rb') as f:
         x = dill.load(f)
```

### Comparing `PromptEHR-0.0.5/promptehr/evaluator.py` & `PromptEHR-0.0.6/promptehr/evaluator.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/model.py` & `PromptEHR-0.0.6/promptehr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .modeling_config import EHRBartOutput
 from .modeling_config import DataTokenizer, ModelTokenizer
 from .modeling_config import EHRBartConfig
 from .modeling_promptbart import PromptBartModel
 from . import constants
 
 class BartForEHRSimulation(BartPretrainedModel, EHRGenerationMixin):
-    def __init__(self, config: EHRBartConfig, model_tokenizer: ModelTokenizer=None):
+    def __init__(self, config: EHRBartConfig, model_tokenizer: ModelTokenizer=None, data_tokenizer: DataTokenizer=None):
         super().__init__(config)
 
         config.is_decoder = False
         config.is_encoder_decoder = True # use both the inputs for encoders and decoders
 
         self.model = PromptBartModel(config)
 
@@ -36,14 +36,15 @@
         self.init_weights()
 
         # set embedding vocab new size
         self.resize_token_embeddings(config.data_tokenizer_num_vocab)
 
         # for specific modal generation
         self.model_tokenizer = model_tokenizer
+        self.data_tokenizer = data_tokenizer
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         decoder_input_ids=None,
         decoder_attention_mask=None,
```

### Comparing `PromptEHR-0.0.5/promptehr/modeling_bart.py` & `PromptEHR-0.0.6/promptehr/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/promptehr/modeling_config.py` & `PromptEHR-0.0.6/promptehr/modeling_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             tokenizer_dict[key] = specific_tokenizer
 
         # each code type has its own tokenizer corresponding to specific LM heads
         self.tokenizer_dict = tokenizer_dict
         self.num_token_dict = num_token_dict
         self.label_offset = offset
 
+
     def encode(self, input_ids, code_type):
         if len(input_ids.shape) > 1: # a batch
             ids = self.encode_batch(input_ids, code_type)
         else:
             ids = self.tokenizer_dict[code_type].encode(input_ids.cpu().numpy().astype(str), is_pretokenized=True).ids
             ids = torch.tensor(ids, device=input_ids.device)
         return ids
```

### Comparing `PromptEHR-0.0.5/promptehr/modeling_promptbart.py` & `PromptEHR-0.0.6/promptehr/modeling_promptbart.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,18 @@
 
     def forward(self, input_ids_shape: torch.Size, past_key_values_length: int = 0):
         """`input_ids_shape` is expected to be [bsz x seqlen]."""
         bsz, seq_len = input_ids_shape[:2]
         positions = torch.arange(
             past_key_values_length, past_key_values_length + seq_len, dtype=torch.long, device=self.weight.device
         )
-        return super().forward(positions + self.offset)
+        positions = positions + self.offset
+        positions = torch.minimum(positions, torch.ones_like(positions).to(positions.device)*1024)
+        res = super().forward(positions)
+        return res
 
 class PromptBartEncoder(BartEncoder):
     def __init__(self, config: BartConfig, embed_tokens: Optional[nn.Embedding] = None):
         super().__init__(config, embed_tokens)
         embed_dim = config.d_model
         self.embed_positions = BartLearnedPositionalEmbedding(
             config.max_position_embeddings,
```

### Comparing `PromptEHR-0.0.5/promptehr/promptehr.py` & `PromptEHR-0.0.6/promptehr/promptehr.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pdb
 import json
 import math
 import glob
 import random
 import copy
 from collections import defaultdict
+import warnings
 
 import dill
 import torch
 from torch import nn
 from torch.utils.data.dataloader import DataLoader
 from transformers import TrainingArguments
 import numpy as np
@@ -508,19 +509,21 @@
                 unq_codes = list(set(v))
                 self.data_tokenizer.add_token_to_code_vocab(unq_codes, k)
         
         self.model_tokenizer = ModelTokenizer(self.data_tokenizer)
         self.configuration = EHRBartConfig(self.data_tokenizer, self.model_tokenizer, n_num_feature=self.config['n_num_feature'], cat_cardinalities=self.config['cat_cardinalities'])
         self.data_tokenizer.update_special_token_config(code_types=self.config['code_type'])
 
-        # self.data_tokenizer.decode([50508, 51324,51461, 50597, 50918,]) 
-
-
     def _build_model(self):
-        self.model = BartForEHRSimulation(self.configuration, self.model_tokenizer)
+        self.model = BartForEHRSimulation(self.configuration, self.model_tokenizer, self.data_tokenizer)
+
+        # check if cuda is available using torch
+        if not torch.cuda.is_available():
+            warnings.warn('No GPU found, using CPU instead.')
+            self.device = 'cpu'
 
         if isinstance(self.device, list): 
             self._set_visible_device(self.device)
             self.model.cuda()
         elif 'cuda' in self.device: 
             self.model.cuda()
         else:
@@ -676,18 +679,23 @@
                         sample_gen_kwargs['x_num'] = data['x_num']
 
                     new_next_tokens = self.model.generate(input_ids, **sample_gen_kwargs)
 
                     # randomly pick / rm sub code overlap
                     new_next_tokens = new_next_tokens[:,1:-1]
                     new_next_tokens = np.setdiff1d(new_next_tokens[0].cpu(), code_prompt_idx[0].cpu())
-                    if num_code-len(sub_code) > len(new_next_tokens):
-                        new_sub_idxs = np.unique(np.random.choice(np.arange(len(new_next_tokens)), num_code-len(sub_code), replace=True))
-                    else:
-                        new_sub_idxs = np.unique(np.random.choice(np.arange(len(new_next_tokens)), num_code-len(sub_code), replace=False))
+                    
+                    try:
+                        if num_code-len(sub_code) > len(new_next_tokens):
+                            new_sub_idxs = np.unique(np.random.choice(np.arange(len(new_next_tokens)), num_code-len(sub_code), replace=True))
+                        else:
+                            new_sub_idxs = np.unique(np.random.choice(np.arange(len(new_next_tokens)), num_code-len(sub_code), replace=False))
+                    except:
+                        pdb.set_trace()
+                        pass
                     new_next_tokens = torch.tensor(new_next_tokens[None, new_sub_idxs]).to(code_prompt_idx.device)
 
                     # append to the synthetic record dict
                     code_str_list = tokenizer.batch_decode(new_next_tokens)[0]
 
                     # remove special tokens ahead of original code event
                     # e.g., `diag_384` -> `384`
```

### Comparing `PromptEHR-0.0.5/promptehr/trainer.py` & `PromptEHR-0.0.6/promptehr/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,19 @@
         
         with torch.no_grad():
             if has_labels:
                 with self.autocast_smart_context_manager():
                     loss, outputs = self.compute_loss(model, inputs, return_outputs=True, return_perplexity=True)
 
                 if loss is not None:
-                    loss = loss.item() # return ppl is a 0-d tensor
+                    if not isinstance(loss, torch.Tensor):
+                        # if more than one device is used
+                        raise ValueError("In prediction phase only one GPU should be used, expected `torch.Tensor` loss, get `{}` instead.".format(type(loss)))
+                    else:
+                        loss = loss.item() # return ppl is a 0-d tensor
                     loss = torch.tensor([loss])
 
                 if isinstance(outputs, dict):
                     logits = tuple(v for k, v in outputs.items() if k not in ignore_keys + ["loss"])
                 else:
                     logits = outputs[1:]
             else:
```

### Comparing `PromptEHR-0.0.5/pytrial/data/demo_data.py` & `PromptEHR-0.0.6/pytrial/data/demo_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         x['feature'] = x['feature'][:n_sample]
 
     return x
 
 
 def load_mimic_ehr_sequence(input_dir=None, n_sample=None):
     '''
-    Load real EHR patient sequence data, which needs to be accessed via https://physionet.org/content/mimiciii/1.4/.
+    Load EHR patient sequence data, which needs to be accessed via https://physionet.org/content/mimiciii/1.4/.
 
     Parameters
     ----------
     input_dir: str
         The folder that stores the demo data. If None, we will look for the demo data in
         './demo_data/demo_patient_sequence/ehr'.
     
@@ -164,45 +164,48 @@
         'visit_stage':v_stage,
         'relapse':label_relapse,
         'mortality':label_mortality,
     }
 
 def load_trial_outcome_data(input_dir=None, phase='I', split='train'):
     '''
-    Load trial outcome prediction (TOP) benchmark data from https://github.com/futianfan/clinical-trial-outcome-prediction.
+    Load trial outcome prediction (TOP) benchmark data.
 
     Parameters
     ----------
     input_dir: str
         The folder that stores the demo data. If None, we will download the demo data and save it
         to './demo_data/demo_trial_data'. Make sure to remove this folder if it is empty.
 
     phase: {'I','II','III'}
         The phase of the trial data. Can be 'I', 'II', 'III'.
     
     split: {'train', 'test', 'valid'}
         The split of the trial data. Can be 'train', 'test', 'valid'.
     '''
+
+    BENCHMARK_DATA_URL = 'https://storage.googleapis.com/pytrial/HINT-benchmark-data/hint_benchmark_dataset_w_date.zip'
+
     if input_dir is None:
-        input_dir = './demo_data/demo_trial_data'
-    
-    filename = 'phase_{}_{}.csv'.format(phase, split)
+        input_dir = './demo_data/demo_trial_outcome_data'
 
-    if not os.path.exists(os.path.join(input_dir, filename)):
-        if not os.path.exists(input_dir):
-            os.makedirs(input_dir)
-        url = TOP_URL + filename
-        df = pd.read_csv(url)
-        df.to_csv(os.path.join(input_dir, filename))
+    if not os.path.exists(input_dir):
+        os.makedirs(input_dir)
+        # download the benchmark data
+        wget.download(BENCHMARK_DATA_URL, out=input_dir)
+        # unzip filename
+        import zipfile
+        with zipfile.ZipFile(os.path.join(input_dir, 'hint_benchmark_dataset_w_date.zip'), 'r') as zip_ref:
+            zip_ref.extractall(input_dir)
         print(f'\n Download trial data to {input_dir}.')
     
-    else:
-        filename = os.path.join(input_dir, filename)
-        # load patient data
-        df = pd.read_csv(filename)
+    filename = 'phase_{}_{}.csv'.format(phase, split)
+    filename = os.path.join(input_dir, filename)
+    # load patient data
+    df = pd.read_csv(filename)
     return {'data':df}
 
 def load_trial_document_data(input_dir=None, 
     n_sample=None,
     source='preprocessed',
     date='20221001',
     ):
```

### Comparing `PromptEHR-0.0.5/pytrial/data/patient_data.py` & `PromptEHR-0.0.6/pytrial/data/patient_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 Basic patient data functions.
 '''
 import warnings
 import pdb
 import json
 import pickle
 import dill
-from collections import defaultdict
+from collections import defaultdict, OrderedDict
 import torch
 
 from torch.utils.data import Dataset, DataLoader
 import numpy as np
 
 from ..utils.tabular_utils import HyperTransformer
+from ..utils.tabular_utils import get_transformer
 
 class TabularPatientBase(Dataset):
     '''
     Base dataset class for tabular patient records. Subclass it if additional properties and functions
     are required to add for specific tasks. We make use `rdt`: https://docs.sdv.dev/rdt for transform
     and reverse transform of the tabular data.
 
@@ -26,19 +27,21 @@
         The input patient tabular format records.
 
     metadata: dict
         Contains the meta setups of the input data. It should contain the following keys:
 
         (1) `sdtypes`: dict, the data types of each column in the input data. The keys are the column
             names and the values are the data types. The data types can be one of the following:
-            'numerical', 'categorical', 'datetime'.
+            'numerical', 'categorical', 'datetime', 'boolean'.
 
         (2) `transformers`: dict, the transformers to be used for each column. The keys are the column
             names and the values are the transformer names. The transformer names can be one in
             https://docs.sdv.dev/rdt/transformers-glossary/browse-transformers.
+            In addition, we also support inputting a transformer string name, e.g., {'column1': 'OneHotEncoder'}.
+
 
         metadata = {
 
         'sdtypes': {
 
         'column1': 'numerical',
         'column2': 'boolean',
@@ -95,14 +98,17 @@
                 self.ht.detect_initial_config(df)
                 self.metadata = self.ht.get_config()
                 self.ht.fit(df)
 
             else:
                 # parse the metadata and update hypertransformer's config
                 self._parse_metadata()
+            
+            # create a mapping from column name before to column name after transformation
+            self._create_transformed_col2col()
 
             # replace data with the transformed one
             self.df = self.transform(df)
 
     def __getitem__(self, index):
         # TODO: support better indexing
         '''
@@ -174,14 +180,22 @@
         
         if 'sdtypes' in metadata:
             self.ht.update_sdtypes(metadata['sdtypes'])
 
         self.ht.fit(self.df)
         self.metadata.update(self.ht.get_config())
 
+    def _create_transformed_col2col(self):
+        # create transformed column id to the original columns
+        transformed_col2col = OrderedDict()
+        for idx, col in enumerate(self.df.columns):
+            col_transformer = self.metadata['transformers'][col]
+            transformed_col2col[col] = col_transformer.output_columns
+        self.metadata['transformed_col2col'] = transformed_col2col
+
 
 class SequencePatientBase(Dataset):
     '''
     Load sequential patient inputs for longitudinal patient records generation.
 
     Parameters
     ----------
```

### Comparing `PromptEHR-0.0.5/pytrial/data/trial_data.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/models/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,192 +1,255 @@
-from collections import defaultdict
-import pdb
+'''
+TODO: add .from_pretrained to load pretrained trial search model
+from cloud storage.
+'''
+import abc
 import os
-from typing import Any, Callable, Dict, List, NewType, Optional, Tuple, Union
+import json
+import pdb
 
+import torch
 import pandas as pd
-from torch.utils.data import Dataset, DataLoader
 
-from ..utils.trial_utils import ClinicalTrials
-from ..utils.tabular_utils import read_csv_to_df
-from ..data.vocab_data import Vocab
+from pytrial.utils.check import check_model_dir
+from pytrial.utils.check import make_dir_if_not_exist
 
-class TrialDatasetBase(Dataset):
-    '''
-    The basic trial datasets loader.
+class TrialSearchBase(abc.ABC):
+    '''Abstract class for all trial search algroithms.
 
     Parameters
     ----------
-    data: pd.DataFrame
-        Contain the trial document in tabular format.
+    experiment_id: str, optional (default = 'test')
+        The name of current experiment.
+
     '''
-    inc_ec_embedding = None # inclusion criteria embedding
-    inc_vocab = None # inclusion criteria vocab
-    exc_ec_embedding = None # exclusion criteria embedding
-    exc_vocab = None # exclusion criteria vocab
-
-    def __init__(self, data):
-        self.df = data
-        self._process_ec()
-        self._collect_cleaned_sentence_set()
-    
-    def __len__(self):
-        return len(self.df)
+    @abc.abstractmethod
+    def __init__(self, experiment_id='test'):
+        check_model_dir(experiment_id)
+        self.checkout_dir = os.path.join('./experiments_records', experiment_id,
+                                         'checkpoints')
+        self.result_dir = os.path.join('./experiments_records', experiment_id,
+                                       'results')
+        make_dir_if_not_exist(self.checkout_dir)
+        make_dir_if_not_exist(self.result_dir)
+
+
+    @abc.abstractmethod
+    def fit(self, train_data, valid_data):
+        '''
+        Fit the model with training data. Need to implement in subclass.
+
+        Parameters
+        ----------
+        train_data: dict
+            Training data for model fitting.
+
+            train_data = {
+
+            'x': pd.DataFrame,
+            
+            'fields': list[str],
+            
+            'y': pd.Series or np.array,
+            
+            }
+
+        valid_data: dict
+            Validation data.
+            
+            valid_data = {
+                
+            'x': pd.DataFrame,
+            
+            'fields': list[str],
+            
+            'y': pd.Series or np.array,
+            
+            }
+
+        Returns
+        -------
+        self: object
+            The trained model.
+
+        '''
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def predict(self, test_data):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def load_model(self, checkpoint):
+        '''
+        Parameters
+        ----------
+        checkpoint: str
+            The path to the saved model.
+
+        Returns
+        -------
+        self: object
+            The loaded pretrained model.
+        '''
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def save_model(self, output_dir):
+        '''
+        Parameters
+        ----------
+        output_dir: str
+            The directory to save the model states.
+
+        '''
+        raise NotImplementedError
 
-    def __getitem__(self, index):
-        return self.df.iloc[index:index+1]
+    @abc.abstractmethod
+    def encode(self, inputs):
+        '''
+        Encode input documents into embeddings.
+
+        Parameters
+        ----------
+        inputs: dict
+            The input documents.
+        '''
+        raise NotImplementedError
+
+    def train(self, mode=True):
+        self.training = mode
+        self.model.train()
+        return self
     
-    def get_ec_sentence_embedding(self):
+    def eval(self, mode=False):
+        self.training = mode
+        self.model.eval()
+        return self
+
+    @abc.abstractmethod
+    def _build_model(self):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def __getitem__(self, tag):
         '''
-        Process the eligibility criteria of each trial,
-        get the criterion-level emebddings stored in dict.
+        Get the embeddings of documents by the trial tags.
+
+        Parameters
+        ----------
+        tag: str, int, list[str], list[int]
+            The tag (or tags) to be looked up in the model.
+
+        Returns
+        -------
+        The embeddings of each document.
         '''
-        self._get_ec_emb()
+        raise NotImplementedError
 
-    def _process_ec(self):
-        res = self.df['criteria'].apply(lambda x: self._split_protocol(x))
-        self.df['inclusion_criteria'] = res.apply(lambda x: x[0])
-        self.df['exclusion_criteria'] = res.apply(lambda x: x[1])
-
-    def _get_ec_emb(self):
-        # create EC embedding with indexed ECs
-        from pytrial.model_utils.bert import BERT
-        bert_model = BERT(device='cuda:0')
-        self.inc_ec_embedding = bert_model.encode(self.inc_vocab.words, batch_size=64)
-        self.exc_ec_embedding = bert_model.encode(self.exc_vocab.words, batch_size=64)
-        self.inc_ec_embedding = self.inc_ec_embedding.cpu()
-        self.exc_ec_embedding = self.exc_ec_embedding.cpu()
-        
-
-    def _collect_cleaned_sentence_set(self):
-        # create a vocab for ec sentences
-        self.inc_vocab = Vocab()
-        self.exc_vocab = Vocab()
-        self.inc_vocab.add_sentence(['[PAD]']) # 0 belongs to the pad token
-        self.exc_vocab.add_sentence(['[PAD]']) # 0 belongs to the pad token
-
-        inc_index_set, exc_index_set = [], []
-        for idx, row in self.df.iterrows():
-            row_inc_set, row_exc_set = [], []
-            inc = row['inclusion_criteria']
-            exc = row['exclusion_criteria']
-            for sent in inc:
-                self.inc_vocab.add_sentence(sent)
-                row_inc_set.append(self.inc_vocab.word2idx[sent])
-            for sent in exc:
-                self.exc_vocab.add_sentence(sent)
-                row_exc_set.append(self.exc_vocab.word2idx[sent])
-            inc_index_set.append(list(set(row_inc_set)))
-            exc_index_set.append(list(set(row_exc_set)))
-        self.df['inclusion_criteria_index'] = inc_index_set
-        self.df['exclusion_criteria_index'] = exc_index_set
-
-    def _clean_protocol(self, protocol):
-        protocol = protocol.lower()
-        protocol_split = protocol.split('\n')
-        filter_out_empty_fn = lambda x: len(x.strip())>0
-        strip_fn = lambda x: x.strip()
-        protocol_split = list(filter(filter_out_empty_fn, protocol_split))	
-        protocol_split = list(map(strip_fn, protocol_split))
-        return protocol_split
-
-    def _split_protocol(self, protocol):
-        protocol_split = self._clean_protocol(protocol)
-        inclusion_idx, exclusion_idx = len(protocol_split), len(protocol_split)	
-        for idx, sentence in enumerate(protocol_split):
-            if "inclusion" in sentence:
-                inclusion_idx = idx
-                break
-        for idx, sentence in enumerate(protocol_split):
-            if "exclusion" in sentence:
-                exclusion_idx = idx 
-                break 		
-        if inclusion_idx + 1 < exclusion_idx + 1 < len(protocol_split):
-            inclusion_criteria = protocol_split[inclusion_idx:exclusion_idx]
-            exclusion_criteria = protocol_split[exclusion_idx:]
-            if not (len(inclusion_criteria) > 0 and len(exclusion_criteria) > 0):
-                print(len(inclusion_criteria), len(exclusion_criteria), len(protocol_split))
-                exit()
-            return inclusion_criteria, exclusion_criteria ## list, list 
-        else:
-            return protocol_split, []
 
 
-class TrialDataset(Dataset):
-    '''
-    Basic trial datasets loader.
+    def _save_checkpoint(self, state,
+                        epoch_id=0,
+                        is_best=False,
+                        output_dir=None,
+                        filename='checkpoint.pth.tar'):
+        if output_dir is None:
+            output_dir = self.checkout_dir
+
+        if epoch_id < 1:
+            filepath = os.path.join(output_dir, 'latest.' + filename)
+        elif is_best:
+            filepath = os.path.join(output_dir, 'best.' + filename)
+        else:
+            filepath = os.path.join(self.checkout_dir,
+                                    str(epoch_id) + '.' + filename)
+        torch.save(state, filepath)
+
+    def _save_model_config(self, model_config, output_dir=None):
+        if output_dir is None:
+            output_dir = self.checkout_dir
+        temp_path = os.path.join(output_dir, "model_config.json")
+        if os.path.exists(temp_path):
+            os.remove(temp_path)
+        with open(temp_path, "w", encoding='utf-8') as f:
+            f.write(json.dumps(model_config, indent=4))
+
+    def _load_model_config(self, checkpoint=''):
+        if checkpoint == '':
+            temp_path = os.path.join(self.checkout_dir,
+                                     'model_config.json')
+            assert os.path.exists(
+                temp_path), 'cannot find predictor_config.json, please it in dir {0}'.format(
+                self.checkout_dir)
+        else:
+            temp_path = checkpoint
+            assert os.path.exists(
+                temp_path), 'cannot find checkpoint file from path: {0}'.format(
+                checkpoint)
+        print('load predictor config file from {0}'.format(temp_path))
+        with open(temp_path, 'r') as f:
+            predictor_config = json.load(f)
+        return predictor_config
 
-    Parameters
-    ----------
-    input_dir: str
-        The path to the trial dataset in tabular form (.csv).
-        If a directory is given, the code will automatically pick the only '.csv' file under this dir.
-    '''
-    def __init__(self, input_dir=None) -> None:
-        if os.path.isfile(input_dir):
-            self.df = read_csv_to_df(input_dir, index_col=0)
-
-        if os.path.isdir(input_dir):
-            csv_names = [name for name in os.listdir(input_dir) if name.endswith('.csv')]
-            if len(csv_names) > 1:
-                raise Exception(f'`input_dir` {input_dir} is given where more than one csv files are found under this path.')
-            if len(csv_names) == 0:
-                raise Exception(f'`input_dir` {input_dir} is given where no csv file is found under this path.')
-            self.df = read_csv_to_df(os.path.join(input_dir, csv_names[0]), index_col=0)
-
-    def __len__(self):
-        return len(self.df)
-
-    def __getitem__(self, index):
-        return self.df.iloc[index:index+1]
-
-class TrialDataCollator:
-    '''The basic trial data collator.
-    Subclass it and override the `__init__` & `__call__` function if need operations inside this step.
-
-    Returns
-    -------
-    batch_df: pd.DataFrame
-        A dataframe contains multiple fields for each trial.
-    '''
-    def __init__(self) -> None:
-        # subclass to add tokenizer
-        # subclass to add feature preprocessor
-        pass
-
-    def __call__(self, examples):
-        batch_df = pd.concat(examples, 0)
-        batch_df.fillna('none',inplace=True)
-        return batch_df
+    def _input_data_check(self, inputs):
+        '''
+        Check the training / testing data fits the formats.
+        Target to (1) check if inputs valid,
+                    if not, give tips about the data problem.
+
+        Parameters
+        ----------
+        inputs: {
+                'x': pd.DataFrame,
+                'fields': list[str],
+                'tag': str,
+                }
+        '''
+        # check overall input format
+        assert 'x' in inputs, 'No input trial doc dataframe found in inputs.'
+        df = inputs['x']
+        if 'fields' in inputs:
+            try:
+                _ = df[inputs['fields']]
+            except:
+                raise Exception('Cannot find the specified `fields` in inputs dataframe.')
+        if 'tag' in inputs:
+            try:
+                _ = df[inputs['tag']]
+            except:
+                raise Exception('Cannot find the specified `tag` in inputs dataframe.')
+
+        # check data type
+        try:
+            _ = df.applymap(str)
+        except:
+            raise Exception('Cannot transform the input dataframe to str type, please check the inputs.')
+
+    def _process_dataframe(self, df, fields):
+        if fields is not None:
+            df = df[fields]
+        if 'nct_id' in df:
+            df = df.drop(['nct_id'], axis=1)
+        df = df.applymap(str)
+        df = df.apply(lambda x: x.name + ': ' + x)
+        df = df.applymap(lambda x: x.lower())
+        df_raw_texts = df.agg(' '.join, axis=1)
+        df_raw_texts = pd.DataFrame(df_raw_texts, columns=['text'])
+        return df_raw_texts
 
 
-class TrialOutcomeDatasetBase(Dataset):
+def whitening_torch_final(embeddings):
     '''
-    Basic trial outcome datasets loader.
+    Whitening the embeddings.
 
     Parameters
     ----------
-    data: pd.DataFrame
-        Contain the trial document in tabular format.
+    embeddings: torch.Tensor
+        The embeddings to be whitened. The shape is (n, d).
     '''
-    columns = ['nctid', 'label', 'smiless',  'icdcodes', 'criteria']
-    def __init__(self, data, columns=None) -> None:
-        self.data = data
-        if columns is not None:
-            self.columns = columns
-    
-    def __len__(self):
-        return len(self.data)
-    
-    def __getitem__(self, index):
-        row = self.data.iloc[index]
-        return row[self.columns[0]], row[self.columns[1]], row[self.columns[2]], row[self.columns[3]], row[self.columns[4]]
-
-def test():
-    trialdata = TrialDataset('./datasets/AACT-ClinicalTrial/')
-    trial_collate_fn = TrialDataCollator()
-    trialoader = DataLoader(trialdata, batch_size=10, shuffle=False, collate_fn=trial_collate_fn)
-    batch = next(iter(trialoader))
-    print(batch)
-
-if __name__ == '__main__':
-    test()
+    mu = torch.mean(embeddings, dim=0, keepdim=True)
+    cov = torch.mm((embeddings - mu).t(), embeddings - mu)
+    u, s, vt = torch.svd(cov)
+    W = torch.mm(u, torch.diag(1/torch.sqrt(s)))
+    embeddings = torch.mm(embeddings - mu, W)
+    return embeddings
```

### Comparing `PromptEHR-0.0.5/pytrial/data/utils.py` & `PromptEHR-0.0.6/pytrial/data/utils.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/model_utils/bert.py` & `PromptEHR-0.0.6/pytrial/model_utils/bert.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     device: str
         The device of this model, typically be 'cpu' or 'cuda:0'.
 
     Examples
     --------
     >>> model = BERT()
-    >>> emb = BERT.encode('The goal of life is comfort.')
+    >>> emb = model.encode('The goal of life is comfort.')
     >>> print(emb.shape)
     '''
     is_train=None
     def __init__(self, bertname='emilyalsentzer/Bio_ClinicalBERT', proj_dim=None, max_length=512, device='cpu'):
         super().__init__()
         self.projection_head = None
         self.model = AutoModel.from_pretrained(bertname, output_hidden_states=True)
@@ -47,14 +47,31 @@
         if proj_dim is not None:
             self.projection_head = nn.Linear(768, proj_dim, bias=False)
             self.projection_head.to(device)
         self.device = device
         self.model.to(device)
 
     def forward(self, input_ids, attention_mask=None, token_type_ids=None, return_hidden_states=False):
+        '''
+        Forward pass of the model. 
+        
+        Parameters
+        ----------
+        input_ids: torch.Tensor
+            The input token ids with shape [batch_size, seq_len].
+        
+        attention_mask: torch.Tensor
+            The attention mask with shape [batch_size, seq_len].
+        
+        token_type_ids: torch.Tensor
+            The token type ids with shape [batch_size, seq_len].
+        
+        return_hidden_states: bool
+            Whether to return the hidden states of all layers.
+        '''
         output = self.model(input_ids=input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids, return_dict=True)
         if not return_hidden_states:
             embed = output['pooler_output']
             if self.projection_head is not None:
                 embed = self.projection_head(embed)
             return embed
         else:
```

### Comparing `PromptEHR-0.0.5/pytrial/model_utils/drug.py` & `PromptEHR-0.0.6/pytrial/model_utils/drug.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,28 @@
 from networkx.readwrite import json_graph
 import pandas as pd
 from tqdm import tqdm
 
 from ..utils.tabular_utils import read_csv_to_df, read_txt_to_df, read_excel_to_df
 from ..utils.check import make_dir_if_not_exist
 
-DRUG_DDI_URL = 'https://uofi.box.com/shared/static/xdfgrnhzotz6ktyrdsrikrnz1th97fic.csv'
-DRUG_BANK_URL = 'https://uofi.box.com/shared/static/4f3g4dvdfyz5goubazeqfzdi0abcgzwf.csv'
+# DRUG_DDI_URL = 'https://uofi.box.com/shared/static/xdfgrnhzotz6ktyrdsrikrnz1th97fic.csv'
+DRUG_DDI_URL = 'https://storage.googleapis.com/pytrial/drug-DDI.csv'
+# DRUG_BANK_URL = 'https://uofi.box.com/shared/static/4f3g4dvdfyz5goubazeqfzdi0abcgzwf.csv'
+DRUG_BANK_URL = 'https://storage.googleapis.com/pytrial/drugbank_drugs_info.csv'
 RXCUI_ATC4_NDC11_URL = 'https://github.com/RyanWangZf/PyTrial/raw/main/resources/rxcui_atc4_ndc11.zip'
 NDC_NAME_URL = 'https://github.com/RyanWangZf/PyTrial/raw/main/resources/ndc_name.csv'
 NAME_SMILES_URL = 'https://github.com/RyanWangZf/PyTrial/raw/main/resources/drug_smiles.csv'
 NAME_ATC_URL ='https://github.com/RyanWangZf/PyTrial/raw/main/resources/atc_drug.csv'
-ATC5_NDC_URL = 'https://uofi.box.com/shared/static/dk07wip4l4hkbolp09e3rz3un4hokocb.zip'
-ATC_DEF_URL = 'https://uofi.box.com/shared/static/tdz6glo9waf353mwxvqw44l6r43vrfqm.zip'
-FDA_NDC_NAME_URL = 'https://uofi.box.com/shared/static/ah6gk3ljaj0uz0cr2yoecmd3so2onih7.zip'
+# ATC5_NDC_URL = 'https://uofi.box.com/shared/static/dk07wip4l4hkbolp09e3rz3un4hokocb.zip'
+ATC5_NDC_URL = 'https://storage.googleapis.com/pytrial/atc5_ndc.zip'
+# ATC_DEF_URL = 'https://uofi.box.com/shared/static/tdz6glo9waf353mwxvqw44l6r43vrfqm.zip'
+ATC_DEF_URL = 'https://storage.googleapis.com/pytrial/ATC.csv.zip'
+# FDA_NDC_NAME_URL = 'https://uofi.box.com/shared/static/ah6gk3ljaj0uz0cr2yoecmd3so2onih7.zip'
+FDA_NDC_NAME_URL = 'https://storage.googleapis.com/pytrial/fda_ndc.zip'
 
 class DrugTransformer:
     '''
     Provide a series of drug-related functions for
 
     (1) drug name to atc / atc to drug name
     (2) drug name to ndc-11 / ndc-11 to drug name
```

### Comparing `PromptEHR-0.0.5/pytrial/model_utils/icd.py` & `PromptEHR-0.0.6/pytrial/model_utils/icd.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 NIH_API_PREFIX_ICD10 = 'https://clinicaltables.nlm.nih.gov/api/icd10cm/v3/search?sf=code,name&terms='
 NIH_API_PREFIX_ICD9_DX = 'https://clinicaltables.nlm.nih.gov/api/icd9cm_dx/v3/search?sf=code,long_name&terms='
 NIH_API_PREFIX_ICD9_SG = 'https://clinicaltables.nlm.nih.gov/api/icd9cm_sg/v3/search?sf=code,long_name&terms='
 NIH_API_PREFIX_ICD9_CONDITION = 'https://clinicaltables.nlm.nih.gov/api/conditions/v3/search?df=primary_name&terms='
 NIH_API_PREFIX_ICD10_CONDITION = 'https://clinicaltables.nlm.nih.gov/api/conditions/v3/search?df=term_icd10cm_codes,primary_name&terms='
 ICD9_SG_URL = 'https://github.com/RyanWangZf/PyTrial/raw/main/resources/CMS32_DESC_LONG_SHORT_SG.xlsx'
 ICD9_DX_URL = 'https://github.com/RyanWangZf/PyTrial/raw/main/resources/CMS32_DESC_LONG_SHORT_DX.xlsx'
+ICD9_GRAPH_URL = 'https://storage.googleapis.com/pytrial/resources/icd-9-hierarchy.json'
 
 def get_icd10_from_nih(term):
     '''
     Query related ICD-10 codes for input terms.
 
     Parameters
     ----------
@@ -255,40 +256,58 @@
     -------
     self.graph: nx.DiGraph
         The hierarchy of ICD codes stored as graph in networkx.
 
     self.codes: list[str]
         All the unique codes.
     '''
-    def __init__(self, input_dir):
+    def __init__(self, input_dir=None):
+        if input_dir is None:
+            input_dir = './resources/icd9'
+        
+        if not os.path.exists(input_dir):
+            os.makedirs(input_dir)
+            # download the ICD9 hierarchy
+            wget.download(ICD9_GRAPH_URL, input_dir)
+        
         filename = os.path.join(input_dir, 'icd-9-hierarchy.json')
         super().__init__(filename)
 
 
 class ICD10Graph(ICDGraphBase):
     '''
     Get an ICD-10 knowledge graph to query parental and children nodes for each code.
 
     Parameters
     ----------
     input_dir: str
         The dir that stores the hierarchy files.
 
-    version: {'2021','2020','2019'}
+    version: {'2022', '2021','2020','2019'}
         The version of ICD-10 codes.
 
     Returns
     -------
     self.graph: nx.DiGraph
         The hierarchy of ICD codes stored as graph in networkx.
 
     self.codes: list[str]
         All the unique codes.
     '''
-    def __init__(self, input_dir, version='2021'):
+    def __init__(self, input_dir=None, version='2021'):
+
+        if input_dir is None:
+            input_dir = './resources/icd10'
+
+        if not os.path.exists(input_dir):
+            os.makedirs(input_dir)
+            # download the ICD10 hierarchy
+            url = f'https://github.com/icd-codex/icd-codex/raw/dev/icdcodex/data/icd-10-{version}-hierarchy.json'
+            wget.download(url, input_dir)
+
         filename = os.path.join(input_dir, f'icd-10-{version}-hierarchy.json')
         super().__init__(filename)
 
 class ICD9_DX_VOC:
     '''
     Get a vocabulary containing the mapping of ICD9 Diagnosis code and its names.
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/data.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/data.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/losses.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,9 +56,11 @@
     def __init__(self, model) -> None:
         super().__init__()
         self.model = model
         self.loss = nn.MSELoss()
 
     def forward(self, inputs):
         logits = self.model(inputs)
-        loss = self.loss(logits, inputs['y'])
+        # transform the inputs['y'] to the float type
+        y = inputs['y'].float()
+        loss = self.loss(logits, y)
         return {'loss_value':loss}
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/metrics.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/metrics.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/base.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
         if mode == 'multiclass':
             return [XentLoss(self.model)]
 
         if mode == 'multilabel':
             return [MultilabelBinaryXentLoss(self.model)]
 
-        if mode == 'binary':
+        if mode == 'regression':
             return [MSELoss(self.model)]
 
     def _prepare_input(self, data):
         '''
         Prepare inputs for sequential patient record predictive models.
 
         Parameters
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/dipole.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/dipole.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,13 +458,20 @@
             'multiclass': 'acc',
             'regression': 'mse',
             'multilabel': 'f1', # take average of F1 scores
             }
         train_dataloader = self.get_train_dataloader(train_data)
         loss_models = self._build_loss_model()
         train_objectives = [(train_dataloader, loss_model) for loss_model in loss_models]
+
+        if self.config['mode'] == 'regression':
+            less_is_better = True
+        else:
+            less_is_better = False
+
         trainer = IndivSeqTrainer(model=self,
             train_objectives=train_objectives,
             test_data=valid_data,
             test_metric=test_metric_dict[self.config['mode']],
+            less_is_better=less_is_better,
             )
         trainer.train(**self.config)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/raim.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/raim.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,21 @@
             'binary': 'auc',
             'multiclass': 'acc',
             'regression': 'mse',
             'multilabel': 'f1', # take average of F1 scores
             }
         train_dataloader = self.get_train_dataloader(train_data)
         loss_models = self._build_loss_model()
+
+        if self.config['mode'] == 'regression':
+            less_is_better = True
+        else:
+            less_is_better = False
+    
         train_objectives = [(train_dataloader, loss_model) for loss_model in loss_models]
         trainer = IndivSeqTrainer(model=self,
             train_objectives=train_objectives,
             test_data=valid_data,
             test_metric=test_metric_dict[self.config['mode']],
+            less_is_better=less_is_better,
             )
         trainer.train(**self.config)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/retain.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/retain.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,13 +306,20 @@
             'multiclass': 'acc',
             'regression': 'mse',
             'multilabel': 'f1', # take average of F1 scores
             }
         train_dataloader = self.get_train_dataloader(train_data)
         loss_models = self._build_loss_model()
         train_objectives = [(train_dataloader, loss_model) for loss_model in loss_models]
+
+        if self.config['mode'] == 'regression':
+            less_is_better = True
+        else:
+            less_is_better = False
+
         trainer = IndivSeqTrainer(model=self,
             train_objectives=train_objectives,
             test_data=valid_data,
             test_metric=test_metric_dict[self.config['mode']],
+            less_is_better=less_is_better,
             )
         trainer.train(**self.config)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/rnn.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/rnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,14 +103,17 @@
     
     batch_size: int
         Batch size when doing SGD optimization.
 
     epochs: int
         Maximum number of iterations taken for the solvers to converge.
 
+    evaluation_steps: int
+        Number of steps to evaluate the model on validation set or report the training loss.
+
     num_worker: int
         Number of workers used to do dataloading during training.
 
     device: str
         The model device.
 
     experiment_id: str
@@ -126,14 +129,15 @@
         n_rnn_layer=2,
         rnn_type='lstm',
         bidirectional=False,
         learning_rate=1e-4,
         weight_decay=1e-4,
         batch_size=64,
         epochs=10,
+        evaluation_steps=100,
         num_worker=0,
         device='cuda:0',
         experiment_id='test',
         ):
         super().__init__(experiment_id, mode=mode, output_dim=output_dim)
         self.config = {
             'mode':self.mode,
@@ -147,14 +151,15 @@
             'device':device,
             'learning_rate':learning_rate,
             'batch_size':batch_size,
             'weight_decay':weight_decay,
             'epochs':epochs,
             'num_worker':num_worker,
             'orders':orders,
+            'evaluation_steps':evaluation_steps,
             }
         self.config['total_vocab_size'] = sum(vocab_size)
         self.device = device
         self._build_model()
 
     def fit(self, train_data, valid_data=None):
         '''
@@ -351,27 +356,34 @@
             'multiclass': 'acc',
             'regression': 'mse',
             'multilabel': 'f1', # take average of F1 scores
             }
         train_dataloader = self.get_train_dataloader(train_data)
         loss_models = self._build_loss_model()
         train_objectives = [(train_dataloader, loss_model) for loss_model in loss_models]
+
+        if self.config['mode'] == 'regression':
+            less_is_better = True
+        else:
+            less_is_better = False
+
         trainer = IndivSeqTrainer(model=self,
             train_objectives=train_objectives,
             test_data=valid_data,
             test_metric=test_metric_dict[self.config['mode']],
+            less_is_better=less_is_better,
             )
         trainer.train(**self.config)
 
     def _build_loss_model(self):
         mode = self.config['mode']
         if mode == 'binary':
             return [BinaryXentLoss(self.model)]
 
         if mode == 'multiclass':
             return [XentLoss(self.model)]
 
         if mode == 'multilabel':
             return [MultilabelBinaryXentLoss(self.model)]
 
-        if mode == 'binary':
+        if mode == 'regression':
             return [MSELoss(self.model)]
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/sequence/stagenet.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/sequence/stagenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,13 +406,20 @@
             'multiclass': 'acc',
             'regression': 'mse',
             'multilabel': 'f1', # take average of F1 scores
             }
         train_dataloader = self.get_train_dataloader(train_data)
         loss_models = self._build_loss_model()
         train_objectives = [(train_dataloader, loss_model) for loss_model in loss_models]
+
+        if self.config['mode'] == 'regression':
+            less_is_better = True
+        else:
+            less_is_better = False
+
         trainer = IndivSeqTrainer(model=self,
             train_objectives=train_objectives,
             test_data=valid_data,
             test_metric=test_metric_dict[self.config['mode']],
+            less_is_better=less_is_better,
             )
         trainer.train(**self.config)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/base.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,19 +159,25 @@
         test_metric_dict = {
             'binary': 'auc',
             'multiclass': 'acc',
             'regression': 'mse',
             'multilabel': 'f1', # take average of F1 scores
         }
 
+        if mode == 'regression':
+            less_is_better = True
+        else:
+            less_is_better = False
+
         trainer = IndivTabTrainer(
             model=self,
             train_objectives=train_objectives,
             test_data=valid_data,
             test_metric=test_metric_dict[mode],
+            less_is_better=less_is_better,
         )
 
         trainer.train(
             **self.config
         )
 
     def _parse_input_data(self, inputs):
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/mlp.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/mlp.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/transtab.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/transtab.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/tabular/xgboost.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/tabular/xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,34 +165,33 @@
             if 'y' in test_data:
                 pickle.dump(test_data['y'], open(os.path.join(self.result_dir, 'label.pkl'), 'wb'))
 
         return ypred
 
     def save_model(self, output_dir=None):
         '''
-        Save the learned logistic regression model to the disk.
+        Save the learned XGBoost model to the disk.
 
         Parameters
         ----------
         output_dir: str or None
             The dir to save the learned model.
             If set None, will save model to `self.checkout_dir`.
         '''
-        if output_dir is not None:
-            make_dir_if_not_exist(output_dir)
-        else:
+        if output_dir is None:
             output_dir = self.checkout_dir
+        make_dir_if_not_exist(output_dir)
 
         self._save_config(self.config, output_dir=output_dir)
         ckpt_path = os.path.join(output_dir, 'indiv-tabular.model')
         joblib.dump(self.model, ckpt_path)
 
     def load_model(self, checkpoint=None):
         '''
-        Save the learned logistic regression model to the disk.
+        Load the learned XGBoost model from the disk.
 
         Parameters
         ----------
         checkpoint: str or None
             - If a directory, the only checkpoint file `.model` will be loaded.
             - If a filepath, will load from this file;
             - If None, will load from `self.checkout_dir`.
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/indiv_outcome/trainer.py` & `PromptEHR-0.0.6/pytrial/tasks/indiv_outcome/trainer.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/base.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/base.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/hint.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pickle
 from copy import deepcopy 
 import os
 import json
+import joblib
 
 from sklearn.metrics import roc_auc_score, f1_score, average_precision_score, precision_score, recall_score, accuracy_score
 import matplotlib.pyplot as plt
 import numpy as np 
 from tqdm import tqdm 
 import torch 
 from torch import nn 
@@ -36,17 +37,14 @@
         weight_decay = 0, 
         ):
         super(Interaction, self).__init__()
         icdcode2ancestor_dict = build_icdcode2ancestor_dict()
         self.disease_encoder = GRAM(embedding_dim = disease_embedding_dim, icdcode2ancestor = icdcode2ancestor_dict, device = device)
         self.protocol_encoder = Protocol_Embedding(output_dim = protocol_output_dim, highway_num=3, device = device)
         self.molecule_encoder = MPNN(mpnn_hidden_size = molecule_embedding_dim, mpnn_depth=3, device = device)
-        # self.molecule_encoder = molecule_encoder 
-        # self.disease_encoder = disease_encoder 
-        # self.protocol_encoder = protocol_encoder 
         self.global_embed_size = global_embed_size 
         self.highway_num_layer = highway_num_layer 
         self.feature_dim = self.molecule_encoder.embedding_size + self.disease_encoder.embedding_size + self.protocol_encoder.embedding_size
         self.epoch = epoch 
         self.lr = lr 
         self.weight_decay = weight_decay 
         self.save_name = prefix_name + '_interaction'
@@ -445,15 +443,14 @@
             'epoch': epoch,
             'lr': lr,
             'batch_size': batch_size,
             'weight_decay': weight_decay,
             'prefix_name': prefix_name,            
             }
 
-
     def predict(self, test_data):
         '''
         Make trial outcome prediction for test data.
         
         Parameters
         ----------
         test_data: TrialOutcomeDatasetBase
@@ -506,66 +503,101 @@
                 loss = self.loss(output, label_vec.float())
                 train_loss_record.append(loss.item())
                 opt.zero_grad() 
                 loss.backward() 
                 opt.step()
                 print('epoch: {}, loss: {}'.format(ep, loss.item()))
             
-            valid_loss = self.test(valid_loader, return_loss=True)
-            valid_loss_record.append(valid_loss)
-            if valid_loss < best_valid_loss:
-                best_valid_loss = valid_loss 
-                best_model = deepcopy(self)
+            if valid_data is not None:
+                # only check valid loss when valid_data is not None
+                valid_loss = self.test(valid_loader, return_loss=True)
+                valid_loss_record.append(valid_loss)
+                if valid_loss < best_valid_loss:
+                    print('best valid loss: {} -> {}'.format(best_valid_loss, valid_loss))
+                    best_valid_loss = valid_loss 
+                    best_model = deepcopy(self)
 
         # self.plot_learning_curve(train_loss_record, valid_loss_record)
         self = deepcopy(best_model)
         # auc_score, f1score, prauc_score, precision, recall, accuracy, predict_1_ratio, label_1_ratio = self.test(test_loader, return_loss = False, validloader = valid_loader)
 
     def save_model(self, output_dir = None):
         '''
         Save the learned HINT model to the disk.
 
         Parameters
         ----------
         output_dir: str or None
             The output folder to save the learned model.
-            If set None, will save model to `save_model/model.ckpt`.
+            If set None, will save model to `checkpoints/model.ckpt`.
         '''
         if output_dir is None:
-            output_dir = 'save_model'
+            output_dir = 'checkpoints'
         if not os.path.exists(output_dir): os.makedirs(output_dir)
-        filename = os.path.join(output_dir, 'model.ckpt')
-        torch.save(self, filename)
+        filename = os.path.join(output_dir, 'model.pkl')
+
+        # save self using joblib
+        joblib.dump(self, filename)
 
         config_filename = os.path.join(output_dir, 'config.json')
         with open(config_filename, 'w') as f:
             json.dump(self.config, f)
 
     def load_model(self, checkpoint=None):
         '''
         Load the learned HINT model from the disk.
 
         Parameters
         ----------
+        checkpoint: str
+            The checkpoint folder to load the learned model.
+            The checkpoint under this folder should be `model.ckpt`.
+        '''
+        if checkpoint is None:
+            ckpt_dir = 'checkpoints'
+            checkpoint = os.path.join(ckpt_dir, 'model.pkl')
+        else:
+            checkpoint = os.path.join(checkpoint, 'model.pkl')
+        
+        # load model using joblib
+        model = joblib.load(checkpoint)
+
+        ckpt_dir = os.path.dirname(checkpoint)
+        config_filename = os.path.join(ckpt_dir, 'config.json')
+        with open(config_filename, 'r') as f:
+            model.config = json.load(f)
+        
+        # replace self with the loaded object
+        self.__dict__.update(model.__dict__)
+
+    @staticmethod
+    def from_pretrained(checkpoint=None):
+        '''
+        Load the learned HINT model from the disk.
+
+        Parameters
+        ----------
         checkpoint: str 
             The checkpoint folder to load the learned model.
             The checkpoint under this folder should be `model.ckpt`.
         '''
         if checkpoint is None:
-            ckpt_dir = 'save_model'
-            checkpoint = os.path.join(ckpt_dir, 'model.ckpt')
+            ckpt_dir = 'checkpoints'
+            checkpoint = os.path.join(ckpt_dir, 'model.pkl')
         else:
-            checkpoint = os.path.join(checkpoint, 'model.ckpt')
+            checkpoint = os.path.join(checkpoint, 'model.pkl')
         
-        self = torch.load(checkpoint)
+        # load model using joblib
+        self = joblib.load(checkpoint)
 
         ckpt_dir = os.path.dirname(checkpoint)
         config_filename = os.path.join(ckpt_dir, 'config.json')
         with open(config_filename, 'r') as f:
             self.config = json.load(f)
+        return self
 
     def generate_adj(self):        								
         ##### consistent with HINT_nograph.forward
         lst = ["molecule", "disease", "criteria", 'INTERACTION', 'risk_disease', 'augment_interaction', 'A', 'D', 'M', 'E', 'T', 'PK', "final"]
         edge_lst = [("disease", "molecule"), ("disease", "criteria"), ("molecule", "criteria"), 
                     ("disease", "INTERACTION"), ("molecule", "INTERACTION"),  ("criteria", "INTERACTION"), 
                     ("disease", "risk_disease"), ('risk_disease', 'augment_interaction'), ('INTERACTION', 'augment_interaction'),
@@ -872,37 +904,36 @@
         embeds = self.feed_lst_of_module(embeds, self.admet_model[idx]) 
         output = self.admet_pred[idx](embeds)
         return output 
 
     def test(self, valid_loader):
         pass 
 
+    # def fit(self, train_loader, valid_loader, idx):
+    #     opt = torch.optim.Adam(self.parameters(), lr = self.lr, weight_decay = self.weight_decay)
+    #     train_loss_record = [] 
+    #     valid_loss = self.test(valid_loader, return_loss=True)
+    #     valid_loss_record = [valid_loss]
+    #     best_valid_loss = valid_loss
+    #     best_model = deepcopy(self)
+
+    #     for ep in tqdm(range(self.epoch)):
+    #         for smiles_lst in train_loader:
+    #             output = self.forward(smiles_lst).view(-1)  #### 32, 1 -> 32, ||  label_vec 32,
+    #             loss = self.loss(output, label_vec.float())
+    #             train_loss_record.append(loss.item())
+    #             opt.zero_grad() 
+    #             loss.backward() 
+    #             opt.step()
+    #         valid_loss = self.test(valid_loader, return_loss=True)
+    #         valid_loss_record.append(valid_loss)
+    #         if valid_loss < best_valid_loss:
+    #             best_valid_loss = valid_loss 
+    #             best_model = deepcopy(self)
 
-    def fit(self, train_loader, valid_loader, idx):
-        opt = torch.optim.Adam(self.parameters(), lr = self.lr, weight_decay = self.weight_decay)
-        train_loss_record = [] 
-        valid_loss = self.test(valid_loader, return_loss=True)
-        valid_loss_record = [valid_loss]
-        best_valid_loss = valid_loss
-        best_model = deepcopy(self)
-
-        for ep in tqdm(range(self.epoch)):
-            for smiles_lst in train_loader:
-                output = self.forward(smiles_lst).view(-1)  #### 32, 1 -> 32, ||  label_vec 32,
-                loss = self.loss(output, label_vec.float())
-                train_loss_record.append(loss.item())
-                opt.zero_grad() 
-                loss.backward() 
-                opt.step()
-            valid_loss = self.test(valid_loader, return_loss=True)
-            valid_loss_record.append(valid_loss)
-            if valid_loss < best_valid_loss:
-                best_valid_loss = valid_loss 
-                best_model = deepcopy(self)
-
-        self = deepcopy(best_model)
+    #     self = deepcopy(best_model)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/logistic_regression.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/mlp.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/mlp.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/dataloader.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 	icdcode_embedding 
 
 '''
 
 import csv, re, pickle, os
 import pdb
 from functools import reduce 
-import icd10
+import wget
 from collections import defaultdict
 
 import pandas as pd
 import torch 
 from torch import nn 
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+import icd10
 
 ICDCODE_ANCESTOR_URL = 'https://github.com/futianfan/clinical-trial-outcome-prediction/raw/main/data/raw_data.csv'
+icdcode2ancestor_dict_url = "https://storage.googleapis.com/pytrial/HINT-benchmark-data/icdcode2ancestor_dict.pkl"
 
 def text_2_lst_of_lst(text):
 	"""
 		"[""['F53.0', 'P91.4', 'Z13.31', 'Z13.32']""]"
 	"""
 	text = text[2:-2]
 	code_sublst = []
@@ -74,15 +76,20 @@
 			ancestor = ancestor[:-1]
 		if icd10.find(ancestor) is not None:
 			icdcode2ancestor[icdcode].append(ancestor)
 	return
 
 
 def build_icdcode2ancestor_dict():
-	pkl_file = "demo_data/demo_trial_outcome_data/icdcode2ancestor_dict.pkl"
+	pkl_file = "pretrained_model/icdcode2ancestor/icdcode2ancestor_dict.pkl"
+
+	if not os.path.exists('pretrained_model/icdcode2ancestor'):
+		os.makedirs('pretrained_model/icdcode2ancestor')
+		wget.download(icdcode2ancestor_dict_url, pkl_file)
+
 	if os.path.exists(pkl_file):
 		icdcode2ancestor = pickle.load(open(pkl_file, 'rb'))
 		return icdcode2ancestor
 	all_code = collect_all_icdcodes()
 	icdcode2ancestor = defaultdict(list)
 	for code in all_code:
 		find_ancestor_for_icdcode(code, icdcode2ancestor)
@@ -111,15 +118,18 @@
 
 class GRAM(nn.Sequential):
 	"""	
 		return a weighted embedding 
 	"""
 
 	def __init__(self, embedding_dim, icdcode2ancestor, device):
-		super(GRAM, self).__init__()		
+		super(GRAM, self).__init__()
+		if icdcode2ancestor is None: 
+			icdcode2ancestor = build_icdcode2ancestor_dict()
+
 		self.icdcode2ancestor = icdcode2ancestor 
 		self.all_code_lst = GRAM.codedict_2_allcode(self.icdcode2ancestor)
 		self.code_num = len(self.all_code_lst)
 		self.maxlength = 5
 		self.code2index = {code:idx for idx,code in enumerate(self.all_code_lst)}
 		self.index2code = {idx:code for idx,code in enumerate(self.all_code_lst)}
 		self.padding_matrix = torch.zeros(self.code_num, self.maxlength).long()
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/module.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/module.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -226,14 +226,19 @@
 		self.mpnn_hidden_size = mpnn_hidden_size
 		self.mpnn_depth = mpnn_depth 
 
 		self.W_i = nn.Linear(ATOM_FDIM + BOND_FDIM, self.mpnn_hidden_size, bias=False)
 		self.W_h = nn.Linear(self.mpnn_hidden_size, self.mpnn_hidden_size, bias=False)
 		self.W_o = nn.Linear(ATOM_FDIM + self.mpnn_hidden_size, self.mpnn_hidden_size)
 
+		# initialize weights
+		nn.init.xavier_uniform_(self.W_i.weight)
+		nn.init.xavier_uniform_(self.W_h.weight)
+		nn.init.xavier_uniform_(self.W_o.weight)
+
 		self.device = device
 		self = self.to(self.device)
 
 	def set_device(self, device):
 		self.device = device 
 
 
@@ -353,15 +358,14 @@
 		self.device = device 
 		self = self.to(device)
 
 	def set_device(self, device):
 		self.device = device 
 		self.molecule_encoder.set_device(device)
 
-
 	def forward_smiles_lst_embedding(self, smiles_lst, idx):
 		embed_all = self.molecule_encoder.forward_smiles_lst(smiles_lst)
 		output = self.highway_nn_lst[idx](embed_all)
 		return output 
 
 	def forward_embedding_to_pred(self, embeded, idx):
 		return self.fc_output_lst[idx](embeded)
@@ -378,46 +382,14 @@
 			for smiles_lst, label_vec in dataloader_lst[idx]:
 				output = self.forward_smiles_lst_pred(smiles_lst, idx).view(-1)
 				loss = self.loss(output, label_vec.to(self.device).float())
 				single_loss_lst.append(loss.item())
 			loss_lst.append(np.mean(single_loss_lst))
 		return np.mean(loss_lst)
 
-	def train(self, train_loader_lst, valid_loader_lst):
-		opt = torch.optim.Adam(self.parameters(), lr = self.lr, weight_decay = self.weight_decay)
-		train_loss_record = [] 
-		valid_loss = self.test(valid_loader_lst, return_loss=True)
-		valid_loss_record = [valid_loss]
-		best_valid_loss = valid_loss 
-		best_model = deepcopy(self)
-		for ep in tqdm(range(self.epoch)):
-			data_iterator_lst = [iter(train_loader_lst[idx]) for idx in range(5)]
-			try: 
-				while True:
-					for idx in range(1):
-						smiles_lst, label_vec = next(data_iterator_lst[idx])
-						output = self.forward_smiles_lst_pred(smiles_lst, idx).view(-1)
-						loss = self.loss(output, label_vec.float()) 
-						opt.zero_grad() 
-						loss.backward()
-						opt.step()	
-			except:
-				pass 
-			valid_loss = self.test(valid_loader_lst, return_loss = True)
-			valid_loss_record.append(valid_loss)						
-
-			if valid_loss < best_valid_loss:
-				best_valid_loss = valid_loss 
-				best_model = deepcopy(self)
-
-		self = deepcopy(best_model)
-
-
-
-
 
 if __name__ == "__main__":
 	model = MPNN(mpnn_hidden_size = 50, mpnn_depth = 3)
 	dataloader = data_loader()
 	for smiles_feature, labels in dataloader:
 		embedding = model(smiles_feature) 
 		print(embedding.shape)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/model_utils/utils.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/model_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 	fp_mat = np.concatenate(fp_lst, 0)
 	fp = np.mean(fp_mat,0)
 	return fp	
 
 
 #################  for data loader  #################
 def clean_protocol(protocol):
-	protocol = protocol.lower()
+	protocol = str(protocol).lower()
 	protocol_split = protocol.split('\n')
 	filter_out_empty_fn = lambda x: len(x.strip())>0
 	strip_fn = lambda x:x.strip()
 	protocol_split = list(filter(filter_out_empty_fn, protocol_split))	
 	protocol_split = list(map(strip_fn, protocol_split))
 	return protocol_split
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_outcome/xgboost.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_outcome/xgboost.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/data.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/data.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/losses.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/losses.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/base.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/base.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/compose.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/compose.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/models/deepenroll.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/models/deepenroll.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_patient_match/trainer.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_patient_match/trainer.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/data.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/data.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/losses.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/losses.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/metrics.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/metrics.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/models/base.py` & `PromptEHR-0.0.6/pytrial/tasks/site_selection/pgentropy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,255 +1,230 @@
-'''
-TODO: add .from_pretrained to load pretrained trial search model
-from cloud storage.
-'''
-import abc
-import os
-import json
+from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
 import pdb
 
 import torch
-import pandas as pd
+from torch import nn
+from torch.utils.data import DataLoader
 
-from pytrial.utils.check import check_model_dir
-from pytrial.utils.check import make_dir_if_not_exist
-
-class TrialSearchBase(abc.ABC):
-    '''Abstract class for all trial search algroithms.
+from pytrial.utils.check import (
+    check_checkpoint_file, check_model_dir, check_model_config_file, make_dir_if_not_exist
+)
+from pytrial.data.site_data import SiteBaseDemographics
+from .base import SiteSelectionBase
+from .data import TrialSiteSimple, SiteSelectionBaseCollator
+from .losses import PolicyGradientLossEnrollment, PolicyGradientLossCombined
+from .trainer import SiteSelectTrainer
+
+device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+      
+class BuildModel(nn.Module):
+    def __init__(self, 
+        trial_dim,
+        site_dim,
+        embedding_dim
+        ) -> None:
+        super().__init__()
+        
+        self.site_encoder = nn.Linear(site_dim, embedding_dim)
+        self.trial_encoder = nn.Linear(trial_dim, embedding_dim)
+        self.site_fc = nn.Linear(embedding_dim, embedding_dim)
+        self.trial_fc = nn.Linear(embedding_dim, embedding_dim)
+        self.score_encoder = nn.Linear(2*embedding_dim, 2*embedding_dim)
+        self.fc = nn.Linear(2*embedding_dim, embedding_dim)
+        self.output = nn.Linear(embedding_dim, 1)
+        
+    def forward(self, inputs):
+        trial = inputs['trial']
+        investigators = inputs['site']
+        num_inv = investigators.size(1)
+        site_encoding = torch.relu(self.site_fc(torch.relu(self.site_encoder(investigators))))
+        trial_encoding = torch.relu(self.trial_fc(torch.relu(self.trial_encoder(trial))))
+        trial_encoding = trial_encoding.unsqueeze(1).repeat(1, num_inv, 1)
+        network_input = torch.cat((site_encoding, trial_encoding), dim=-1)
+        network_input = torch.relu(self.score_encoder(network_input))
+        score = self.output(torch.relu(self.fc(network_input))).squeeze(-1)
+        return score
 
+class PolicyGradientEntropy(SiteSelectionBase):
+    '''
+    Implement Policy Gradient Entropy model for selecting clinical trial sites based on possibly missing multi-model site features. [1]_
+    
     Parameters
     ----------
-    experiment_id: str, optional (default = 'test')
-        The name of current experiment.
+    
+    trial_dim: list[int]
+        Size of the trial representation
 
-    '''
-    @abc.abstractmethod
-    def __init__(self, experiment_id='test'):
-        check_model_dir(experiment_id)
-        self.checkout_dir = os.path.join('./experiments_records', experiment_id,
-                                         'checkpoints')
-        self.result_dir = os.path.join('./experiments_records', experiment_id,
-                                       'results')
-        make_dir_if_not_exist(self.checkout_dir)
-        make_dir_if_not_exist(self.result_dir)
+    site_dim: int
+        Size of the site representation
+
+    embedding_dim: int
+        Size of all of the modality and other intermediate embeddings
+    
+    Notes
+    -----
+    .. [1] Srinivasa, R. S., Qian, C., Theodorou, B., Spaeder, J., Xiao, C., Glass, L., & Sun, J. (2022). Clinical trial site matching with improved diversity using fair policy learning. arXiv preprint arXiv:2204.06501.
 
+    '''
+    def __init__(self, 
+        trial_dim=211, 
+        site_dim=124, 
+        embedding_dim=64, 
+        enrollment_only=True,
+        K=10,
+        lam=1,
+        learning_rate=1e-4,
+        weight_decay=1e-4,
+        batch_size=64,
+        epochs=10,
+        num_worker=0,
+        device='cuda:0',
+        experiment_id='test',
+        ) -> None:
+        super().__init__(experiment_id)
+        self.config = {
+            'trial_dim':trial_dim,
+            'site_dim':site_dim,
+            'embedding_dim':embedding_dim,
+            'enrollment_only':enrollment_only,
+            'K':K,
+            'lambda':lam,
+            'learning_rate':learning_rate,
+            'weight_decay':weight_decay,
+            'batch_size':batch_size,
+            'epochs':epochs,
+            'num_worker':num_worker,
+            'device':device,
+            'experiment_id':experiment_id,
+            }
+        self.device = device
+        self._build_model()
 
-    @abc.abstractmethod
-    def fit(self, train_data, valid_data):
+    def fit(self, train_data):
         '''
-        Fit the model with training data. Need to implement in subclass.
+        Train model with historical trial-site enrollments.
 
         Parameters
         ----------
-        train_data: dict
-            Training data for model fitting.
-
-            train_data = {
-
-            'x': pd.DataFrame,
-            
-            'fields': list[str],
-            
-            'y': pd.Series or np.array,
-            
-            }
-
-        valid_data: dict
-            Validation data.
-            
-            valid_data = {
-                
-            'x': pd.DataFrame,
-            
-            'fields': list[str],
-            
-            'y': pd.Series or np.array,
-            
-            }
-
-        Returns
-        -------
-        self: object
-            The trained model.
-
+        train_data: TrialSiteSimple
+            A `TrialSiteSimple` contains trials, sites, and enrollments.
         '''
-        raise NotImplementedError
+        self._input_data_check(train_data)
+        self._fit_model(train_data)
 
-    @abc.abstractmethod
     def predict(self, test_data):
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def load_model(self, checkpoint):
         '''
-        Parameters
-        ----------
-        checkpoint: str
-            The path to the saved model.
-
-        Returns
-        -------
-        self: object
-            The loaded pretrained model.
+        Make prediction for site selection.
         '''
-        raise NotImplementedError
+        selections = []
+        self._input_data_check(test_data)
+        dataloader = DataLoader(test_data,
+            batch_size=self.config['batch_size'],
+            num_workers=self.config['num_worker'],
+            pin_memory=True,
+            shuffle=False,
+            collate_fn=SiteSelectionBaseCollator(
+                config={
+                    'has_demographics':isinstance(test_data.sites, SiteBaseDemographics)
+                    }
+                ),
+            )
+        for data in dataloader:
+            inputs = self._prepare_input(data)
+            scores = self.model(inputs)
+            selections += [l[:self.config['K']] for l in scores.argsort(dim=1, descending=True).tolist()]
+        return selections
 
-    @abc.abstractmethod
     def save_model(self, output_dir):
         '''
+        Save the learned patient-match model to the disk.
+
         Parameters
         ----------
-        output_dir: str
-            The directory to save the model states.
-
+        output_dir: str or None
+            The dir to save the learned model.
+            If set None, will save model to `self.checkout_dir`.
         '''
-        raise NotImplementedError
+        if output_dir is not None:
+            make_dir_if_not_exist(output_dir)
+        else:
+            output_dir = self.checkout_dir
+        self._save_config(self.config, output_dir=output_dir)
+        self._save_checkpoint({'model':self.model}, output_dir=output_dir)
 
-    @abc.abstractmethod
-    def encode(self, inputs):
+    def load_model(self, checkpoint):
         '''
-        Encode input documents into embeddings.
+        Load model and the pre-encoded trial embeddings from the given
+        checkpoint dir.
 
         Parameters
         ----------
-        inputs: dict
-            The input documents.
-        '''
-        raise NotImplementedError
-
-    def train(self, mode=True):
-        self.training = mode
-        self.model.train()
-        return self
+        checkpoint: str
+            The input dir that stores the pretrained model.
+            If a directory, the only checkpoint file `*.pth.tar` will be loaded.
+            If a filepath, will load from this file.
+        '''
+        checkpoint_filename = check_checkpoint_file(checkpoint)
+        config_filename = check_model_config_file(checkpoint)
+        state_dict = torch.load(checkpoint_filename)
+        if config_filename is not None:
+            config = self._load_config(config_filename)
+            self.config.update(config)
+        self.model = state_dict['model']
     
-    def eval(self, mode=False):
-        self.training = mode
-        self.model.eval()
-        return self
+    def get_train_dataloader(self, train_data):
+        dataloader = DataLoader(train_data,
+            batch_size=self.config['batch_size'],
+            num_workers=self.config['num_worker'],
+            pin_memory=True,
+            shuffle=True,
+            collate_fn=SiteSelectionBaseCollator(
+                config={
+                    'has_demographics': isinstance(train_data.sites, SiteBaseDemographics)
+                    }
+                ),
+            )
+        return dataloader
 
-    @abc.abstractmethod
     def _build_model(self):
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def __getitem__(self, tag):
-        '''
-        Get the embeddings of documents by the trial tags.
-
-        Parameters
-        ----------
-        tag: str, int, list[str], list[int]
-            The tag (or tags) to be looked up in the model.
-
-        Returns
-        -------
-        The embeddings of each document.
-        '''
-        raise NotImplementedError
-
-
-
-    def _save_checkpoint(self, state,
-                        epoch_id=0,
-                        is_best=False,
-                        output_dir=None,
-                        filename='checkpoint.pth.tar'):
-        if output_dir is None:
-            output_dir = self.checkout_dir
-
-        if epoch_id < 1:
-            filepath = os.path.join(output_dir, 'latest.' + filename)
-        elif is_best:
-            filepath = os.path.join(output_dir, 'best.' + filename)
+        self.model = BuildModel(
+            trial_dim=self.config['trial_dim'],
+            site_dim=self.config['site_dim'],
+            embedding_dim=self.config['embedding_dim']
+            )
+    
+    def _build_loss_model(self):
+        if self.config['enrollment_only']:
+            return PolicyGradientLossEnrollment(self.model, self.config['K'])
         else:
-            filepath = os.path.join(self.checkout_dir,
-                                    str(epoch_id) + '.' + filename)
-        torch.save(state, filepath)
+            return PolicyGradientLossCombined(self.model, self.config['K'], self.config['lambda'])     
 
-    def _save_model_config(self, model_config, output_dir=None):
-        if output_dir is None:
-            output_dir = self.checkout_dir
-        temp_path = os.path.join(output_dir, "model_config.json")
-        if os.path.exists(temp_path):
-            os.remove(temp_path)
-        with open(temp_path, "w", encoding='utf-8') as f:
-            f.write(json.dumps(model_config, indent=4))
-
-    def _load_model_config(self, checkpoint=''):
-        if checkpoint == '':
-            temp_path = os.path.join(self.checkout_dir,
-                                     'model_config.json')
-            assert os.path.exists(
-                temp_path), 'cannot find predictor_config.json, please it in dir {0}'.format(
-                self.checkout_dir)
-        else:
-            temp_path = checkpoint
-            assert os.path.exists(
-                temp_path), 'cannot find checkpoint file from path: {0}'.format(
-                checkpoint)
-        print('load predictor config file from {0}'.format(temp_path))
-        with open(temp_path, 'r') as f:
-            predictor_config = json.load(f)
-        return predictor_config
-
-    def _input_data_check(self, inputs):
-        '''
-        Check the training / testing data fits the formats.
-        Target to (1) check if inputs valid,
-                    if not, give tips about the data problem.
+    def _fit_model(self, train_data):
+        train_dataloader = self.get_train_dataloader(train_data)
+        loss_model = self._build_loss_model()
+        train_objectives = [(train_dataloader, loss_model)]
+        trainer = SiteSelectTrainer(
+            model=self,
+            train_objectives=train_objectives
+            )
+        trainer.train(**self.config)
+        
+    def _prepare_input(self, data):
+        '''
+        Prepare inputs to model.
 
         Parameters
         ----------
-        inputs: {
-                'x': pd.DataFrame,
-                'fields': list[str],
-                'tag': str,
-                }
-        '''
-        # check overall input format
-        assert 'x' in inputs, 'No input trial doc dataframe found in inputs.'
-        df = inputs['x']
-        if 'fields' in inputs:
-            try:
-                _ = df[inputs['fields']]
-            except:
-                raise Exception('Cannot find the specified `fields` in inputs dataframe.')
-        if 'tag' in inputs:
-            try:
-                _ = df[inputs['tag']]
-            except:
-                raise Exception('Cannot find the specified `tag` in inputs dataframe.')
-
-        # check data type
-        try:
-            _ = df.applymap(str)
-        except:
-            raise Exception('Cannot transform the input dataframe to str type, please check the inputs.')
-
-    def _process_dataframe(self, df, fields):
-        if fields is not None:
-            df = df[fields]
-        if 'nct_id' in df:
-            df = df.drop(['nct_id'], axis=1)
-        df = df.applymap(str)
-        df = df.apply(lambda x: x.name + ': ' + x)
-        df = df.applymap(lambda x: x.lower())
-        df_raw_texts = df.agg(' '.join, axis=1)
-        df_raw_texts = pd.DataFrame(df_raw_texts, columns=['text'])
-        return df_raw_texts
-
+        data: dict[list]
+            A batch of trials with their corresponding sites.
+        '''
+        inputs = {
+            'trial': data['trial'].to(self.device),
+            'site': data['site'].to(self.device),
+            'label': data['label'].to(self.device),
+            'eth_label': None if data['eth_label'] is None else data['eth_label'].to(self.device)
+            }
 
-def whitening_torch_final(embeddings):
-    '''
-    Whitening the embeddings.
+        return inputs
 
-    Parameters
-    ----------
-    embeddings: torch.Tensor
-        The embeddings to be whitened. The shape is (n, d).
-    '''
-    mu = torch.mean(embeddings, dim=0, keepdim=True)
-    cov = torch.mm((embeddings - mu).t(), embeddings - mu)
-    u, s, vt = torch.svd(cov)
-    W = torch.mm(u, torch.diag(1/torch.sqrt(s)))
-    embeddings = torch.mm(embeddings - mu, W)
-    return embeddings
+    def _input_data_check(self, inputs):
+        assert isinstance(inputs, TrialSiteSimple), f'`site_selection` models require input training data in `TrialSiteSimple`, find {type(inputs)} instead.'
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/models/doc2vec.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/models/doc2vec.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/models/trial2vec.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/models/trial2vec.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_search/models/whiten_bert.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_search/models/whiten_bert.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/data.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/data.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/losses.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/losses.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/base.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import abc
 import pdb
 import os
 import json
 import math
+from collections import defaultdict
 
+import numpy as np
+import pandas as pd
 import torch
 from torch import nn
 from torch.nn.utils.rnn import pad_sequence
+from tqdm import tqdm
 
 from pytrial.utils.check import check_model_dir
 from pytrial.utils.check import make_dir_if_not_exist
 from pytrial.tasks.trial_simulation.data import SequencePatient
 
 class SequenceSimulationBase(abc.ABC):
     '''Abstract class for all sequential patient data simulations.
@@ -315,8 +319,63 @@
             bidirectional=bidirectional,
             batch_first=True,
         )
         self.bidirectional = bidirectional
     
     def forward(self, x):
         outputs = self.model(x)[0]
-        return outputs
+        return outputs
+
+
+def transform_sequence_to_table(data, order, voc):
+    # init the outputs
+    outputs = defaultdict(list)
+    outputs['pid'] = []
+    outputs['vid'] = []
+    columns = []
+    for od in order:
+        for k in voc[od].word2idx.keys():
+            columns.append(f'{od}_{k}')
+
+    output_list = []
+    for pid, sample in tqdm(enumerate(data),desc='Transforming sequence to tabular format', total=len(data)):
+        for vid, visit in enumerate(sample):
+            visit_ = []
+            for i, event_type in enumerate(order):
+                visit_.extend([columns.index(f'{event_type}_{voc[event_type].idx2word[v]}') for v in visit[i]])
+
+            visit_mh = np.zeros(len(columns))
+            visit_mh[visit_] = 1
+            outputs['pid'].append(pid)
+            outputs['vid'].append(vid)
+            output_list.append(visit_mh)
+
+    output_df = pd.DataFrame(output_list, columns=columns)
+    index_df = pd.DataFrame(outputs)
+    output_df = pd.concat([index_df, output_df], axis=1)
+    return output_df
+
+def transform_table_to_sequence(data, order, voc):
+    '''
+    data: pd.DataFrame
+    one column for each event type
+    one row for each visit
+    pid: patient id
+    vid: visit id
+    transform the outputs to the original format
+    v = [[event1, event2, ...], [event1, event2, ...], ], [event1, event2, ...], ...]
+    each v[i] is a patient
+    each v[i][j] is a visit
+    each v[i][j][k] is a list of that type of events
+    '''
+    outputs = []
+    pid_list = []
+    for pid, sample in tqdm(data.groupby('pid'), desc='Transforming tabular format to sequence', total=len(data['pid'].unique())):
+        output = []
+        for vid, visit in sample.groupby('vid'):
+            visit_ = []
+            for i, event_type in enumerate(order):
+                visit_.append([voc[event_type].word2idx[k.split('_')[-1]] for k in visit.columns if k.startswith(event_type) and visit[k].values[0]==1])
+            output.append(visit_)
+        outputs.append(output)
+        pid_list.append(pid)
+    return outputs, pid_list
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/eva.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/eva.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/promptehr.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/promptehr.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,24 @@
         baseline features are **ALWAYS** numerical feature first. That is to say,
         the input baseline ``feature = [num1, num2, .., num_n, cat1, cat2,...]``.
 
     cat_cardinalities: list[int]
         The number of categories for each categorical patient baseline features.
         The input baseline ``feature = [num1, num2, .., num_n, cat1, cat2,...]``.
 
-    epoch: int
+    epochs: int
         Num training epochs in total.
 
     batch_size: int
         Training batch size.
 
     eval_batch_size: int
         Evaluation batch size.
     
-    eval_step: int
+    evaluation_steps: int
         How many steps of updates then try to evaluate the trained models.
     
     learning_rate: float
         Training learning rate.
     
     weight_decay: float
         Training weight decay.
@@ -76,33 +76,33 @@
         'temperature': 1.0,
         'max_length': 6,
     }
     def __init__(self,
         code_type=None,
         n_num_feature=None,
         cat_cardinalities=None,
-        epoch=50,
+        epochs=50,
         batch_size=16,
         eval_batch_size=16,
-        eval_step=1000,
+        evaluation_steps=1000,
         learning_rate=5e-5,
         weight_decay=1e-4,
         num_worker=8,
         device='cuda:0',
         experiment_id='trial_simulation.sequence.promptehr',
         ):
         super().__init__(experiment_id)
         self.config = {
             'code_type': code_type,
             'n_num_feature':n_num_feature,
             'cat_cardinalities':cat_cardinalities,
-            'epoch':epoch,
+            'epoch':epochs,
             'batch_size':batch_size,
             'eval_batch_size':eval_batch_size,
-            'eval_step':eval_step,
+            'eval_step':evaluation_steps,
             'learning_rate':learning_rate,
             'weight_decay':weight_decay,
             'num_worker':num_worker,
             'output_dir':self.checkout_dir,
             'device':device,
         }
         config = deepcopy(self.config)
@@ -217,11 +217,20 @@
         ----------
         input_dir: str
             The path to the pretrained model. If no found, will download from online and save
             to this folder.
         '''
         self.model.from_pretrained(input_dir=input_dir)
         self.config.update(self.model.config)
+    
+    def update_config(self, config):
+        '''
+        Update the model configuration. Will be useful when load pretrained model
+        and want to finetune on new data.
 
-    # def _build_model(self):
-    #     config = deepcopy(self.config)
-    #     self.model = BuildModel(config)
+        Parameters
+        ----------
+        config: dict
+            The configuration for the model.
+        '''
+        self.config.update(config)
+        self.model.update_config(config)
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/rnn_gan.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/rnn_gan.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/sequence/synteg.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/sequence/synteg.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/base.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/copula_gan.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/copula_gan.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,16 +214,15 @@
             cuda=config['cuda'],
             )
         return model
 
 
 class CopulaGAN(TabularSimulationBase):
     '''
-    Implement CopulaGAN model for tabular simulation
-    prediction in clinical trials.
+    Implement CopulaGAN model for tabular patient data simulation [1]_.
 
     Parameters
     ----------
     embedding_dim: int
         Size of the random sample passed to the Generator. Defaults to 128.
 
     generator_dim: tuple or list of int:
@@ -270,14 +269,18 @@
     
     cuda: bool or str
         - If ``True``, use CUDA. If a ``str``, use the indicated device.
         - If ``False``, do not use cuda at all.
         
     experiment_id: str, optional
         The name of current experiment. Decide the saved model checkpoint name.
+
+    Notes
+    -----
+    .. [1] Xu, L., Skoularidou, M., Cuesta-Infante, A., & Veeramachaneni, K. (2019). Modeling tabular data using conditional gan. Advances in Neural Information Processing Systems, 32.
     '''
     def __init__(
         self,
         embedding_dim=128,
         generator_dim=(256, 256),
         discriminator_dim=(256, 256),
         generator_lr=2e-4,
@@ -331,29 +334,29 @@
         if isinstance(train_data, dict): 
             dataset = TabularPatientBase(train_data, transform=True)
             dataset = dataset.df
         self._fit_model(dataset)
         self.metadata = train_data.metadata
         self.raw_dataset = train_data
         
-    def predict(self, number_of_predictions=200):
+    def predict(self, n=200):
         '''
         Simulate new tabular data with number_of_predictions.
 
         Parameters
         ----------
-        number_of_predictions: int
+        n: int
             The number of synthetic data to generate.
 
         Returns
         -------
         ypred: TabularPatientBase
             A new tabular data simulated by the model
         '''
-        ypred = self.model.sample(number_of_predictions)  # build df
+        ypred = self.model.sample(n)  # build df
         ypred = self.raw_dataset.reverse_transform(ypred) # transform back
         return ypred # output: dataset, same as the input dataset
 
     def save_model(self, output_dir=None):
         '''
         Save the learned CopulaGAN model to the disk.
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/ct_gan.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/ct_gan.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,70 +35,73 @@
             )
 
         return model
 
 
 class CTGAN(TabularSimulationBase):
     '''
-    Implement CTGAN model for tabular simulation
-    prediction in clinical trials.
+    Implement CTGAN model for patient level tabular data generation [1]_.
 
     Parameters
     ----------
-    embedding_dim (int):
+    embedding_dim: int
         Size of the random sample passed to the Generator. Defaults to 128.
 
-    generator_dim (tuple or list of ints):
+    generator_dim: tuple or list of ints
         Size of the output samples for each one of the Residuals. A Residual Layer
         will be created for each one of the values provided. Defaults to (256, 256).
     
-    discriminator_dim (tuple or list of ints):
+    discriminator_dim: tuple or list of ints
         Size of the output samples for each one of the Discriminator Layers. A Linear Layer
         will be created for each one of the values provided. Defaults to (256, 256).
     
-    generator_lr (float):
+    generator_lr: float
         Learning rate for the generator. Defaults to 2e-4.
     
-    generator_decay (float):
+    generator_decay: float
         Generator weight decay for the Adam Optimizer. Defaults to 1e-6.
     
-    discriminator_lr (float):
+    discriminator_lr: float
         Learning rate for the discriminator. Defaults to 2e-4.
     
-    discriminator_decay (float):
+    discriminator_decay: float
         Discriminator weight decay for the Adam Optimizer. Defaults to 1e-6.
     
-    batch_size (int):
+    batch_size: int
         Number of data samples to process in each step.
     
-    discriminator_steps (int):
+    discriminator_steps: int
         Number of discriminator updates to do for each generator update.
         From the WGAN paper: https://arxiv.org/abs/1701.07875. WGAN paper
         default is 5. Default used is 1 to match original CTGAN implementation.
     
-    log_frequency (boolean):
+    log_frequency: bool
         Whether to use log frequency of categorical levels in conditional
         sampling. Defaults to ``True``.
     
-    verbose (boolean):
+    verbose: bool
         Whether to have print statements for progress results. Defaults to ``True``.
     
-    epochs (int):
+    epochs: int
         Number of training epochs. Defaults to 300.
     
-    pac (int):
+    pac: int
         Number of samples to group together when applying the discriminator.
         Defaults to 10.
     
-    cuda (bool or str):
+    cuda: bool or str
         If ``True``, use CUDA. If a ``str``, use the indicated device.
         If ``False``, do not use cuda at all.
 
     experiment_id: str, optional (default='trial_simulation.tabular.ctgan')
         The name of current experiment. Decide the saved model checkpoint name.
+
+    Notes
+    -----
+    .. [1] Xu, L., Skoularidou, M., Cuesta-Infante, A., & Veeramachaneni, K. (2019). Modeling tabular data using conditional gan. Advances in Neural Information Processing Systems, 32.
     '''
     def __init__(
             self,
             embedding_dim=128,
             generator_dim=(256, 256),
             discriminator_dim=(256, 256),
             generator_lr=2e-4,
@@ -133,20 +136,20 @@
             'experiment_id': experiment_id,
             'model_name': 'ct_gan',
         }
         self._save_config(self.config)
 
     def fit(self, train_data):
         '''
-        Train CTGAN model to simulate patient outcome
-        with tabular input data.
+        Train CTGAN model to simulate tabular patient data.
         
         Parameters
         ----------
-        train_data: tabular data
+        train_data: TabularPatientBase
+            The training data.
         '''
         self._input_data_check(train_data)
         self._build_model()
         if isinstance(train_data, TabularPatientBase):  # transform=True
             self.metadata = train_data.metadata
             self.raw_dataset = train_data
         if isinstance(train_data, dict):
@@ -161,57 +164,56 @@
             field_name = field.replace('.value', '')
             if field_name in fields_names:
                 meta = fields_names[field_name]
                 if meta == 'categorical':
                     categoricals.append(field)
         self._fit_model(dataset, categoricals)
 
-    def predict(self, number_of_predictions=200):
+    def predict(self, n=200):
         '''
         simulate a new tabular data with number_of_predictions.
 
         Parameters
         ----------
-        number_of_predictions: number of predictions
+        n: int
+            number of synthetic records going to generate.
 
         Returns
         -------
         ypred: dataset, same as the input dataset
             A new tabular data simulated by the model
         '''
-        ypred = self.model.sample(number_of_predictions)  # build df
+        ypred = self.model.sample(n)  # build df
         return ypred  # output: dataset, same as the input dataset, don't need to transform back
 
     def save_model(self, output_dir=None):
         '''
         Save the learned CTGAN model to the disk.
 
         Parameters
         ----------
-
         output_dir: str or None
             The dir to save the learned model.
             If set None, will save model to `self.checkout_dir`.
         '''
-        if output_dir is not None:
-            make_dir_if_not_exist(output_dir)
-        else:
+        if output_dir is None:
             output_dir = self.checkout_dir
 
+        make_dir_if_not_exist(output_dir)
+
         self._save_config(self.config, output_dir=output_dir)
         ckpt_path = os.path.join(output_dir, 'ctgan.model')
         joblib.dump(self.model, ckpt_path)
 
     def load_model(self, checkpoint=None):
         '''
         Save the learned CTGAN model to the disk.
 
         Parameters
         ----------
-        
         checkpoint: str or None
             If a directory, the only checkpoint file `.model` will be loaded.
             If a filepath, will load from this file;
             If None, will load from `self.checkout_dir`.
         '''
         if checkpoint is None:
             checkpoint = self.checkout_dir
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/evaluation.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/evaluation.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 class BuildModel:
     def __new__(self) -> GaussianMultivariate:
         return GaussianMultivariate()
 
 class GaussianCopula(TabularSimulationBase):
     '''
-    Implement Gaussian Copula model for tabular simulation
-    prediction in clinical trials.
+    Implement Gaussian Copula model for tabular patient simulation.
 
     Parameters
     ----------
     experiment_id: str, optional (default='trial_simulation.tabular.gaussiancopula')
         The name of current experiment. Decide the saved model checkpoint name.
     '''
     def __init__(
@@ -51,29 +50,29 @@
         if isinstance(train_data, dict): 
             dataset = TabularPatientBase(train_data, transform=True)
             dataset = dataset.df
         self._fit_model(dataset)
         self.metadata = train_data.metadata
         self.raw_dataset = train_data
 
-    def predict(self, number_of_predictions=200):
+    def predict(self, n=200):
         '''
         simulate a new tabular data with number_of_predictions.
 
         Parameters
         ----------
-        number_of_predictions: int
+        n: int
             The number of synthetic samples to generation.
 
         Returns
         -------
         ypred: TabularPatientBase
             A new tabular data simulated by the model
         '''
-        ypred = self.model.sample(number_of_predictions) # build df
+        ypred = self.model.sample(n) # build df
         ypred = self.raw_dataset.reverse_transform(ypred) # transform back
         return ypred # output: dataset, same as the input dataset
 
     def save_model(self, output_dir=None):
         '''
         Save the learned gaussian copula model to the disk.
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/tabular/tvae.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/tabular/tvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,15 @@
             )
 
         return model
 
 
 class TVAE(TabularSimulationBase):
     '''
-    Implement TVAE model for tabular simulation
-    prediction in clinical trials.
+    Implement TVAE model for tabular patient data simulation [1]_.
 
     Parameters
     ----------
     embedding_dim: int
         Size of the random sample passed to the Generator. Defaults to 128.
 
     compress_dims: tuple or list[int]
@@ -132,14 +131,18 @@
     
     cuda: bool or str
         - If ``True``, use CUDA. If a ``str``, use the indicated device.
         - If ``False``, do not use cuda at all.
 
     experiment_id: str, optional
         The name of current experiment. Decide the saved model checkpoint name.
+
+    Notes
+    -----
+    .. [1] Xu, L., Skoularidou, M., Cuesta-Infante, A., & Veeramachaneni, K. (2019). Modeling tabular data using conditional gan. Advances in Neural Information Processing Systems, 32.
     '''
     def __init__(
         self,
         embedding_dim=128,
         compress_dims=(128, 128),
         decompress_dims=(128, 128),
         l2scale=1e-5,
@@ -194,29 +197,29 @@
             if field_name in fields_before_transform:
                 meta = fields_before_transform[field_name]
                 if meta == 'categorical':
                     categoricals.append(field)
 
         self._fit_model(dataset, categoricals) 
 
-    def predict(self, number_of_predictions=200):
+    def predict(self, n=200):
         '''
-        simulate a new tabular data with number_of_predictions.
+        simulate a new tabular data with n.
 
         Parameters
         ----------
-        number_of_predictions: int
+        n: int
             The number of new data to simulate.
 
         Returns
         -------
         ypred: TanularPatientBase
             A new tabular data simulated by the model
         '''
-        ypred = self.model.sample(number_of_predictions) # build df
+        ypred = self.model.sample(n) # build df
         return ypred # output: dataset, same as the input dataset not transform back
 
     def save_model(self, output_dir=None):
         '''
         Save the learned TVAE model to the disk.
 
         Parameters
```

### Comparing `PromptEHR-0.0.5/pytrial/tasks/trial_simulation/trainer.py` & `PromptEHR-0.0.6/pytrial/tasks/trial_simulation/trainer.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/utils/check.py` & `PromptEHR-0.0.6/pytrial/utils/check.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/utils/mimic_utils.py` & `PromptEHR-0.0.6/pytrial/utils/mimic_utils.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/utils/parallel.py` & `PromptEHR-0.0.6/pytrial/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/pytrial/utils/tabular_utils.py` & `PromptEHR-0.0.6/pytrial/utils/tabular_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,30 +8,34 @@
 max_categories and min_frequencies, refer to https://scikit-learn.org/stable/modules/preprocessing.html.
 '''
 from collections import defaultdict
 import pickle
 from pathlib import Path
 import pdb
 import os
+from copy import deepcopy
 
 import pandas as pd
 import numpy as np
 from sklearn.preprocessing import StandardScaler as sk_standardscaler
 from sklearn.preprocessing import MinMaxScaler as sk_minmaxscaler
 import rdt
 from rdt.hyper_transformer import Config
+from rdt.errors import InvalidConfigError
+from rdt.transformers import BaseTransformer
 from rdt.transformers import LabelEncoder, BinaryEncoder, UnixTimestampEncoder
 from rdt.transformers.numerical import FloatFormatter
+from rdt.transformers.categorical import OneHotEncoder, FrequencyEncoder
 
 class StandardScaler(FloatFormatter):
     '''Transformer for numerical data.
 
     This transformer scales all numerical values within the same column using
     `sklearn.preprocessing.StandardScaler`.
-
+    
     Null values are replaced using a `NullTransformer` from rdt.
 
     Parameters
     ----------
     missing_value_replacement: object or None
         Indicate what to do with the null values. If an integer or float is given,
         replace them with the given value. If the strings ``'mean'`` or ``'mode'`` are
@@ -43,36 +47,57 @@
         max values seen during ``fit``. Defaults to ``False``.
 
     learn_rounding_scheme (bool):
         Whether or not to learn what place to round to based on the data seen during ``fit``.
         If ``True``, the data returned by ``reverse_transform`` will be rounded to that place.
         Defaults to ``False``.
 
+    missing_value_generation (str or None):
+        The way missing values are being handled. There are three strategies:
+
+            * ``random``: Randomly generates missing values based on the percentage of
+                missing values.
+            * ``from_column``: Creates a binary column that describes whether the original
+                value was missing. Then use it to recreate missing values.
+            * ``None``: Do nothing with the missing values on the reverse transform. Simply
+                pass whatever data we get through.
+
+    computer_representation (dtype):
+        Accepts ``'Int8'``, ``'Int16'``, ``'Int32'``, ``'Int64'``, ``'UInt8'``, ``'UInt16'``,
+        ``'UInt32'``, ``'UInt64'``, ``'Float'``.
+        Defaults to ``'Float'``.
+
     model_missing_values (bool):
-        Whether to create a new column to indicate which values were null or not. The column
+        **Deprecated** Whether to create a new column to indicate which values were null or not. The column
         will be created only if there are null values. If ``True``, create the new column if
         there are null values. If ``False``, do not create the new column even if there
         are null values. Defaults to ``False``.
     '''
     _dtype = None
     _min_value = None
     _max_value = None
+    random_states = None
 
     def __init__(self,
         missing_value_replacement=None,
         enforce_min_max_values=False,
         learn_rounding_scheme=False,
+        computer_representation='Float',
+        missing_value_generation="random",
         model_missing_values=None,
-        computer_representation='Float'
         ):
-        self.missing_value_replacement = missing_value_replacement
-        self.enforce_min_max_values=enforce_min_max_values
-        self.learn_rounding_scheme=learn_rounding_scheme
-        self.model_missing_values = model_missing_values
-        self.computer_representation = computer_representation
+        self.output_properties = {None: {'sdtype': 'float', 'next_transformer': None}}
+        super().__init__(
+            missing_value_replacement=missing_value_replacement,
+            model_missing_values=model_missing_values,
+            learn_rounding_scheme=learn_rounding_scheme,
+            enforce_min_max_values=enforce_min_max_values,
+            computer_representation=computer_representation,
+            missing_value_generation=missing_value_generation,
+        )
         self.standard_transformer = sk_standardscaler()
 
     def _fit(self, data):
         '''
         Fit the transformer to the data.
 
         Parameters
@@ -190,14 +215,21 @@
         self.standard_transformer = sk_minmaxscaler()
 
 
 class HyperTransformer(rdt.HyperTransformer):
     '''
     A subclass of `rdt.HyperTransformer` to set special setups.
     '''
+    _DTYPES_TO_SDTYPES = {
+        'i': 'categorical', # change the default from numerical to categorical for integers
+        'f': 'numerical',
+        'O': 'categorical',
+        'b': 'boolean',
+        'M': 'datetime',
+    }
     def __init__(self):
         self._default_sdtype_transformers = {
             'numerical': StandardScaler(missing_value_replacement='mean'),
             'categorical': LabelEncoder(),
             'boolean': BinaryEncoder(missing_value_replacement='mode'),
             'datetime': UnixTimestampEncoder(missing_value_replacement='mean'),
         }
@@ -244,14 +276,55 @@
             'transformers': self.field_transformers
         })
 
         if verbose:
             self._user_message('Config:')
             self._user_message(config)
 
+    @staticmethod
+    def _validate_transformers(column_name_to_transformer):
+        """Validate the given transformers are valid.
+        Args:
+            column_name_to_transformer (dict):
+                Dict mapping column names to transformers to be used for that column.
+        Raises:
+            Error:
+                Raises an error if ``column_name_to_transformer`` contains one or more
+                invalid transformers.
+        """
+        invalid_transformers_columns = []
+        update_transformers = {}
+        for column_name, transformer in column_name_to_transformer.items():
+            if transformer and not isinstance(transformer, BaseTransformer):
+                if isinstance(transformer, str):
+                    if get_transformer(transformer) is None:
+                        invalid_transformers_columns.append(column_name)
+                    else:
+                        # update the column_name_to_transformer dict with str inputs
+                        update_transformers[column_name] = get_transformer(transformer)()
+
+        if invalid_transformers_columns:
+            raise InvalidConfigError(
+                f'Invalid transformers for columns: {invalid_transformers_columns}. '
+                'Please assign an rdt transformer instance to each column name.'
+            )
+        
+        column_name_to_transformer.update(update_transformers)
+    
+    def _set_field_sdtype(self, data, field):
+        clean_data = data[field].dropna()
+        kind = clean_data.infer_objects().dtype.kind
+        if kind == 'i':
+            # decide if it is categorical or binary for input integers
+            if len(clean_data.unique()) <= 2:
+                kind = 'b'
+            else:
+                kind = 'O'
+        self.field_sdtypes[field] = self._DTYPES_TO_SDTYPES[kind]
+
 
 def read_csv_to_df(file_loc, header_lower=True, usecols=None, dtype=None,
                    low_memory=True, encoding=None, index_col=None):
     """Read in csv files with necessary processing
     Parameters
     ----------
     file_loc
@@ -365,8 +438,22 @@
 
     return {
         'columns': all_feat_list,
         'num_feat': num_feat_list,
         'bin_feat': bin_feat_list,
         'cat_feat': cat_feat_list,
         'cat_cardinalities': cat_cardinalities,
-    }
+    }
+
+def get_transformer(name):
+    mapping = {
+        'labelencoder':LabelEncoder,
+        'onehotencoder':OneHotEncoder,
+        'binaryencoder':BinaryEncoder,
+        'floatformatter':FloatFormatter,
+        'frequencyencoder':FrequencyEncoder,
+        'unixtimeformatter':UnixTimestampEncoder,
+    }
+    if isinstance(name, str):
+        return mapping.get(name.lower(), None)
+    else:
+        raise ValueError('The input transformer name must be a string. Get {} instead.'.format(type(name)))
```

### Comparing `PromptEHR-0.0.5/pytrial/utils/trainer.py` & `PromptEHR-0.0.6/pytrial/utils/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,36 +114,39 @@
         **kwargs,
         ):
         '''
         Kick of training using the provided loss model and train dataloaders.
 
         Parameters
         ----------
-        epochs: int, optional (default=10)
-            Number of iterations (epochs) over the corpus. Defaults to 10 for Doc2Vec.
+        epochs: int (default=10)
+            Number of iterations (epochs) over the corpus.
 
-        learning_rate: float, optional (default=3e-5)
+        learning_rate: float (default=3e-5)
             The learning rate.
 
-        weight_decay: float, optional (default=1e-4)
+        weight_decay: float (default=1e-4)
             Weight decay applied for regularization.
 
         warmup_ratio: float (default=0)
-            How many steps used for warmup training. If set 0, not warmup.
+            How many steps used for warmup training. 
+            
+            If set 0, not warmup.
 
-        scheduler: str (default='warmupcosine')
+        scheduler: {'constantlr','warmupconstant','warmuplinear','warmupcosine','warmupcosinewithhardrestarts'}
             Pick learning rate scheduler for warmup. Ignored if warmup_ratio <= 0.
-            in ['constantlr','warmupconstant','warmuplinear','warmupcosine','warmupcosinewithhardrestarts'].
 
         evaluation_steps: int (default=10)
-            How many iterations while we print the training loss and
+            How many iterations 
+            
+            while we print the training loss and
             conduct evaluation if evaluator is given.
 
         max_grad_norm: float (default=0.5)
-            Clip the gradient to avoid NaN in some cases.
+            Clip the gradient to avoid NaN.
 
         use_amp: bool (default=False)
             Whether or not use mixed precision training.
         '''
         self.best_score = np.inf if self.less_is_better else -np.inf
 
         self.score_logs = defaultdict(list)
@@ -225,27 +228,23 @@
                         # update best score and save checkpoints
                         best_score = self._update_best_metric(self.best_score, metric_value, self.less_is_better)
                         if best_score != self.best_score:
                             self.score_logs['best_global_step'] = global_step
                             model = unwrap_model(self.model)
                             model.save_model(self.best_dir)
                             self.best_score = best_score
+                            print(f'Best checkpoint is updated at {global_step} with {self.test_metric} {self.best_score}.')
 
-                            best_score = self._update_best_metric(self.best_score, metric_value, self.less_is_better)
-                            if best_score != self.best_score:
-                                self.score_logs['best_global_step'] = global_step
-                                model = unwrap_model(self.model)
-                                model.save_model(self.best_dir)
-                                self.best_score = best_score
-
-                    # save model checkpoint
-                    output_dir = os.path.join(self.output_dir, f'./{global_step}')
-                    make_dir_if_not_exist(output_dir)
-                    model = unwrap_model(self.model)
-                    model.save_model(output_dir)
+                    else:
+                        # save model checkpoint
+                        output_dir = os.path.join(self.output_dir, f'./{global_step}')
+                        make_dir_if_not_exist(output_dir)
+                        model = unwrap_model(self.model)
+                        model.save_model(output_dir)
+                        print("Checkpoint saved in {} at {} steps.".format(output_dir, global_step))
 
         # after training
         self._save_log(self.output_dir)
         if self.load_best_at_end and self.test_dataloader is not None and self.evaluated:
             print(f'Load best ckpt from `{self.best_dir}`.')
             self.model.load_model(self.best_dir)
 
@@ -377,27 +376,30 @@
             return transformers.get_cosine_with_hard_restarts_schedule_with_warmup(optimizer, num_warmup_steps=warmup_steps, num_training_steps=t_total)
         else:
             raise ValueError("Unknown scheduler {}".format(scheduler))
 
     def _update_best_metric(self, best_score, metric_value, less_is_better):
         if less_is_better:
             if metric_value < best_score:
+                print("New best score: from {} to {}".format(best_score, metric_value))
                 return metric_value
             else:
                 return best_score
         else:
             if metric_value > best_score:
+                print("New best score: from {} to {}".format(best_score, metric_value))
                 return metric_value
             else:
                 return best_score
 
     def _save_log(self, output_dir):
         log_filename = os.path.join(output_dir, 'train_logs.json')
         with open(log_filename, 'w') as f:
-            f.write(json.dumps(self.score_logs))
+            score_logs = str(self.score_logs)
+            f.write(json.dumps(score_logs, indent=4, sort_keys=True))
 
     def _wrap_model(self, model):
         # wrap model to be paralleled
         model = DataParallelModel(model)
         return model
 
     def _compute_num_train_samples(self, dataloader):
```

### Comparing `PromptEHR-0.0.5/pytrial/utils/trial_utils.py` & `PromptEHR-0.0.6/pytrial/utils/trial_utils.py`

 * *Files identical despite different names*

### Comparing `PromptEHR-0.0.5/setup.py` & `PromptEHR-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'PromptEHR',
-    version = '0.0.5',
+    version = '0.0.6',
     author = 'Zifeng Wang',
     author_email = 'zifengw2@illinois.edu',
     description = 'Sequence patient electronic healthcare record generation with large language models (LLMs) as the neural database.',
     url = 'https://github.com/RyanWangZf/PromptEHR',
-    keywords=['healthcare','EHR','deep learning','AI'],
+    keywords=['synthetic data','healthcare','EHR','deep learning','AI'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude=['test']),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

