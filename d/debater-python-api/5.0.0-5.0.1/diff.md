# Comparing `tmp/debater_python_api-5.0.0.tar.gz` & `tmp/debater_python_api-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debater_python_api-5.0.0.tar", last modified: Mon Jun  5 12:57:00 2023, max compression
+gzip compressed data, was "debater_python_api-5.0.1.tar", last modified: Thu Jun  8 10:47:07 2023, max compression
```

## Comparing `debater_python_api-5.0.0.tar` & `debater_python_api-5.0.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.259941 debater_python_api-5.0.0/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    11358 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/LICENSE
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-05 12:57:00.259727 debater_python_api-5.0.0/PKG-INFO
--rw-r--r--   0 yoavkantor   (501) staff       (20)      169 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/README.md
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.246186 debater_python_api-5.0.0/debater_python_api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.247191 debater_python_api-5.0.0/debater_python_api/api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.251223 debater_python_api-5.0.0/debater_python_api/api/clients/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4503 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/abstract_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1147 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/argument_quality_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1548 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/claim_and_evidence_detection_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      934 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/claim_boundaries_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6203 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/clustering_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3034 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/embedding_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1999 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/index_searcher_client.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.252076 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/
--rw-r--r--   0 yoavkantor   (501) staff       (20)      478 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    35911 2023-06-05 12:56:29.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/KpsResult.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13092 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/docx_generator.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    14916 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/graph_generator.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3923 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/utils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6969 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_admin_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    39177 2023-06-05 12:50:31.000000 debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1894 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_pairs_infer_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13830 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/narrative_generation_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1230 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/pro_con_client.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.252351 debater_python_api-5.0.0/debater_python_api/api/clients/response_data/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/response_data/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1597 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/response_data/speech_response.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1790 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/term_relater_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1563 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/term_wikifier_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3394 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/theme_extraction_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3263 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/debater_api.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.252597 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.253750 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      142 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     5079 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1001 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1314 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3576 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1516 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.256659 debater_python_api-5.0.0/debater_python_api/examples/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      803 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/argument_quality_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      854 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/claim_boundaries_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1002 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/claim_detection_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      932 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/clustering_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      860 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/embedding_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1014 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/evidence_detection_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    85859 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/example_of_sc_args.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1480 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/index_searcher_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1204 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/examples/keypoints_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1428 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/pro_con_example.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257144 debater_python_api-5.0.0/debater_python_api/examples/resources/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    23817 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/arguments.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257313 debater_python_api-5.0.0/debater_python_api/examples/resources/filters_output/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/filters_output/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2530 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/pro_con_scores.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     9581 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/run_all_services.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      870 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/speech_construction_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      480 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/term_relater_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      907 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/term_wikifier_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1154 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/theme_extraction_example.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257753 debater_python_api-5.0.0/debater_python_api/examples/usecases/
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4943 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/usecases/kp_based_survey.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6036 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/usecases/mining_to_narrative.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    10191 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/usecases/survey.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257910 debater_python_api-5.0.0/debater_python_api/integration_tests/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.258032 debater_python_api-5.0.0/debater_python_api/integration_tests/api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.258635 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2708 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    11791 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesIT.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4630 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesLoad.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.259448 debater_python_api-5.0.0/debater_python_api/utils/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      992 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/clusters_refiner.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1574 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/general_utils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      604 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/kp_analysis_conf.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.246908 debater_python_api-5.0.0/debater_python_api.egg-info/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4041 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)        1 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)       87 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/requires.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)       19 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/top_level.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)      879 2023-06-05 12:56:29.000000 debater_python_api-5.0.0/pyproject.toml
--rw-r--r--   0 yoavkantor   (501) staff       (20)       38 2023-06-05 12:57:00.259987 debater_python_api-5.0.0/setup.cfg
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.989193 debater_python_api-5.0.1/
+-rw-r--r--   0 lilache    (501) staff       (20)    11358 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/LICENSE
+-rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-08 10:47:07.988965 debater_python_api-5.0.1/PKG-INFO
+-rw-r--r--   0 lilache    (501) staff       (20)      169 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/README.md
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.974087 debater_python_api-5.0.1/debater_python_api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.975126 debater_python_api-5.0.1/debater_python_api/api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.978248 debater_python_api-5.0.1/debater_python_api/api/clients/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4503 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/abstract_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1147 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/argument_quality_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1548 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/claim_and_evidence_detection_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)      934 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/claim_boundaries_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6203 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/clustering_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3034 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/embedding_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1999 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/index_searcher_client.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.979230 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/
+-rw-r--r--   0 lilache    (501) staff       (20)      478 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
+-rw-r--r--   0 lilache    (501) staff       (20)    35911 2023-06-08 10:37:54.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/KpsResult.py
+-rw-r--r--   0 lilache    (501) staff       (20)    13092 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/docx_generator.py
+-rw-r--r--   0 lilache    (501) staff       (20)    15390 2023-06-08 10:23:01.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/graph_generator.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3923 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/utils.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6969 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_admin_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)    39175 2023-06-08 10:37:54.000000 debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1894 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_pairs_infer_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)    13830 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/narrative_generation_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1230 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/pro_con_client.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.979609 debater_python_api-5.0.1/debater_python_api/api/clients/response_data/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/response_data/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1597 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/response_data/speech_response.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1790 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/term_relater_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1563 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/term_wikifier_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3394 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/clients/theme_extraction_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3263 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/api/debater_api.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.979777 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.981181 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      142 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
+-rw-r--r--   0 lilache    (501) staff       (20)     5079 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1001 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1314 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3576 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1516 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.984779 debater_python_api-5.0.1/debater_python_api/examples/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      803 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/argument_quality_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      854 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/claim_boundaries_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1002 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/claim_detection_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      932 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/clustering_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      860 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/embedding_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1014 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/evidence_detection_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)    85859 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/example_of_sc_args.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1480 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/index_searcher_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1204 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/examples/keypoints_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1428 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/pro_con_example.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.985423 debater_python_api-5.0.1/debater_python_api/examples/resources/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)    23817 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/arguments.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.985638 debater_python_api-5.0.1/debater_python_api/examples/resources/filters_output/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/filters_output/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     2530 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/resources/pro_con_scores.py
+-rw-r--r--   0 lilache    (501) staff       (20)     9581 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/run_all_services.py
+-rw-r--r--   0 lilache    (501) staff       (20)      870 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/speech_construction_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      480 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/term_relater_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      907 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/term_wikifier_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1154 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/theme_extraction_example.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.986132 debater_python_api-5.0.1/debater_python_api/examples/usecases/
+-rw-r--r--   0 lilache    (501) staff       (20)     4943 2023-06-08 10:37:54.000000 debater_python_api-5.0.1/debater_python_api/examples/usecases/kp_based_survey.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6036 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/usecases/mining_to_narrative.py
+-rw-r--r--   0 lilache    (501) staff       (20)    10191 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/examples/usecases/survey.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.986318 debater_python_api-5.0.1/debater_python_api/integration_tests/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.986460 debater_python_api-5.0.1/debater_python_api/integration_tests/api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.987469 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/
+-rw-r--r--   0 lilache    (501) staff       (20)     2708 2023-05-22 15:52:47.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
+-rw-r--r--   0 lilache    (501) staff       (20)    11791 2023-06-05 13:38:02.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesIT.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4630 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesLoad.py
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.988554 debater_python_api-5.0.1/debater_python_api/utils/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/utils/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      992 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/utils/clusters_refiner.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1574 2022-12-12 10:25:59.000000 debater_python_api-5.0.1/debater_python_api/utils/general_utils.py
+-rw-r--r--   0 lilache    (501) staff       (20)      604 2023-05-22 16:30:58.000000 debater_python_api-5.0.1/debater_python_api/utils/kp_analysis_conf.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-08 10:47:07.974867 debater_python_api-5.0.1/debater_python_api.egg-info/
+-rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 lilache    (501) staff       (20)     4041 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lilache    (501) staff       (20)        1 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lilache    (501) staff       (20)       87 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/requires.txt
+-rw-r--r--   0 lilache    (501) staff       (20)       19 2023-06-08 10:47:07.000000 debater_python_api-5.0.1/debater_python_api.egg-info/top_level.txt
+-rw-r--r--   0 lilache    (501) staff       (20)      879 2023-06-08 10:37:43.000000 debater_python_api-5.0.1/pyproject.toml
+-rw-r--r--   0 lilache    (501) staff       (20)       38 2023-06-08 10:47:07.989242 debater_python_api-5.0.1/setup.cfg
```

### Comparing `debater_python_api-5.0.0/LICENSE` & `debater_python_api-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/PKG-INFO` & `debater_python_api-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater_python_api
-Version: 5.0.0
+Version: 5.0.1
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/abstract_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/argument_quality_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/argument_quality_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/claim_and_evidence_detection_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/claim_and_evidence_detection_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/claim_boundaries_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/claim_boundaries_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/clustering_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/clustering_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/embedding_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/embedding_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/index_searcher_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/index_searcher_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/KpsResult.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/KpsResult.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ordered_kps = []
     cols = ['key point']
     for title in titles:
         n_comments_per_kp_per_title = results_to_kp_to_n_comments[title]
         new_kps = set(n_comments_per_kp_per_title.keys()).difference(set(ordered_kps))
         new_kps = sorted(new_kps, key= lambda x:n_comments_per_kp_per_title[x] ,reverse=True)
         ordered_kps += new_kps
