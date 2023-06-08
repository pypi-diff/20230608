# Comparing `tmp/ml4floods-0.0.4.tar.gz` & `tmp/ml4floods-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4floods-0.0.4.tar", last modified: Thu Dec  1 11:13:46 2022, max compression
+gzip compressed data, was "ml4floods-0.0.5.tar", last modified: Thu Jun  8 11:14:30 2023, max compression
```

## Comparing `ml4floods-0.0.4.tar` & `ml4floods-0.0.5.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2022-12-01 09:51:06.000000 ml4floods-0.0.4/LICENSE
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4165 2022-12-01 11:13:46.482077 ml4floods-0.0.4/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3843 2022-12-01 11:06:05.000000 ml4floods-0.0.4/README.md
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.474076 ml4floods-0.0.4/ml4floods/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       22 2022-12-01 11:13:42.000000 ml4floods-0.0.4/ml4floods/__init__.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/data/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    31569 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/S2_SAFE_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13843 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/cmkappazeta.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3549 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/cms2cloudless.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3845 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/config.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/data/configuration/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    30407 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/configuration/train_test_split_extra_dataset.json
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    21711 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/configuration/train_test_split_original_dataset.json
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/data/copernicusEMS/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/copernicusEMS/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    23784 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/copernicusEMS/activations.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1051 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/copernicusEMS/utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18967 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/create_gt.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6575 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/dataset.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    31501 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/ee_download.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/data/index/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/index/__init__.py
--rwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)     1522 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/index/geographic_index.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4725 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/index/indexer.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      861 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/index/indexer_arg_parser.py
--rwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)     2276 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/index/map_data.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      692 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/index/map_data_factory.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5536 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/save_cog.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/data/unosat/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/unosat/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10779 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/unosat/unosat_download.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1387 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/unosat/unosat_download_arg_parser.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6525 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/data/worldfloods/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/worldfloods/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2096 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/worldfloods/configs.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18431 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/worldfloods/create_worldfloods_dataset.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     8971 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/worldfloods/dataset.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2445 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/worldfloods/download.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6668 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/data/worldfloods/lightning.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/models/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/__init__.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.478077 ml4floods-0.0.4/ml4floods/models/architectures/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/architectures/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      833 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/architectures/baselines.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    19082 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/architectures/hrnet_seg.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      281 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/architectures/layer_factory.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1354 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/architectures/ndwi.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3180 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/architectures/unets.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2554 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/config_setup.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/models/configurations/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/configurations/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1595 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/configurations/worldfloods_template.json
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1676 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/configurations/worldfloods_template_v2.json
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1572 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/configurations/worldfloods_uncertainty.json
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14884 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/dataset_setup.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12125 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/model_setup.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28555 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/postprocess.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/models/utils/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/utils/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      579 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/utils/configuration.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5291 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/utils/losses.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    20799 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/utils/metrics.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7785 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/utils/uncertainty.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    20031 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/models/worldfloods_model.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/preprocess/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5376 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/tiling.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9052 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/transformations.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1246 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/preprocess/worldfloods/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/worldfloods/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1403 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/worldfloods/normalize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1623 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/preprocess/worldfloods/prepare_patches.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/scripts/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/scripts/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13324 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/scripts/inference.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/serve/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2415 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/serve/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5273 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/serve/read_tile.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.482077 ml4floods-0.0.4/ml4floods/visualization/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/visualization/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    21175 2022-12-01 09:51:07.000000 ml4floods-0.0.4/ml4floods/visualization/plot_utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2022-12-01 11:13:46.474076 ml4floods-0.0.4/ml4floods.egg-info/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4165 2022-12-01 11:13:46.000000 ml4floods-0.0.4/ml4floods.egg-info/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2690 2022-12-01 11:13:46.000000 ml4floods-0.0.4/ml4floods.egg-info/SOURCES.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2022-12-01 11:13:46.000000 ml4floods-0.0.4/ml4floods.egg-info/dependency_links.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      373 2022-12-01 11:13:46.000000 ml4floods-0.0.4/ml4floods.egg-info/requires.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2022-12-01 11:13:46.000000 ml4floods-0.0.4/ml4floods.egg-info/top_level.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      299 2022-12-01 11:13:46.482077 ml4floods-0.0.4/setup.cfg
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1926 2022-12-01 10:42:52.000000 ml4floods-0.0.4/setup.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-05-04 11:13:19.000000 ml4floods-0.0.5/LICENSE
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4372 2023-06-08 11:14:30.670760 ml4floods-0.0.5/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4050 2023-05-04 11:13:19.000000 ml4floods-0.0.5/README.md
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.662760 ml4floods-0.0.5/ml4floods/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       22 2023-06-08 11:14:12.000000 ml4floods-0.0.5/ml4floods/__init__.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/data/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    31569 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/S2_SAFE_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2775 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/cmcloudsen12.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13823 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/cmkappazeta.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3549 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/cms2cloudless.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3917 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/config.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/data/configuration/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    30407 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/configuration/train_test_split_extra_dataset.json
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    21711 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/configuration/train_test_split_original_dataset.json
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/data/copernicusEMS/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/copernicusEMS/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    23784 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/copernicusEMS/activations.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1051 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/copernicusEMS/utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18980 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/create_gt.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6575 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/dataset.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    31625 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/ee_download.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/data/index/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/index/__init__.py
+-rwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)     1522 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/index/geographic_index.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4725 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/index/indexer.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      861 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/index/indexer_arg_parser.py
+-rwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)     2276 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/index/map_data.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      692 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/index/map_data_factory.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5536 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/save_cog.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/data/unosat/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/unosat/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10779 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/unosat/unosat_download.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1387 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/unosat/unosat_download_arg_parser.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6779 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2180 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/vectorize.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/data/worldfloods/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/worldfloods/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2096 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/worldfloods/configs.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    19195 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/worldfloods/create_worldfloods_dataset.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     8971 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/worldfloods/dataset.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2445 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/worldfloods/download.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6668 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/data/worldfloods/lightning.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/models/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/__init__.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.666760 ml4floods-0.0.5/ml4floods/models/architectures/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/architectures/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      833 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/architectures/baselines.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    19082 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/architectures/hrnet_seg.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      281 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/architectures/layer_factory.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1354 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/architectures/ndwi.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3180 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/architectures/unets.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2477 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/config_setup.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/models/configurations/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/configurations/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1595 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/configurations/worldfloods_template.json
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1676 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/configurations/worldfloods_template_v2.json
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1572 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/configurations/worldfloods_uncertainty.json
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14984 2023-06-08 10:57:35.000000 ml4floods-0.0.5/ml4floods/models/dataset_setup.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12125 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/model_setup.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    29527 2023-06-08 10:57:35.000000 ml4floods-0.0.5/ml4floods/models/postprocess.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/models/utils/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/utils/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      579 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/utils/configuration.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5291 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/utils/losses.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    20799 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/utils/metrics.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7785 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/utils/uncertainty.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    20031 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/models/worldfloods_model.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/preprocess/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5376 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/tiling.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9052 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/transformations.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1246 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/preprocess/worldfloods/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/worldfloods/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1403 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/worldfloods/normalize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1623 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/preprocess/worldfloods/prepare_patches.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/scripts/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/scripts/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13324 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/scripts/inference.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/serve/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2415 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/serve/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5273 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/serve/read_tile.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.670760 ml4floods-0.0.5/ml4floods/visualization/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-05-04 11:13:19.000000 ml4floods-0.0.5/ml4floods/visualization/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    24327 2023-05-11 13:23:20.000000 ml4floods-0.0.5/ml4floods/visualization/plot_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-06-08 11:14:30.662760 ml4floods-0.0.5/ml4floods.egg-info/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4372 2023-06-08 11:14:30.000000 ml4floods-0.0.5/ml4floods.egg-info/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2749 2023-06-08 11:14:30.000000 ml4floods-0.0.5/ml4floods.egg-info/SOURCES.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2023-06-08 11:14:30.000000 ml4floods-0.0.5/ml4floods.egg-info/dependency_links.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      365 2023-06-08 11:14:30.000000 ml4floods-0.0.5/ml4floods.egg-info/requires.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2023-06-08 11:14:30.000000 ml4floods-0.0.5/ml4floods.egg-info/top_level.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      299 2023-06-08 11:14:30.670760 ml4floods-0.0.5/setup.cfg
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1926 2023-05-04 11:13:20.000000 ml4floods-0.0.5/setup.py
```

### Comparing `ml4floods-0.0.4/LICENSE` & `ml4floods-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/PKG-INFO` & `ml4floods-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4floods
-Version: 0.0.4
+Version: 0.0.5
 Summary: Machine learning models for end-to-end flood extent segmentation.
 Author: SpaceML-org
 Keywords: floods pytorch machine-learning earth
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 Provides-Extra: docs
@@ -17,20 +17,30 @@
 
 ML4Floods is an end-to-end ML pipeline for flood extent estimation: from data preprocessing, model training, model deployment to visualization.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/spaceml-org/ml4floods/main/jupyterbook/content/ml4ops/ts_albania.gif" alt="awesome flood extent estimation" width="100%">
 </p>
 
