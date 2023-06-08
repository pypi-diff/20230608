# Comparing `tmp/molgraph-0.3.6.tar.gz` & `tmp/molgraph-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.3.6.tar", last modified: Wed Jun  7 13:26:14 2023, max compression
+gzip compressed data, was "molgraph-0.3.8.tar", last modified: Thu Jun  8 16:06:27 2023, max compression
```

## Comparing `molgraph-0.3.6.tar` & `molgraph-0.3.8.tar`

### file list

```diff
@@ -1,108 +1,118 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.6/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-07 13:26:14.190172 molgraph-0.3.6/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3122 2023-05-26 15:32:21.000000 molgraph-0.3.6/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.182171 molgraph-0.3.6/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.6/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.6/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.6/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.6/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.6/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.6/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.6/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.6/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12448 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11175 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9188 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11222 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10436 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14857 2023-06-07 13:20:34.000000 molgraph-0.3.6/molgraph/layers/attentional/gt_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13283 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/layers/base.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.6/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9825 2023-06-07 12:59:58.000000 molgraph-0.3.6/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9663 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10612 2023-06-07 13:00:51.000000 molgraph-0.3.6/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.6/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.6/molgraph/layers/geometric/_radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9364 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10190 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/geometric/gcf_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.6/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22003 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15527 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/message_passing/mpnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.6/molgraph/layers/ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.6/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10713 2023-06-07 13:25:59.000000 molgraph-0.3.6/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.186172 molgraph-0.3.6/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.6/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-07 12:34:11.000000 molgraph-0.3.6/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.6/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.6/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11080 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-06 20:54:37.000000 molgraph-0.3.6/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9592 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11858 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6753 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20494 2023-06-06 21:11:15.000000 molgraph-0.3.6/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.6/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.6/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4613 2023-04-14 12:58:07.000000 molgraph-0.3.6/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.6/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.6/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.6/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.6/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.6/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.6/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.6/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.6/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.6/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7883 2023-04-14 12:58:07.000000 molgraph-0.3.6/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7065 2023-06-07 12:49:03.000000 molgraph-0.3.6/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.6/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.6/molgraph/models/interpretability/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.6/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6831 2023-04-14 12:58:07.000000 molgraph-0.3.6/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.6/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.6/molgraph/models/pretraining/attribute_masking.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.190172 molgraph-0.3.6/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.6/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.6/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.6/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    39597 2023-06-06 14:24:00.000000 molgraph-0.3.6/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-07 13:26:14.182171 molgraph-0.3.6/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3842 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3234 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-07 13:26:14.000000 molgraph-0.3.6/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-07 13:26:14.190172 molgraph-0.3.6/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-04-06 16:32:34.000000 molgraph-0.3.6/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.918886 molgraph-0.3.8/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.3.8/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5709 2023-06-08 16:06:27.918886 molgraph-0.3.8/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4989 2023-06-08 14:54:16.000000 molgraph-0.3.8/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.902886 molgraph-0.3.8/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      408 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      954 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.3.8/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.3.8/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15266 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13722 2022-09-20 11:37:26.000000 molgraph-0.3.8/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21456 2023-04-12 17:28:19.000000 molgraph-0.3.8/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.3.8/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.3.8/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3823 2023-06-06 20:54:37.000000 molgraph-0.3.8/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.3.8/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12448 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11175 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9188 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11222 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10436 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14857 2023-06-07 13:20:34.000000 molgraph-0.3.8/molgraph/layers/attentional/gt_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13283 2023-06-07 13:25:59.000000 molgraph-0.3.8/molgraph/layers/base.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.3.8/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9825 2023-06-07 12:59:58.000000 molgraph-0.3.8/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9663 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10612 2023-06-07 13:00:51.000000 molgraph-0.3.8/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.3.8/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1613 2022-09-02 11:38:53.000000 molgraph-0.3.8/molgraph/layers/geometric/_radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9364 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10190 2023-06-07 12:34:11.000000 molgraph-0.3.8/molgraph/layers/geometric/gcf_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.3.8/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16685 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13978 2023-06-07 15:46:32.000000 molgraph-0.3.8/molgraph/layers/message_passing/mpnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6419 2023-04-17 15:25:58.000000 molgraph-0.3.8/molgraph/layers/ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.3.8/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10713 2023-06-07 13:25:59.000000 molgraph-0.3.8/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.910886 molgraph-0.3.8/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.3.8/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2538 2023-06-07 15:46:32.000000 molgraph-0.3.8/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2008 2022-08-18 17:05:41.000000 molgraph-0.3.8/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.3.8/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11080 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4557 2023-06-06 20:54:37.000000 molgraph-0.3.8/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9592 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4234 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11858 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6753 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20494 2023-06-06 21:11:15.000000 molgraph-0.3.8/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.3.8/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6710 2023-05-26 15:46:41.000000 molgraph-0.3.8/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4628 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3296 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6250 2022-09-14 11:22:14.000000 molgraph-0.3.8/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5418 2022-09-14 10:36:59.000000 molgraph-0.3.8/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.3.8/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2192 2022-06-01 11:22:01.000000 molgraph-0.3.8/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5182 2022-08-15 09:20:55.000000 molgraph-0.3.8/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.3.8/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2071 2022-06-01 11:25:29.000000 molgraph-0.3.8/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      517 2022-06-01 11:21:46.000000 molgraph-0.3.8/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      486 2023-04-06 15:13:35.000000 molgraph-0.3.8/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7765 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6947 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       84 2022-08-12 12:53:20.000000 molgraph-0.3.8/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      223 2022-07-14 20:09:09.000000 molgraph-0.3.8/molgraph/models/interpretability/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6733 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11937 2022-09-20 11:35:03.000000 molgraph-0.3.8/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6854 2023-06-07 16:34:42.000000 molgraph-0.3.8/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.914886 molgraph-0.3.8/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:32.000000 molgraph-0.3.8/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-05 19:46:46.000000 molgraph-0.3.8/molgraph/models/pretraining/attribute_masking.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.918886 molgraph-0.3.8/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2022-08-08 12:38:45.000000 molgraph-0.3.8/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.3.8/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1844 2022-08-18 15:00:21.000000 molgraph-0.3.8/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    40311 2023-06-08 14:54:16.000000 molgraph-0.3.8/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.906886 molgraph-0.3.8/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5709 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3448 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-06-08 16:06:27.000000 molgraph-0.3.8/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-08 16:06:27.918886 molgraph-0.3.8/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1510 2023-06-08 09:43:15.000000 molgraph-0.3.8/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-08 16:06:27.918886 molgraph-0.3.8/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3633 2022-09-20 11:35:03.000000 molgraph-0.3.8/tests/test_chemistry.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15601 2022-09-20 11:35:03.000000 molgraph-0.3.8/tests/test_interpretability.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15816 2023-06-08 14:54:16.000000 molgraph-0.3.8/tests/test_layers.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3425 2023-04-06 13:54:41.000000 molgraph-0.3.8/tests/test_models.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2409 2023-04-06 15:41:44.000000 molgraph-0.3.8/tests/test_models_2.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17467 2023-05-30 09:41:48.000000 molgraph-0.3.8/tests/test_tensors.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11741 2023-05-30 09:41:50.000000 molgraph-0.3.8/tests/test_tensors_2.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11755 2023-05-30 09:41:51.000000 molgraph-0.3.8/tests/test_tensors_3.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12678 2023-05-30 09:41:54.000000 molgraph-0.3.8/tests/test_tensors_4.py
```

### Comparing `molgraph-0.3.6/LICENSE` & `molgraph-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/_filter_warnings.py` & `molgraph-0.3.8/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/__init__.py` & `molgraph-0.3.8/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.3.8/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.3.8/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.3.8/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.3.8/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/conformer_generator.py` & `molgraph-0.3.8/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/conformer_utils.py` & `molgraph-0.3.8/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/encoders.py` & `molgraph-0.3.8/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/features.py` & `molgraph-0.3.8/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.3.8/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/ops.py` & `molgraph-0.3.8/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/chemistry/vis.py` & `molgraph-0.3.8/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/__init__.py` & `molgraph-0.3.8/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.3.8/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.3.8/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.3.8/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.3.8/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.3.8/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.3.8/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/base.py` & `molgraph-0.3.8/molgraph/layers/base.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.3.8/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.3.8/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.3.8/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.3.8/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/geometric/_radial_basis.py` & `molgraph-0.3.8/molgraph/layers/geometric/_radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.3.8/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.3.8/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.3.8/molgraph/layers/message_passing/edge_conv.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,33 +21,31 @@
 from molgraph.layers.ops import propagate_node_features
 
 
 Config = TypeVar('Config', bound=dict)
 
 
 @keras.utils.register_keras_serializable(package='molgraph')