-        cols.extend([f"{title}_n_comments", f"{title}_precent"])
+        cols.extend([f"{title}_n_comments", f"{title}_percent"])
 
     if "none" in ordered_kps:
         ordered_kps.remove("none")
 
     add_change = False
     if len(titles) == 2:
         cols.append("change_percent")
```

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/docx_generator.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/docx_generator.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/graph_generator.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/graph_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,22 @@
 
     edges = [e for e in edges if (e['data']['source'] in nodes_ids and e['data']['target'] in nodes_ids)]
 
     if filter_big_to_small_edges:
         edges = [e for e in edges if int(id_to_node[e['data']['source']]['data']['n_matches']) <= int(
             id_to_node[e['data']['target']]['data']['n_matches'])]
 
+        # if source and target have the same number of matches - a cycle can still remain
+        edges_source_target = [(e['data']['source'], e['data']['target']) for e in edges]
+        to_remove = []
+        for (s_id, t_id) in edges_source_target:
+            if s_id < t_id and (t_id, s_id) in edges_source_target:
+                to_remove.append((s_id, t_id))
+        edges = [e for e in edges if (e['data']['source'], e['data']['target']) not in to_remove]
+
     source_target_to_score = {(e['data']['source'], e['data']['target']): e['data']['score'] for e in edges}
 
     # keep only edges to max parent
     id_to_parents = create_dict_to_list([(e['data']['source'], e['data']['target']) for e in edges])
     id_to_max_parent = {}
     for id, parents in id_to_parents.items():
         scores = [source_target_to_score[(id, parent)] if (id, parent) in source_target_to_score else 0.0 for parent in
@@ -300,13 +308,13 @@
     for root in root_ids:
         get_unique_matches_subtree(root, kp_id_to_data, id_to_kids, id_to_n_matches_subtree_sent, kp_to_dicts, by_sentence=True)
         get_unique_matches_subtree(root, kp_id_to_data, id_to_kids, id_to_n_matches_subtree_comments, kp_to_dicts,
                                    by_sentence=False)
 
     for id in kp_id_to_data:
         kp_id_to_data[id].update({'parent':id_to_parent.get(id),
-                                  'n_matching_sents_in_subtree':id_to_n_matches_subtree_sent[id],
-                                  'n_matching_comments_in_subtree':id_to_n_matches_subtree_comments[id],
+                                  'n_matching_sents_in_subtree':id_to_n_matches_subtree_sent.get(id),
+                                  'n_matching_comments_in_subtree':id_to_n_matches_subtree_comments.get(id),
                                   "kids":id_to_kids.get(id, []),
                                   'kp_stance':kp_to_stance[kp_id_to_data[id]['kp']],
                                   'n_matching_comments':kp_to_n_matching_comments[kp_id_to_data[id]['kp']]})
     return kp_id_to_data
```

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/utils.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/key_point_summarization/utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_admin_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_admin_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
         return self._get(self.host + comments_limit_endpoint, {}, timeout=180)
 
     def run_self_check(self):
         '''
         Checks the connection to the service and if the service is UP and running.
         :return: a json with 'status': that have the value UP if all is well and DOWN otherwise.
         '''