-Install the package:
+## Install
+
+Install from [pip](https://pypi.org/project/ml4floods/):
+```bash
+pip install ml4floods
+```
+
+Install the latest version from GitHub:
 
 ```bash
 pip install git+https://github.com/spaceml-org/ml4floods#egg=ml4floods
 ```
 
+## Docs
+[spaceml-org.github.io/ml4floods](https://spaceml-org.github.io/ml4floods)
+
 These tutorials may help you explore the datasets and models:
 * [Project rationale](https://spaceml-org.github.io/ml4floods/content/intro/introduction.html).
 * [Run the model on time series of Sentinel-2 images](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_inference_on_image_time_series.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_inference_on_image_time_series.ipynb)
 * [ML-models step by step](https://spaceml-org.github.io/ml4floods/content/ml_overview.html)
     * [Training](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_Train_models.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_Train_models.ipynb)
     * [Inference on new data](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_Run_Inference_on_new_data.html) (a Sentinel-2 image) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_Run_Inference_on_new_data.ipynb)
     * [Perf metrics](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_performance_metrics_workflow.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_performance_metrics_workflow.ipynb)
```

### Comparing `ml4floods-0.0.4/README.md` & `ml4floods-0.0.5/ml4floods.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,46 @@
+Metadata-Version: 2.1
+Name: ml4floods
+Version: 0.0.5
+Summary: Machine learning models for end-to-end flood extent segmentation.
+Author: SpaceML-org
+Keywords: floods pytorch machine-learning earth
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tests
+Provides-Extra: docs
+License-File: LICENSE
+
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/spaceml-org/ml4floods/main/jupyterbook/ml4floods_banner.png" alt="awesome ml4floods" width="50%">
 </p>
 
 ML4Floods is an end-to-end ML pipeline for flood extent estimation: from data preprocessing, model training, model deployment to visualization.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/spaceml-org/ml4floods/main/jupyterbook/content/ml4ops/ts_albania.gif" alt="awesome flood extent estimation" width="100%">
 </p>
 
-Install the package:
+## Install
+
+Install from [pip](https://pypi.org/project/ml4floods/):
+```bash
+pip install ml4floods
+```
+
+Install the latest version from GitHub:
 
 ```bash
 pip install git+https://github.com/spaceml-org/ml4floods#egg=ml4floods
 ```
 
+## Docs
+[spaceml-org.github.io/ml4floods](https://spaceml-org.github.io/ml4floods)
+
 These tutorials may help you explore the datasets and models:
 * [Project rationale](https://spaceml-org.github.io/ml4floods/content/intro/introduction.html).
 * [Run the model on time series of Sentinel-2 images](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_inference_on_image_time_series.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_inference_on_image_time_series.ipynb)
 * [ML-models step by step](https://spaceml-org.github.io/ml4floods/content/ml_overview.html)
     * [Training](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_Train_models.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_Train_models.ipynb)
     * [Inference on new data](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_Run_Inference_on_new_data.html) (a Sentinel-2 image) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_Run_Inference_on_new_data.ipynb)
     * [Perf metrics](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_performance_metrics_workflow.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_performance_metrics_workflow.ipynb)
```

### Comparing `ml4floods-0.0.4/ml4floods/data/S2_SAFE_reader.py` & `ml4floods-0.0.5/ml4floods/data/S2_SAFE_reader.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/cmkappazeta.py` & `ml4floods-0.0.5/ml4floods/data/cmkappazeta.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 import tensorflow as tf
 import os
 import numpy as np
 from typing import Callable, Tuple, Optional
 import itertools
 from ml4floods.visualization.plot_utils import get_cmap_norm_colors
-from ml4floods.models import postprocess
+from ml4floods.data import vectorize
 import geopandas as gpd
 import pandas as pd
 import rasterio.transform
 
 
 COLORS_KAPPAZETA = np.array([[255, 0, 0], # 0: invalid
                              [139, 64, 0], # 1: land
@@ -81,16 +81,16 @@
     for c in [2, 3, 4]:
         if c == 3:
             binary_mask = (prediction == 3) | (prediction == 4)
             class_name = "THICK AND THIN CLOUDS"
         else:
             binary_mask = prediction == c
             class_name = CLASSES_KAPPAZETA[c]
-        geoms_polygons = postprocess.get_water_polygons(binary_mask,
-                                                        transform=transform)
+        geoms_polygons = vectorize.get_polygons(binary_mask,
+                                                transform=transform)
         if len(geoms_polygons) > 0:
             data_out.append(gpd.GeoDataFrame({"geometry": geoms_polygons,
                                               "id": np.arange(start, start + len(geoms_polygons)),
                                               "class": class_name},
                                              crs=crs))
             start += len(geoms_polygons)
```

### Comparing `ml4floods-0.0.4/ml4floods/data/cms2cloudless.py` & `ml4floods-0.0.5/ml4floods/data/cms2cloudless.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/config.py` & `ml4floods-0.0.5/ml4floods/data/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,19 @@
     # "Flood trace": 1,  # 'probable flash flood-affected land' DUPLICATED
     "satellite detected water": 1,
     # "Not Applicable": 1,  # unknown see document DUPLICATED
     "possible saturated, wet soil/ possible flood water": 1,
     "aquaculture (wet rice)": 1,
     "tsunami-affected land": 1,
     "ran of kutch water": 1,
-    "maximum flood water extent (cumulative)": 1
+    "maximum flood water extent (cumulative)": 1,
+    # Preds
+    "flood-trace": 1,
+    "water": 1,
+    "flood_trace": 1
 }
 
 CLASS_LAND_COPERNICUSEMSHYDRO = ["BH090-Land Subject to Inundation", "BA030-Island", 'BA010-Coastline']
 
 ACCEPTED_FIELDS = list(CODES_FLOODMAP.keys()) + CLASS_LAND_COPERNICUSEMSHYDRO
```

### Comparing `ml4floods-0.0.4/ml4floods/data/configuration/train_test_split_extra_dataset.json` & `ml4floods-0.0.5/ml4floods/data/configuration/train_test_split_extra_dataset.json`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/configuration/train_test_split_original_dataset.json` & `ml4floods-0.0.5/ml4floods/data/configuration/train_test_split_original_dataset.json`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/copernicusEMS/activations.py` & `ml4floods-0.0.5/ml4floods/data/copernicusEMS/activations.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/copernicusEMS/utils.py` & `ml4floods-0.0.5/ml4floods/data/copernicusEMS/utils.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/create_gt.py` & `ml4floods-0.0.5/ml4floods/data/create_gt.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             if clouds_vec.shape[0] == 0:
                 cloud_prob = np.zeros(s2_img.shape[1:], dtype=np.float32)
             else:
                 # Convert clouds_vec crs to s2 crs
                 if str(clouds_vec.crs).lower() != crs:
                     clouds_vec.to_crs(crs=crs, inplace=True)
 
-                clouds_vec = clouds_vec[clouds_vec["class"] == "CLOUD"]
+                clouds_vec = clouds_vec[clouds_vec["class"].isin(["CLOUD", "cloud"])]
                 shapes_rasterise = (
                     (g, 1)
                     for g,w in clouds_vec[["geometry", "class"]].itertuples(
                     index=False, name=None
                 )
                 )
                 cloud_prob = features.rasterize(
@@ -454,15 +454,14 @@
     return np.sqrt(np.sum(rgb_img, axis=0))
 
 
 CLOUDS_THRESHOLD = .5
 BRIGHTNESS_THRESHOLD = 3_500
 
 
-
 def _generate_gt_fromarray(
     s2_img: np.ndarray,
     cloudprob: np.ndarray,
     water_mask: np.ndarray,
     custom_clouds: bool=False,
 ) -> np.ndarray:
     """
```

### Comparing `ml4floods-0.0.4/ml4floods/data/dataset.py` & `ml4floods-0.0.5/ml4floods/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/ee_download.py` & `ml4floods-0.0.5/ml4floods/data/ee_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from glob import glob
 from typing import Optional, Callable, List, Tuple, Union
 from shapely.geometry import mapping, Polygon
 import numpy as np
 import geopandas as gpd
 import pandas as pd
-import fsspec
+from ml4floods.data.utils import get_filesystem
 from datetime import datetime, timezone
 import math
 
 BANDS_NAMES = {
     # Sentinel-2 L1C COPERNICUS/S2 COPERNICUS/S2_HARMONIZED
     "COPERNICUS/S2_HARMONIZED" : ["B1","B2","B3","B4", "B5", "B6", "B7", "B8", "B8A", "B9", "B10", "B11", "B12", "QA60"],
     # Sentinel-2 L2A COPERNICUS/S2_SR
@@ -290,15 +290,15 @@
     return False
 
 
 def mayberun(filename, desc, function, export_task, overwrite=False, dry_run=False, verbose=1,
              bucket_name="worldfloods"):
 
     if bucket_name is not None:
-        fs = fsspec.filesystem("gs", requester_pays=True)
+        fs = get_filesystem("gs://")
     
         files_in_bucket = fs.glob(f'gs://{bucket_name}/{filename}*')
         if len(files_in_bucket) > 0:
             if overwrite:
                 print("\tFile %s exists in the bucket. removing" % filename)
                 for b in files_in_bucket:
                     fs.remove(f"gs://{b}")
@@ -421,15 +421,15 @@
         resolution_meters:
 
     Returns:
         List of GEE tasks if triggered
     """
     assert path_bucket.startswith("gs://"), f"Path bucket: {path_bucket} must start with gs://"
 
-    fs = fsspec.filesystem("gs", requester_pays = requester_pays)
+    fs = get_filesystem("gs://")
     filename_full_path = os.path.join(path_bucket, f"{date_search.year}.tif")
     if fs.exists(filename_full_path):
         print(f"File {filename_full_path} exists. It will not be downloaded again")
         return
 
     ee.Initialize()
     
@@ -470,14 +470,23 @@
         export_task_fun_img,
         overwrite=False,
         dry_run=False,
         bucket_name=bucket_name,
         verbose=2,
     )
 
+
+def permanent_water_image(year:int, pol:ee.Geometry) -> ee.Image:
+    if year >= 2021:
+        year = 2021
+    
+    img_export = ee.Image(f"JRC/GSW1_4/YearlyHistory/{year}")
+    return img_export.clip(pol)
+
+
 def download_merit_layer(area_of_interest: Polygon,
                          path_bucket: str, crs:str='EPSG:4326',
                          name_task:Optional[str]=None, resolution_meters:int=10) -> Optional[ee.batch.Task]:
     """
     Downloads MERIT Hydro product ("MERIT/Hydro/v1_0_1") from GEE
 
     Args:
@@ -489,15 +498,15 @@
         resolution_meters:
 
     Returns:
         List of GEE tasks if triggered
     """
     assert path_bucket.startswith("gs://"), f"Path bucket: {path_bucket} must start with gs://"
 
-    fs = fsspec.filesystem("gs",requester_pays = True)
+    fs = get_filesystem("gs://")
     
     filename_full_path = os.path.join(path_bucket, "merit").replace("\\",'/')
     if fs.exists(filename_full_path):
         print(f"File {filename_full_path} exists. It will not be downloaded again")
         return
 
     ee.Initialize()
@@ -574,15 +583,15 @@
         path_csv:
         fs:
 
     Returns:
         dataframe with processed date fields and column indicating if the s2 file is available
     """
     if fs is None:
-        fs = fsspec.filesystem("gs", requester_pays=True)
+        fs = get_filesystem("gs://")
     
     if path_csv.startswith("gs"):
         with fs.open(path_csv, "r") as fh:
             datas2 = pd.read_csv(fh)
     else:
         datas2 = pd.read_csv(path_csv)
         
@@ -684,15 +693,15 @@
 
     assert path_bucket.startswith("gs://"), f"Path bucket: {path_bucket} must start with gs://"
 
     path_bucket_no_gs = path_bucket.replace("gs://", "")
     bucket_name = path_bucket_no_gs.split("/")[0]
     path_no_bucket_name = "/".join(path_bucket_no_gs.split("/")[1:])
 
-    fs = fsspec.filesystem("gs", requester_pays = True)
+    fs = get_filesystem("gs://")
 
     if collection_name == "Landsat":
         path_csv = os.path.join(path_bucket, "landsatinfo.csv")
     elif collection_name == "S2":
         collection_name = "COPERNICUS/S2_HARMONIZED"
         path_csv = os.path.join(path_bucket, "s2info.csv")
     else:
@@ -829,8 +838,8 @@
             if task.status()["state"] != "COMPLETED":
                 print("Error in task {}:\n {}".format(t, task.status()))
                 task_error += 1
 
         task_down = task_down_new
         time.sleep(60)
 
-    print("Tasks failed: %d" % task_error)
+    print("Tasks failed: %d" % task_error)
```

### Comparing `ml4floods-0.0.4/ml4floods/data/index/geographic_index.py` & `ml4floods-0.0.5/ml4floods/data/index/geographic_index.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/index/indexer.py` & `ml4floods-0.0.5/ml4floods/data/index/indexer.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/index/indexer_arg_parser.py` & `ml4floods-0.0.5/ml4floods/data/index/indexer_arg_parser.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/index/map_data.py` & `ml4floods-0.0.5/ml4floods/data/index/map_data.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/index/map_data_factory.py` & `ml4floods-0.0.5/ml4floods/data/index/map_data_factory.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/save_cog.py` & `ml4floods-0.0.5/ml4floods/data/save_cog.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/unosat/unosat_download.py` & `ml4floods-0.0.5/ml4floods/data/unosat/unosat_download.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/unosat/unosat_download_arg_parser.py` & `ml4floods-0.0.5/ml4floods/data/unosat/unosat_download_arg_parser.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/utils.py` & `ml4floods-0.0.5/ml4floods/data/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,20 +85,23 @@
         # torch or tensorflow -> list, pretty straightforward.
         if hasattr(obj_to_encode, "numpy"):
             return obj_to_encode.numpy().tolist()
         # If none of the above apply, we'll default back to the standard JSON encoding
         # routines and let it work normally.
         return super().default(obj_to_encode)
 
+REQUESTER_PAYS_DEFAULT = True
 
-def get_filesystem(path: Union[str, Path]):
+def get_filesystem(path: Union[str, Path], requester_pays:Optional[bool]=None):
+    if requester_pays is None:
+        requester_pays = REQUESTER_PAYS_DEFAULT
     path = str(path)
     if "://" in path:
         # use the fileystem from the protocol specified
-        return fsspec.filesystem(path.split(":", 1)[0],requester_pays = True)
+        return fsspec.filesystem(path.split(":", 1)[0], requester_pays=requester_pays)
     else:
         # use local filesystem
         return fsspec.filesystem("file")
 
 
 def write_geojson_to_gcp(gs_path: str, geojson_val: gpd.GeoDataFrame) -> None:
     fs = get_filesystem(gs_path)
@@ -107,15 +110,15 @@
         with fs.open(gs_path, "w") as fh:
             json.dump(eval(geojson_val.to_json()), fh)
     else:
         with fs.open(gs_path, "wb") as fh:
             geojson_val.to_file(fh, driver="GeoJSON")
 
 
-def check_requester_pays_gcp_available() -> bool:
+def check_gdal_requester_pays_gcp_available() -> bool:
     """
     Requester pays for GCP is available from GDAL 3.4
 
     rasterio issue: https://github.com/rasterio/rasterio/issues/1948
     Commit GDAL: https://github.com/OSGeo/gdal/pull/3883/commits/8d551953dea9290b21bd9747ec9ed22c81ca0409
 
     Returns:
@@ -130,19 +133,22 @@
             return True
     except Exception as e:
         pass
 
     return False
 
 
-REQUESTER_PAYS_AVAILABLE = check_requester_pays_gcp_available()
+REQUESTER_PAYS_AVAILABLE = check_gdal_requester_pays_gcp_available()
 
 
 @contextmanager
-def rasterio_open_read(tifffile:str, requester_pays:bool=True) -> rasterio.DatasetReader:
+def rasterio_open_read(tifffile:str, requester_pays:Optional[bool]=None) -> rasterio.DatasetReader:
+    if requester_pays is None:
+        requester_pays = REQUESTER_PAYS_DEFAULT
+
     if requester_pays and tifffile.startswith("gs"):
         if REQUESTER_PAYS_AVAILABLE:
             assert "GS_USER_PROJECT" in os.environ, \
                 "'GS_USER_PROJECT' env variable not found and requester_pays=True set a project name to read rasters from the bucket" \
                 "(i.e. -> export GS_USER_PROJECT='myprojectname')"
 
             with rasterio.open(tifffile) as src:
```

### Comparing `ml4floods-0.0.4/ml4floods/data/worldfloods/configs.py` & `ml4floods-0.0.5/ml4floods/data/worldfloods/configs.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/worldfloods/create_worldfloods_dataset.py` & `ml4floods-0.0.5/ml4floods/data/worldfloods/create_worldfloods_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sys
 import warnings
 import traceback
 
 import tqdm
 import pandas as pd
 from datetime import datetime
-from ml4floods.data import utils
+from ml4floods.data import utils, vectorize
 from ml4floods.data.ee_download import process_metadata
 import os
+import numpy as np
 
 from pathlib import Path
 from typing import Optional, Callable, Tuple, Dict, Any
 import geopandas as gpd
 import fsspec
 from ml4floods.data import save_cog
 
@@ -264,15 +265,15 @@
         return False
     try:
         # generate gt, gt meta and copy all files to path_write
         fsdest = utils.get_filesystem(s2_image_path_dest)
 
         if not fsdest.exists(gt_path_dest) or not fsdest.exists(meta_json_path_dest) or overwrite:
             if pbar is not None:
-                pbar.set_description(f"Generating Ground Truth {file_name}...")
+                pbar.write(f"Generating Ground Truth {file_name}...")
 
             # Copy s2_image_path to local before reading?
             # If so we will need also to copy cloudprob_path and permanent_water_path
 
             gt, gt_meta = gt_fun(
                 s2_image_path,
                 floodmap,
@@ -282,63 +283,84 @@
                 permanent_water_image_path=permanent_water_path,  # Could be None!
             )
 
             if len(gt.shape) == 2:
                 gt = gt[None]
 
             if pbar is not None:
-                pbar.set_description(f"Saving GT {file_name}...")
+                pbar.write(f"Saving GT {file_name}...")
 
             if gt.shape[0] == 2:
                 desc = ["invalid/clear/cloud", "invalid/land/water"]
             else:
                 desc = ["invalid/land/water/cloud"]
 
             save_cog.save_cog(gt, gt_path_dest,
                               {"crs": gt_meta["crs"], "transform":gt_meta["transform"] ,"RESAMPLING": "NEAREST",
                                "compress": "lzw", "nodata": 0}, # In both gts 0 is nodata
                               descriptions=desc,
                               tags=gt_meta)
 
             # upload meta json to bucket
             if pbar is not None:
-                pbar.set_description(f"Saving meta {file_name}...")
+                pbar.write(f"Saving meta {file_name}...")
 
             # save meta in local json file
             gt_meta["crs"] = str(gt_meta["crs"])
             gt_meta["transform"] = [gt_meta["transform"].a, gt_meta["transform"].b, gt_meta["transform"].c,
                                     gt_meta["transform"].d, gt_meta["transform"].e, gt_meta["transform"].f]
 
             utils.write_json_to_gcp(meta_json_path_dest, gt_meta)
 
+        # Copy cloudprob
+        if cloudprob_path_dest and (not fsdest.exists(cloudprob_path_dest) or overwrite):
+            if pbar is not None:
+                pbar.write(f"Saving cloud probs {file_name}...")
+
+            with utils.rasterio_open_read(gt_path_dest) as rst:
+                gt = rst.read()
+                transform = rst.transform
+                crs = rst.crs
+
+            if gt.shape[0] == 2:
+                clouds = gt[0] == 2
+            else:
+                clouds = gt[0] == 3
+
+            # vectorize clouds
+            geoms_polygons = vectorize.get_polygons(clouds,
+                                                    transform=transform)
+            if len(geoms_polygons) > 0:
+                clouds_vec = gpd.GeoDataFrame({"geometry": geoms_polygons,
+                                               "class": "cloud"},
+                                              crs=crs)
+            else:
+                clouds_vec = gpd.GeoDataFrame(data={"class": []},
+                                              geometry=[], crs=crs)
+
+            utils.write_geojson_to_gcp(cloudprob_path_dest, clouds_vec)
+
         # Copy floodmap shapefiles
         if not fsdest.exists(floodmap_path_dest) or overwrite:
             if pbar is not None:
-                pbar.set_description(f"Saving floodmap {file_name}...")
+                pbar.write(f"Saving floodmap {file_name}...")
 
             utils.write_geojson_to_gcp(floodmap_path_dest, floodmap)                
         
         # Copy S2 image
         if not fsdest.exists(s2_image_path_dest) or overwrite:
             if pbar is not None:
-                pbar.set_description(f"Saving S2 image {file_name}...")
+                pbar.write(f"Saving S2 image {file_name}...")
             
             _copy(s2_image_path, s2_image_path_dest, fs)
-        
-        # Copy cloudprob
-        if cloudprob_path is not None and cloudprob_path_dest and (not fsdest.exists(cloudprob_path_dest) or overwrite):
-            if pbar is not None:
-                pbar.set_description(f"Saving cloud probs {file_name}...")
-            
-            _copy(cloudprob_path, cloudprob_path_dest, fs)
-        
+
         # Copy permanent water
         if (permanent_water_image_path_dest is not None) and (not fsdest.exists(permanent_water_image_path_dest) or overwrite):
             if pbar is not None:
-                pbar.set_description(f"Saving permanent water image {file_name}...")
+                pbar.write(f"Saving permanent water image {file_name}...")
 
             _copy(permanent_water_path, permanent_water_image_path_dest, fs)
 
     except Exception:
         warnings.warn(f"File input: {main_path} output S2 file: {s2_image_path_dest} problem when computing Ground truth")
         traceback.print_exc(file=sys.stdout)
 
@@ -416,15 +438,15 @@
         permanent_water_image_path_dest = None
 
     output_path = str(output_path)
     s2_image_path_dest = os.path.join(output_path,"S2",file_name+".tif").replace("\\", "/")
     meta_parent_path = os.path.join(output_path,"meta",file_name+".json").replace("\\", "/")
 
     if clouds_available:
-        cloudprob_path_dest = os.path.join(output_path, "cloudprob",file_name+".tif").replace("\\", "/")
+        cloudprob_path_dest = os.path.join(output_path, "cloud_vec",file_name+".geojson").replace("\\", "/")
     else:
         cloudprob_path_dest = None
 
     floodmap_path_dest = os.path.join(output_path,"floodmaps",file_name+".geojson").replace("\\", "/")
     gt_path = os.path.join(output_path,"gt",file_name+".tif").replace("\\", "/")
 
     # makedir if not gs
```

### Comparing `ml4floods-0.0.4/ml4floods/data/worldfloods/dataset.py` & `ml4floods-0.0.5/ml4floods/data/worldfloods/dataset.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/worldfloods/download.py` & `ml4floods-0.0.5/ml4floods/data/worldfloods/download.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/data/worldfloods/lightning.py` & `ml4floods-0.0.5/ml4floods/data/worldfloods/lightning.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/architectures/baselines.py` & `ml4floods-0.0.5/ml4floods/models/architectures/baselines.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/architectures/hrnet_seg.py` & `ml4floods-0.0.5/ml4floods/models/architectures/hrnet_seg.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/architectures/ndwi.py` & `ml4floods-0.0.5/ml4floods/models/architectures/ndwi.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/architectures/unets.py` & `ml4floods-0.0.5/ml4floods/models/architectures/unets.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/config_setup.py` & `ml4floods-0.0.5/ml4floods/models/config_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     Args:
         args: args to populate the config
 
     Returns:
         config: config object
 
     """
-    import pprint
-    pp = pprint.PrettyPrinter(indent=4)
     
     # 1. Load config json from argparse input
     config = load_json(args.config)
     
     # 2. Add additional fields to config using worldfloods constants etc
     from ml4floods.data.worldfloods.configs import CHANNELS_CONFIGURATIONS
 
@@ -35,16 +33,15 @@
     assert config['model_params']['hyperparameters']['channel_configuration'] ==  config['data_params']['channel_configuration'],\
          f"Set the same channel configuration: {config['model_params']['hyperparameters']['channel_configuration']} {config['data_params']['bands']}"
     
     config['model_params']['hyperparameters']['num_channels'] = len(CHANNELS_CONFIGURATIONS[config['model_params']['hyperparameters']['channel_configuration']])
     
     config = AttrDict.from_nested_dicts(config)
 
-    print('Loaded Config for experiment: ', config.experiment_name)
-    pp.pprint(config)
+    # print(f'Loaded Config for experiment: {config.experiment_name}')
     
     # 3. return config to training
     return config
 
 
 def get_default_config(config_fp) -> AttrDict:
     """
```

### Comparing `ml4floods-0.0.4/ml4floods/models/configurations/worldfloods_template.json` & `ml4floods-0.0.5/ml4floods/models/configurations/worldfloods_template.json`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/configurations/worldfloods_template_v2.json` & `ml4floods-0.0.5/ml4floods/models/configurations/worldfloods_template_v2.json`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/configurations/worldfloods_uncertainty.json` & `ml4floods-0.0.5/ml4floods/models/configurations/worldfloods_uncertainty.json`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/dataset_setup.py` & `ml4floods-0.0.5/ml4floods/models/dataset_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,19 +153,20 @@
                 assert (path_to_splits is not None) and os.path.exists(path_to_splits), \
                     f"path_to_splits {path_to_splits} doesn't exists or not provided ad requested to download the data"
 
                 for input_target_folder in [input_folder, target_folder]:
                     folder_local = os.path.join(path_to_splits, isplit, input_target_folder)
                     os.makedirs(folder_local, exist_ok=True)
                     basename = os.path.basename(filename)
+                    file_src = filenames_train_test[isplit][input_target_folder][idx]
                     file_dest = os.path.join(folder_local, basename)
                     if not os.path.isfile(file_dest):
-                        fs.get_file(filename, file_dest)
-                        print(f"Downloaded ({idx}/{len(filenames_train_test[isplit][input_folder])}) {filename}")
-                    filenames_train_test[isplit][input_folder][idx] = file_dest
+                        fs.get_file(file_src, file_dest)
+                        print(f"Downloaded ({idx}/{len(filenames_train_test[isplit][input_target_folder])}) {file_src}")
+                    filenames_train_test[isplit][input_target_folder][idx] = file_dest
 
     return filenames_train_test
 
 
 def get_dataset(data_config) -> pl.LightningDataModule:
     """
     Function to set up dataloaders for model training
```

### Comparing `ml4floods-0.0.4/ml4floods/models/model_setup.py` & `ml4floods-0.0.5/ml4floods/models/model_setup.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/postprocess.py` & `ml4floods-0.0.5/ml4floods/models/postprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from skimage import measure
 from skimage.segmentation import watershed
 from skimage.feature import peak_local_max
 from scipy import ndimage as ndi
 import numpy as np
 from typing import List, Optional, Union
 from ml4floods.data.create_gt import get_brightness, BRIGHTNESS_THRESHOLD
-from ml4floods.data import utils
+from ml4floods.data import utils, vectorize
 import torch
 import geopandas as gpd
 from shapely.ops import unary_union
 from shapely import validation
 import pandas as pd
 import warnings
 from tqdm import tqdm
@@ -58,56 +58,15 @@
         tolerance: to simplify the polygons, in pixel units
         transform: affine transformation of the binary_water_mask raster
 
     Returns:
         list of rasterised polygons
 
     """
-    assert binary_water_mask.ndim == 2, f"Expected mask with 2 dim found {binary_water_mask.shape}"
-
-    geoms_polygons = []
-    polygon_generator = features.shapes(binary_water_mask.astype(np.int16),
-                                        binary_water_mask)
-
-    for polygon, value in polygon_generator:
-        p = shape(polygon)
-        if polygon_buffer > 0:
-            p = p.buffer(polygon_buffer)
-        if p.area >= min_area:
-            p = p.simplify(tolerance=tolerance)
-            if transform is not None:
-                p = transform_polygon(p, transform) # Convert polygon to raster coordinates
-            geoms_polygons.append(p)
-
-    return geoms_polygons
-
-def transform_polygon(polygon:Polygon, transform: rasterio.Affine) -> Polygon:
-    """
-    Transforms a polygon from pixel coordinates to the coordinates specified by the affine transform
-
-    Args:
-        polygon: polygon to transform
-        transform: Affine transformation
-
-    Returns:
-        polygon with coordinates transformed by the affine transformation
-
-    """
-    geojson_dict = mapping(polygon)
-    out_coords = []
-    for pol in geojson_dict["coordinates"]:
-        pol_out = []
-        for coords in pol:
-            pol_out.append(transform * coords)
-
-        out_coords.append(pol_out)
-
-    geojson_dict["coordinates"] = out_coords
-
-    return shape(geojson_dict)
+    return vectorize.get_polygons(binary_water_mask, min_area, polygon_buffer, tolerance, transform)
 
 
 def get_mask_watertypes(mndwi: Union[np.ndarray, torch.Tensor],
                         water_mask:Union[np.ndarray, torch.Tensor],
                         permanent_water:Optional[Union[np.ndarray, torch.Tensor]]=None) -> Union[np.ndarray, torch.Tensor]:
     """
     This function returns a single mask that differenciates flood_water from permanent_water and flood traces.
@@ -221,14 +180,42 @@
     # Remove Lines or Points from missing area
     if area_missing_or_cloud.type == "GeometryCollection":
         area_missing_or_cloud = unary_union(
             [gc for gc in area_missing_or_cloud.geoms if (gc.type == "Polygon") or (gc.type == "MultiPolygon")])
 
     return area_missing_or_cloud
 
+def get_area_missing_or_cloud_or_land(floodmap:gpd.GeoDataFrame,
+                                      area_imaged:Union[Polygon,MultiPolygon]) -> Union[Polygon, MultiPolygon]:
+    """
+    Returns a Polygon with the area of the floodmap that hasn't been imaged (i.e. is out of `floodmap[floodmap['class'] == "area_imaged"]`)
+    and that is not covered by clouds or land.
+
+    Args:
+        floodmap: GeoDataFrame with column 'class' with values 'area_imaged' and 'cloud'
+        area_imaged: Polygon that indicates the area imaged.
+
+    Returns:
+        Polygon with the area of the floodmap that hasn't been imaged and that is not covered by clouds or land
+    """
+    
+    area_missing = area_imaged.difference(unary_union(floodmap[(floodmap["class"] == "area_imaged")].geometry))
+    area_imaged_current = unary_union(floodmap[floodmap["class"] == "area_imaged"].geometry)
+    clouds = unary_union(floodmap[(floodmap["class"] == "cloud")].geometry)
+    polygons_in_floodmap = unary_union(make_valid(floodmap[floodmap["class"] != "area_imaged"]).geometry)
+    land = area_imaged_current.difference(polygons_in_floodmap)
+    area_missing_or_cloud_or_land =  clouds.union(area_missing).union(land)
+
+    # Remove Lines or Points from missing area
+    if area_missing_or_cloud_or_land.type == "GeometryCollection":
+        area_missing_or_cloud_or_land = unary_union(
+            [gc for gc in area_missing_or_cloud_or_land.geoms if (gc.type == "Polygon") or (gc.type == "MultiPolygon")])
+    
+    return area_missing_or_cloud_or_land
+
 
 def get_area_valid(floodmap:gpd.GeoDataFrame) -> Union[Polygon, MultiPolygon]:
     """
     Returns the polygon with the area valid (i.e. area that is imaged and is not cloud)
 
     Args:
         floodmap: GeoDataFrame with column 'class' with values 'area_imaged' and 'cloud'
@@ -281,21 +268,24 @@
     # Sort data based on ccs
     idx_sorted = np.argsort(ccs)
     datas_sorted = [datas[idxdates] for idxdates in idx_sorted]
 
     return mosaic_floodmaps(datas_sorted, area_imaged, verbose=verbose)
 
 
-def get_floodmap_post(geojsons:List[str],verbose:bool=False) -> gpd.GeoDataFrame:
+def get_floodmap_post(geojsons:List[str],verbose:bool=False,
+                      mode:str="first") -> gpd.GeoDataFrame:
     """
     From a list of sorted GeoJSONs returns the GeoDataFrame with all flood water smartly joined
 
     Args:
         geojsons: List[GeoDataFrame] with column 'class' with values {"water", "cloud", "area_imaged", "flood_trace"}
         verbose:
+        mode: "first" or "max". If "first" it will prioritize the water and land of the first floodmap.
+            If "max" it will take the maximum of water of all floodmaps.
 
     Returns:
         floodmap with lowest cloud coverage. Classes: {"water", "cloud", "area_imaged"}
 
     """
 
     # fill the clouds in pre with data from other geojsons
@@ -311,62 +301,71 @@
         elif crs != data.crs:
             data = data.to_crs(crs=crs)
         data = data[["class","geometry"]].copy()
 
         area_imaged = unary_union(data[data["class"] == "area_imaged"].geometry).union(area_imaged)
         datas.append(data)
 
-    return mosaic_floodmaps(datas, area_imaged, classes_water=["water", "flood_trace"], verbose=verbose)
+    return mosaic_floodmaps(datas, area_imaged, 
+                            classes_water=["water", "flood_trace"], 
+                            verbose=verbose, mode=mode)
 
 
 def mosaic_floodmaps(datas:List[gpd.GeoDataFrame],
                      area_imaged:Union[Polygon, MultiPolygon],
                      classes_water:List[str]=["water"],
-                     verbose:bool=False) -> gpd.GeoDataFrame:
+                     verbose:bool=False,
+                     mode:str="first") -> gpd.GeoDataFrame:
     """
     Mosaics the floodmaps iteratively taking into account the valid area of each of them.
 
     Args:
         datas: List[GeoDataFrame] with column 'class' with values {"water", "cloud", "area_imaged", "flood_trace"}
         area_imaged: Polygon with the total area imaged
         classes_water: which water classes from ["water", "flood_trace"] to include in the output floodmap. For pre-flood
         maps we don't include the flood_trace class.
         verbose:
+        mode: "first" or "max". If "first" it will take the water from the first floomap. If "max" it will return
+        the maximum water area from all floodmaps.
 
     Returns:
         a GeoDataFrame with the mosaic of the input dataframes
     """
 
     # Loop data computing pre-flood water
     warnings.filterwarnings('ignore', 'GeoSeries.isna', UserWarning)
     best_floodmap = datas[0]
     crs = best_floodmap.crs
     area_missing_or_cloud = get_area_missing_or_cloud(best_floodmap, area_imaged=area_imaged)
+    if mode == "max":
+        area_not_mapped = get_area_missing_or_cloud_or_land(best_floodmap, area_imaged=area_imaged)
+    else:
+        area_not_mapped = area_missing_or_cloud
 
     # This dataframe will be filled with water polygons
     condition = None
     for c in classes_water:
         if condition is None:
             condition = best_floodmap["class"] == c
         else:
             condition|= (best_floodmap["class"] == c)
 
     best_floodmap = best_floodmap[condition].copy()
     for idx, data in enumerate(datas[1:]):
-        if area_missing_or_cloud.is_empty or not (area_missing_or_cloud.type in ["Polygon", "MultiPolygon", "GeometryCollection"]):
+        if area_not_mapped.is_empty or not (area_not_mapped.type in ["Polygon", "MultiPolygon", "GeometryCollection"]):
             if verbose:
-                print(f"All area is covered in idx {idx+1}. Area missing empty: {area_missing_or_cloud.is_empty} Geom type: {area_missing_or_cloud.type}")
+                print(f"All area is covered in idx {idx+1}. Area missing empty: {area_not_mapped.is_empty} Geom type: {area_not_mapped.type}")
             break
 
         if data.crs != best_floodmap.crs:
             data = data.to_crs(data.crs, inplace=False)
 
         # Add water polygons that intersect the missing data
         for c in classes_water:
-            water_geoms = data[data["class"] == c].geometry.apply(lambda g: g.intersection(area_missing_or_cloud))
+            water_geoms = data[data["class"] == c].geometry.apply(lambda g: g.intersection(area_not_mapped))
 
             water_geoms = water_geoms[~water_geoms.isna() & ~water_geoms.is_empty]
             water_geoms = water_geoms.explode(ignore_index=True)
             water_geoms = water_geoms[water_geoms.geometry.type == "Polygon"]
 
             if water_geoms.shape[0] > 0:
                 water_data = gpd.GeoDataFrame(geometry=water_geoms, crs=crs)
@@ -375,14 +374,20 @@
 
         # Update area missing or cloud
         area_missing_or_cloud = get_area_missing_or_cloud(data, area_imaged).intersection(area_missing_or_cloud)
 
         # Remove points or LineStrings
         if area_missing_or_cloud.type == "GeometryCollection":
             area_missing_or_cloud = unary_union([gc for gc in area_missing_or_cloud.geoms if (gc.type == "Polygon") or (gc.type == "MultiPolygon")])
+        
+        # update area_missing
+        if mode == "max":
+            area_not_mapped = get_area_missing_or_cloud_or_land(best_floodmap, area_imaged=area_imaged).intersection(area_not_mapped)
+        else:
+            area_not_mapped = area_missing_or_cloud
 
 
     # Join adjacent polygons
     best_floodmap = best_floodmap.dissolve(by="class").reset_index()
     # Explode multipoligons to polygons
     best_floodmap = best_floodmap.explode(ignore_index=True)
     stuff_concat = [best_floodmap]
@@ -517,25 +522,22 @@
     for f in tqdm(floodmaps_paths):
         data = utils.read_geojson_from_gcp(f)
         data = data[~data.geometry.isna() & ~data.geometry.is_empty & (data.geometry.area > 10 ** 2)].copy()
         data = data.to_crs(dst_crs)
 
         is_valid_geoms = data.is_valid
         if not is_valid_geoms.all():
-            reasons_invalidity = [f"{validation.explain_validity(g)}\n" for g in data.geometry[~is_valid_geoms]]
-            print(f"\tProduct {f} There are {(~is_valid_geoms).sum()} geoms invalid of {is_valid_geoms.shape[0]}\n {reasons_invalidity}")
+            # reasons_invalidity = [f"{validation.explain_validity(g)}\n" for g in data.geometry[~is_valid_geoms]]
+            # print(f"\tProduct {f} There are {(~is_valid_geoms).sum()} geoms invalid of {is_valid_geoms.shape[0]}\n {reasons_invalidity}")
             data = make_valid(data)
 
         if data_all is None:
             data_all = data
         else:
             data_all = pd.concat([data_all, data], ignore_index=True)
-            # data_all = data_all.dissolve(by="class").reset_index()
-            # data_all = data_all.explode(ignore_index=True)
-            # data_all = data_all[~data_all.geometry.isna() & ~data_all.geometry.is_empty]
 
     print(f"\t{len(floodmaps_paths)} Products joined {data_all.shape}")
     # Save as geojson
     data_all = data_all.dissolve(by="class").reset_index()
     print(f"\t{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} Correctly dissolved. New shape: {data_all.shape}")
     data_all = data_all.explode(ignore_index=True)
     print(f"\t{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} Correctly exploded. New shape: {data_all.shape}")
```

### Comparing `ml4floods-0.0.4/ml4floods/models/utils/configuration.py` & `ml4floods-0.0.5/ml4floods/models/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/utils/losses.py` & `ml4floods-0.0.5/ml4floods/models/utils/losses.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/utils/metrics.py` & `ml4floods-0.0.5/ml4floods/models/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/utils/uncertainty.py` & `ml4floods-0.0.5/ml4floods/models/utils/uncertainty.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/models/worldfloods_model.py` & `ml4floods-0.0.5/ml4floods/models/worldfloods_model.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/preprocess/tiling.py` & `ml4floods-0.0.5/ml4floods/preprocess/tiling.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/preprocess/transformations.py` & `ml4floods-0.0.5/ml4floods/preprocess/transformations.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/preprocess/utils.py` & `ml4floods-0.0.5/ml4floods/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/preprocess/worldfloods/normalize.py` & `ml4floods-0.0.5/ml4floods/preprocess/worldfloods/normalize.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/preprocess/worldfloods/prepare_patches.py` & `ml4floods-0.0.5/ml4floods/preprocess/worldfloods/prepare_patches.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/scripts/inference.py` & `ml4floods-0.0.5/ml4floods/scripts/inference.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/serve/__init__.py` & `ml4floods-0.0.5/ml4floods/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/serve/read_tile.py` & `ml4floods-0.0.5/ml4floods/serve/read_tile.py`

 * *Files identical despite different names*

### Comparing `ml4floods-0.0.4/ml4floods/visualization/plot_utils.py` & `ml4floods-0.0.5/ml4floods/visualization/plot_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 import matplotlib.axes
 import rasterio
 from rasterio import plot as rasterioplt
 import rasterio.windows
 from matplotlib import colors
 import matplotlib.patches as mpatches
+import matplotlib.pyplot as plt
 import numpy as np
-from typing import Union, Optional, List, Tuple
+from typing import Union, Optional, List, Tuple, Dict, Any
 from ml4floods.data.worldfloods.configs import BANDS_S2, BANDS_L8
 from ml4floods.models.model_setup import get_channel_configuration_bands
 from ml4floods.data.worldfloods import configs
 from ml4floods.data import utils
 from matplotlib.patches import Patch
 import geopandas as gpd
 
@@ -144,14 +145,49 @@
     output = output[window_slices]
     if transform is not None:
         transform = transform if window is None else rasterio.windows.transform(window, transform)
 
     return output, transform
 
 
+def show(add_scalebar:bool=False, kwargs_scalebar:Optional[Dict[str, Any]]=None, **kwargs):
+    """
+    Shows the current plot with a scalebar if `add_scalebar` is True.
+
+    Args:
+        add_scalebar: whether to add a scalebar or not
+        kwargs_scalebar: kwargs for the scalebar
+        kwargs: kwargs for the plot
+    """
+    if "ax" in kwargs:
+        ax = kwargs.pop("ax")
+    else:
+        ax = plt.gca()
+
+    rasterioplt.show(**kwargs, ax=ax)
+
+    if add_scalebar:
+        try:
+             from matplotlib_scalebar.scalebar import ScaleBar
+        except ImportError as e:
+            raise ImportError("Install matplotlib-scalebar to use scalebar"
+                              "pip install matplotlib-scalebar"
+                              f"{e}")
+        
+        assert "transform" in kwargs, "transform must be in passed to the function to add scalebar"
+        
+        if kwargs_scalebar is None:
+            kwargs_scalebar = {"dx":1}
+        if "dx" not in kwargs_scalebar:
+            kwargs_scalebar["dx"] = 1
+        ax.add_artist(ScaleBar(**kwargs_scalebar))
+    
+    return ax
+
+
 def plot_rgb_image(input: Union[str, np.ndarray], transform:Optional[rasterio.Affine]=None,
                    window:Optional[rasterio.windows.Window]=None,
                    max_clip_val:Optional[float]=3000.,
                    min_clip_val:Optional[float]=0.,
                    channel_configuration:str="all",
                    collection_name:str="S2",
                    size_read:Optional[int]=None,
@@ -197,15 +233,15 @@
     image, transform = get_image_transform(input, transform=transform, bands=bands, window=window,
                                            size_read=size_read)
 
     if max_clip_val is not None:
         min_clip_val = 0 if min_clip_val is None else min_clip_val
         image = np.clip((image-min_clip_val)/(max_clip_val - min_clip_val), 0, 1)
 
-    return rasterioplt.show(image, transform=transform, **kwargs)
+    return show(source=image, transform=transform, **kwargs)
 
 COLORS_FLOODMAP = {"water": "#0010F6",
                    # "cloud": "#CFCFCF",
                    "cloud": "#4B4B4B",
                    "flood_trace": "#F66F00",
                    "flood-trace": "#F66F00",
                    "water-post-flood": "#FF09E3",
@@ -306,15 +342,15 @@
     image, transform = get_image_transform(input, transform=transform, bands=bands, window=window,
                                            size_read=size_read)
 
     if max_clip_val is not None:
         min_clip_val = 0 if min_clip_val is None else min_clip_val
         image = np.clip((image-min_clip_val)/(max_clip_val - min_clip_val), 0, 1)
 
-    return rasterioplt.show(image, transform=transform, **kwargs)
+    return show(source=image, transform=transform, **kwargs)
 
 
 def plots_preds_v1(prediction: Union[str, np.ndarray],transform:Optional[rasterio.Affine]=None,
                    window:Optional[rasterio.windows.Window]=None, legend=True,
                    size_read:Optional[int]=None,
                    **kwargs) -> matplotlib.axes.Axes:
     """
@@ -367,16 +403,16 @@
     """
     prediction, transform = get_image_transform(prediction, transform=transform, bands=[0], window=window,
                                                 size_read=size_read)
     prediction_show = prediction + 1
     cmap_preds, norm_preds, patches_preds = get_cmap_norm_colors(configs.COLORS_WORLDFLOODS_INVLANDWATER,
                                                                  INTERPRETATION_INVLANDWATER)
 
-    ax = rasterioplt.show(prediction_show, transform=transform, cmap=cmap_preds, norm=norm_preds,
-                          interpolation='nearest',**kwargs)
+    ax = show(source=prediction_show, transform=transform, cmap=cmap_preds, norm=norm_preds,
+              interpolation='nearest',**kwargs)
 
     if legend:
         ax.legend(handles=patches_preds,
                   loc='upper right')
 
     return ax
 
@@ -399,16 +435,16 @@
 
     target, transform = get_image_transform(target,transform=transform, bands=[0], window=window,
                                             size_read=size_read)
     target = target[0]
     cmap_preds, norm_preds, patches_preds = get_cmap_norm_colors(configs.COLORS_WORLDFLOODS,
                                                                  INTERPRETATION_WORLDFLOODS)
 
-    ax = rasterioplt.show(target, transform=transform, cmap=cmap_preds, norm=norm_preds,
-                          interpolation='nearest', **kwargs)
+    ax = show(source=target, transform=transform, cmap=cmap_preds, norm=norm_preds,
+              interpolation='nearest', **kwargs)
 
     if legend:
         ax.legend(handles=patches_preds,
                   loc='upper right')
 
     return ax
 
@@ -440,16 +476,16 @@
 
     v1gt = land_water.copy() # {0: invalid, 1: land, 2: water}
     v1gt[clear_clouds == 2] = 3
 
     cmap_preds, norm_preds, patches_preds = get_cmap_norm_colors(configs.COLORS_WORLDFLOODS,
                                                                  INTERPRETATION_WORLDFLOODS)
 
-    ax = rasterioplt.show(v1gt, transform=transform, cmap=cmap_preds, norm=norm_preds,
-                          interpolation='nearest', **kwargs)
+    ax = show(source=v1gt, transform=transform, cmap=cmap_preds, norm=norm_preds,
+              interpolation='nearest', **kwargs)
 
     if legend:
         ax.legend(handles=patches_preds,
                   loc='upper right')
 
     return ax
 
@@ -475,16 +511,16 @@
         permanent, _ = get_image_transform(permanent, transform=transform, bands=bands, window=window,
                                            size_read=min(target.shape))
         permanent = permanent[0]
         target = gt_v1_with_permanent_water(target, permanent)
 
     cmap_gt, norm_gt, patches_gt = get_cmap_norm_colors(COLORS_WORLDFLOODS_PERMANENT, INTERPRETATION_WORLDFLOODS_PERMANENT)
 
-    ax = rasterioplt.show(target,transform=transform, cmap=cmap_gt, norm=norm_gt,
-                          interpolation='nearest', **kwargs)
+    ax = show(source=target,transform=transform, cmap=cmap_gt, norm=norm_gt,
+              interpolation='nearest', **kwargs)
 
     if legend:
         ax.legend(handles=patches_gt,
                   loc='upper right')
 
     return ax
 
@@ -507,8 +543,64 @@
     image[positives == 1] = colors.to_rgb('C9')
     image[positives == 2] = colors.to_rgb('orange')
     image[positives == 3] = colors.to_rgb('blue')
 
     cmap_colors = ['orange','C9', 'blue']
     cmap = colors.ListedColormap(cmap_colors)
     
-    return rasterioplt.show(np.moveaxis(image,-1,0), cmap = cmap, transform = transform, title = title, **kwargs)
+    return show(source=np.moveaxis(image,-1,0), cmap = cmap, transform = transform, title = title, **kwargs)
+
+
+def plot_segmentation_mask(mask, color_array,
+                           transform:Optional[rasterio.Affine]=None,
+                           interpretation_array:Optional[List[str]]=None,
+                           legend:bool=True, ax:Optional[matplotlib.axes.Axes]=None) -> matplotlib.axes.Axes:
+    """
+    Args:
+        mask: (H, W) np.array
+        color_array: colors for values 0,...,len(color_array)-1 of mask
+        transform:
+        interpretation_array: interpretation for classes 0, ..., len(color_array)-1
+        legend: plot the legend
+        ax:
+
+    """
+    cmap_categorical = colors.ListedColormap(color_array)
+
+    norm_categorical = colors.Normalize(vmin=-.5,
+                                        vmax=color_array.shape[0] - .5)
+
+    color_array = np.array(color_array)
+    if interpretation_array is not None:
+        assert len(interpretation_array) == color_array.shape[
+            0], f"Different numbers of colors and interpretation {len(interpretation_array)} {color_array.shape[0]}"
+
+
+    ax = show(source=mask,transform=transform, ax=ax,
+              cmap=cmap_categorical, norm=norm_categorical, interpolation='nearest')
+
+    if legend:
+        patches = []
+        for c, interp in zip(color_array, interpretation_array):
+            patches.append(mpatches.Patch(color=c, label=interp))
+
+        ax.legend(handles=patches,
+                  loc='upper right')
+    return ax
+
+
+INTERPRETATION_CLOUDSEN12 = ["clear", "Thick cloud", "Thin cloud", "Cloud shadow"]
+
+COLORS_CLOUDSEN12 = np.array([[139, 64, 0], # clear
+                              [220, 220, 220], # Thick cloud
+                              [180, 180, 180], # Thin cloud
+                              [60, 60, 60]], # cloud shadow
+                             dtype=np.float32) / 255
+
+def plot_cloudSEN12mask(mask, legend: bool = True, ax=None):
+    """
+    Args:
+        mask: (H, W) np.array
+    """
+
+    return plot_segmentation_mask(mask=mask, color_array=COLORS_CLOUDSEN12,
+                                  interpretation_array=INTERPRETATION_CLOUDSEN12, legend=legend, ax=ax)
```

### Comparing `ml4floods-0.0.4/ml4floods.egg-info/PKG-INFO` & `ml4floods-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1
-Name: ml4floods
-Version: 0.0.4
-Summary: Machine learning models for end-to-end flood extent segmentation.
-Author: SpaceML-org
-Keywords: floods pytorch machine-learning earth
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
-Provides-Extra: docs
-License-File: LICENSE
-
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/spaceml-org/ml4floods/main/jupyterbook/ml4floods_banner.png" alt="awesome ml4floods" width="50%">
 </p>
 
 ML4Floods is an end-to-end ML pipeline for flood extent estimation: from data preprocessing, model training, model deployment to visualization.
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/spaceml-org/ml4floods/main/jupyterbook/content/ml4ops/ts_albania.gif" alt="awesome flood extent estimation" width="100%">
 </p>
 
-Install the package:
+## Install
+
+Install from [pip](https://pypi.org/project/ml4floods/):
+```bash
+pip install ml4floods
+```
+
+Install the latest version from GitHub:
 
 ```bash
 pip install git+https://github.com/spaceml-org/ml4floods#egg=ml4floods
 ```
 
+## Docs
+[spaceml-org.github.io/ml4floods](https://spaceml-org.github.io/ml4floods)
+
 These tutorials may help you explore the datasets and models:
 * [Project rationale](https://spaceml-org.github.io/ml4floods/content/intro/introduction.html).
 * [Run the model on time series of Sentinel-2 images](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_inference_on_image_time_series.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_inference_on_image_time_series.ipynb)
 * [ML-models step by step](https://spaceml-org.github.io/ml4floods/content/ml_overview.html)
     * [Training](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_Train_models.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_Train_models.ipynb)
     * [Inference on new data](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_Run_Inference_on_new_data.html) (a Sentinel-2 image) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_Run_Inference_on_new_data.ipynb)
     * [Perf metrics](https://spaceml-org.github.io/ml4floods/content/ml4ops/HOWTO_performance_metrics_workflow.html) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/spaceml-org/ml4floods/blob/main/jupyterbook/content/ml4ops/HOWTO_performance_metrics_workflow.ipynb)
```

### Comparing `ml4floods-0.0.4/ml4floods.egg-info/SOURCES.txt` & `ml4floods-0.0.5/ml4floods.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 ml4floods.egg-info/PKG-INFO
 ml4floods.egg-info/SOURCES.txt
 ml4floods.egg-info/dependency_links.txt
 ml4floods.egg-info/requires.txt
 ml4floods.egg-info/top_level.txt
 ml4floods/data/S2_SAFE_reader.py
 ml4floods/data/__init__.py
+ml4floods/data/cmcloudsen12.py
 ml4floods/data/cmkappazeta.py
 ml4floods/data/cms2cloudless.py
 ml4floods/data/config.py
 ml4floods/data/create_gt.py
 ml4floods/data/dataset.py
 ml4floods/data/ee_download.py
 ml4floods/data/save_cog.py
 ml4floods/data/utils.py
+ml4floods/data/vectorize.py
 ml4floods/data/configuration/train_test_split_extra_dataset.json
 ml4floods/data/configuration/train_test_split_original_dataset.json
 ml4floods/data/copernicusEMS/__init__.py
 ml4floods/data/copernicusEMS/activations.py
 ml4floods/data/copernicusEMS/utils.py
 ml4floods/data/index/__init__.py
 ml4floods/data/index/geographic_index.py
```

### Comparing `ml4floods-0.0.4/setup.py` & `ml4floods-0.0.5/setup.py`

 * *Files identical despite different names*