-class EdgeConv(keras.layers.Layer):
+class EdgeConv(tf.keras.layers.Layer):
 
-    """Edge convolutional layer, used to build DMPNN [#]_ and DGIN [#]_ like models.
+    '''Edge convolutional layer, used to build DMPNN [#]_ and DGIN [#]_ like models.
 
     **Important:**
 
     As of now, EdgeConv only works on (sub)graphs with at least one edge/bond. If your dataset consists
     of molecules with a single atom, please add self loops: 
     ``molgraph.chemistry.MolecularGraphEncoder(..., self_loops=True)``
 
     **Examples:**
 
     Build a DGIN model. Note that the DGIN model below differs from `molgraph.models.DGIN` in some
     ways. For instance, it uses the very previous edge states (in `molgraph.layers.EdgeConv`) and 
     node states (in `molgraph.layers.GINConv`) as residual ("skip connections") rather than the very 
     initial edge states and node states respectively. Furthermore, this implementation also allows us to use
-    GRU as the update function, though default is to use a Dense layer. Like the models
-    (`molgraph.models.DGIN` and `molgraph.models.DMPNN`), this implementation allows for both shared 
-    ("weight tying") and unshared weights. Simply pass the previous layer via the `tie_layer` argument.
+    GRU as the update function, though default is to use a Dense layer. 
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
     ...         'node_feature': [
     ...             [1.0, 0.0],
@@ -68,86 +66,34 @@
     ...             [0.0, 1.0]
     ...         ],
     ...     }
     ... )
     >>> # Build a DGIN model for binary classificaton
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' field
-    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' field
+    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' component
+    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' component
     ...     molgraph.layers.NodeReadout(target='edge_state'),       # target='edge_state' is default
     ...     molgraph.layers.GINConv(32),
     ...     molgraph.layers.GINConv(32),
     ...     molgraph.layers.Readout(),
     ...     tf.keras.layers.Dense(1, activation='sigmoid')
     ... ])
     >>> gnn_model.output_shape
     (None, 1)
 
-    Tie weights of the previous layers with the subsequent layers:
-
-    >>> graph_tensor = molgraph.GraphTensor(
-    ...     data={
-    ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
-    ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
-    ...         'node_feature': [
-    ...             [1.0, 0.0],
-    ...             [1.0, 0.0],
-    ...             [1.0, 0.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0]
-    ...         ],
-    ...         'graph_indicator': [0, 0, 1, 1, 1],
-    ...         'edge_feature': [
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0],
-    ...             [0.0, 1.0],
-    ...             [0.0, 1.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0],
-    ...             [1.0, 0.0],
-    ...             [0.0, 1.0]
-    ...         ],
-    ...     }
-    ... )
-    >>> # Build a model with EdgeConv
-    >>> edge_conv_1 = molgraph.layers.EdgeConv(
-    ...     units=16, 
-    ...     update_mode='gru'       # lets use GRU updates instead (as per Gilmer et al. (2017))
-    ... )
-    >>> edge_conv_2 = molgraph.layers.EdgeConv(
-    ...     units=32,               # will be ignored as EdgeConv layer is passed to `tie_layer`
-    ...     update_mode='gru',      # will be ignored as EdgeConv layer is passed to `tie_layer`
-    ...     tie_layer=edge_conv_1
-    ... )
-    >>> edge_conv_3 = molgraph.layers.EdgeConv(
-    ...     units=16,               # will be ignored as EdgeConv layer is passed to `tie_layer`
-    ...     update_mode='gru',      # will be ignored as EdgeConv layer is passed to `tie_layer`
-    ...     tie_layer=edge_conv_1   # specifying edge_conv_2 would be equivalent
-    ... )
-    >>> gnn_model = tf.keras.Sequential([
-    ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     edge_conv_1,
-    ...     edge_conv_2,
-    ...     edge_conv_3,
-    ...     molgraph.layers.NodeReadout()
-    ... ])
-    >>> gnn_model.output_shape
-    (None, 16)
-
     Args:
         units (int, None):
             Number of output units.
         update_mode (bool):
             Specify what type of update will be performed. Either 'dense' or 'gru'. 
-            If 'gru' is specified, make sure weight tying is performed
-            (see 'tie_layer' argument above). Default to 'dense'.
-        tie_layer (molgraph.layers.message_passing.edge_conv.EdgeConv, None):
-            Pass the previous EdgeConv layer to perform weight tying. If None, weight tying
-            will not be performed (each layer has its own weights). Default to None.
+            Default to 'gru'.
+        update_fn (tf.keras.layers.GRUCell, tf.keras.layers.Dense, None):
+            Optionally pass update function (GRUCell or Dense) for weight-tying 
+            of the update step (GRU step or Dense step). Default to None.
         activation (tf.keras.activations.Activation, callable, str, None):
             Activation function applied to the updated edge states. If None is set, either 'relu'
             (for `update_mode='dense'`) or 'tanh' (for `update_mode='gru'`) will be used. 
             Default to None.
         recurrent_activation (tf.keras.activations.Activation, callable, str, None):
             Activation function applied to the recurrent step (only relevant if ``update_mode='gru'``).
             Default to to 'sigmoid'.
@@ -177,140 +123,156 @@
         kernel_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the kernels. Default to None.
         bias_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the biases. Default to None.
         recurrent_constraint (tf.keras.constraints.Constraint, None):
             Constraint function applied to the recurrent kernel (only relevant if ``update_mode='gru'``).
             Default to None.
-        automatically_infer_gru_activation (bool):
-            Whether to automatically infer the activation for GRU (when `activation=None`). Default to True.
-        parallel_iterations (int, None):
-            Number of ``parallel_iterations`` to be set for ``tf.map_fn`` to find
-            the reverse edge states to be subtracted from the aggregated edge states.
 
     References:
         .. [#] https://arxiv.org/pdf/1904.01561.pdf
         .. [#] https://www.mdpi.com/1420-3049/26/20/6185
-    """
-
+    '''
+    
     def __init__(
         self,
-        units: Optional[int] = None,
+        units: Optional[int],
         update_mode: str = 'dense',
-        tie_layer: Optional['EdgeConv'] = None,
+        update_fn: Optional[Union[
+            tf.keras.layers.GRUCell, tf.keras.layers.Dense]] = None,
         activation: Union[str, None, Callable[[tf.Tensor], tf.Tensor]] = None,
         recurrent_activation: Union[str, None, Callable[[tf.Tensor], tf.Tensor]] = 'sigmoid',
         use_bias: Optional[bool] = None,
         kernel_initializer: Union[str, None, initializers.Initializer] = None,
         bias_initializer: Union[str, None, initializers.Initializer] = 'zeros',
         recurrent_initializer: Union[str, None, initializers.Initializer] = 'orthogonal',
         kernel_regularizer: Optional[regularizers.Regularizer] = None,
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         recurrent_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
         bias_constraint: Optional[constraints.Constraint] = None,
         recurrent_constraint: Optional[constraints.Constraint] = None,
-        automatically_infer_gru_activation: bool = True,
-        parallel_iterations: Optional[int] = None,
         **kwargs
     ):
+        self_projection = kwargs.pop('self_projection', False)
+
+        if self_projection:
+            raise ValueError('`EdgeConv` does not support self projection.')
+        
         super().__init__(**kwargs)
+
+        if units is None:
+            raise ValueError('`EdgeConv` requires units (int) to be passed.')
+        
         self.units = units
-        self.update_mode = update_mode
-        self.tie_layer = tie_layer
-        if not activation and update_mode != 'dense' and automatically_infer_gru_activation:
-            activation = 'tanh'
-        self.activation = activations.get(activation)
-        self.recurrent_activation = activations.get(recurrent_activation)
+        self.update_fn = update_fn
+        self.update_mode = update_mode.lower()
+        if activation is None:
+            if self.update_mode.startswith('gru'):
+                self.activation = 'tanh'
+            else:
+                self.activation = 'linear'
+        else:
+            self.activation = activation
         if use_bias is None:
-            use_bias = False if update_mode == 'dense' else True
+            use_bias = True if update_mode.startswith('gru') else True
         self.use_bias = use_bias
+        self.recurrent_activation = activations.get(recurrent_activation)
         if kernel_initializer is None:
             kernel_initializer = (
-                initializers.TruncatedNormal(stddev=0.005) if update_mode == 'dense' 
-                else 'glorot_uniform')
+                'glorot_uniform' if self.update_mode.startswith('gru') 
+                else initializers.TruncatedNormal(stddev=0.005)
+            )
         self.kernel_initializer  = initializers.get(kernel_initializer)
         self.bias_initializer = initializers.get(bias_initializer or 'zeros')
         self.recurrent_initializer = initializers.get(recurrent_initializer or 'orthogonal')
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.bias_regularizer = regularizers.get(bias_regularizer)
         self.activity_regularizer = regularizers.get(activity_regularizer)
         self.recurrent_regularizer = regularizers.get(recurrent_regularizer)
         self.kernel_constraint = constraints.get(kernel_constraint)
         self.bias_constraint = constraints.get(bias_constraint)
-        self.recurrent_constraint = constraints.get(recurrent_constraint)
-        self._parallel_iterations = parallel_iterations
-        self._automatically_infer_gru_activation = automatically_infer_gru_activation
+        self.recurrent_constraint = constraints.get(recurrent_constraint)     
         self._initialize_edge_state = None
         self._built = False
 
-    def _build(self, units, initialize_edge_state):
+    def _build(self, initialize_edge_state):
+        
+        with tf_utils.maybe_init_scope(self):
 
-        if self.tie_layer:
-            self.update_projection = self._get_tied_layer_projection()
-            self.units = self.tie_layer.units
-        else:
             if initialize_edge_state:
-                self.initial_projection = self._get_dense(units)
-            self.update_projection = (
-                self._get_dense(units) if self.update_mode == 'dense' 
-                else self._get_gru(units))
+                self._initialize_edge_state = True
+                self.initial_projection = self._get_dense(self.units)
+            else:
+                self._initialize_edge_state = False
+
+            if self.update_fn is None:
+                self.update_fn = (
+                    self._get_gru(self.units) if self.update_mode.startswith('gru')
+                    else self._get_dense(self.units)
+                )
+            elif self.units != self.update_fn.units:
+                raise ValueError(
+                    'units of `update_fn` needs to match units of this layer.')
+
+            self._built = True
 
     def call(self, tensor: GraphTensor) -> GraphTensor:
 
         tensor_orig = tensor
         if isinstance(tensor.node_feature, tf.RaggedTensor):
             tensor = tensor.merge()
 
         # EdgeConv requires edge features, so if edge features do not exist,
         # we force edge features by initializing them as ones vector
         if not hasattr(tensor, 'edge_feature'):
             tensor = tensor.update({
                 'edge_feature': tf.ones(
                     shape=[tf.shape(tensor.edge_dst)[0], 1], dtype=tf.float32)})
-
+            
         if not self._built:
-            with tf_utils.maybe_init_scope(self):
-                self._initialize_edge_state = (
-                    True if not hasattr(tensor, 'edge_state') else False)
-                if not (self.units and (self._initialize_edge_state or self.update_mode == 'dense')):
-                    if hasattr(tensor, 'edge_state'):
-                        self.units = tensor.edge_state.shape[-1]
-                    else:
-                        self.units = tensor.node_feature.shape[-1] + tensor.edge_feature.shape[-1]
-                self._build(self.units, self._initialize_edge_state)
-                self._built = True
+            initialize_edge_state = (
+                True if not hasattr(tensor, 'edge_state') else False)
+            self._build(initialize_edge_state)
 
         if self._initialize_edge_state:
             edge_state = tf.gather(tensor.node_feature, tensor.edge_src)
             edge_state = tf.concat([edge_state, tensor.edge_feature], axis=-1)
             edge_state = self.initial_projection(edge_state)
             tensor = tensor.update({'edge_state': edge_state})
-                
+        
         edge_state_update = edge_message_step(
             edge_feature=tensor.edge_state,
             edge_src=tensor.edge_src,
-            edge_dst=tensor.edge_dst,
-            graph_indicator=tensor.graph_indicator,
-            parallel_iterations=self._parallel_iterations)
+            edge_dst=tensor.edge_dst)
 
         edge_state_update = edge_update_step(
             edge_feature=edge_state_update,
             edge_feature_prev=tensor.edge_state,
-            update_projection=self.update_projection)
+            update_projection=self.update_fn)
         
         return tensor_orig.update({'edge_state': edge_state_update})
 
+    @classmethod
+    def from_config(cls: Type['EdgeConv'], config: Config) -> 'EdgeConv':
+        initialize_edge_state = config.pop('initialize_edge_state') 
+        layer = cls(**config)
+        if initialize_edge_state is None:
+            pass
+        else:
+            layer._build(initialize_edge_state)
+        return layer
+    
     def get_config(self) -> Config:
         base_config = super().get_config()
         config = {
             'units': self.units,
             'update_mode': self.update_mode,
-            'tie_layer': keras.layers.serialize(self.tie_layer),
+            'update_fn': tf.keras.layers.serialize(self.update_fn),
             'activation':
                 activations.serialize(self.activation),
             'recurrent_activation':
                 activations.serialize(self.recurrent_activation),
             'use_bias':
                 self.use_bias,
             'kernel_initializer':
@@ -329,27 +291,18 @@
                 regularizers.serialize(self.recurrent_regularizer),
             'kernel_constraint':
                 constraints.serialize(self.kernel_constraint),
             'bias_constraint':
                 constraints.serialize(self.bias_constraint),
             'recurrent_constraint':
                 constraints.serialize(self.recurrent_constraint),
-            'automatically_infer_gru_activation': self._automatically_infer_gru_activation,
-            'parallel_iterations': self._parallel_iterations,
             'initialize_edge_state': self._initialize_edge_state,
         }
         base_config.update(config)
         return base_config
-
-    @classmethod
-    def from_config(cls: Type['EdgeConv'], config: Config) -> 'EdgeConv':
-        initialize_edge_state = config.pop('initialize_edge_state')
-        layer = cls(**config)
-        layer._build(config['units'], initialize_edge_state)
-        return layer
     
     def compute_output_shape(
         self,
         input_shape
     ) -> tf.TensorShape:
         return input_shape
     
@@ -374,108 +327,54 @@
             activation=self.activation,
             recurrent_activation=self.recurrent_activation,
             use_bias=self.use_bias,
             kernel_initializer=self.kernel_initializer.from_config(
                 self.kernel_initializer.get_config()),
             bias_initializer=self.bias_initializer.from_config(
                 self.bias_initializer.get_config()),
-            recurrent_initializer=self.recurrent_initializer,
+            recurrent_initializer=self.recurrent_initializer.from_config(
+                self.recurrent_initializer.get_config()),
             kernel_regularizer=self.kernel_regularizer,
             bias_regularizer=self.bias_regularizer,
             recurrent_regularizer=self.recurrent_regularizer,
             kernel_constraint=self.kernel_constraint,
             bias_constraint=self.bias_constraint,
             recurrent_constraint=self.recurrent_constraint)
-
-    def _get_tied_layer_projection(self):
-        self._check_layer_types()
-        update_projection = getattr(self.tie_layer, 'update_projection', None)
-        if not update_projection:
-            raise ValueError(
-                f'`{self.tie_layer.name}` is not built. Make sure `{self.tie_layer.name}` is ' +
-                f'built before building this layer (`{self.name}`). `{self.tie_layer.name}` should ' + 
-                f'come before this layer (`{self.name}`) in the sequence (model).')   
-        return update_projection
-
-    def _check_layer_types(self):
-        if type(self) != type(self.tie_layer):
-            raise ValueError(
-                f'`{self.tie_layer.name}` needs to be the same type as this layer (`{self.name}`)')
-
     
 def edge_update_step(
     edge_feature: tf.Tensor, 
     edge_feature_prev: tf.Tensor,
     update_projection: Union[
         keras.layers.Dense, keras.layers.GRUCell, keras.layers.LSTMCell],
 ) -> tf.Tensor:
     if isinstance(update_projection, keras.layers.Dense):
         edge_feature_update = update_projection(
             tf.concat([edge_feature_prev, edge_feature], axis=1))
-    else: # if keras.layers.GRUCell
+    else:
         edge_feature_update, _ = update_projection(
             inputs=edge_feature,
             states=edge_feature_prev)
     return edge_feature_update
 
 def edge_message_step(
-    edge_feature: tf.Tensor, # or 'edge_state'
+    edge_feature: tf.Tensor,
     edge_src: tf.Tensor,
     edge_dst: tf.Tensor,
-    graph_indicator: tf.Tensor,
-    parallel_iterations: Optional[int] = None
 ) -> tf.Tensor:
     num_nodes = tf.maximum(tf.reduce_max(edge_src), tf.reduce_max(edge_dst)) + 1
     message = tf.math.unsorted_segment_sum(edge_feature, edge_dst, num_nodes)
     message = tf.gather(message, edge_src)
-    message -= _get_reverse_edge_features(
-        edge_feature, edge_src, edge_dst, graph_indicator, parallel_iterations)
+    message -= _get_reverse_edge_features(edge_feature, edge_src, edge_dst)
     return message
 
-@tf.function
-def _get_reverse_edge_features(
-    edge_feature: tf.Tensor, 
-    edge_src: tf.Tensor,
-    edge_dst: tf.Tensor,
-    graph_indicator: tf.Tensor,
-    parallel_iterations: Optional[int] = None
-) -> tf.Tensor:
-    # Make tensors ragged to that they can be iterated over by tf.map_fn
-    graph_indicator_edges = tf.gather(graph_indicator, edge_dst)
-    edge_feature, edge_src, edge_dst = tf.nest.map_structure(
-        lambda x: tf.RaggedTensor.from_value_rowids(x, graph_indicator_edges),
-        (edge_feature, edge_src, edge_dst))
-    # Define appropriate output spec
-    output_spec = tf.RaggedTensorSpec(
-        shape=[None, edge_feature.shape[-1]], 
-        ragged_rank=0, 
-        dtype=tf.float32)
-    # Find all reverse edge features in the whole graph
-    reverse_edge_state = tf.map_fn(
-        fn=_get_reverse_edge_features_fn, 
-        elems=(edge_feature, edge_src, edge_dst), 
-        fn_output_signature=output_spec,
-        parallel_iterations=parallel_iterations)
-    # Convert ragged tensor output to a tensor.
-    return reverse_edge_state.merge_dims(outer_axis=0, inner_axis=1)
-
-def _get_reverse_edge_features_fn(
-    inputs: Tuple[tf.Tensor, tf.Tensor, tf.Tensor], 
-) -> tf.Tensor:
-    '''This function finds the reverse edge features/states for each molecule/subgraph.
-
-    Will be called by `tf.map_fn` in `_get_reverse_edge_features`.
-    '''
-    edge_feature, edge_src, edge_dst = inputs
-    # Find the index of "reverse" edge of "forward" edge edge_src->edge_dst
+def _get_reverse_edge_features(edge_feature, edge_src, edge_dst):
     edge_exclude = tf.logical_and(
-        edge_src[:, None] == edge_dst,
-        edge_dst[:, None] == edge_src)
-    # Obtain index of edge_src->edge_dst ("forward") and its corresponding
-    # edge_src<-edge_dst ("reverse"). For molecules: forward and reverse
-    # edges are usually the same and always exist. 
+        edge_dst[:, None] == edge_dst,
+        edge_src[:, None] == edge_src)
+        
     edge_forward, edge_reverse = tf.split(tf.where(edge_exclude), 2, axis=-1)
+
     return tf.tensor_scatter_nd_add(
         tf.zeros_like(edge_feature), 
         tf.expand_dims(edge_forward, -1), 
-        tf.gather(edge_feature, edge_reverse))
-
+        tf.gather(edge_feature, edge_reverse)
+    )
```

### Comparing `molgraph-0.3.6/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.3.8/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 class MPNNConv(BaseLayer):
 
     """Message passing neural network layer (MPNN)
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to Gilmer
     et al. this implementation does not use weight tying by default; for neither the 
     message function nor the update function. Furthermore, instead of the GRU-based
-    update function, here, a simple fully-connected (dense) layer is used by default. 
-    However, optionally, the previous MPNNConv layer can be passed to the current layer
-    via `tie_layer` (see below for example) to perform weight tying.
+    update function, here, a simple fully-connected (dense) layer can be used too.
+    Though default is GRU. 
 
     **Examples:**
 
     Inputs a ``GraphTensor`` encoding (two) subgraphs:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
@@ -90,15 +89,15 @@
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
     ...     molgraph.layers.MPNNConv(16, activation='relu'),
     ...     molgraph.layers.MPNNConv(16, activation='relu')
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
-    Tie weights of the previous layer with the subsequent layers:
+    Pass the same GRU cell to each layer to perform weight sharing:
 
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [0, 1, 2, 2, 3, 3, 4, 4],
     ...         'edge_src': [1, 0, 3, 4, 2, 4, 3, 2],
     ...         'node_feature': [
     ...             [1.0, 0.0],
@@ -116,50 +115,33 @@
     ...             [1.0, 0.0],
     ...             [0.0, 1.0],
     ...             [1.0, 0.0],
     ...             [0.0, 1.0]
     ...         ],
     ...     }
     ... )
+    >>> gru_cell = tf.keras.layers.GRUCell(16) # same units as MPNNConv
     >>> # Build a model with MPNNConv
-    >>> mpnn_conv_1 = molgraph.layers.MPNNConv(
-    ...     units=16, 
-    ...     update_mode='gru'       # lets use GRU updates instead (as per Gilmer et al. (2017))
-    ... )
-    >>> mpnn_conv_2 = molgraph.layers.MPNNConv(
-    ...     units=32,               # will be ignored as MPNNConv layer is passed to `tie_layer`
-    ...     update_mode='gru',      # will be ignored as MPNNConv layer is passed to `tie_layer`
-    ...     tie_layer=mpnn_conv_1
-    ... )
-    >>> mpnn_conv_3 = molgraph.layers.MPNNConv(
-    ...     units=16,               # will be ignored as MPNNConv layer is passed to `tie_layer`
-    ...     update_mode='gru',      # will be ignored as MPNNConv layer is passed to `tie_layer`
-    ...     tie_layer=mpnn_conv_1   # specifying mpnn_conv_2 would be equivalent
-    ... )
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     mpnn_conv_1,
-    ...     mpnn_conv_2,
-    ...     mpnn_conv_3,
+    ...     molgraph.layers.MPNNConv(16, update_fn=gru_cell),
+    ...     molgraph.layers.MPNNConv(16, update_fn=gru_cell)
     ... ])
     >>> gnn_model.output_shape
     (None, 16)
 
     Args:
         units (int, None):
             Number of output units.
-        use_edge_features (bool):
-            Whether or not to use edge features. Default to True.
-        tie_layer (molgraph.layers.message_passing.mpnn_conv.MPNNConv, None):
-            Pass the previous MPNNConv layer to perform weight tying. If None, weight tying
-            will not be performed (each layer has its own weights). Default to None.
-        update_mode (str):
-            Specify what type of update will be performed. Either of 'dense' or 'gru'.
-            If 'gru' is passed to MPNNConv layers, make sure weight tying is performed
-            (see 'tie_layer' argument above). Default to 'dense'.
+        update_mode (bool):
+            Specify what type of update will be performed. Either 'dense' or 'gru'. 
+            Default to 'gru'.
+        update_fn (tf.keras.layers.GRUCell, tf.keras.layers.Dense, None):
+            Optionally pass update function (GRUCell or Dense) for weight-tying 
+            of the update step (GRU step or Dense step). Default to None.
         self_projection (bool):
             Whether to apply self projection. Default to True.
         batch_norm: (bool):
             Whether to apply batch normalization to the output. Default to True.
         residual: (bool)
             Whether to add skip connection to the output. Default to True.
         dropout: (float, None):
@@ -193,17 +175,17 @@
         .. [#] https://arxiv.org/pdf/1704.01212.pdf
 
     """
 
     def __init__(
         self,
         units: Optional[int] = None,
-        use_edge_features: bool = True,
-        update_mode: str = 'dense',
-        tie_layer: Optional['MPNNConv'] = None,
+        update_mode: str = 'gru',
+        update_fn: Optional[Union[
+            keras.layers.GRUCell, keras.layers.Dense]] = None,
         self_projection: bool = True,
         batch_norm: bool = True,
         residual: bool = True,
         dropout: Optional[float] = None,
         update_activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = None,
         activation: Union[None, str, Callable[[tf.Tensor], tf.Tensor]] = 'relu',
         use_bias: bool = True,
@@ -213,123 +195,116 @@
         bias_regularizer: Optional[regularizers.Regularizer] = None,
         activity_regularizer: Optional[regularizers.Regularizer] = None,
         kernel_constraint: Optional[constraints.Constraint] = None,
         bias_constraint: Optional[constraints.Constraint] = None,
         **kwargs
     ):
         super().__init__(
-            units=units if not tie_layer else None,
+            units=units,
             batch_norm=batch_norm,
             residual=residual,
             dropout=dropout,
             activation=activation,
             use_bias=use_bias,
             kernel_initializer=kernel_initializer,
             bias_initializer=bias_initializer,
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs)
 
-        self.use_edge_features = use_edge_features
-        self.apply_self_projection = self_projection
-        self.update_activation = update_activation
+        self.update_fn = update_fn
         self.update_mode = update_mode.lower()
-        self.tie_layer = tie_layer 
+        self.apply_self_projection = self_projection
+        if update_activation is None:
+            if self.update_mode.startswith('gru'):
+                self.update_activation = 'tanh'
+            else:
+                self.update_activation = 'linear'
+        else:
+            self.update_activation = update_activation
 
     def subclass_build(
         self,
         node_feature_shape: tf.TensorShape,
         edge_feature_shape: Optional[tf.TensorShape] = None
     ) -> None:
      
-        if self.tie_layer:
-            if type(self) != type(self.tie_layer):
-                raise ValueError(
-                    f'`{self.tie_layer.name}` needs to be the same type as this layer (`{self.name}`)'
-                )
-            self.message_projection = getattr(self.tie_layer, 'message_projection', None)
-            if not self.message_projection:
-                raise ValueError(
-                    f'`{self.tie_layer.name}` is not built. Make sure `{self.tie_layer.name}` is ' +
-                    f'built before building this layer (`{self.name}`). `{self.tie_layer.name}` should ' + 
-                    f'come before this layer (`{self.name}`) in the sequence (model).'
-                )
-            self.update_projection = self.tie_layer.update_projection
-            self.self_projection = self.tie_layer.self_projection
-            
-        else:
-            self.message_projection = self.get_dense(self.units * self.units)
-            
-            if self.update_mode == 'dense':
-                self.update_projection = keras.layers.Dense(
-                    self.units, self.update_activation)
-            else:
-                self.update_projection = keras.layers.GRUCell(self.units)
-
-            if (
-                self.units != node_feature_shape[-1] and
-                not hasattr(self, 'node_resample')
-            ):
-                self.node_resample = self.get_dense(self.units)
+        self.message_projection = self.get_dense(self.units * self.units)
 
-            if self.apply_self_projection:
-                self.self_projection = self.get_dense(self.units)
+        if self.update_fn is None:
+            if self.update_mode.startswith('gru'):
+                common_kwargs = self.get_common_kwargs()
+                common_kwargs['kernel_initializer'] = 'glorot_uniform'
+                common_kwargs['recurrent_initializer'] = 'orthogonal'
+                common_kwargs.pop('activity_regularizer', None)
+                self.update_fn = tf.keras.layers.GRUCell(
+                    self.units, 
+                    activation=self.update_activation,
+                    **common_kwargs)
             else:
-                self.self_projection = None
+                self.update_fn = self.get_dense(
+                    self.units, self.update_activation)
+        if (
+            self.units != node_feature_shape[-1] and
+            not hasattr(self, 'node_resample')
+        ):
+            self.node_resample = self.get_dense(self.units)
+
+        if self.apply_self_projection:
+            self.self_projection = self.get_dense(self.units)
+        else:
+            self.self_projection = None
 
     def subclass_call(self, tensor: GraphTensor) -> GraphTensor:
 
         if hasattr(self, 'node_resample'):
             tensor = tensor.update({
                 'node_feature': self.node_resample(tensor.node_feature)})
 
         # MPNN requires edge features, if edge features do not exist,
         # we force edge features by initializing them as ones vector
-        if not hasattr(tensor, 'edge_feature') or not self.use_edge_features:
+        if not hasattr(tensor, 'edge_feature'):
             tensor = tensor.update({
                 'edge_feature': tf.ones(
                     shape=[tf.shape(tensor.edge_dst)[0], 1], dtype=tf.float32)})
 
         node_feature_aggregated = message_step(
             node_feature=tensor.node_feature,
             edge_feature=tensor.edge_feature,
             edge_dst=tensor.edge_dst,
             edge_src=tensor.edge_src,
             projection=self.message_projection)
 
         node_feature_update = update_step(
             node_feature=node_feature_aggregated,
             node_feature_prev=tensor.node_feature,
-            update_projection=self.update_projection,
+            update_projection=self.update_fn,
             self_projection=self.self_projection)
         
         return tensor.update({'node_feature': node_feature_update})
 
     def get_config(self):
         base_config = super().get_config()
         config = {
-            'use_edge_features': self.use_edge_features,
             'update_mode': self.update_mode,
-            'tie_layer': keras.layers.serialize(self.tie_layer),
+            'update_fn': tf.keras.layers.serialize(self.update_fn),
             'self_projection': self.apply_self_projection,
             'update_activation': self.update_activation
         }
         base_config.update(config)
         return base_config
 
 
 def update_step(
     node_feature: tf.Tensor, 
     node_feature_prev: tf.Tensor,
-    update_projection: Union[
-        keras.layers.Dense, keras.layers.GRUCell, keras.layers.LSTMCell
-    ],
+    update_projection: Union[keras.layers.GRUCell, keras.layers.Dense],
     self_projection: keras.layers.Dense,
 ) -> tf.Tensor:
     if self_projection:
         node_feature += self_projection(node_feature_prev)
     if isinstance(update_projection, keras.layers.Dense):
         node_feature = update_projection(
             tf.concat([node_feature_prev, node_feature], axis=1))
@@ -347,21 +322,21 @@
     edge_src: tf.Tensor,
     projection: keras.layers.Dense,
 ) -> tf.Tensor:
     '''Performs a message passing step.
 
     Args:
         node_feature (tf.Tensor):