-        return self._get(self.host + self_check_endpoint, None, timeout=180)
+        return self._get(self.host + self_check_endpoint, {}, timeout=180)
 
     def get_unmapped_sentences_for_kps_result(self, kps_result: KpsResult):
         '''
         Retrieve all unmapped sentences associated with the kps_result.
         :param kps_result: KpsResult object storing the results.
         :return: a dataframe with all unmapped sentences and their data, or None if domain
         '''
```

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_pairs_infer_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/keypoints_pairs_infer_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/narrative_generation_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/narrative_generation_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/pro_con_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/pro_con_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/response_data/speech_response.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/response_data/speech_response.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/term_relater_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/term_relater_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/term_wikifier_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/term_wikifier_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/clients/theme_extraction_client.py` & `debater_python_api-5.0.1/debater_python_api/api/clients/theme_extraction_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/debater_api.py` & `debater_python_api-5.0.1/debater_python_api/api/debater_api.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_client.py` & `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py` & `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py` & `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_base.py` & `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_base.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_request.py` & `debater_python_api-5.0.1/debater_python_api/api/sentence_level_index/client/sentence_query_request.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/argument_quality_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/argument_quality_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/claim_boundaries_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/claim_boundaries_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/claim_detection_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/claim_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/clustering_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/clustering_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/embedding_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/embedding_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/evidence_detection_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/evidence_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/example_of_sc_args.py` & `debater_python_api-5.0.1/debater_python_api/examples/example_of_sc_args.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/index_searcher_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/index_searcher_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/keypoints_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/keypoints_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/pro_con_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/pro_con_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/resources/arguments.py` & `debater_python_api-5.0.1/debater_python_api/examples/resources/arguments.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/resources/pro_con_scores.py` & `debater_python_api-5.0.1/debater_python_api/examples/resources/pro_con_scores.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/run_all_services.py` & `debater_python_api-5.0.1/debater_python_api/examples/run_all_services.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/speech_construction_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/speech_construction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/term_wikifier_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/term_wikifier_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/theme_extraction_example.py` & `debater_python_api-5.0.1/debater_python_api/examples/theme_extraction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/usecases/kp_based_survey.py` & `debater_python_api-5.0.1/debater_python_api/examples/usecases/kp_based_survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/usecases/mining_to_narrative.py` & `debater_python_api-5.0.1/debater_python_api/examples/usecases/mining_to_narrative.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/examples/usecases/survey.py` & `debater_python_api-5.0.1/debater_python_api/examples/usecases/survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py` & `debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesIT.py` & `debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesIT.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesLoad.py` & `debater_python_api-5.0.1/debater_python_api/integration_tests/api/clients/ServicesLoad.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/utils/clusters_refiner.py` & `debater_python_api-5.0.1/debater_python_api/utils/clusters_refiner.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/utils/general_utils.py` & `debater_python_api-5.0.1/debater_python_api/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api/utils/kp_analysis_conf.py` & `debater_python_api-5.0.1/debater_python_api/utils/kp_analysis_conf.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/debater_python_api.egg-info/PKG-INFO` & `debater_python_api-5.0.1/debater_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater-python-api
-Version: 5.0.0
+Version: 5.0.1
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.0/debater_python_api.egg-info/SOURCES.txt` & `debater_python_api-5.0.1/debater_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.0/pyproject.toml` & `debater_python_api-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debater_python_api"
-version = "5.0.0"
+version = "5.0.1"
 description = "Project Debater Early Access Program API sdk for python"
 readme = "README.md"
 authors = [{ name = "Elad Venezian", email = "eladv@il.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