-            Node features; field of GraphTensor.
+            Node features; component of GraphTensor.
         edge_feature (tf.Tensor):
-            Edge features; field of GraphTensor.
+            Edge features; component of GraphTensor.
         edge_dst (tf.Tensor):
-            Destination node indices; field of GraphTensor.
+            Destination node indices; component of GraphTensor.
         edge_src (tf.Tensor):
-            Source node indices; field of GraphTensor.
+            Source node indices; component of GraphTensor.
         projection (keras.layers.Dense):
             Dense layer that transforms edge features.
 
     Returns (tf.Tensor):
         Returns updated (aggregated) node features.
     '''
     output_units = int(math.sqrt(projection.units))
```

### Comparing `molgraph-0.3.6/molgraph/layers/ops.py` & `molgraph-0.3.8/molgraph/layers/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.3.8/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.3.8/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     ... )
     >>> model = tf.keras.Sequential([
     ...     tf.keras.layers.Input(type_spec=graph_tensor.unspecific_spec),
     ...     molgraph.layers.DotProductIncident()
     ... ])
     >>> model(graph_tensor)
     <tf.RaggedTensor [[4.0, 4.0], [9.0, 0.0, 9.0, 0.0, 0.0, 0.0]]>
+
+    Args:
+        apply_sigmoid (bool):
+            Whether to apply a sigmoid activaton on the edge scores. 
+            Default to False.
     '''
     def __init__(self, apply_sigmoid: bool = False, **kwargs):
         super().__init__(**kwargs)
         self._apply_sigmoid = apply_sigmoid
 
     def call(self, tensor: GraphTensor) -> GraphTensor:
         '''Defines the computation from inputs to outputs.
```

### Comparing `molgraph-0.3.6/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.3.8/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.3.8/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/masking.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/projection.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.3.8/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.3.8/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/readout/node_readout.py` & `molgraph-0.3.8/molgraph/layers/readout/node_readout.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,41 +37,41 @@
     ...             [0.0, 1.0]
     ...         ],
     ...     }
     ... )
     >>> # Build a DGIN model for binary classificaton
     >>> gnn_model = tf.keras.Sequential([
     ...     tf.keras.Input(type_spec=graph_tensor.unspecific_spec),
-    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' field
-    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' field
+    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' component
+    ...     molgraph.layers.EdgeConv(16),                           # will produce 'edge_state' component
     ...     molgraph.layers.NodeReadout(target='edge_state'),       # target='edge_state' is default
     ...     molgraph.layers.GINConv(32),
     ...     molgraph.layers.GINConv(32),
     ...     molgraph.layers.Readout(),
     ...     tf.keras.layers.Dense(1, activation='sigmoid')
     ... ])
     >>> gnn_model.output_shape
     (None, 1)
 
 
     Args:
         target (str):
-            Specifies which field to aggregate. Default to 'edge_state' which is the
-            field produced by ``molgraph.layers.EdgeConv``.
+            Specifies which component to aggregate. Default to 'edge_state' which is the
+            component produced by ``molgraph.layers.EdgeConv``.
         apply_transform (bool):
             Whether to perform a transformaton after the aggregation. Default to False.
         dense_kwargs (None, dict):
             Parameters to be passed to the dense layer in the transformation. Only relevant
             if ``apply_transform=True``. If None is passed, ``units`` is set to ``input_shape[-1]``
             and ``activation`` is set to ``relu``. Default to None.
     '''
     def __init__(
         self, 
         target: str = 'edge_state', 
-        apply_transform: bool = False,
+        apply_transform: bool = True,
         dense_kwargs: Optional[dict] = None,
         **kwargs
     ):
         super().__init__(**kwargs)
         self.target = target 
         self.apply_transform = apply_transform
         self.dense_kwargs = {} if dense_kwargs is None else dense_kwargs
```

### Comparing `molgraph-0.3.6/molgraph/layers/readout/segment_pool.py` & `molgraph-0.3.8/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/readout/set_gather.py` & `molgraph-0.3.8/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.3.8/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/losses/link_losses.py` & `molgraph-0.3.8/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/losses/masked_losses.py` & `molgraph-0.3.8/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/metrics/masked_metrics.py` & `molgraph-0.3.8/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/metrics/mean_relative_error.py` & `molgraph-0.3.8/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/models/dgin.py` & `molgraph-0.3.8/molgraph/models/dgin.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,15 @@
         tensor = tensor.update({'edge_feature': edge_feature})
         
         for _ in range(self.edge_message_steps):
             
             message = edge_message_step(
                 edge_feature=tensor.edge_feature,
                 edge_src=tensor.edge_src,
-                edge_dst=tensor.edge_dst,
-                graph_indicator=tensor.graph_indicator,
-                parallel_iterations=self.parallel_iterations)
+                edge_dst=tensor.edge_dst)
 
             edge_feature = self.activation(
                 self.update_projection(message) + edge_feature)
             
             if self.dropout is not None:
                 edge_feature = self.dropout(edge_feature)
```

### Comparing `molgraph-0.3.6/molgraph/models/dmpnn.py` & `molgraph-0.3.8/molgraph/models/dmpnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,15 @@
         tensor = tensor.update({'edge_feature': edge_feature})
         
         for _ in range(self.steps):
             
             message = edge_message_step(
                 edge_feature=tensor.edge_feature,
                 edge_src=tensor.edge_src,
-                edge_dst=tensor.edge_dst,
-                graph_indicator=tensor.graph_indicator,
-                parallel_iterations=self.parallel_iterations)
+                edge_dst=tensor.edge_dst)
     
             edge_feature = self.activation(
                 self.update_projection(message) + edge_feature)
             
             if self.dropout is not None:
                 edge_feature = self.dropout(edge_feature)
```

### Comparing `molgraph-0.3.6/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.3.8/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/models/interpretability/saliency.py` & `molgraph-0.3.8/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/models/mpnn.py` & `molgraph-0.3.8/molgraph/models/mpnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 class MPNN(keras.layers.Layer):
 
     '''Message passing neural network (MPNN) with weight tying.
 
     Implementation is based on Gilmer et al. (2017) [#]_. In contrast to
     ``MPNNConv``, which performs a single step of message passing, ``MPNN``
     performs n-steps of message passing. Furthermore, the weights are shared
-    between the message functions of the different steps. And the update
-    functions correspond to a single GRU.
+    by default between the message functions of the different steps. 
+    And the update functions correspond to a single GRU by default.
 
     **Example:**
 
     >>> # Obtain GraphTensor
     >>> graph_tensor = molgraph.GraphTensor(
     ...     data={
     ...         'edge_dst': [[0, 1], [0, 0, 1, 1, 2, 2]],
```

### Comparing `molgraph-0.3.6/molgraph/tensors/_graph_tensor.py` & `molgraph-0.3.8/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.3.8/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.3.6/molgraph/tensors/graph_tensor.py` & `molgraph-0.3.8/molgraph/tensors/graph_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -893,14 +893,23 @@
     return tf.range(start, stop, step)
 
 def _maybe_mark_used(assert_op):
     if hasattr(assert_op, 'mark_used'):
         assert_op.mark_used()
     return
 
+@tf.experimental.dispatch_for_api(tf.shape)
+def graph_tensor_tf_shape(
+    input: GraphTensor,
+    out_type=tf.dtypes.int32,
+    name=None
+):
+    return tf.shape(
+        input=input.node_feature, out_type=out_type, name=name)
+
 @tf.experimental.dispatch_for_api(tf.gather)
 def graph_tensor_gather(
     params: GraphTensor,
     indices,
     validate_indices=None,
     axis=None,
     batch_dims=0,
@@ -932,15 +941,19 @@
 
 @tf.experimental.dispatch_for_api(tf.concat)
 def graph_tensor_concat(
     values: List[GraphTensor],
     axis: int = 0,
     name: str = 'concat'
 ) -> GraphTensor:
-    'Concatenates list of graph tensors into a single graph tensor.'
+    '''Concatenates list of graph tensors into a single graph tensor.
+    
+    This is important for tf.keras.Model.predict, as it concatenates
+    the batches (of possibly `GraphTensor`s).
+    '''
 
     if axis is not None and axis != 0:
         raise ValueError(
             f'axis=0 is required for `{values[0].__class__.__name__}`s.')
 
     def fast_ragged_stack(component_data, dtype):
         row_lengths = [len(x) for x in component_data]
@@ -959,34 +972,46 @@
             'Found both nested ragged tensors and tensors of the `GraphTensor`s')
     else:
         # If first element is ragged, the rest is also ragged, and vice versa
         ragged = ragged[0]
 
     flat_sequence = tf.nest.map_structure(
         lambda x: tf.nest.flatten(x, expand_composites=True), values)
-
+    
     dtype = values[0]['edge_dst'].dtype
 
     if ragged:
         # Keep only values (resulting from tf.nest.flatten)
-        flat_sequence = [f[::2] for f in flat_sequence]
-
+        row_splits = [f[1::2] for f in flat_sequence]
+        flat_sequence = [f[0::2] for f in flat_sequence]
+        flat_sequence = tf.nest.map_structure(
+            lambda v, r: tf.RaggedTensor.from_row_splits(v, r),
+            flat_sequence, row_splits)
+        
     flat_sequence = list(zip(*flat_sequence))
-    flat_sequence_stacked = [
-        fast_ragged_stack(x, dtype) for x in flat_sequence
-    ]
+
+    if ragged:
+        flat_sequence_stacked = [
+            tf.concat(x, axis=0) for x in flat_sequence
+        ]
+    else:
+        flat_sequence_stacked = [
+            fast_ragged_stack(x, dtype) for x in flat_sequence
+        ]
+
     values = tf.nest.pack_sequence_as(structure, flat_sequence_stacked)
 
     values = GraphTensor(values)
 
     if ragged:
         return values
 
     return values.merge()
 
+
 @tf.experimental.dispatch_for_api(tf.matmul)
 def graph_tensor_matmul(
     a: GraphTensor,
     b,
     transpose_a=False,
     transpose_b=False,
     adjoint_a=False,
```

### Comparing `molgraph-0.3.6/molgraph.egg-info/SOURCES.txt` & `molgraph-0.3.8/molgraph.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -79,8 +79,17 @@
 molgraph/models/interpretability/activation_maps.py
 molgraph/models/interpretability/saliency.py
 molgraph/models/pretraining/__init__.py
 molgraph/models/pretraining/attribute_masking.py
 molgraph/tensors/__init__.py
 molgraph/tensors/_graph_tensor.py
 molgraph/tensors/graph_keras_tensor.py
-molgraph/tensors/graph_tensor.py
+molgraph/tensors/graph_tensor.py
+tests/test_chemistry.py
+tests/test_interpretability.py
+tests/test_layers.py
+tests/test_models.py
+tests/test_models_2.py
+tests/test_tensors.py
+tests/test_tensors_2.py
+tests/test_tensors_3.py
+tests/test_tensors_4.py
```

### Comparing `molgraph-0.3.6/setup.py` & `molgraph-0.3.8/setup.py`

 * *Files identical despite different names*

