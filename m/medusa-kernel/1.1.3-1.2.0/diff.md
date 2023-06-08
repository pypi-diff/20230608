# Comparing `tmp/medusa-kernel-1.1.3.tar.gz` & `tmp/medusa-kernel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medusa-kernel-1.1.3.tar", last modified: Fri Dec  9 12:28:25 2022, max compression
+gzip compressed data, was "medusa-kernel-1.2.0.tar", last modified: Thu Jun  8 10:18:31 2023, max compression
```

## Comparing `medusa-kernel-1.1.3.tar` & `medusa-kernel-1.2.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.399196 medusa-kernel-1.1.3/medusa/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/artifact_removal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.399196 medusa-kernel-1.1.3/medusa/bci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/bci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60846 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/bci/cvep_spellers.py
--rw-r--r--   0 runner    (1001) docker     (123)   106152 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/bci/erp_spellers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/bci/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    53652 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/bci/mi_paradigms.py
--rw-r--r--   0 runner    (1001) docker     (123)    40321 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/bci/nft_paradigms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/classification_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    67251 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.399196 medusa-kernel-1.1.3/medusa/connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20610 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/connectivity/amplitude_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/connectivity/phase_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    66724 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/deep_learning_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/emg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/epoching.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/frequency_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.403197 medusa-kernel-1.1.3/medusa/graph_theory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/assortativity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/betweeenness_centrality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/clustering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/degree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/eigen_centrality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/modularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/participation_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/path_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/surrogate_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/graph_theory/transitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.403197 medusa-kernel-1.1.3/medusa/local_activation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/local_activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   330752 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/local_activation/computeLZC.dll
--rw-r--r--   0 runner    (1001) docker     (123)    19618 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/local_activation/nonlinear_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/local_activation/spectral_parameteres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/local_activation/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.403197 medusa-kernel-1.1.3/medusa/meeg/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-05_2D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-05_3D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-10_2D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-10_3D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-20_2D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-20_3D.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    33507 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/meeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/meeg/meeg_montages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/nirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/notify_me.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/pearson_corr_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/performance_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/medusa/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/brain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/erp_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/generic_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    27632 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/mi_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/optimal_subplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/timeplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    20116 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/plots/topographic_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/signal_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/signal_orthogonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26109 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/spatial_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/tensorflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/medusa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/medusa_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2022-12-09 12:28:25.000000 medusa-kernel-1.1.3/medusa_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2022-12-09 12:28:25.000000 medusa-kernel-1.1.3/medusa_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 12:28:25.000000 medusa-kernel-1.1.3/medusa_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-09 12:28:25.000000 medusa-kernel-1.1.3/medusa_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-09 12:28:25.000000 medusa-kernel-1.1.3/medusa_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/tests/local_activation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/local_activation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:25.407197 medusa-kernel-1.1.3/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/plots/test_topographics_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/test_signal_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-09 12:28:13.000000 medusa-kernel-1.1.3/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.679426 medusa-kernel-1.2.0/medusa/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/artifact_removal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.679426 medusa-kernel-1.2.0/medusa/bci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60653 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/cvep_spellers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106155 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/erp_spellers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59073 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/mi_paradigms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38619 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/bci/nft_paradigms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/classification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67256 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.683426 medusa-kernel-1.2.0/medusa/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20650 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/connectivity/amplitude_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/connectivity/phase_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67167 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/deep_learning_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/emg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/epoching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/frequency_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.687425 medusa-kernel-1.2.0/medusa/graph_theory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/betweeenness_centrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/clustering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/degree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/eigen_centrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/modularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/participation_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/surrogate_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/graph_theory/transitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.687425 medusa-kernel-1.2.0/medusa/local_activation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   330752 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/computeLZC.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/nonlinear_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/spectral_parameteres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/local_activation/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.691425 medusa-kernel-1.2.0/medusa/meeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_2D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_3D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_2D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_3D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-20_2D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-20_3D.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/meeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/meeg/meeg_montages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/nirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/notify_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/performance_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.691425 medusa-kernel-1.2.0/medusa/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/brain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/erp_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/generic_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20860 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/head_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/mi_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/optimal_subplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21087 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/timeplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20211 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/plots/topographic_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/signal_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/signal_orthogonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34207 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/spatial_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/tensorflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/medusa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/medusa_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 10:18:31.000000 medusa-kernel-1.2.0/medusa_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/tests/local_activation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/local_activation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:31.695425 medusa-kernel-1.2.0/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/plots/test_topographics_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/test_signal_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 10:18:19.000000 medusa-kernel-1.2.0/tests/test_transforms.py
```

### Comparing `medusa-kernel-1.1.3/LICENSE` & `medusa-kernel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/PKG-INFO` & `medusa-kernel-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: medusa-kernel
-Version: 1.1.3
+Version: 1.2.0
 Summary: Advanced biosignal processing toolbox
 Home-page: https://medusabci.com/
 Author: Eduardo Santamaría-Vázquez, Víctor Martínez-Cagigal, Diego Marcos-Martínez, Víctor Rodríguez-González, Sergio Pérez-Velasco
 Author-email: support@medusabci.com
 License: CC Attribution-NonCommercial-NoDerivs 2.0
 Keywords: Signal,Biosignal,EEG,BCI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
+Provides-Extra: TF
 License-File: LICENSE
 
 # MEDUSA© Kernel
 
 MEDUSA© is a software ecosystem for the development of BCIs and neuroscience experiments. It has two independent components with dfferent goals: MEDUSA© Kernel and MEDUSA© Platform. 
 
 MEDUSA© Kernel is a Python package that contains readyto- use methods to analyze brain signals, including advanced signal processing, machine learning, deep learning, and miscellaneous high-level analyses. It also includes logical functions and classes to handle different biosignals, such as electroencephalography (EEG) and magnetoencephalography (MEG), save experimental data or implement standalone processing pipelines.
```

### Comparing `medusa-kernel-1.1.3/README.md` & `medusa-kernel-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/bci/cvep_spellers.py` & `medusa-kernel-1.2.0/medusa/bci/cvep_spellers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Created on Friday October 01 10:09:11 2021
-
+"""
 In this module you will find useful functions and classes to operate with data
 recorded using spellers based on code-modulated visual evoked potentials
 (c-VEP), which are widely used by the BCI community. Enjoy!
 
 @author: Víctor Martínez-Cagigal
 """
 import medusa as mds
@@ -263,18 +262,14 @@
                 'track_mode': 'append',
                 'parent': experiment_att_key
             }
         }
 
         if experiment_mode == 'train':
             default_track_attributes_train = {
-                'cvep_labels': {
-                    'track_mode': 'concatenate',
-                    'parent': experiment_att_key
-                },
                 'spell_target': {
                     'track_mode': 'append',
                     'parent': experiment_att_key
                 }
             }
             default_track_attributes = {
                 **default_track_attributes,
```

### Comparing `medusa-kernel-1.1.3/medusa/bci/erp_spellers.py` & `medusa-kernel-1.2.0/medusa/bci/erp_spellers.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             entity of the paradigm and only one can be used in each trial.
             The units are smaller entities that are used in multi-level
             paradigms, such as the Hex-O-spell (HOS) paradigm [1]. In this
             case, each level can use a different unit, affecting the selected
             command for the trial. For instance, in the HOS paradigm,
             you should define 1 matrix with 7 units, one for the initial menu
             and 6 for the second level of each command (letters).
-            Importantly, commands must be univocally defined in each matrix.
+            Importantly, commands must be unequivocally defined in each matrix.
             Therefore, units cannot share command identifiers. Then, the groups
             describe aggregations of commands that are highlighted at the
             same time. For instance, the row-column paradigm (RCP) [2]
             has 2 groups of commands (i.e., rows and columns), whereas the
             HOS has only 1 (i.e., each command is highlighted individually).
             Finally, batches contain the commands IDs defined in each group.
             In an RCP matrix of 6x6, each of the 2 groups has 6 batches,
```

### Comparing `medusa-kernel-1.1.3/medusa/bci/metrics.py` & `medusa-kernel-1.2.0/medusa/bci/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-""" Last edit: Víctor Martínez-Cagigal (07 Dec 2021) """
-
 import numpy as np
 
 
 def itr(accuracy, n_commands, selections_per_min):
     """
     Calculates the information transfer rate (ITR) in bits/min. This metric is
     widely used to assess the performance of a BCI. However, it has serious
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medusa-kernel-1.1.3/medusa/bci/mi_paradigms.py` & `medusa-kernel-1.2.0/medusa/bci/mi_paradigms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-"""Created on Monday February 14 09:27:14 2022
-
+"""
 In this module you will find useful functions and classes to operate with data
 recorded using motor imagery paradigms, which are widely used by the BCI
 community. Enjoy!
 
-@author: Sergio Pérez-Velasco
+@author: Sergio Pérez-Velasco & Víctor Martínez-Cagigal
 """
 # Built-in imports
 import copy, warnings
 from abc import abstractmethod
 
 # External imports
 import numpy as np
@@ -19,15 +18,15 @@
 # Medusa imports
 from medusa import IIRFilter, car
 from medusa.epoching import normalize_epochs
 from medusa import get_epochs_of_events, resample_epochs
 from medusa import components
 from medusa import meeg
 from medusa.spatial_filtering import CSP, LaplacianFilter
-
+from medusa import classification_utils as cu
 
 class MIData(components.ExperimentData):
     # TODO: Check everything
 
     """Class with the necessary attributes to define motor imagery (MI)
     experiments. It provides compatibility with high-level functions for this
     MI paradigms in BCI module.
@@ -109,17 +108,17 @@
     def to_serializable_obj(self):
         rec_dict = self.__dict__
         for key in rec_dict.keys():
             if type(rec_dict[key]) == np.ndarray:
                 rec_dict[key] = rec_dict[key].tolist()
         return rec_dict
 
-    @staticmethod
-    def from_serializable_obj(dict_data):
-        return MIData(**dict_data)
+    @classmethod
+    def from_serializable_obj(cls, dict_data):
+        return cls(**dict_data)
 
 
 class MIDataset(components.Dataset):
     """This class inherits from medusa.data_structures.Dataset, increasing
     its functionality for datasets with data from MI experiments. It
     provides common ground for the rest of functions in the module.
     """
@@ -179,15 +178,14 @@
         # Check errors
         if experiment_mode is not None:
             if experiment_mode not in ('train', 'test', 'guided test'):
                 raise ValueError('Parameter experiment_mode must be '
                                  '{train|test|guided test|None}')
 
         # Default track attributes
-        # TODO: esto no va a funcionar con MIDataOld
         default_track_attributes = {
             'subject_id': {
                 'track_mode': 'append',
                 'parent': None
             },
             'onsets': {
                 'track_mode': 'concatenate',
@@ -334,15 +332,15 @@
 
 class StandardPreprocessing(components.ProcessingMethod):
     """Just the common preprocessing applied in MI-based BCI. Simple,
     quick and effective: frequency IIR filter followed by common average
     reference (CAR) spatial filter.
     """
 
-    def __init__(self, order=5, cutoff=[0.05, 63], btype='bandpass',
+    def __init__(self, order=5, cutoff=[8, 30], btype='bandpass',
                  temp_filt_method='sosfiltfilt'):
         super().__init__(fit_transform_signal=['signal'],
                          fit_transform_dataset=['dataset'])
         # Parameters
         self.order = order
         self.cutoff = cutoff
         self.btype = btype
@@ -377,14 +375,37 @@
         signal: np.array or list
             Signal to transform. Shape [n_samples x n_channels]
         """
         signal = self.iir_filter.transform(signal)
         signal = car(signal)
         return signal
 
+    def transform_dataset(self, dataset: MIDataset, show_progress_bar=True,
+                          **kwargs):
+        """Transforms an MIDataset applying IIR filtering and CAR sequentially
+
+        Parameters
+        ----------
+        signal: np.array or list
+            Signal to transform. Shape [n_samples x n_channels]
+        """
+        pbar = None
+        if show_progress_bar:
+            pbar = tqdm(total=len(dataset.recordings),
+                        desc='Preprocessing')
+        for rec in dataset.recordings:
+            eeg = getattr(rec, dataset.biosignal_att_key)
+            eeg.signal = self.transform_signal(eeg.signal)
+            setattr(rec, dataset.biosignal_att_key, eeg)
+            if show_progress_bar:
+                pbar.update(1)
+        if show_progress_bar:
+            pbar.close()
+        return dataset
+
     def fit_transform_signal(self, signal, fs):
         """Fits the IIR filter and transforms an EEG signal applying IIR
         filtering and CAR sequentially
 
         Parameters
         ----------
         signal: np.array or list
@@ -424,200 +445,216 @@
                 pbar.update(1)
         if show_progress_bar:
             pbar.close()
         return dataset
 
 
 class StandardFeatureExtraction(components.ProcessingMethod):
-    """Standard feature extraction method for MI-based spellers. Basically,
+    """
+    Standard feature extraction method for MI-based spellers. Basically,
     it gets the raw epoch for each MI event.
     """
 
-    def __init__(self, w_epoch_t=(0, 3000), target_fs=128,
-                 baseline_mode='trial',
-                 w_baseline_t=(-1500, -500), norm='z',
-                 concatenate_channels=False, safe_copy=True):
-        """Class constructor
+    def __init__(self, safe_copy=True):
+        """
+        Class constructor. All parameters except "safe_copy" must be specified
+        in each method.
 
-        w_epoch_t : list
-            Temporal window in ms for each epoch relative to the event onset
-            (e.g., [0, 3000])
-        target_fs : float of None
-            Target sample rate of each epoch. If None, all the recordings must
-            have the same sample rate, so it is strongly recommended to set this
-            parameter to a suitable value to avoid problems and save time
-        baseline_mode : {'run', 'trial', None}
-            If "run" selected it will use the w_baseline_t of the beginning of
-            each run.
-            If "trial" selected it will use the w_baseline_t previous to each
-            epoch extracted.
-            If None it will not perform the baseline extraction.
-        w_baseline_t : list, np.ndarray or "auto"
-            Temporal window in ms to be used for baseline normalization.
-            If baseline_mode = "run" it will use the temporal window since start
-            of trial.
-            If baseline_mode = "trial", for each epoch it will use the time
-            relative to the event onset (e.g., [-1500, -500]).
-            If "auto" selected:
-                If baseline_mode = "run" will use the time between the
-                MedusaData.experiment.start and MedusaData.experiment.calibration
-                information stored in the run.
-                If baseline_mode = "trial" will use the time between
-                [-1500,-500]ms takes the baseline from -1500ms to -500ms before
-                each onset (0 ms represents the onset).
-                If baseline_mode = None it will not be used.
-        norm : str {'z'|'dc'}
-            Type of baseline normalization. Set to 'z' for Z-score normalization
-            or 'dc' for DC normalization
-        concatenate_channels : bool
-            This parameter controls the shape of the feature array. If True, all
-            channels will be concatenated, returning an array of shape [n_events
-            x (samples x channels)]. If false, the array will have shape
-            [n_events x samples x channels]
+        Parameters
+        -----------
         safe_copy : bool
             Makes a safe copy of the signal to avoid changing the original
-            samples due to references
+            samples due to references.
         """
         super().__init__(transform_signal=['x'],
                          transform_dataset=['x', 'x_info'])
-        self.w_epoch_t = w_epoch_t
-        self.target_fs = target_fs
-        self.baseline_mode = baseline_mode
-        self.w_baseline_t = w_baseline_t
-        self.norm = norm
-        self.concatenate_channels = concatenate_channels
         self.safe_copy = safe_copy
 
-    def transform_signal(self, times, signal, fs, onsets,
-                         w_epoch_t = None):
-        """Function to extract MI features from raw signal. It returns a 3D
-        feature array with shape [n_events x n_samples x n_channels]. This
-        function does not track any other attributes. Use for online processing
-        and custom higher level functions.
+    def transform_signal(self, times, signal, fs, onsets, w_epoch_t=(0, 3000),
+                         baseline_mode="trial", w_baseline_t=(-1500, -500),
+                         norm='z', target_fs=128, concatenate_channels=False,
+                         **kwargs):
+        """
+        Method to extract epochs from an individual signal.
 
         Parameters
-        ----------
-        times : list or numpy.ndarray
-                1D numpy array [n_samples]. Timestamps of each sample. If they
-                are not available, generate them artificially. Nevertheless,
-                all signals and events must have the same temporal origin
-        signal : list or numpy.ndarray
-            2D numpy array [n_samples x n_channels]. EEG samples (the units
-            should be defined using kwargs)
-        fs : int or float
-            Sample rate of the recording.
-        onsets : list or numpy.ndarray [n_events x 1]
-                Timestamp of each event
+        -----------------
+        times : ndarray (n_samples,)
+            Timestamp array
+        signal: ndarray (n_samples x n_channels)
+            Signal data.
+        fs : int
+            Sampling frequency.
+        onsets: ndarray (n_trials,)
+            Timestamps for the MI event onsets.
+        w_epoch_t : list, tuple, or ndarray
+            Temporal window in ms for each epoch relative to the event onset
+            (e.g., [0, 3000])
+        baseline_mode : basestring {'run', 'trial', None}
+            If "run", the baseline will be extracted from the very beginning
+            of the run (i.e., the first samples of the signal).
+            If "trial" (default), the baseline will be extracted for each
+            trial relative to the onset.
+            If None, no baseline extraction will be performed.
+        w_baseline_t : list, tuple, or ndarray
+            Temporal window in ms to be used for baseline normalization.
+            If baseline_mode = "run", the window is relative to the start of
+            the signal.
+            If baseline_mode = "trial", the window is relative to each trial
+            onset (e.g., [-1500, -500]).
+        norm : str {'z'|'dc'}
+            Type of baseline normalization. Set to 'z' for Z-score
+            normalization (subtract the mean and divide by the std),
+            or 'dc' for DC normalization (subtract the mean).
+        target_fs : float of None
+            Target sample rate of each epoch. If None, no resampling will be
+            applied. Please note that, in this case, all the recordings must
+            have the same sample rate.
+        concatenate_channels : bool
+            This parameter controls the shape of the feature array. If True, all
+            channels will be concatenated, returning an array of shape [n_events
+            x (samples x channels)]. If false, the array will have shape
+            [n_events x samples x channels].
 
         Returns
-        -------
-        features : np.ndarray [n_events x n_samples x n_channels]
-            Feature array with the epochs of signal
+        -----------
+        features : ndarray
+            MI epochs extracted with shape [n_events x samples x channels], or
+            [n_events x (samples x channels)] if concatenate_channels == True.
         """
-        if w_epoch_t is None:
-            w_epoch_t = self.w_epoch_t
         # Avoid changes in the original signal (this may not be necessary)
         if self.safe_copy:
             signal = signal.copy()
+
         # Baseline options
-        norm = self.norm
-        assert self.baseline_mode in ('run', 'trial', None), \
+        if baseline_mode == "sliding":
+            baseline_mode = "trial"
+        assert baseline_mode in ('run', 'trial', None), \
             ValueError('Parameter baseline_mode must be {"run", "trial", None}')
-        if self.baseline_mode is None:
-            assert self.w_baseline_t is None, 'If baseline_mode is None, ' \
-                                              'parameter w_baseline_t must be ' \
-                                              'None'
-            w_baseline_trial_t = None
-        elif self.baseline_mode == 'trial':
-            if self.w_baseline_t == 'auto':
-                w_baseline_trial_t = w_epoch_t
-            else:
-                w_baseline_trial_t = self.w_baseline_t
-        elif self.baseline_mode == 'run':
+        if baseline_mode in ('run', None):
+            w_baseline_t = None
             norm = None
-            w_baseline_trial_t = None
 
         # Extract features
-        features = get_epochs_of_events(timestamps=times, signal=signal,
-                                        onsets=onsets, fs=fs,
-                                        w_epoch_t=w_epoch_t,
-                                        w_baseline_t=w_baseline_trial_t,
-                                        norm=norm)
-
-        if self.baseline_mode == "run":
-            if self.w_baseline_t == 'auto':
-                norm_epoch_t = [0, 5000]
-            else:
-                norm_epoch_t = self.w_baseline_t
-            norm_epoch_s = np.array(norm_epoch_t * fs / 1000, dtype=int)
-            norm_epoch = np.expand_dims(signal[norm_epoch_s], axis=0)
+        features = get_epochs_of_events(
+            timestamps=times, signal=signal, onsets=onsets, fs=fs,
+            w_epoch_t=w_epoch_t,
+            w_baseline_t=w_baseline_t, norm=norm
+        )
+
+        # Common baseline for the entire run
+        if baseline_mode == "run":
+            # Here baseline is taken relative to the start of the signal
+            norm_epoch_s = np.array(w_baseline_t * fs / 1000, dtype=int)
+            norm_epoch = np.expand_dims(signal[norm_epoch_s, :], axis=0)
             features = normalize_epochs(features, norm_epochs=norm_epoch,
                                         norm=self.norm)
-        # Resample each epoch to the target frequency
-        if self.target_fs is not None:
-            if self.target_fs > fs:
+
+        # Apply resampling if required
+        if target_fs is not None:
+            if target_fs > fs:
                 raise warnings.warn('Target fs is greater than data fs')
-            features = resample_epochs(features,
-                                       self.w_epoch_t,
-                                       self.target_fs)
-        # Reshape epochs and concatenate the channels
-        if self.concatenate_channels:
-            features = np.squeeze(features.reshape((features.shape[0],
-                                                    features.shape[1] *
-                                                    features.shape[2], 1)))
+            features = resample_epochs(features, w_epoch_t, target_fs)
+
+        # Channel concatenation if desired
+        if concatenate_channels:
+            features = np.squeeze(features.reshape(
+                (features.shape[0], features.shape[1] * features.shape[2], 1)))
+
         return features
 
     def transform_dataset(self, dataset, show_progress_bar=True,
-                          continuous=False):
-        #TODO: Review with modifications of Eduardo in erp_spellers (SERGIO)
-        """High level function to easily extract features from EEG recordings
+                          w_epoch_t=(0, 3000), baseline_mode="trial",
+                          w_baseline_t=(-1500, -500), norm='z',
+                          target_fs=128, concatenate_channels=False,
+                          sliding_w_lims_t=None, sliding_t_step=None,
+                          sliding_win_len=None, **kwargs):
+        """
+        Method to extract epochs from an entire MIDataset
+
+        High level function to easily extract features from EEG recordings
         and save useful info for later processing. Nevertheless, the provided
         functionality has several limitations and it will not be suitable for
         all cases and processing pipelines. If it does not fit your needs,
         create a custom function iterating the recordings and using
         extract_erp_features, a much more low-level and general function. This
         function does not apply any preprocessing to the signals, this must
-        be done before
+        be done before.
+
+        Most parameters are shared with
+        StandardFeatureExtraction.transform_signal() method, check it for
+        more information. Only the new parameters or those that behave
+        differently than the aforementioned method are detailed below. These
+        new parameters are related to a continuous extraction of epochs using a
+        sliding window between a desired epoch range, instead of extracting only
+        one epoch for each onset.
 
         Parameters
         ----------
         dataset: MIDataset
-            List of data_structures.Recordings or data_structures.Dataset. If this
-            parameter is a list of recordings, the consistency of the dataset will
-            be checked. Otherwise, if the parameter is a dataset, this function
-            assumes that the consistency is already checked
+            MIDataset instance containing the MIData recordings.
         show_progress_bar: bool
-            Show progress bar
+            Boolean to show (or not) the progress bar info.
+        sliding_w_lims_t: list, tuple, ndarray, or None
+            2D window that indicates the range (start, end) for the sliding
+            window approach. If None, no sliding window would be applied.
+            This parameter delimits the number of windows to be extracted for
+            each onset, so none of them can fall outside the range (excluding
+            baseline).
+        sliding_t_step: int, None
+            Step in samples that is used to separate the sliding windows. If
+            None, no sliding window would be applied.
+        sliding_win_len: int, None
+            Length in samples of the sliding windows. Please note that the
+            w_epoch_t parameter would not be used if the sliding window approach
+            is used. If None, no sliding window would be applied.
+        baseline_mode : {'run', 'trial', None, 'sliding'}
+            The baseline_mode has an additional feature when sliding window is
+            used:
+                - "run": common baseline extracted from the start of the run.
+                - "trial": common baseline for the trial, i.e., all the windows
+                that belongs to an onset; extracted relative to the onset.
+                - None: no baseline.
+                - "sliding": baseline is applied to each sliding window,
+                and it is relative to the start of each sliding window.
 
         Returns
         -------
         features : numpy.ndarray
-            Array with the biosignal samples arranged in epochs
+            Array with the biosignal samples arranged in epochs.
         track_info : dict
-            Dictionary with tracked information across all recordings
-
+            Dictionary with tracked information across all recordings.
         """
+
+        # Continuous settings
+        use_continuous = False
+        if sliding_w_lims_t is not None or sliding_t_step is not None or \
+                sliding_win_len is not None:
+            assert sliding_w_lims_t is not None and sliding_t_step is not \
+                   None and sliding_win_len is not None, \
+                ValueError("All these three parameters {sliding_w_lims_t, "
+                           "sliding_t_step, sliding_win_len} must be "
+                           "specified to use sliding windows. If not desired, "
+                           "then put all three to None. Aborting.")
+            use_continuous = True
+
         # Avoid changes in the original recordings (this may not be necessary)
         if self.safe_copy:
             dataset = copy.deepcopy(dataset)
+
         # Avoid consistency problems
-        if dataset.fs is None and self.target_fs is None:
+        if dataset.fs is None and target_fs is None:
             raise ValueError('The consistency of the features is not assured '
                              'since dataset.fs and target_fs are both None. '
                              'Specify one of these parameters')
 
         # Additional track attributes
         track_attributes = dataset.track_attributes
-        # track_attributes['run_idx'] = {
-        #     'track_mode': 'concatenate',
-        #     'parent': dataset.experiment_att_key
-        # }
 
         # Initialization
-        features = None
         track_info = dict()
         for key, value in track_attributes.items():
             if value['track_mode'] == 'append':
                 track_info[key] = list()
             elif value['track_mode'] == 'concatenate':
                 track_info[key] = None
             else:
@@ -626,139 +663,126 @@
         # Init progress bar
         pbar = None
         if show_progress_bar:
             pbar = tqdm(total=len(dataset.recordings),
                         desc='Extracting features')
 
         # Compute features
+        features = None
         for run_counter, rec in enumerate(dataset.recordings):
             # Extract recording experiment and biosignal
             rec_exp = getattr(rec, dataset.experiment_att_key)
             rec_sig = getattr(rec, dataset.biosignal_att_key)
 
-            # Get features
-            # Get features
-            list_w_epoch_t = list()
-            if not continuous:
-                list_w_epoch_t.append(self.w_epoch_t)
-            if continuous:
-                start = self.w_epoch_t - np.diff(self.w_epoch_t) / 2
-                stop = rec_exp.w_trial_t[1] - self.w_epoch_t[1]
-                steps_0 = np.arange(start=start[0], stop=stop + 1, step=250,
-                                    dtype=int)
-                steps_1 = np.arange(start=start[1], stop=rec_exp.w_trial_t[
-                                                             1] + 1, step=250,
-                                    dtype=int)
-                for i in range(len(steps_0)):
-                    list_w_epoch_t.append([steps_0[i], steps_1[i]])
+            # If continuous: get different windows relative to the onsets
+            if use_continuous:
+                # Get windows
+                start, stop = sliding_w_lims_t      # respect to each onset
+                step_array = np.arange(0, (stop - start - sliding_win_len) //
+                                       sliding_t_step + 1)
+                win_0 = start + step_array * sliding_t_step
+                win_1 = win_0 + sliding_win_len
+                list_w_epoch_t = [(w0, w1) for w0, w1 in zip(win_0, win_1)
+                                  if w1 <= stop]
+
+                # Get baselines
+                if baseline_mode == "sliding":
+                    bas_0 = start + w_baseline_t[0] + step_array * sliding_t_step
+                    bas_1 = start + w_baseline_t[1] + step_array * sliding_t_step
+                    list_w_bas_t = [(w0, w1) for w0, w1 in zip(bas_0, bas_1)]
+                elif baseline_mode == "trial":
+                    bas_0 = start + w_baseline_t[0] + step_array * 0
+                    bas_1 = start + w_baseline_t[1] + step_array * 0
+                    list_w_bas_t = [(w0, w1) for w0, w1 in zip(bas_0, bas_1)]
+                elif baseline_mode == "run":
+                    list_w_bas_t = [w_baseline_t for _ in range(len(
+                        list_w_epoch_t))]
+                else:
+                    list_w_bas_t = [None for _ in range(len(list_w_epoch_t))]
+
+                # Modify the mi_labels
+                if hasattr(rec.midata, "mi_labels"):
+                    rec.midata.mi_labels = \
+                        np.tile(rec.midata.mi_labels,
+                                (len(list_w_epoch_t), 1)).flatten()
+            else:
+                list_w_epoch_t = [w_epoch_t]
+                list_w_bas_t = [w_baseline_t]
 
-            for w_epoch_t in list_w_epoch_t:
+            # For each window
+            for i in range(len(list_w_epoch_t)):
 
+                # Get features
                 rec_feat = self.transform_signal(
                     times=rec_sig.times,
                     signal=rec_sig.signal,
                     fs=rec_sig.fs,
                     onsets=rec_exp.onsets,
-                    w_epoch_t=w_epoch_t
-                    # ,
-                    # calibration_t=rec_exp.calibration_t
+                    w_epoch_t=list_w_epoch_t[i],
+                    w_baseline_t=list_w_bas_t[i],
+                    baseline_mode=baseline_mode,
+                    norm=norm,
+                    target_fs=target_fs,
+                    concatenate_channels=concatenate_channels
                 )
-
                 features = np.concatenate((features, rec_feat), axis=0) \
                     if features is not None else rec_feat
 
-                # Special attributes that need tracking across runs to assure the
-                # consistency of the dataset
-                # rec_exp.run_idx = run_counter * np.ones_like(rec_exp.trial_idx)
-
-                # Track experiment info
-                for key, value in track_attributes.items():
-                    if value['parent'] is None:
-                        parent = rec
-                    else:
-                        parent = rec
-                        for p in value['parent'].split('.'):
-                            parent = getattr(parent, p)
-                    att = getattr(parent, key)
-                    if value['track_mode'] == 'append':
-                        track_info[key].append(att)
-                    elif value['track_mode'] == 'concatenate':
-                        track_info[key] = np.concatenate(
-                            (track_info[key], att), axis=0
-                        ) if track_info[key] is not None else att
-                    else:
-                        raise ValueError('Unknown track mode')
-
+            # Track experiment info
+            for key, value in track_attributes.items():
+                if value['parent'] is None:
+                    parent = rec
+                else:
+                    parent = rec
+                    for p in value['parent'].split('.'):
+                        parent = getattr(parent, p)
+                att = getattr(parent, key)
+                if value['track_mode'] == 'append':
+                    track_info[key].append(att)
+                elif value['track_mode'] == 'concatenate':
+                    track_info[key] = np.concatenate(
+                        (track_info[key], att), axis=0
+                    ) if track_info[key] is not None else att
+                else:
+                    raise ValueError('Unknown track mode')
             if show_progress_bar:
                 pbar.update(1)
         if show_progress_bar:
             pbar.close()
 
         return features, track_info
 
 
-class CSPFeatureExtraction(StandardFeatureExtraction):
+class CSPFeatureExtraction(components.ProcessingMethod):
     """Common Spatial Patterns (CSP) feature extraction method for MI-based
     spellers.
 
     Processing pipeline:
     - Use of StandardFeatureExtraction to get the raw epoch of each MI event.
     - Extract CSP features of those MI events.
+    - Log-var features
     """
 
-    def __init__(self, n_filters=4, w_epoch_t=(500, 4000), target_fs=None,
-                 baseline_mode='trial',
-                 w_baseline_t=(-1500, -500), norm='z',
-                 concatenate_channels=False, safe_copy=True, **kwargs):
-        """Class constructor
+    def __init__(self, n_filters=4, safe_copy=True,
+                 normalize_log_vars=True, **kwargs):
+        """Class constructor.
 
-        n_filter : int or None
+        n_filters : int or None
             Number of most discriminant CSP filters to decompose the signal
             into (must be less or equal to the number of channels in your
-            signal).
-            If int it will return that number of filters.
-            If None it will return the all calculated filters.
-        w_epoch_t : list
-            Temporal window in ms for each epoch relative to the event onset
-            (e.g., [0, 3000])
-        target_fs : float of None
-            Target sample rate of each epoch. If None, all the recordings must
-            have the same sample rate, so it is strongly recommended to set this
-            parameter to a suitable value to avoid problems and save time
-        baseline_mode : {'run', 'trial', None}
-            If "run" selected it will use the w_baseline_t of the beginning of
-            each run.
-            If "trial" selected it will use the w_baseline_t previous to each
-            epoch extracted.
-            If None it will not perform the baseline extraction.
-        w_baseline_t : list, np.ndarray or "auto"
-            Temporal window in ms to be used for baseline normalization.
-            If baseline_mode = "run" it will use the temporal window since start
-            of trial.
-            If baseline_mode = "trial", for each epoch it will use the time
-            relative to the event onset (e.g., [0, 3000]).
-            If "auto" selected:
-                If baseline_mode = "run" will use the time between the
-                MedusaData.experiment.start and MedusaData.experiment.calibration
-                information stored in the run.
-                If baseline_mode = "trial" will use the time between
-                [-1500,-500]ms takes the baseline from -1500ms to -500ms before
-                each onset (0 ms represents the onset).
-                If baseline_mode = None it will not be used.
-        norm : str {'z'|'dc'}
-            Type of baseline normalization. Set to 'z' for Z-score normalization
-            or 'dc' for DC normalization
-        concatenate_channels : bool
-            This parameter controls the shape of the feature array. If True, all
-            channels will be concatenated, returning an array of shape [n_events
-            x (samples x channels)]. If false, the array will have shape
-            [n_events x samples x channels]
+            signal). If None, all filters will be used.
         safe_copy : bool
             Makes a safe copy of the signal to avoid changing the original
             samples due to references
+        normalize_log_vars : bool
+            If true, log-var features are normalized.
+        **kwargs : dict()
+            Parameters from StandardFeatureExtraction are not detailed here.
+            Please refer to the StandardFeatureExtraction documentation to know
+            more, as they are passed through kwargs.
 
         After using the function self.fit(), the attributes are computed:
 
         Attributes
         ----------
         CSP : CSP class with attributes filters, eigenvalues, patterns and
             methods fit and project.
@@ -766,106 +790,105 @@
             filters : {(…, M, M) numpy.ndarray, (…, M, M) matrix}
                 Mixing matrix (spatial filters are stored in columns).
             eigenvalues : (…, M) numpy.ndarray
                 Eigenvalues of w.
             patterns : numpy.ndarray
                 De-mixing matrix (activation patterns are stored in columns).
         """
-        super().__init__(w_epoch_t=w_epoch_t, target_fs=target_fs,
-                         baseline_mode=baseline_mode,
-                         w_baseline_t=w_baseline_t, norm=norm,
-                         concatenate_channels=concatenate_channels,
-                         safe_copy=safe_copy)
-        self.CSP = CSP(n_filters=n_filters)
-
-    def fit(self, X, y):
-        """Train Common Spatial Patterns (CSP) filters
-
-        Train Common Spatial Patterns (CSP) filters with support to >2
-        classes based on support multiclass CSP by means of approximate
-        joint diagonalization. In this case, the spatial filter selection
-        is achieved according to [1].
-
-        Adapted from http://github.com/alexandrebarachant/pyRiemann
-
-        Parameters
-        ----------
-        X : numpy.ndarray, [n_trials, samples, channels]
-            Epoched data of shape (n_trials, samples, channels)
+        self.normalize_log_vars = normalize_log_vars
+        self.feature_extractor = StandardFeatureExtraction(safe_copy=safe_copy)
+        self.CSP = CSP(n_filters=n_filters, selection="extremes")
+
+    def fit_signal(self, labels, times, signal, fs, onsets, **kwargs):
+        # Standard extraction: just epoching (epochs x samples x channels)
+        features = self.feature_extractor.transform_signal(
+            times=times, signal=signal, fs=fs, onsets=onsets, **kwargs
+        )
 
-        y : numpy.ndarray, [n_trials,]
-            Labels for epoched data of shape (n_trials,)
+        # Fit the CSP filter
+        self.CSP.fit(X=features, y=labels)
+        return features
 
-        References
-        ----------
-        [1] Grosse-Wentrup, Moritz, and Martin Buss. "Multiclass common
-        spatial patterns and information theoretic feature extraction."
-        Biomedical Engineering, IEEE Transactions on 55, no. 8 (2008):
-        1991-2000.
-        """
-        self.CSP.fit(X=X, y=y)
-
-    def project(self, times, signal, fs, onsets):
-        """Function to extract MI features from raw signal. It returns a 3D
-        feature array with shape [n_events x n_samples x n_channels]. This
-        function does not track any other attributes. Use for online processing
-        and custom higher level functions.
+    def fit_dataset(self, dataset, show_progress_bar=True, **kwargs):
+        # Standard extraction: just epoching (epochs x samples x channels)
+        features, track_info = self.feature_extractor.transform_dataset(
+            dataset=dataset, show_progress_bar=show_progress_bar, **kwargs
+        )
 
-        Parameters
-        ----------
-        times : list or numpy.ndarray
-                1D numpy array [n_samples]. Timestamps of each sample. If they
-                are not available, generate them artificially. Nevertheless,
-                all signals and events must have the same temporal origin
-        signal : list or numpy.ndarray
-            2D numpy array [n_samples x n_channels]. EEG samples (the units
-            should be defined using kwargs)
-        fs : int or float
-            Sample rate of the recording.
-        onsets : list or numpy.ndarray [n_events x 1]
-                Timestamp of each event
+        # Fit the CSP filter
+        self.CSP.fit(X=features, y=track_info['mi_labels'])
+        return features, track_info
 
-        Returns
-        -------
-        features : numpy.ndarray [n_events x n_samples x n_channels]
-            Feature array with the epochs of signal projected in the CSP space
-        """
-        features = super().transform_signal(times, signal, fs, onsets)
+    def transform_signal(self, times, signal, fs, onsets, **kwargs):
+        if not self.CSP.is_fitted:
+            raise ValueError('CSPFeatureExtraction must be fitted before '
+                             'predict!')
+
+        # Standard extraction: just epoching (epochs x samples x channels)
+        features = self.feature_extractor.transform_signal(
+            times=times, signal=signal, fs=fs, onsets=onsets, **kwargs
+        )
 
-        features = self.CSP.project(X=features)
-        return features
+        # Project using CSP
+        projection = self.CSP.project(X=features) # trials x samples x projects
 
-    def extract_log_var_features(self, X):
-        """This method computes the standard motor imagery log-variance features
-        given the CSP .
+        # Log-variance features across samples
+        log_var = self._get_log_vars(projection, self.normalize_log_vars)
+        return log_var
+
+    def transform_dataset(self, dataset, show_progress_bar=True, **kwargs):
+        if not self.CSP.is_fitted:
+            raise ValueError('CSPFeatureExtraction must be fitted before '
+                             'predict!')
+
+        # Standard extraction: just epoching (epochs x samples x channels)
+        features, track_info = self.feature_extractor.transform_dataset(
+            dataset=dataset, show_progress_bar=show_progress_bar, **kwargs
+        )
 
-        Parameters
-        ----------
-        X : numpy.ndarray, [n_trials, samples, channels]
-            Epoched data of shape (n_trials, samples, channels)
-        Returns
-        -------
-        features : numpy.ndarray [n_events x n_channels]
-            Feature array with the epochs of signal projected in the CSP space
-        """
-        features = self.CSP.project(X=X)
-        # Obtain log-variance features given the CSP features
-        features = np.log(np.var(features, axis=-1))
-        return features
+        # Project using CSP
+        projection = self.CSP.project(X=features)
 
-    def transform_dataset(self, dataset, show_progress_bar=True):
-        features, track_info = super().transform_dataset(
-            dataset=dataset, show_progress_bar=show_progress_bar)
-        # Fit CSP filter
-        self.fit(X=features, y=track_info['mi_labels'])
-        # Project features into CSP space and obtain log-variance features given
-        # the CSP features
-        features = self.extract_log_var_features(X=features)
+        # Log-variance features
+        log_var = self._get_log_vars(projection, self.normalize_log_vars)
+        return log_var, track_info
+
+    def fit_transform_signal(self, labels, times, signal, fs, onsets, **kwargs):
+        # Fit
+        features = self.fit_signal(labels, times, signal, fs, onsets, **kwargs)
+
+        # Project using CSP
+        projection = self.CSP.project(X=features)  # trials x samples x projects
+
+        # Log-variance features across samples
+        log_var = self._get_log_vars(projection, self.normalize_log_vars)
+        return log_var
+
+    def fit_transform_dataset(self, dataset, show_progress_bar=True, **kwargs):
+        # Fit
+        features, track_info = self.fit_dataset(
+            dataset, show_progress_bar=show_progress_bar, **kwargs)
+
+        # Project using CSP
+        projection = self.CSP.project(X=features)
+
+        # Log-variance features
+        log_var = self._get_log_vars(projection, self.normalize_log_vars)
+        return log_var, track_info
 
-        return features, track_info
+    @staticmethod
+    def _get_log_vars(projection, normalize):
+        if normalize:
+            return np.log(
+                np.var(projection, axis=1) /
+                np.tile(np.sum(np.var(projection, axis=1), axis=1),
+                        (projection.shape[2], 1)).T
+            )
+        else:
+            return np.log(np.var(projection, axis=1))
 
 
 class MIModel(components.Algorithm):
     """Skeleton class for MI-based BCIs models. This class inherits from
     components.Algorithm. Therefore, it can be used to create standalone
     algorithms that can be used in compatible apps from medusa-platform
     for online experiments. See components.Algorithm to know more about this
@@ -980,63 +1003,81 @@
                                   fs=fs, x_info=x_info, **kwargs)
 
 
 class MIModelCSP(MIModel):
     """Decoding model for MI-based BCI applications based on
     Common Spatial Patterns (CSP).
 
-    Dataset features:
+    It is strongly recommended to update the default settings by passing
+    arguments through **kwargs. See the different algorithms to know more
+    about the possible parameters: StandardPreprocessing,
+    CSPFeatureExtraction and StandardFeatureExtraction.
 
+    Dataset features:
     - Sample rate of the signals > 60 Hz. The model can handle recordings
         with different sample rates.
-    - Recommended channels: ['C3', 'C4'].
+    - Recommended channels to be present: ['C3', 'C4'].
 
     Processing pipeline:
     - Preprocessing (medusa.bci.erp_spellers.StandardPreprocessing):
-
         - IIR Filter (order=5, cutoff=(8, 30) Hz: unlike FIR filters, IIR
             filters are quick and can be applied in small signal chunks. Thus,
             they are the preferred method for frequency filter in online
             systems.
         - Common average reference (CAR): widely used spatial filter that
             increases the signal-to-noise ratio of the MI control signals.
     - Feature extraction (medusa.bci.mi_paradigms.CSPFeatureExtraction):
-
-        - Epochs (window=(500, 4000) ms, resampling to 60 HZ): the epochs of
+        - Epochs (window=(0, 2000) ms, resampling to 60 HZ): the epochs of
             signal are extracted for each stimulation. Baseline normalization
-            is also applied, taking the window (-1500, -500) ms relative to the
+            is also applied, taking the window (-1000, 0) ms relative to the
             stimulus onset.
         - CSP projection: Epochs are then projected according to a CSP filter
             previously trained.
-
+        - Log variance: Log variance features are extracted from the CSP
+            projection.
     - Feature classification (
     sklearn.discriminant_analysis.LinearDiscriminantAnalysis)
-
         - Regularized linear discriminant analysis (rLDA): we use the sklearn
             implementation, with eigen solver and auto shrinkage paramers. See
             reference in sklearn doc.
     """
 
     def __init__(self):
         super().__init__()
 
-    def configure(self, p_filt_cutoff=(8, 30), f_w_epoch_t=(500, 4000),
-                  f_target_fs=60, **kwargs):
+    def configure(self, p_filt_cutoff=(8, 30), w_epoch_t=(0, 2000),
+                  w_baseline_t=(-1000, 0), target_fs=60, **kwargs):
+        """ Configures the default settings. """
         self.settings = {
+            # StandardPreprocessing
             'p_filt_cutoff': p_filt_cutoff,
-            'f_w_epoch_t': f_w_epoch_t,
-            'f_target_fs': f_target_fs
+            # CSPFeatureExtraction
+            'n_filters': 4,
+            'normalize_log_vars': False,
+            # StandardFeatureExtraction
+            'w_epoch_t': w_epoch_t,
+            'baseline_mode': 'trial',
+            'w_baseline_t': w_baseline_t,
+            'norm': 'z',
+            'target_fs': target_fs,
+            'concatenate_channels': False,
+            'sliding_w_lims_t': None,
+            'sliding_t_step': None,
+            'sliding_win_len': None
         }
         self.settings = dict(self.settings, **kwargs)
         # Update state
         self.is_configured = True
         self.is_built = False
         self.is_fit = False
 
     def build(self):
+        """ Initializes the different methods that comprise the MIModelCSP
+        pipeline.
+        """
         # Check errors
         if not self.is_configured:
             raise ValueError('Function configure must be called first!')
         # Preprocessing (default: bandpass IIR filter [8, 30] Hz + CAR)
         self.add_method('prep_method', StandardPreprocessing(
             cutoff=self.settings['p_filt_cutoff']
         ))
@@ -1049,61 +1090,185 @@
             fit=[], predict_proba=['y_pred']
         )
         self.add_method('clf_method', clf)
         # Update state
         self.is_built = True
         self.is_fit = False
 
-    def fit_dataset(self, dataset, **kwargs):
+    def fit_dataset(self, dataset, get_training_accuracy=True,
+                    k_fold=5, **kwargs):
+        """ Function to fit a dataset using MIModelCSP.
+
+        Parameters
+        -------------
+        dataset : MIDataset
+            MI dataset used for training.
+        get_training_accuracy : bool
+            Whether to perform an estimation on training accuracy after fitting.
+        k_fold : int
+            Number of k-folds used in the k-fold cross-validation procedure
+            to estimate the training accuracy.
+        **kwargs : dict
+            These parameters will be overwritten over self.settings.
+
+        Returns
+        -------------
+        assessment : dict
+            Dictionary containing the details of the training accuracy
+            estimation.
+        """
         # Check errors
         if not self.is_built:
             raise ValueError('Function build must be called first!')
+
+        # Merge settings
+        settings = dict(self.settings, **kwargs)
+        self.channel_set = dataset.channel_set
+
         # Preprocessing
         dataset = self.get_inst('prep_method').fit_transform_dataset(dataset)
+
         # Extract CSP features
-        x, x_info = self.get_inst('ext_method').transform_dataset(dataset)
+        x, x_info = self.get_inst('ext_method').fit_transform_dataset(
+            dataset, **settings)
 
-        # Classification
+        # Training accuracy using a k-fold cross-validation
+        assessment = None
+        if get_training_accuracy:
+            folds_decoding = list()
+            k_fold_iter = cu.k_fold_split(x, x_info['mi_labels'], k_fold)
+            k_fold_acc = 0
+            for iter in k_fold_iter:
+                self.get_inst('clf_method').fit(
+                    iter["x_train"], iter["y_train"])
+                y_test_pred = self.get_inst('clf_method').predict(
+                    iter["x_test"])
+                y_test_prob = self.get_inst('clf_method').predict_proba(
+                    iter["x_test"])
+                fold_acc = np.sum(y_test_pred == iter["y_test"]) / \
+                           len(iter["y_test"])
+                k_fold_acc += fold_acc
+                folds_decoding.append({
+                    "y_pred": y_test_pred,
+                    "y_prob": y_test_prob,
+                    "accuracy": fold_acc,
+                })
+            k_fold_acc /= len(k_fold_iter)
+
+            assessment = {
+                'x': x,
+                'x_info': x_info,
+                'k-fold': folds_decoding,
+                'accuracy': k_fold_acc
+            }
+
+        # Fit classifier with all the data
         self.get_inst('clf_method').fit(x, x_info['mi_labels'])
+
+        # Save info
+        self.channel_set = dataset.channel_set
+
+        # Update state
+        self.is_fit = True
+        return assessment
+
+    def predict(self, times, signal, fs, channel_set, x_info, **kwargs):
+        """ Function to predict an individual signal in MIModelCSP.
+
+        Parameters
+        --------------
+        times : ndarray (n_samples,)
+            Timestamp array
+        signal: ndarray (n_samples x n_channels)
+            Signal data.
+        fs : int
+            Sampling frequency.
+        channel_set : EEGChannelSet or similar
+            Channel montage.
+        x_info : dict
+            Dictionary containing the trial "onsets" and "mi_labels". If the
+            latter is not specified, accuracy is not calculated.
+        **kwargs : dict
+            These parameters will be overwritten over self.settings.
+
+        Returns
+        -------------
+        decoding : dict
+            Dictionary containing the decoding.
+        """
+        # Check errors
+        if not self.is_fit:
+            raise ValueError('Function fit_dataset must be called first!')
+        # Merge settings
+        settings = dict(self.settings, **kwargs)
+        # Check channel set
+        if self.channel_set.l_cha != channel_set.l_cha:
+            warnings.warn('The channel set is not the same that was used to '
+                          'fit the model. Be careful!')
+        # Preprocessing
+        signal = self.get_inst('prep_method').transform_signal(signal)
+
+        # Extract features
+        x = self.get_inst('ext_method').transform_signal(
+            times, signal, fs, x_info['onsets'], **settings)
+
+        # Classification
         y_prob = self.get_inst('clf_method').predict_proba(x)
         y_pred = self.get_inst('clf_method').predict(x)
 
-        # Accuracy
-        accuracy = np.sum((y_pred == x_info['mi_labels'])) / len(y_pred)
-        clf_report = classification_report(x_info['mi_labels'], y_pred,
-                                           output_dict=True)
-        assessment = {
+        # Decoding
+        accuracy = None
+        clf_report = None
+        if x_info['mi_labels'] is not None:
+            accuracy = np.sum((y_pred == x_info['mi_labels'])) / len(y_pred)
+            clf_report = classification_report(x_info['mi_labels'], y_pred,
+                                               output_dict=True)
+        decoding = {
             'x': x,
             'x_info': x_info,
             'y_prob': y_prob,
             'y_pred': y_pred,
             'accuracy': accuracy,
             'report': clf_report
         }
-        # Save info
-        self.channel_set = dataset.channel_set
-        # Update state
-        self.is_fit = True
-        return assessment
+        return decoding
 
-    def predict(self, times, signal, fs, channel_set, x_info, **kwargs):
+    def predict_dataset(self, dataset, **kwargs):
+        """ Function to predict a dataset using MIModelCSP.
+
+        Parameters
+        -------------
+        dataset : MIDataset
+            Test dataset.
+        **kwargs : dict
+            These parameters will be overwritten over self.settings.
+
+        Returns
+        -------------
+        decoding : dict
+            Dictionary containing the decoding.
+        """
         # Check errors
         if not self.is_fit:
             raise ValueError('Function fit_dataset must be called first!')
         # Check channel set
-        if self.channel_set.channels != channel_set.channels:
+        if self.channel_set.l_cha != dataset.channel_set.l_cha:
             warnings.warn('The channel set is not the same that was used to '
                           'fit the model. Be careful!')
+        # Merge settings
+        settings = dict(self.settings, **kwargs)
+
         # Preprocessing
-        signal = self.get_inst('prep_method').fit_transform_signal(signal, fs)
+        dataset = self.get_inst('prep_method').transform_dataset(dataset,
+                                                                 **settings)
 
         # Extract features
-        x = self.get_inst('ext_method').transform_signal(times, signal, fs,
-                                                         x_info['onsets'])
-        x = self.get_inst('ext_method').extract_log_var_features(x)
+        x, x_info = self.get_inst('ext_method').transform_dataset(
+            dataset, **settings)
+
         # Classification
         y_prob = self.get_inst('clf_method').predict_proba(x)
         y_pred = self.get_inst('clf_method').predict(x)
 
         # Decoding
         accuracy = None
         clf_report = None
@@ -1185,16 +1350,15 @@
             raise ValueError('Function configure must be called first!')
         # Only import deep learning models if necessary
         from medusa.deep_learning_models import EEGSym
         # Preprocessing (bandpass IIR filter [0.5, 45] Hz + CAR)
         self.add_method('prep_method',
                         StandardPreprocessing(cutoff=49, btype='lowpass'))
         # Feature extraction (epochs [0, 2000] ms + resampling to 128 Hz)
-        self.add_method('ext_method', StandardFeatureExtraction(w_epoch_t=(
-            0, 2000), target_fs=128, w_baseline_t=(0, 2000),))
+        self.add_method('ext_method', StandardFeatureExtraction(safe_copy=True))
         # Feature classification
         clf = EEGSym(
             input_time=2000,
             fs=128,
             n_cha=self.settings['cnn_n_cha'],
             ch_lateral=self.settings['ch_lateral'],
             filters_per_branch=24,
@@ -1218,27 +1382,33 @@
     def fit_dataset(self, dataset, continuous=False, **kwargs):
         # Check errors
         if not self.is_built:
             raise ValueError('Function build must be called first!')
         # Preprocessing
         dataset = self.get_inst('prep_method').fit_transform_dataset(dataset)
         # Extract features
-        x, x_info = self.get_inst('ext_method').transform_dataset(dataset,
-                                                                  continuous=continuous)
+        # TODO: perform sliding window? if so, we need the lims
+        # TODO: hardcoded?
+        x, x_info = self.get_inst('ext_method').transform_dataset(
+            dataset, w_epoch_t=(0, 2000), baseline_mode="trial",
+            w_baseline_t=(0, 2000), norm="z", target_fs=128,
+            sliding_w_lims_t=None, sliding_t_step=None, sliding_win_len=None
+        )
         # Put channels in symmetric order
-        x = self.get_inst('clf_method').symmetric_channels(x,
-                                                           dataset.channel_set.l_cha)
+        x, _ = self.get_inst('clf_method').symmetric_channels(
+            x, dataset.channel_set.l_cha)
 
         # Classification
-        self.get_inst('clf_method').fit(x, x_info['mi_labels'],
-                                        fine_tuning=self.settings['fine_tuning'],
-                                        shuffle_before_fit=self.settings['shuffle_before_fit'],
-                                        validation_split=self.settings['validation_split'],
-                                        augmentation=self.settings['augmentation'],
-                                        **kwargs)
+        self.get_inst('clf_method').fit(
+            x, x_info['mi_labels'],
+            fine_tuning=self.settings['fine_tuning'],
+            shuffle_before_fit=self.settings['shuffle_before_fit'],
+            validation_split=self.settings['validation_split'],
+            augmentation=self.settings['augmentation'],
+            **kwargs)
         y_prob = self.get_inst('clf_method').predict_proba(x)
         y_pred = y_prob.argmax(axis=-1)
 
         # Accuracy
         accuracy = np.sum((y_pred == x_info['mi_labels'])) / len(y_pred)
         clf_report = classification_report(x_info['mi_labels'], y_pred,
                                            output_dict=True)
@@ -1264,19 +1434,25 @@
         if self.channel_set.channels != channel_set.channels:
             warnings.warn('The channel set is not the same that was used to '
                           'fit the model. Be careful!')
         # Preprocessing
         signal = self.get_inst('prep_method').fit_transform_signal(signal, fs)
 
         # Extract features
-        x = self.get_inst('ext_method').transform_signal(times, signal, fs,
-                                                         x_info['onsets'])
+        # TODO: hardcoded?
+        x = self.get_inst('ext_method').transform_signal(
+            times=times, signal=signal, fs=fs, onsets=x_info['onsets'],
+            w_epoch_t=(0, 2000), baseline_mode="trial", w_baseline_t=(0, 2000),
+            norm="z", target_fs=128
+        )
+
         # Put channels in symmetric order
-        x = self.get_inst('clf_method').symmetric_channels(x,
-                                                           self.channel_set.l_cha)
+        x, _ = self.get_inst('clf_method').symmetric_channels(
+            x, self.channel_set.l_cha)
+
         # Classification
         y_prob = self.get_inst('clf_method').predict_proba(x)
         y_pred = y_prob.argmax(axis=-1)
 
         # Decoding
         accuracy = None
         clf_report = None
@@ -1288,8 +1464,8 @@
             'x': x,
             'x_info': x_info,
             'y_pred': y_pred,
             'y_prob': y_prob,
             'accuracy': accuracy,
             'report': clf_report
         }
-        return decoding
+        return decoding
```

### Comparing `medusa-kernel-1.1.3/medusa/bci/nft_paradigms.py` & `medusa-kernel-1.2.0/medusa/bci/nft_paradigms.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                                                  btype='bandpass',
                                                  filt_method='sosfiltfilt')
         self.offset_line_removal.fit(fs, len(self.l_cha))
 
         # Define filters for filtering over epochs
         for filter in self.filter_dict:
             for f in filter['cutoff']:
-                iir = mds.IIRFilter(order=1,
+                iir = mds.IIRFilter(order=3,
                                     cutoff=f,
                                     btype='bandpass',
                                     filt_method='sosfiltfilt')
 
                 if self.target_channels is None:
                     iir.fit(fs, len(self.l_cha))
                 else:
@@ -437,27 +437,21 @@
             to the artifacts  to avoid. [n_artifact_bands, n_samples, n_channels].
         filtered_signal: numpy.ndarray
             Signal filtered in the narrow band for training. [n_samples, n_channels].
         Returns
         -------
         baseline_value: float
         """
-        # Delete borders to avoid effect borders
-        dif_window = round((signal.shape[0] - self.w_signal_samples_calibration)/2)
-        if dif_window <= 0:
-            raise ValueError('The duration of the signal for the baseline '
-                             'calculation should be slightly longer than the '
-                             'window time taken for the baseline calculation. ')
-        epochs_original, index = make_windows(signal[dif_window:-dif_window, :]
-                                , self.fs, self.update_feature_window,
-                                self.update_rate)
+        epochs_original, index = make_windows(signal, self.fs,
+                                              self.update_feature_window,
+                                              self.update_rate)
         filtered_epochs = make_windows(
-                filtered_signal[dif_window:-dif_window, :], self.fs,
-                self.update_feature_window, self.update_rate,
-                reject=False)[~index, :, :]
+            filtered_signal, self.fs,
+            self.update_feature_window, self.update_rate,
+            reject=False)[~index, :, :]
 
         adj_mat = self.calculate_adj_mat(filtered_epochs)
 
         # Parallel computing baseline values
         filt_threads = []
         baseline_values = []
         for epoch_mat in adj_mat:
@@ -491,28 +485,20 @@
         Returns
         -------
         c_value: float
         """
         if self.baseline_value is None:
             raise ValueError(
                 '[ConnectivityExtraction] Calibration not performed.')
-        # Delete borders
-        dif_window = round((signal.shape[0] - self.w_signal_samples)/2)
-        if dif_window <= 0:
-            raise ValueError('The duration of the signal for feedback '
-                             'calculation should be slightly longer than the '
-                             'window time taken for the feedback calculation. ')
-
-        adj_mat = self.calculate_adj_mat(signal[dif_window:-dif_window, :])
+        adj_mat = self.calculate_adj_mat(signal)
         c_value = self.calculate_feature(np.squeeze(adj_mat)) \
                   - self.baseline_value
         # Check if artifact bands are defined
         if signal_artifacts is not None:
-            if ignore_noisy_windows(signal_artifacts[:,dif_window:-dif_window,
-                                    self.target_channels], self.thresholds,
+            if ignore_noisy_windows(signal_artifacts[:, :, self.target_channels], self.thresholds,
                                     self.pct_tol):
                 return c_value
             else:
                 return None
         return c_value
 
     def calculate_adj_mat(self, signal):
@@ -635,23 +621,15 @@
         signal_artifacts: numpy.ndarray
             Signal filtered in the frequency bands associated to the artifacts
             to be avoided. [n_artifact_bands, n_samples, n_channels].
         Returns
         ------
         baseline_power: float
         """
-        # Delete borders
-        dif_window = round(
-            (signal.shape[0] - self.w_signal_samples_calibration) / 2)
-        if dif_window <= 0:
-            raise ValueError('The duration of the signal for the baseline '
-                             'calculation should be slightly longer than the '
-                             'window time taken for the baseline calculation.')
-        epochs, _ = make_windows(signal[dif_window:-dif_window, :]
-                                 , self.fs, self.update_feature_window,
+        epochs, _ = make_windows(signal, self.fs, self.update_feature_window,
                                  self.update_rate)
         _, psd = scipy.signal.welch(epochs, self.fs, 'hamming',
                                     self.w_signal_samples,
                                     axis=1,scaling='density')
 
         b_power = self.power(psd)
 
@@ -685,23 +663,15 @@
         Returns
         ------
         b_power: float or None
         """
 
         if self.baseline_power is None:
             raise ValueError('[PowerExtraction] Calibration not performed.')
-
-        dif_window = round(
-            (signal.shape[0] - self.w_signal_samples) / 2)
-        if dif_window <= 0:
-            raise ValueError('The duration of the signal for the feedback '
-                             'calculation should be slightly longer than the '
-                             'window time taken for the feedback calculation. ')
-
-        _, psd = scipy.signal.welch(signal[dif_window:-dif_window], self.fs, 'hamming',
+        _, psd = scipy.signal.welch(signal, self.fs, 'hamming',
                                     self.w_signal_samples,
                                     axis=0,scaling='density')
         b_power_uncorrected = self.power(psd)
         if self.mode == 'single':
             b_power = b_power_uncorrected[0] - self.baseline_power
 
         elif self.mode == 'ratio':
```

### Comparing `medusa-kernel-1.1.3/medusa/classification_utils.py` & `medusa-kernel-1.2.0/medusa/classification_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,18 +47,19 @@
         of the k-fold algorithm.
 
     Examples
     --------
     >>> k_fold_iter = k_fold_split(x, y, k)
     >>> k_fold_acc = 0
     >>> for iter in k_fold_iter:
-    >>>     model.fit(iter[x_train, y_train])
-    >>>     y_test_pred = model.predict(iter[x_test, y_test])
-    >>>     k_fold_acc += np.sum(y_test_pred == y_test)/len(y_test)
-    >>>     k_fold_acc = k_fold_acc/len(k_fold_iter)
+    >>>     model.fit(iter["x_train"], iter["y_train"])
+    >>>     y_test_pred = model.predict(iter["x_test"], iter["y_test"])
+    >>>     k_fold_acc += np.sum(y_test_pred == iter["y_test"])/len(iter["y_test"])
+    >>> k_fold_acc = k_fold_acc/len(k_fold_iter)
+
     """
     # Convert to numpy arrays
     x = np.array(x)
     y = np.array(y)
     # If keys is None, each observation is treated independently
     if keys is None:
         keys = np.arange(len(x))
```

### Comparing `medusa-kernel-1.1.3/medusa/components.py` & `medusa-kernel-1.2.0/medusa/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""Created on Monday March 15 19:27:14 2021
-
-In this module, you will find the main components of medusa, which provide
-skeletons for particular implementations. Enjoy!
-
-@author: Eduardo Santamaría-Vázquez
-"""
-
 # Built-in imports
 import json, bson
 import warnings
 from abc import ABC, abstractmethod
 import sys, inspect
 import copy, collections
 from threading import Thread
@@ -266,15 +258,15 @@
 
         Parameters
         ----------
         key: str
             Tree item key
         info: str
             Information about this item
-        value_type: str ['string'|'number'|'boolean'|'dict'|'list'], optional
+        value_type: str ['string'|'number'|'integer'|'boolean'|'dict'|'list'], optional
             Type of the data stored in attribute value. Leave to None if the
             item is going to be a tree.
         value: str, int, float, bool, dict or list, optional
             Tree item value. It must be one of the JSON types to be compatible
             with serialization. Leave to None if the item is going to be a tree.
         """
         # Init attributes
@@ -310,14 +302,19 @@
                     assert isinstance(value, str), \
                         'Parameter value must be of type %s' % str
             elif t == 'number':
                 if value is not None:
                     assert isinstance(value, int) or isinstance(value, float), \
                         'Parameter value must be of types %s or %s' % \
                         (int, float)
+            elif t == 'integer':
+                if value is not None:
+                    assert isinstance(value, int), \
+                        'Parameter value must be of types %s or %s' % \
+                        (int, float)
             elif t == 'boolean':
                 if value is not None:
                     assert isinstance(value, bool), \
                         'Parameter value must be of type %s' % bool
             elif t == 'list':
                 if value is not None:
                     assert isinstance(value, list), \
@@ -342,15 +339,15 @@
         self.value_type = orig_value_type
         self.value = value
         self.items = list()
 
     def add_item(self, item):
         """Adds tree item to the tree. Use this function to build a custom tree.
         Take into account that if this function is used, attributes value and
-        type will be set to None and 'tree', respectively.
+        type will be set to None.
 
         Parameters
         ----------
         item: SettingsTreeItem
             Tree item to add
         """
         if not isinstance(item, SettingsTreeItem):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medusa-kernel-1.1.3/medusa/connectivity/amplitude_connectivity.py` & `medusa-kernel-1.2.0/medusa/connectivity/amplitude_connectivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-"""
-In this module you will find useful functions to apply optimized amplitude-based
-connectivity metrics. Enjoy!
-
-@authors: Víctor Rodríguez-González and Diego Marcos-Martínez
-"""
-
 # Built-in imports
-import warnings
+import warnings, os
 
 # External imports
 import numpy as np
 from scipy import stats as sp_stats
-import tensorflow as tf
-from tensorflow_probability import stats as tfp_stats
 
 # Medusa imports
 import medusa.components
 from medusa import signal_orthogonalization as orthogonalizate
 from medusa.transforms import hilbert
-from medusa import pearson_corr_matrix as corr
 from medusa.utils import check_dimensions
+from medusa import tensorflow_integration
+
+
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
+    import tensorflow_probability as tfp
 
 
 def __aec_gpu(data):
     """ This method implements the amplitude envelope correlation using GPU.
 
     NOTE: See the orthogonalized version.
 
@@ -44,15 +40,15 @@
     data = check_dimensions(data)
 
     # AEC computation
     hilb = hilbert(data)
     envelope = tf.math.abs(hilb) 
     env = tf.math.log(tf.math.square(envelope))
 
-    aec = tfp_stats.correlation(env,sample_axis=1)
+    aec = tfp.stats.correlation(env,sample_axis=1)
 
     return aec.numpy()
 
 
 def __aec_cpu(data):
     """ This method implements the amplitude envelope correlation using CPU.
 
@@ -95,14 +91,15 @@
         t.start()
 
     for epoch_idx, thread in enumerate(w_threads):
         aec[epoch_idx, :, :] = thread.join()
 
     return aec
 
+
 def __aec_ort_gpu(data):
     """ This method implements the orthogonalized version of the amplitude
     envelope correlation using GPU. This orthogonalized version minimizes the
     spurious connectivity caused by common sources (zero-lag correlations).
 
     Parameters
     ----------
@@ -200,14 +197,15 @@
         t.start()
 
     for epoch_idx, thread in enumerate(w_threads):
         aec_ort[epoch_idx,:,:] = thread.join()
 
     return aec_ort
 
+
 def __aec_ort_comp_aux(env, n_cha, ctype='cpu'):
     """
     Auxiliary method that implements a function to compute the orthogonalized AEC.
     Parameters
     ----------
     env: numpy.ndarray
         Array with signal envelope. [n_epochs, n_samples, n_channels x n_channels].
@@ -235,15 +233,15 @@
         aec_upper = np.triu(np.squeeze(aec))
         aec_lower = np.transpose(np.tril(np.squeeze(aec)))
         aec_ort = (aec_upper + aec_lower) / 2
         aec_ort = abs(np.triu(aec_ort, 1) + np.transpose(aec_ort))
         return aec_ort
 
     elif ctype == 'gpu':
-        aec_tmp = tfp_stats.correlation(env)
+        aec_tmp = tfp.stats.correlation(env)
         aec_tmp2 = tf.transpose(
             tf.reshape(
                 tf.transpose(aec_tmp),
                 (tf.cast(aec_tmp.shape[0] * aec_tmp.shape[0] / n_cha,
                          tf.int32), -1)
             )
         )
@@ -253,14 +251,15 @@
         aec_lower = tf.transpose(tf.linalg.band_part(aec, -1, 0))
         aec_ort = tf.math.divide(tf.math.add(aec_upper, aec_lower), 2)
         aux = tf.linalg.band_part(aec_ort, 0, -1) - tf.linalg.band_part(
             aec_ort, 0, 0)
         aec_ort = tf.math.abs(tf.math.add(aux, tf.transpose(aec_ort)))
         return aec_ort
 
+
 def aec(data, ort=True):
     """ This method implements the amplitude envelope correlation (using GPU if
     available). Based on the "ort" param, the signals could be orthogonalized
     before the computation of the amplitude envelope correlation.
 
     REFERENCES:
     Liu, Z., Fukunaga, M., de Zwart, J. A., & Duyn, J. H. (2010).
@@ -287,27 +286,28 @@
 
     Returns
     -------
     aec : numpy.ndarray
         aec-based connectivity matrix. [n_epochs, n_channels, n_channels].
 
     """
-    from medusa import tensorflow_integration
     #  Error check
     if not np.issubdtype(data.dtype, np.number):
         raise ValueError('data matrix contains non-numeric values') 
 
     if not ort:
-        if tensorflow_integration.check_tf_config(autoconfig=True):
+        if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+                tensorflow_integration.check_tf_config(autoconfig=True):
             aec = __aec_gpu(data)
         else:
             aec = __aec_cpu(data)
 
     else:
-        if tensorflow_integration.check_tf_config(autoconfig=True):
+        if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+                tensorflow_integration.check_tf_config(autoconfig=True):
             aec = __aec_ort_gpu(data)
         else:
             aec = __aec_ort_cpu(data)
 
     return aec
 
 
@@ -365,14 +365,15 @@
     diag_mask = tf.linalg.set_diag(diag_mask, tf.zeros(diag_mask.shape[0:-1]),
                                    name=None)
     iac = tf.multiply(iac, tf.repeat(tf.repeat(diag_mask[None,:, :, None], n_samp,
                                      axis=-1), n_epo,axis=0))
 
     return iac.numpy()
 
+
 def __iac_cpu(data):
     """ This method implements the instantaneous amplitude correlation using
     CPU.
 
     NOTE: See the orthogonalized version. In the original paper, the
     orthogonalized version was used
 
@@ -490,14 +491,15 @@
     iac_ort = tf.math.divide(tf.math.add(iac_upper, iac_lower), 2)
     aux = tf.linalg.band_part(iac_ort, 0, -1) - tf.linalg.band_part(iac_ort, 0,
                                                                     0)
     iac_ort = tf.math.abs(tf.math.add(aux, tf.transpose(aux, (0,1, 3, 2))))
 
     return tf.transpose(iac_ort, (0, 2, 3, 1)).numpy()
 
+
 def __iac_ort_cpu(data):
     """ This method implements the orthogonalized version of the instantaneous
     amplitude correlation using CPU. This orthogonalized version minimizes the
     spurious connectivity caused by common sources (zero-lag correlations).
 
     Parameters
     ----------
@@ -587,26 +589,26 @@
     Returns
     -------
     iac : numpy 2D square matrix
         iac-based connectivity matrix.
         [n_epochs, n_channels, n_channels, n_samples].
 
     """
-    from medusa import tensorflow_integration
-
     #  Error check
     if not np.issubdtype(data.dtype, np.number):
         raise ValueError('data matrix contains non-numeric values')
 
     if not ort:
-        if tensorflow_integration.check_tf_config(autoconfig=True):
+        if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+                tensorflow_integration.check_tf_config(autoconfig=True):
             iac = __iac_gpu(data)
         else:
             iac = __iac_cpu(data)
 
     else:
-        if tensorflow_integration.check_tf_config(autoconfig=True):
+        if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+                tensorflow_integration.check_tf_config(autoconfig=True):
             iac = __iac_ort_gpu(data)
         else:
             iac = __iac_ort_cpu(data)
 
     return iac
```

### Comparing `medusa-kernel-1.1.3/medusa/connectivity/phase_connectivity.py` & `medusa-kernel-1.2.0/medusa/connectivity/phase_connectivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""
-In this module you will find useful functions to apply optimized phase-based
-connectivity metrics. Enjoy!
-
-@authors: Víctor Rodríguez-González and Diego Marcos-Martínez
-"""
-
 # Built-in imports
-import warnings
+import warnings, os
 
 # External imports
 import scipy.signal as sp_signal
 import numpy as np
-import tensorflow as tf
 
 # Medusa imports
 from medusa import transforms
 from medusa.utils import check_dimensions
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
 
 
 def __phase_connectivity_cpu(data, measure=None):
     """ This method implements three phase-based connectivity parameters using
     CPU: PLV, PLI, and wPLI.
 
     Parameters
@@ -176,27 +173,28 @@
     if ctype == 'CPU':
         imz = np.sin(angles_1 - angles_2)
         with np.errstate(divide='ignore', invalid='ignore'):
             wpli_vector = np.divide(
                 abs(np.mean(np.multiply(abs(imz), np.sign(imz)), axis=1)),
                 np.mean(abs(imz), axis=1)
             )
-        wpli = np.reshape(wpli_vector, (n_epochs, n_chan, n_chan), order='F')
+        wpli = np.nan_to_num(
+            np.reshape(wpli_vector, (n_epochs, n_chan, n_chan), order='F'))
     elif ctype == 'GPU':
         imz = tf.math.sin(tf.math.subtract(angles_1, angles_2))
         wpli_vector = tf.math.divide(
             tf.math.abs(tf.math.reduce_mean(
                 tf.math.multiply(
                     tf.math.abs(imz),
                     tf.math.sign(imz)),
                 axis=1)),
             tf.math.reduce_mean(tf.math.abs(imz), axis=1))
         wpli = tf.reshape(wpli_vector, (n_epochs, n_chan, n_chan))
-
-    wpli = tf.linalg.set_diag(wpli, np.zeros((wpli.shape[0], wpli.shape[1])))
+        wpli = tf.linalg.set_diag(wpli, np.zeros((wpli.shape[0],
+                                                  wpli.shape[1])))
     return wpli
 
 
 def phase_connectivity(data, measure=None):
     """ This method implements three phase-based connectivity parameters: PLV,
     PLI, and wPLI.
 
@@ -231,24 +229,24 @@
         plv-based connectivity matrix. [n_epochs, n_channels, n_channels].
     pli : numpy 3D square matrix
         pli-based connectivity matrix. [n_epochs, n_channels, n_channels].
     wpli : numpy 3D square matrix
         wpli-based connectivity matrix. [n_epochs, n_channels, n_channels].
 
     """
-    from medusa import tensorflow_integration
     # Error check
     if not np.issubdtype(data.dtype, np.number):
         raise ValueError('data matrix contains non-numeric values')
     if measure is not None and (measure != 'plv' and measure != 'pli' and measure
                                 != 'wpli'):
         raise ValueError('Unknown measure key. Available are: "plv", "pli" or'
                          '"wpli".')
 
-    if tensorflow_integration.check_tf_config(autoconfig=True):
+    if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+            tensorflow_integration.check_tf_config(autoconfig=True):
         if measure is None:
             plv, pli, wpli, = __phase_connectivity_gpu(data, measure)
             return np.asarray(plv), np.asarray(pli), np.asarray(wpli)
         else:
             ph_cnn_measure = __phase_connectivity_gpu(data, measure)
             return np.asarray(ph_cnn_measure)
     else:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medusa-kernel-1.1.3/medusa/deep_learning_models.py` & `medusa-kernel-1.2.0/medusa/deep_learning_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 # Built-in imports
 import warnings
 import os
+
 # External imports
-import tensorflow as tf
-from tensorflow.keras.layers import Activation, Input, Flatten
-from tensorflow.keras.layers import Dropout, BatchNormalization
-from tensorflow.keras.layers import Conv2D, AveragePooling2D, DepthwiseConv2D
-from tensorflow.keras.layers import Dense, SpatialDropout2D, SeparableConv2D
-from tensorflow.keras.layers import Conv3D, AveragePooling3D, Add
-from tensorflow.keras.constraints import max_norm
-from tensorflow.keras.callbacks import EarlyStopping
-import tensorflow.keras as keras
 import sklearn.utils as sk_utils
 import numpy as np
 
 # Medusa imports
 from medusa import components
 from medusa import classification_utils
 from medusa import tensorflow_integration
 
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
+    import tensorflow.keras as keras
+    from tensorflow.keras.layers import Activation, Input, Flatten
+    from tensorflow.keras.layers import Dropout, BatchNormalization
+    from tensorflow.keras.layers import Conv2D, AveragePooling2D
+    from tensorflow.keras.layers import DepthwiseConv2D, Dense
+    from tensorflow.keras.layers import SpatialDropout2D, SeparableConv2D
+    from tensorflow.keras.layers import Conv3D, AveragePooling3D, Add
+    from tensorflow.keras.constraints import max_norm
+    from tensorflow.keras.callbacks import EarlyStopping
+else:
+    raise tensorflow_integration.TFExtrasNotInstalled()
+
 
 class EEGInceptionv1(components.ProcessingMethod):
     """EEG-Inception as described in Santamaría-Vázquez et al. 2020 [1]. This
     model is specifically designed for EEG classification tasks.
 
     References
     ----------
@@ -301,14 +308,15 @@
             'kwargs': kwargs,
             'weights': weights
         }
         return pickleable_obj
 
     @classmethod
     def from_pickleable_obj(cls, pickleable_obj):
+        pickleable_obj['kwargs']['gpu_acceleration'] = None
         model = cls(**pickleable_obj['kwargs'])
         model.model.set_weights(pickleable_obj['weights'])
         return model
 
     def set_weights(self, weights):
         return self.model.set_weights(weights)
 
@@ -630,14 +638,15 @@
             'kwargs': kwargs,
             'weights': weights
         }
         return pickleable_obj
 
     @classmethod
     def from_pickleable_obj(cls, pickleable_obj):
+        pickleable_obj['kwargs']['gpu_acceleration'] = None
         model = cls(**pickleable_obj['kwargs'])
         model.model.set_weights(pickleable_obj['weights'])
         return model
 
     def set_weights(self, weights):
         return self.model.set_weights(weights)
 
@@ -1444,15 +1453,16 @@
                 else:
                     left.append(channel)
             else:
                 middle.append(channel)
         ordered_channels = left + middle + right
         index_channels = [channels.index(channel) for channel in
                           ordered_channels]
-        return X[:, :, index_channels]
+        return np.array(X)[:, :, index_channels], list(np.array(channels)[
+            index_channels])
 
     def predict_proba(self, X):
         """Model prediction scores for the given features.
 
         Parameters
         ----------
         X: np.ndarray
@@ -1486,14 +1496,15 @@
             'kwargs': kwargs,
             'weights': weights
         }
         return pickleable_obj
 
     @classmethod
     def from_pickleable_obj(cls, pickleable_obj):
+        pickleable_obj['kwargs']['gpu_acceleration'] = None
         model = cls(**pickleable_obj['kwargs'])
         model.model.set_weights(pickleable_obj['weights'])
         return model
 
     def set_weights(self, weights):
         return self.model.set_weights(weights)
```

### Comparing `medusa-kernel-1.1.3/medusa/emg.py` & `medusa-kernel-1.2.0/medusa/emg.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/epoching.py` & `medusa-kernel-1.2.0/medusa/epoching.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,22 +56,22 @@
     signal : list or numpy.ndarray
         Biosignal samples
     onsets : list or numpy.ndarray
         Events timestamps
     fs : float
         Sample rate
     w_epoch_t : list or numpy.ndarray
-        Temporal window in ms of the epoch. For example, t_baseline = [0, 1000]
+        Temporal window in ms of the epoch. For example, w_epoch_t = [0, 1000]
         takes the epoch form 0 ms to 1000 ms after each onset (0 ms represents
         the onset).
     w_baseline_t : list or numpy.ndarray, optional
-        Temporal window in ms of the baseline. For example, t_baseline =
-        [-500, 100] takes the baseline form -500 ms before each onset to 100
+        Temporal window in ms of the baseline. For example, w_baseline_t =
+        [-500, 100] takes the baseline from -500 ms before each onset to 100
         ms after each onset (0 ms represents the onset). This chunk of signal is
-        used to normalize the epoch, if aplicable
+        used to normalize the epoch, if applicable.
     norm : str, optional
        Set to 'z' for Z-score normalization or 'dc' for DC normalization.
        Statistical parameters are computed using the whole epoch.
     Returns
     -------
     numpy.ndarray
         Structured data with dimensions [events x samples x channels]
@@ -100,29 +100,28 @@
 
     # Useful parameters
     w_epoch_t = np.array(w_epoch_t)
     w_epoch_s = np.array(w_epoch_t * fs / 1000, dtype=int)
     l_epoch = w_epoch_s[1] - w_epoch_s[0]
     # For each onset
     n_cha = signal.shape[1]
-    epochs_idx = np.searchsorted(timestamps, onsets + w_epoch_t[0] / 1000,
-                                 side='left')
+    epochs_idx = get_nearest_idx(timestamps, onsets)
     epochs = np.lib.stride_tricks.sliding_window_view(
-        signal, (l_epoch, n_cha))[epochs_idx].squeeze(axis=1)
+        signal, (l_epoch, n_cha))[epochs_idx + w_epoch_s[0]].squeeze(axis=1)
     # Baseline normalization
     if w_baseline_t is not None and norm is not None:
         # Baseline start-end (samples)
         w_baseline_t = np.array(w_baseline_t)
         w_baseline_s = np.array(w_baseline_t * fs / 1000, dtype=int)
         l_baseline = w_baseline_s[1] - w_baseline_s[0]
         # Extract baselines
-        baseline_idx = np.searchsorted(
-            timestamps, onsets + w_baseline_t[0] / 1000, side='left')
+        baseline_idx = get_nearest_idx(timestamps, onsets)
         baselines = np.lib.stride_tricks.sliding_window_view(
-            signal, (l_baseline, n_cha))[baseline_idx].squeeze(axis=1)
+            signal, (l_baseline, n_cha))[
+            baseline_idx + w_baseline_s[0]].squeeze(axis=1)
         epochs = normalize_epochs(epochs, norm_epochs=baselines, norm=norm)
     return epochs
 
 
 def normalize_epochs(epochs, norm_epochs=None, norm='z'):
     """
     Normalizes epochs
@@ -308,7 +307,24 @@
     if len(onsets.shape) != 1:
         raise ValueError('Parameter onsets must be a 1D array')
 
     rep_times = np.matlib.repmat(times, onsets.shape[0], 1).T
     rep_onsets = np.matlib.repmat(onsets, times.shape[0], 1)
 
     return np.argmin(np.abs(rep_times - rep_onsets), axis=0)
+
+def get_nearest_idx(timestamps, onsets):
+    """This function returns the indexes of the timestamps that are closest to
+    the onsets.
+    """
+    array = np.array(timestamps)
+
+    # get insert positions
+    idxs = np.searchsorted(array, onsets, side="left")
+
+    # find indexes where previous index is closer
+    prev_idx_is_less = ((idxs == len(array)) | (
+                np.fabs(onsets - array[np.maximum(idxs - 1, 0)]) < np.fabs(
+            onsets - array[np.minimum(idxs, len(array) - 1)])))
+    idxs[prev_idx_is_less] -= 1
+
+    return idxs
```

### Comparing `medusa-kernel-1.1.3/medusa/frequency_filtering.py` & `medusa-kernel-1.2.0/medusa/frequency_filtering.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/assortativity.py` & `medusa-kernel-1.2.0/medusa/graph_theory/assortativity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,21 @@
-import tensorflow as tf
+# Built-in imports
+import warinings, os
+
+# External imports
 import numpy as np
+
+# Medusa imports
 from medusa.graph_theory import degree
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
+
 
 def __assort_gpu(W):
     """
     Calculates the assortativity using GPU
 
     Parameters
     ----------
@@ -13,33 +24,34 @@
         
     Returns
     -------
     global_assort : numpy array
         Global assortativity
         
     """
-    
-    deg = degree.degree(W,'GPU')
+
+    deg = degree.__degree_gpu(W)
     aux = tf.linalg.band_part(W, 0, -1) - tf.linalg.band_part(W, 0, 0)
-    ind = tf.where(aux>0)
-    K = ind.shape[0] # Equal to N choose 2 is there is no 0
-    deg_i = tf.gather(deg, tf.transpose(ind[:,0]))
-    deg_j = tf.gather(deg, tf.transpose(ind[:,1]))
-            
-    num_1 = tf.math.divide(tf.reduce_sum(tf.math.multiply(deg_i,deg_j)),K)
-    num_2 = tf.math.multiply(tf.math.add(deg_i,deg_j),0.5)
-    num_2 = tf.math.square(tf.math.divide(tf.reduce_sum(num_2),K))
+    ind = tf.where(aux > 0)
+    K = ind.shape[0]  # Equal to N choose 2 is there is no 0
+    deg_i = tf.gather(deg, tf.transpose(ind[:, 0]))
+    deg_j = tf.gather(deg, tf.transpose(ind[:, 1]))
+
+    num_1 = tf.math.divide(tf.reduce_sum(tf.math.multiply(deg_i, deg_j)), K)
+    num_2 = tf.math.multiply(tf.math.add(deg_i, deg_j), 0.5)
+    num_2 = tf.math.square(tf.math.divide(tf.reduce_sum(num_2), K))
     num = num_1 - num_2
 
-    den_1 = tf.math.multiply(tf.math.add(tf.math.square(deg_i),tf.math.square(deg_j)),0.5)
-    den_1 = tf.math.divide(tf.reduce_sum(den_1),K)
+    den_1 = tf.math.multiply(
+        tf.math.add(tf.math.square(deg_i), tf.math.square(deg_j)), 0.5)
+    den_1 = tf.math.divide(tf.reduce_sum(den_1), K)
     den_2 = num_2
     den = den_1 - den_2
-    
-    global_assort = tf.math.divide(num,den)    
+
+    global_assort = tf.math.divide(num, den)
     return global_assort
 
 
 def __assort_cpu(W):
     """
     Calculates the assortativity using CPU
 
@@ -50,65 +62,58 @@
         
     Returns
     -------
     global_assort : numpy array
         Global assortativity
         
     """
-    
-    deg = degree.degree(W,'CPU')
-    ind = np.triu_indices(W.shape[0],1,W.shape[1])
+
+    deg = degree.__degree_cpu(W)
+    ind = np.triu_indices(W.shape[0], 1, W.shape[1])
     K = ind[0].shape
     deg_i = deg[ind[0]]
     deg_j = deg[ind[1]]
 
     num_1 = np.sum(deg_i * deg_j) / K
-    num_2 = (np.sum(0.5 *(deg_i + deg_j))/K)**2
+    num_2 = (np.sum(0.5 * (deg_i + deg_j)) / K) ** 2
     num = num_1 - num_2
-    
-    den_1 = np.sum(0.5*(deg_i**2 + deg_j**2)) / K
+
+    den_1 = np.sum(0.5 * (deg_i ** 2 + deg_j ** 2)) / K
     den_2 = num_2
     den = den_1 - den_2
-    
-    global_assort = num / den    
-        
+
+    global_assort = num / den
+
     return global_assort
 
 
-def assortativity(W,mode):
+def assortativity(W, mode):
     """
     Calculates the assortativity, which is a preference of nodes to attach to 
     other nodes that are somehow similar to them
 
     Parameters
     ----------
     W : numpy 2D matrix
         Graph matrix. ChannelsXChannels.
     mode : string
         GPU or CPU
-        
+
     Returns
     -------
     global_assort : numpy array
         Global assortativity
 
     """
     if W.shape[0] is not W.shape[1]:
         raise ValueError('W matrix must be square')
-        
+
     if not np.issubdtype(W.dtype, np.number):
-        raise ValueError('W matrix contains non-numeric values')        
-      
-    if mode == 'CPU':
-        global_assort = __assort_cpu(W)
-    elif mode == 'GPU':
+        raise ValueError('W matrix contains non-numeric values')
+
+    if mode == 'GPU' and os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+            tensorflow_integration.check_tf_config(autoconfig=True):
         global_assort = __assort_gpu(W)
     else:
-        raise ValueError('Unknown mode')
-        
-    return global_assort
-
-# import scipy.io as rmat
+        global_assort = __assort_cpu(W)
 
-# data = rmat.loadmat('D:/OneDrive - Universidad de Valladolid/Scripts/testPython/graphTest.mat')
-# W = data['W']
-# aa = assortativity(W,'CPU')
+    return global_assort
```

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/betweeenness_centrality.py` & `medusa-kernel-1.2.0/medusa/graph_theory/betweeenness_centrality.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/clustering_coefficient.py` & `medusa-kernel-1.2.0/medusa/graph_theory/clustering_coefficient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
-import tensorflow as tf
+# Built-in imports
+import warnings, os
+
+# External imports
 import numpy as np
 
+# Medusa imports
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
+
 def __clustering_gpu(W):
     """
     Calculates the ClC of echa node of the graph contained in the matrix W using GPU
 
     It is calculated as follows:
               ___   ___  
               \     \    Wik * Wli * Wkl
@@ -85,25 +95,27 @@
 
     Parameters
     ----------
     W : numpy 2D matrix
         Graph matrix. ChannelsXChannels.
     mode : string
         GPU or CPU
-        
+
     Returns
     -------
     nodal_clc : numpy array
         Nodal clustering coefficient
 
     """
     if W.shape[0] is not W.shape[1]:
         raise ValueError('W matrix must be square')
       
     if mode == 'CPU':
         nodal_clc = __clustering_cpu(W)
     elif mode == 'GPU':
-        nodal_clc = __clustering_gpu(W)
+        if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+                tensorflow_integration.check_tf_config(autoconfig=True):
+            nodal_clc = __clustering_gpu(W)
     else:
         raise ValueError('Unknown mode')
         
     return nodal_clc
```

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/complexity.py` & `medusa-kernel-1.2.0/medusa/graph_theory/complexity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
+# Built-in imports
+import warnings, os
+
+# External imports
 import numpy as np
-import tensorflow as tf
 import scipy.special as sps
-import tensorflow_probability as tfp
+
+# Medusa imports
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
+    import tensorflow_probability as tfp
 
 def __divergency_cpu(W):
     """
     Calculates the graph divergency. Its the entropic distance (as euclidean
     distance) between a uniform weight distribution (random graph) and the 
     network under study using CPU
     
@@ -236,17 +246,16 @@
 
     """
     if W.shape[0] is not W.shape[1]:
         raise ValueError('W matrix must be square')
         
     if not np.issubdtype(W.dtype, np.number):
         raise ValueError('W matrix contains non-numeric values')        
-      
-    if mode == 'CPU':
-        global_comp = __complexity_cpu(W)
-    elif mode == 'GPU':
+
+    if mode == 'GPU' and os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+            tensorflow_integration.check_tf_config(autoconfig=True):
         global_comp = __complexity_gpu(W)
     else:
-        raise ValueError('Unknown mode')
-        
+        global_comp = __complexity_cpu(W)
+
     return global_comp
```

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/degree.py` & `medusa-kernel-1.2.0/medusa/graph_theory/degree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-import tensorflow as tf
+# Built-in imports
+import warnings, os
+
+# External imports
 import numpy as np
 
+# Medusa imports
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
 
 def __aux_symm_triu_gpu(W):
     N = tf.shape(W)
     aux = tf.subtract(tf.linalg.band_part(tf.ones(N), 0, -1),tf.linalg.band_part(tf.ones(N), 0, 0))
     W = tf.math.multiply(W,tf.cast(aux,tf.float64))
     W = tf.math.add(W,tf.transpose(W))
     W = tf.math.divide(tf.math.reduce_sum(W,axis=0),2)
@@ -95,42 +104,36 @@
         
     if check_symmetry == 0:
         nodal_degree = __aux_no_match_cpu(W)
     elif check_symmetry == 1:
         nodal_degree =  __aux_symm_triu_cpu(W)
     elif check_symmetry == 2:
         nodal_degree = -np.sum(W,axis=0)
-          
     return nodal_degree
 
 
-def degree(W,mode):
+def degree(W, mode):
     """
     Calculates the graph degree.
 
     Parameters
     ----------
     W : numpy 2D matrix
         Graph matrix. ChannelsXChannels.
-    mode : string
-        GPU or CPU
-        
     Returns
     -------
     nodal_degree : numpy array
         Nodal degree.      
 
     """
     if W.shape[0] is not W.shape[1]:
         raise ValueError('W matrix must be square')
         
     if not np.issubdtype(W.dtype, np.number):
-        raise ValueError('W matrix contains non-numeric values')        
-      
-    if mode == 'CPU':
-        nodal_degree = __degree_cpu(W)
-    elif mode == 'GPU':
+        raise ValueError('W matrix contains non-numeric values')
+
+    if mode == 'GPU' and os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+            tensorflow_integration.check_tf_config(autoconfig=True):
         nodal_degree = __degree_gpu(W)
     else:
-        raise ValueError('Unknown mode')
-
+        nodal_degree = __degree_cpu(W)
     return nodal_degree
```

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/density.py` & `medusa-kernel-1.2.0/medusa/graph_theory/density.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,20 @@
-import tensorflow as tf
+# Built-in imports
+import warnings, os
+
+# External imports
 import numpy as np
+
+# Medusa imports
 from medusa.graph_theory import degree
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
 
 def __density_gpu(W):
     """
     Calculates the graph density using GPU.
 
     Parameters
     ----------
@@ -25,15 +35,15 @@
         tf.math.reduce_sum(tf.subtract(tf.linalg.band_part(W, -1, 0),tf.linalg.band_part(W, 0, 0))) == 0,
         lambda: 1, lambda: check_symmetry)
     check_symmetry = tf.cond(
         tf.reduce_all(tf.math.equal(W,-tf.transpose(W))),
         lambda: 2, lambda: check_symmetry)
     
     N = W.shape[0]
-    deg = degree.degree(W,'GPU')
+    deg = degree.__degree_gpu(W)
     
     norm_value = tf.switch_case(tf.cast(check_symmetry,tf.int32), 
                 branch_fns={0: lambda: tf.math.multiply(N,tf.math.subtract(N,1)),
                             1: lambda: tf.math.divide(tf.math.multiply(N,tf.math.subtract(N,1)),2), 
                             2: lambda: tf.math.multiply(N,tf.math.subtract(N,1))})
 
     nodal_den = tf.divide(deg,norm_value)
@@ -65,15 +75,15 @@
     if (W == np.triu(W)).all(): # if upper triangular
         check_symmetry = 1
         
     if (W.transpose() == -W).all(): # if anti-symmetric
         check_symmetry = 2
     
     N = W.shape[0]
-    deg = degree.degree(W,'CPU')
+    deg = degree.__degree_cpu(W)
     
     if check_symmetry == 0 or check_symmetry == 2:
         norm_value = N*(N-1)
     elif check_symmetry == 1:
         norm_value = ((N*(N-1))/2)
         
     nodal_den = np.divide(deg,norm_value)
@@ -102,16 +112,15 @@
 
     """
     if W.shape[0] is not W.shape[1]:
         raise ValueError('W matrix must be square')
         
     if not np.issubdtype(W.dtype, np.number):
         raise ValueError('W matrix contains non-numeric values')        
-      
-    if mode == 'CPU':
-        global_den,nodal_den = __density_cpu(W)
-    elif mode == 'GPU':
+
+    if mode == 'GPU' and os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+            tensorflow_integration.check_tf_config(autoconfig=True):
         global_den,nodal_den = __density_gpu(W)
     else:
-        raise ValueError('Unknown mode')
+        global_den,nodal_den = __density_cpu(W)
         
     return global_den, nodal_den
```

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/efficiency.py` & `medusa-kernel-1.2.0/medusa/graph_theory/efficiency.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/modularity.py` & `medusa-kernel-1.2.0/medusa/graph_theory/modularity.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/participation_coefficient.py` & `medusa-kernel-1.2.0/medusa/graph_theory/participation_coefficient.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/path_length.py` & `medusa-kernel-1.2.0/medusa/graph_theory/path_length.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/surrogate_graph.py` & `medusa-kernel-1.2.0/medusa/graph_theory/surrogate_graph.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/graph_theory/transitivity.py` & `medusa-kernel-1.2.0/medusa/graph_theory/transitivity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,20 @@
-import tensorflow as tf
+# Built-in imports
+import warnings, os
+
+# External imports
 import numpy as np
 
+# Medusa imports
+from medusa import tensorflow_integration
+
+# Extras
+if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1":
+    import tensorflow as tf
+
 def __trans_gpu(W):
     """
     Calculates the transitivity using GPU
 
     Parameters
     ----------
     W : numpy 2D matrix
@@ -69,22 +79,13 @@
 
     """
     if W.shape[0] is not W.shape[1]:
         raise ValueError('W matrix must be square')
         
     if not np.issubdtype(W.dtype, np.number):
         raise ValueError('W matrix contains non-numeric values')        
-      
-    if mode == 'CPU':
-        global_trans = __trans_cpu(W)
-    elif mode == 'GPU':
+    if mode == 'GPU' and os.environ.get("MEDUSA_EXTRAS_GPU_TF") == "1" and \
+            tensorflow_integration.check_tf_config(autoconfig=True):
         global_trans = __trans_gpu(W)
     else:
-        raise ValueError('Unknown mode')
-        
+        global_trans = __trans_cpu(W)
     return global_trans
-
-# import scipy.io as rmat
-
-# data = rmat.loadmat('D:/OneDrive - Universidad de Valladolid/Scripts/testPython/graphTest.mat')
-# W = data['W']
-# aa = transitivity(W,'CPU')
```

### Comparing `medusa-kernel-1.1.3/medusa/local_activation/computeLZC.dll` & `medusa-kernel-1.2.0/medusa/local_activation/computeLZC.dll`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/local_activation/nonlinear_parameters.py` & `medusa-kernel-1.2.0/medusa/local_activation/nonlinear_parameters.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/local_activation/spectral_parameteres.py` & `medusa-kernel-1.2.0/medusa/local_activation/spectral_parameteres.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/local_activation/statistics.py` & `medusa-kernel-1.2.0/medusa/local_activation/statistics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-"""
-Created on Fri Dec 20 12:33:30 2019
-Modified on Tue Jun 21 12:32:00 2022
-
-@author: VICTOR
-"""
 import numpy as np
 
 
 def signed_r2(class1, class2, signed=True, axis=0):
     """ This function computes the basic form of the squared point biserial
     correlation coefficient (r2-value).
```

### Comparing `medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-05_2D.tsv` & `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_2D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-05_3D.tsv` & `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-05_3D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-10_2D.tsv` & `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_2D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-10_3D.tsv` & `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-10_3D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/meeg/eeg_standard_10-20_3D.tsv` & `medusa-kernel-1.2.0/medusa/meeg/eeg_standard_10-20_3D.tsv`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/meeg/meeg.py` & `medusa-kernel-1.2.0/medusa/meeg/meeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-"""Created on Monday March 15 19:27:14 2021
-
-In this module, you will find all functions and data structures related to
-EEG and MEG signals. Enjoy!
-
-References:
-    https://stefanappelhoff.com/eeg_positions
-    https://github.com/sappelhoff/eeg_positions
-    https://mne.tools/dev/auto_tutorials/intro/40_sensor_locations.html
-@author: Eduardo Santamaría-Vázquez
-"""
-
 # Built-in imports
 import math
 
 # External imports
 import warnings
 
 import scipy.io
```

### Comparing `medusa-kernel-1.1.3/medusa/meeg/meeg_montages.py` & `medusa-kernel-1.2.0/medusa/meeg/meeg_montages.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/nirs.py` & `medusa-kernel-1.2.0/medusa/nirs.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/notify_me.py` & `medusa-kernel-1.2.0/medusa/notify_me.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/optimization.py` & `medusa-kernel-1.2.0/medusa/optimization.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/plots/brain_plots.py` & `medusa-kernel-1.2.0/medusa/plots/brain_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-"""
-Created on Mon Mar 21 15:34:18 2022
-
-@author: Diego Marcos-Martínez
-"""
 # Python modules
 import argparse
 import os
 # Medusa modules
 from medusa.meeg import EEGChannelSet
 
 # External modules
@@ -16,15 +11,16 @@
 from vispy.scene.visuals import Mesh, Markers, Text, Graph
 from vispy.scene import transforms
 from vispy.visuals.filters import TextureFilter
 from vispy.color import get_colormap
 from medusa.meeg import EEGChannelSet
 
 
-class TridimentionalBrain():
+class TridimentionalBrain:
+
     def __init__(self, bg_color='black', text_color='white', translucent=None,
                  subplots=None, models=None, names=None):
 
         self.subplots = subplots
         self.bg_color = bg_color
         self.text_color = text_color
         self.translucent = translucent
@@ -43,14 +39,15 @@
         self.labels_text = None
         self.connections_coords = None
         self.connections_values = None
         self.lines = None
         self.lines_cmap = None
         self.n_subplots = None
 
+        # Check subplots
         self.__check_subplot()
 
         # Set canvas and view
         self.__set_canvas()
 
         # Set alpha
         self.__set_alpha()
@@ -79,15 +76,15 @@
         except ValueError:
             print("Subplots must be two-dimensional tuple or None")
 
     def __set_alpha(self):
         try:
             if self.translucent is None:
                 self.translucent = np.ones(self.n_subplots, dtype=bool)
-            elif isinstance(self.translucent,bool):
+            elif isinstance(self.translucent, bool):
                 self.translucent = [self.translucent]
             else:
                 assert len(self.translucent) == self.n_subplots
         except Exception as ex:
             print(ex)
 
     def __set_models(self):
@@ -172,52 +169,54 @@
                     alpha = 0.3
                 else:
                     alpha = 1
                 mesh = Mesh(vertices, faces, shading=shading,
                             color=(1, 1, 1, alpha))
                 mesh.shading_filter.shininess = 1e+2
                 self.brain_visuals.append(mesh)
-                self.attach_headlight(mesh, self.views[i], self.canvas)
+                self.__attach_headlight(mesh, self.views[i], self.canvas)
         except Exception as ex:
             print(ex)
 
-    def add_brains(self):
+    def __add_brains(self):
         try:
             for view_idx in range(len(self.views)):
                 self.views[view_idx].add(self.brain_visuals[view_idx])
         except Exception as ex:
             print(ex)
 
-    def attach_headlight(self, mesh, view, canvas):
+    def __attach_headlight(self, mesh, view, canvas):
         """This function sets the initial light direction """
         light_dir = (1, 0, 1, 1)
         mesh.shading_filter.light_dir = light_dir[:3]
         initial_light_dir = view.camera.transform.imap(light_dir)
 
         @view.scene.transform.changed.connect
         def on_transform_change(event):
             """ This function calculates the illumination every
             time the brain is rotated"""
             transform = view.camera.transform
             mesh.shading_filter.light_dir = transform.map(initial_light_dir)[:3]
 
-    def set_markers(self, locs, sub_plot):
+    def __set_markers(self, locs, sub_plot):
         try:
             if self.markers is None:
                 self.__init_markers()
-            markers = Markers(light_color=self.text_color,size = 100)
-            markers.set_data(locs)
+                
+            markers = Markers(light_color=self.text_color,spherical=True)
+            markers.set_data(locs,size=25,)
+            
             self.markers[sub_plot[0]][sub_plot[1]] = markers
 
             _view_idx = self.__calculate_subplot_idx(sub_plot)
             self.views[_view_idx].add(markers)
         except Exception as ex:
             print(ex)
 
-    def set_labels(self, labels, locs, sub_plot):
+    def __set_labels(self, labels, locs, sub_plot):
         try:
             if self.labels_text is None:
                 self.__init_labels()
 
             # Move the labels over the channels
             text_coord = locs.copy()
             text_coord[:, 2] += 0.1
@@ -253,27 +252,90 @@
                         (2, 1)).reshape(2 * len(self.connections_values[
                                                     sub_plot[0]][sub_plot[1]]),
                                         order='F')
 
             if clim is None:
                 clim = []
                 clim.append(np.round(np.min(self.connections_values[sub_plot[0]]
-                                        [sub_plot[1]]),decimals=2))
+                                        [sub_plot[1]]), decimals=2))
                 clim.append(np.round(np.max(self.connections_values[sub_plot[0]]
-                                   [sub_plot[1]]),decimals = 2))
+                                            [sub_plot[1]]), decimals=2))
 
-            color = self.lines_cmap.map((self.connections_values[sub_plot[0]]
-                                        [sub_plot[1]] - clim[0])/(clim[1] - clim[0]))
+            color = self.lines_cmap.map(
+                (self.connections_values[sub_plot[0]][sub_plot[1]] - clim[0]) /
+                (clim[1] - clim[0]))
             return color, clim
         except Exception as ex:
             print(ex)
 
+    def __calculate_subplot_idx(self, sub_plot):
+        try:
+            _view_idx = sub_plot[1] + self.subplots[1] * sub_plot[0]
+            return _view_idx
+        except Exception as ex:
+            print(ex)
+
+    def __initialize_connections(self):
+        try:
+            subplots = self.subplots
+            if self.n_subplots is None:
+                subplots = (1, 1)
+            self.connections_coords_invariant = np.empty(
+                shape=subplots + (0,)).tolist()
+            self.connections_coords_mutable = np.empty(
+                shape=subplots + (0,)).tolist()
+            self.connections_values = np.empty(shape=subplots + (0,)).tolist()
+            self.lines = np.empty(shape=subplots + (0,)).tolist()
+        except Exception as ex:
+            print(ex)
+
+    def __init_markers(self):
+        try:
+            subplots = self.subplots
+            self.markers = np.empty(shape=subplots + (0,)).tolist()
+        except Exception as ex:
+            print(ex)
+
+    def __init_labels(self):
+        try:
+            subplots = self.subplots
+            self.labels_text = np.empty(shape=subplots + (0,)).tolist()
+        except Exception as ex:
+            print(ex)
+
+    @staticmethod
+    def __extract_conn_values(adj_mat):
+        try:
+            values = np.triu(adj_mat, 1)
+            values = values[np.where(values != 0)]
+            return values
+        except Exception as ex:
+            print(ex)
+
+    @staticmethod
+    def __set_connections_coords(locs, connections_values):
+        try:
+            connections_coords = np.empty((len(connections_values), 2, 3))
+            value_idx = 0
+            for i in range(len(locs)):
+                for j in range(i + 1, len(locs)):
+                    connections_coords[value_idx, 0, 0] = locs[i, 0]
+                    connections_coords[value_idx, 0, 1] = locs[i, 1]
+                    connections_coords[value_idx, 0, 2] = locs[i, 2]
+                    connections_coords[value_idx, 1, 0] = locs[j, 0]
+                    connections_coords[value_idx, 1, 1] = locs[j, 1]
+                    connections_coords[value_idx, 1, 2] = locs[j, 2]
+                    value_idx += 1
+            return connections_coords
+        except Exception as ex:
+            print(ex)
+
     def set_connections(self, adj_mat, locs, sub_plot=None, threshold=0.5,
                         plot_markers=True, labels=None, plot_labels=False,
-                        cmap='seismic', clim = None, cbar = False):
+                        cmap='seismic', clim=None, cbar=False):
         try:
             if sub_plot is None and self.n_subplots == 1:
                 sub_plot = (0, 0)
             assert isinstance(sub_plot, tuple)
             assert sub_plot[0] <= self.subplots[0] and sub_plot[1] <= \
                    self.subplots[1]
             if clim is not None:
@@ -281,42 +343,38 @@
 
             if plot_labels:
                 if labels is None:
                     print("Labels could not been added because labels parameter"
                           "is None")
                 else:
                     assert all(isinstance(elem, str) for elem in labels)
-                    self.set_labels(labels, locs, sub_plot)
+                    self.__set_labels(labels, locs, sub_plot)
 
             if plot_markers:
-                self.set_markers(locs, sub_plot)
-
+                self.__set_markers(locs, sub_plot)
 
             # Extract connectivity values
             self.connections_values[sub_plot[0]][
                 sub_plot[1]] = self.__extract_conn_values(adj_mat)
 
             # Set connections matrix
             self.connections_coords_invariant[sub_plot[0]][
-                sub_plot[1]] = self.__set_connections_coords(locs,
-                                                             self.connections_values
-                                                             [sub_plot[0]][
-                                                                 sub_plot[
-                                                                     1]])
+                sub_plot[1]] = self.__set_connections_coords(
+                locs, self.connections_values
+                [sub_plot[0]][sub_plot[1]])
 
             # Get color map and color connections
             self.lines_cmap = get_colormap(cmap)
             color, clim = self.__set_conn_color(sub_plot, threshold, clim)
 
 
             _view_idx = self.__calculate_subplot_idx(sub_plot)
-            self.lines[sub_plot[0]][sub_plot[1]] = scene.Line(antialias=True,
-                                                              parent=self.views[
-                                                                  _view_idx].scene,
-                                                              )
+            self.lines[sub_plot[0]][sub_plot[1]] = scene.Line(
+                antialias=True,
+                parent=self.views[_view_idx].scene,)
             self.lines[sub_plot[0]][sub_plot[1]].set_data(
                 pos=self.connections_coords_mutable[sub_plot[0]][sub_plot[1]],
                 color=color, width=4)
 
             # Plot color bar (In process)
             if cbar:
                 cbar_widget = scene.ColorBarWidget(clim=clim, cmap=cmap,
@@ -338,109 +396,57 @@
             self.connections_values[sub_plot[0]][
                 sub_plot[1]] = self.__extract_conn_values(adj_mat)
             color = self.__set_conn_color(sub_plot, threshold)
             _view_idx = self.__calculate_subplot_idx(sub_plot)
 
             self.lines[sub_plot[0]][sub_plot[1]].parent = None
 
-            self.lines[sub_plot[0]][sub_plot[1]] = scene.Line(antialias=True,
-                                                              parent=self.views[
-                                                                  _view_idx].scene)
+            self.lines[sub_plot[0]][sub_plot[1]] = scene.Line(
+                antialias=True, parent=self.views[_view_idx].scene)
             self.lines[sub_plot[0]][sub_plot[1]].set_data(
                 pos=self.connections_coords_mutable[sub_plot[0]][sub_plot[1]],
-                color=color, width=4, )
+                color=color, width=4,)
             self.canvas.update()
         except Exception as ex:
             print(ex)
 
-    def __calculate_subplot_idx(self, sub_plot):
-        try:
-            _view_idx = sub_plot[1] + self.subplots[1] * sub_plot[0]
-            return _view_idx
-        except Exception as ex:
-            print(ex)
-
-    def __initialize_connections(self):
-        try:
-            subplots = self.subplots
-            if self.n_subplots is None:
-                subplots = (1, 1)
-            self.connections_coords_invariant = np.empty(
-                shape=subplots + (0,)).tolist()
-            self.connections_coords_mutable = np.empty(
-                shape=subplots + (0,)).tolist()
-            self.connections_values = np.empty(shape=subplots + (0,)).tolist()
-            self.lines = np.empty(shape=subplots + (0,)).tolist()
-        except Exception as ex:
-            print(ex)
-
-    def __init_markers(self):
-        try:
-            subplots = self.subplots
-            self.markers = np.empty(shape=subplots + (0,)).tolist()
-        except Exception as ex:
-            print(ex)
-
-    def __init_labels(self):
-        try:
-            subplots = self.subplots
-            self.labels_text = np.empty(shape=subplots + (0,)).tolist()
-        except Exception as ex:
-            print(ex)
-
-    @staticmethod
-    def __extract_conn_values(adj_mat):
-        try:
-            values = np.triu(adj_mat, 1)
-            values = values[np.where(values != 0)]
-            return values
-        except Exception as ex:
-            print(ex)
-
-    @staticmethod
-    def __set_connections_coords(locs, connections_values):
-        try:
-            connections_coords = np.empty((len(connections_values), 2, 3))
-            value_idx = 0
-            for i in range(len(locs)):
-                for j in range(i + 1, len(locs)):
-                    connections_coords[value_idx, 0, 0] = locs[i, 0]
-                    connections_coords[value_idx, 0, 1] = locs[i, 1]
-                    connections_coords[value_idx, 0, 2] = locs[i, 2]
-                    connections_coords[value_idx, 1, 0] = locs[j, 0]
-                    connections_coords[value_idx, 1, 1] = locs[j, 1]
-                    connections_coords[value_idx, 1, 2] = locs[j, 2]
-                    value_idx += 1
-            return connections_coords
-        except Exception as ex:
-            print(ex)
-
+    def set_activation_map(self, adj_mat, locs, sub_plot=None, threshold=0.5,
+                           plot_markers=True, labels=None, plot_labels=False,
+                           cmap='seismic', clim=None, cbar=False):
+        """Use this function to plot an activation map over the brain's
+        surface
+        """
 
+        pass
 
 
 if __name__ == '__main__':
+
     from vispy.app import use_app
 
     app = use_app("pyqt5")
     app.create()
     # Set canvas
-    triplot = TridimentionalBrain( bg_color='white',
-                                  text_color='black',translucent=[True,True],subplots=(1,2), names=['Prueba1','Prueba2'])
+    
+    triplot = TridimentionalBrain( bg_color='black',
+                                  text_color='white',translucent=[True,True],subplots=(1,2), names=['Prueba1','Prueba2'])
 
     # Define channel set and its coord
     channel_set = EEGChannelSet(dim='3D', coord_system='cartesian')
     channel_set.set_standard_montage(montage='10-20')
     channel_coord = np.zeros((len(channel_set.channels), 3))
     for ch_idx, channel in enumerate(channel_set.channels):
         channel_coord[ch_idx, 0] = 0.8 * (channel['x'])
         channel_coord[ch_idx, 1] = 0.9 * (channel['y'] - 0.2)
         channel_coord[ch_idx, 2] = 0.85 * (channel['z'])
-    adj_mat = np.random.randn(len(channel_set.channels),
+    adj_mat = np.random.rand(len(channel_set.channels),
                               len(channel_set.channels))
-    adj_mat = 2 * adj_mat - 1
-    triplot.set_connections(adj_mat, channel_coord, threshold=[0.6], plot_labels=True,
+
+    # adj_mat = 2 * adj_mat - 1
+    triplot.set_connections(adj_mat, channel_coord, threshold=[0.85], plot_labels=True,
                             labels=channel_set.l_cha, plot_markers=True,cmap='Spectral',sub_plot=(0,0))
     triplot.set_connections(adj_mat, channel_coord, threshold=[0.6], plot_labels=False,
                             labels=channel_set.l_cha, plot_markers=True,cmap='Spectral',sub_plot=(0,1))
     triplot.add_brains()
+
     triplot.canvas.show()
     app.run()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medusa-kernel-1.1.3/medusa/plots/erp_plots.py` & `medusa-kernel-1.2.0/medusa/plots/erp_plots.py`

 * *Files 25% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     return plot_erp(erp_epochs=trials_erp_epochs,
                     noerp_epochs=trials_noerp_epochs,
                     channel=channel,
                     window=window,
                     plot=plot)
 
 
-def plot_erp(erp_epochs, noerp_epochs, channel, window=(0, 1000), plot=True):
+def plot_erp(erp_epochs, noerp_epochs, channel, window=(0, 1000),
+             error_measure="C95", plot=True):
     """Function designed to quickly plot an ERP with 95% confidence interval.
     It does offer limited functions that will be improved in the future.
 
     TODO: a lot of things, very basic functionality
 
 
     Parameters
@@ -75,64 +76,107 @@
         Epochs that contain ERPs (go epochs)
     noerp_epochs: numpy.ndarray
         Epochs that do not contain ERPs (nogo epochs)
     channel: int
         Channel index to plot
     window: list
         List with the lower and upper window time in milliseconds
+    error_measure: str
+        Error measure (default: "C95" or 95% confidence interval). Check
+        parameters of function compute_dev_epochs() for further information.
     plot: bool
         Set to True to plot the ERP
 
     Returns
     -------
     erp_mean: numpy.ndarray
         ERP activity (mean of the go epochs)
     erp_dev: numpy.ndarray
-        95% confidence interval
+        Error measure across observations for ERP activity
     noerp_mean: numpy.ndarray
-        No ERP activity (mean of the nogo epochs)
+        Non-ERP activity (mean of the nogo epochs)
     noerp_dev: numpy.ndarray
-        95% confidence interval
+        Error measure across observations for non-ERP activity
     """
     # Select channel
     erp_epochs = erp_epochs[:, :, channel]
     noerp_epochs = noerp_epochs[:, :, channel]
 
     # Calculate mean and dev measures
     trials_erp_mean = np.mean(erp_epochs, 0)
-    trials_erp_dev = compute_dev_epochs(erp_epochs)
+    trials_erp_dev_pos, trials_erp_dev_neg = \
+        compute_dev_epochs(erp_epochs, measure=error_measure)
     trials_noerp_mean = np.mean(noerp_epochs, 0)
-    trials_noerp_dev = compute_dev_epochs(noerp_epochs)
+    trials_noerp_dev_pos, trials_noerp_dev_neg = \
+        compute_dev_epochs(noerp_epochs, measure=error_measure)
 
     if plot:
         # Plot the data
         t = np.linspace(window[0], window[1], trials_erp_mean.shape[0])
         plt.plot(t, trials_erp_mean)
-        plt.fill_between(t, trials_erp_mean + trials_erp_dev,
-                         trials_erp_mean - trials_erp_dev, alpha=0.3)
+        plt.fill_between(t, trials_erp_dev_neg, trials_erp_dev_pos, alpha=0.3)
         plt.plot(t, trials_noerp_mean)
-        plt.fill_between(t, trials_noerp_mean + trials_noerp_dev,
-                         trials_noerp_mean - trials_noerp_dev, alpha=0.3)
+        plt.fill_between(t, trials_noerp_dev_neg, trials_noerp_dev_pos,
+                         alpha=0.3)
         plt.show()
 
     # Return data
     plot_data = dict()
     plot_data["trials_erp_mean"] = trials_erp_mean
-    plot_data["trials_erp_dev"] = trials_erp_dev
+    plot_data["trials_erp_dev"] = (trials_erp_dev_pos, trials_erp_dev_neg)
     plot_data["trials_noerp_mean"] = trials_noerp_mean
-    plot_data["trials_noerp_dev"] = trials_noerp_dev
+    plot_data["trials_noerp_dev"] = (trials_noerp_dev_pos, trials_noerp_dev_neg)
 
     return plot_data
 
 
+
 def compute_dev_epochs(epochs, measure="C95"):
-    # Compute mean and std
-    std = np.std(epochs, 0)
+    """ Computes the error of a 2D data.
+
+    Parameters
+    -------------
+    epochs: ndarray
+        Data being plotted, with dimensions [observations x signal]
+    error: basestring
+        Type of error being plotted (mean+error, mean-error), which can be:
+        - 'std':    standard deviation
+        - 'sem':    standard error mean
+        - 'var':    variance
+        - Confidence interval:  For this error, the measure parameter must be
+        constituted by 'c' and the desired percentile. E.g. 'c95' for the
+        95% confidence interval, 'c90' for the 90%, 'c99' for the 99%, and
+        so on.
+
+    Returns
+    ----------------
+    pos_deviation: ndarray
+        1D vector containing the positive deviation measure [1 x signal].
+    neg_deviation: ndarray
+        1D vector containing the negative deviation measure [1 x signal].
+    """
+    # Error detection
+    measure = measure.upper()
+    percentile = 95
+    if measure.startswith('C'):
+        percentile = int(measure.split('C')[-1])
+        if percentile >= 100 or percentile <= 0:
+            raise ValueError("[compute_dev_epochs] The confidence interval "
+                             "percentile (%i) must be in the range (0, 100)" %
+                             percentile)
+
     # Compute deviation measure
-    dev = np.zeros([1, epochs.shape[1]])
-    if measure == "C95":
-        dev = (std / np.sqrt(epochs.shape[1])) * 1.96
+    if measure.startswith('C'):
+        pos = np.percentile(epochs, percentile, axis=0)
+        neg = np.percentile(epochs, 100 - percentile, axis=0)
+        return pos, neg
     elif measure == "STD":
-        dev = std
+        pos = np.mean(epochs, axis=0) + np.std(epochs, axis=0)
+        neg = np.mean(epochs, axis=0) - np.std(epochs, axis=0)
+        return pos, neg
     elif measure == "VAR":
-        dev = np.square(std)
-    return dev
+        pos = np.mean(epochs, axis=0) + np.var(epochs, axis=0)
+        neg = np.mean(epochs, axis=0) - np.var(epochs, axis=0)
+        return pos, neg
+    else:
+        raise ValueError("[compute_dev_epochs] Unknown deviation measure %s!"
+                         % measure)
```

### Comparing `medusa-kernel-1.1.3/medusa/plots/generic_plots.py` & `medusa-kernel-1.2.0/medusa/plots/generic_plots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/plots/optimal_subplots.py` & `medusa-kernel-1.2.0/medusa/plots/optimal_subplots.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/plots/topographic_plots.py` & `medusa-kernel-1.2.0/medusa/plots/topographic_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 
 In this module, you will find some functions to represent connectivity graphs
 and topographic plots over a 2D head model. Enjoy!
 
-@authors: Víctor Martínez-Cagigal and Diego Marcos-Martínez
 """
 
 # External imports
 import warnings
 import scipy.interpolate as sp
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 from matplotlib import cm, colors
 import numpy as np
 
 # Medusa imports
 from medusa.meeg import UnlocatedChannel
 
 
+warnings.warn('Module topographic_plots is deprecated and will be removed in '
+              'following versions of MEDUSA Kernel. Use head_plots instead!')
+
+
 def plot_connectivity(channel_set, adj_mat, head_radius=0.7266,
                       plot_channels=True, plot_skin_in_color=True,
                       plot_clabels=True,plot_contour_ch=False,
                       chcontour_radius=None,interp_points=500,
                       cmap='seismic', show=True, clim=None):
 
     """ This function depicts a connectivity map over the
@@ -72,15 +75,15 @@
 
     # Check adjacency matrix  dimensions
     if adj_mat.shape[0] != len(channel_set.channels):
         raise Exception('Adjacency matrix must have the shape '
                         '[n_channels, n_channels]')
 
     # Get connectivity values
-    values_indx = np.tril_indices(adj_mat.shape[0],1)
+    values_indx = np.triu_indices(adj_mat.shape[0],1)
     conn_values = adj_mat[values_indx]
 
     # Map connectivity values to colors
     if clim is None:
         clim = [conn_values.min(),conn_values.max()]
     norm = colors.Normalize(vmin=clim[0],vmax=clim[1],clip=True)
     mapper = cm.ScalarMappable(norm=norm, cmap=cmap)
@@ -511,8 +514,8 @@
     plot_topography(channel_set, dummy_values_topo, plot_clabels=True,
                     plot_contour_ch=True, plot_extra=0.1,
                     plot_skin_in_color=True,cmap='plasma')
 
     # Plot connectivity plot
     plt.figure()
     dummy_values_conn = np.random.randn(16,16)
-    plot_connectivity(channel_set,dummy_values_conn)
+    plot_connectivity(channel_set,dummy_values_conn)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medusa-kernel-1.1.3/medusa/signal_generators.py` & `medusa-kernel-1.2.0/medusa/signal_generators.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa/signal_orthogonalization.py` & `medusa-kernel-1.2.0/medusa/signal_orthogonalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-# from numba import jit
 import warnings
 from medusa.utils import check_dimensions
 
 
 def signal_orthogonalization_cpu(signal_1, signal_2):
 
     """ This method implements the ortogonalization of each channel of signal_1
```

### Comparing `medusa-kernel-1.1.3/medusa/spatial_filtering.py` & `medusa-kernel-1.2.0/medusa/spatial_filtering.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import warnings
+from copy import copy
 import numpy as np
-from medusa import components
 from numpy import linalg as nlinalg
 from scipy import linalg as slinalg
-import warnings
-
+import matplotlib.pyplot as plt
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+from medusa import components
+from medusa.plots.head_plots import TopographicPlot
 
 class LaplacianFilter(components.ProcessingMethod):
     """
     Class for fitting and applying Laplacian Filter to EEG Signals.
     A channel set from EEGChannelSet class must have been defined before calling
     LaplacianFilter class.
 
@@ -221,134 +224,212 @@
         m = np.ones([n_cha, n_cha]) * (-1 / float(n_cha))
         np.fill_diagonal(m, 1 - (1 / float(n_cha)))
         signal = np.dot(signal, m)
     return signal
 
 
 class CSP(components.ProcessingMethod):
-    """ The class CSP performs a Common Spatial Pattern filtering.
+    """ Common Spatial Pattern filtering.
 
     Attributes
     ----------
     filters : {(…, M, M) numpy.ndarray, (…, M, M) matrix}
             Mixing matrix (spatial filters are stored in columns).
     eigenvalues : (…, M) numpy.ndarray
         Eigenvalues of w.
     patterns : numpy.ndarray
         De-mixing matrix (activation patterns are stored in columns).
     """
 
-    def __init__(self, n_filters=4):
+    def __init__(self, n_filters=4, selection="extremes"):
         """
-        n_filter : int or None
-            Number of most discriminant CSP filters to decompose the signal
-            into (must be less or equal to the number of channels in your
-            signal).
-            If int it will return that number of filters.
-            If None it will return all calculated filters."""
-
-        self.filters = None  # Mixing matrix (spatial filters)
-        self.eigenvalues = None  # Eigenvalues
-        self.patterns = None  # De-mixing matrix
-        self.n_filters = n_filters
+
+        Parameters
+        ----------
+        n_filters : int or None
+            Number of filters to select. Use None to return all filters
+            (default: 4).
+        selection : basestring
+            Selection method:
+            - "extremes" (default): classic method that takes the filters
+            from the extremes, which belong to both classes separately. This
+            method cannot be applied in problems with more than 2 classes.
+            - "eigenvalues": the eigenvalues are sorted and the highest ones
+            are eligible to be selected.
+
+        Attributes
+        ----------
+        filters: np.ndarray (n_channels, n_channels)
+            Mixing matrix, or forward model (spatial filters are stored in
+            rows).
+        patterns: np.ndarray (n_channels, n_channels)
+            De-mixing matrix, or backward model (patterns are stored in rows).
+        eigenvalues: np.ndarray (n_channels, )
+            Eigenvalues associated to each filter and pattern.
+        sel_idxs: np.ndarray (n_filters, )
+            Selected indexes to get the desired filters and patterns.
+        sel_filters: np.ndarray (n_filters, n_channels)
+            Selected spatial filters (stored in rows).
+        sel_patterns: np.ndarray (n_filters, n_channels)
+            Selected patterns (stored in rows).
+        sel_eigenvalues: np.ndarray (n_filters, )
+            Selected eigenvalues.
+        """
+        self.n_filters = n_filters      # Number of filters to choose
+        self.selection = selection      # Selection method
+        if self.n_filters is None:
+            self.selection = "none"
+
+        # Generated
+        self.filters = None             # Mixing matrix (spatial filters)
+        self.patterns = None            # De-mixing matrix
+        self.eigenvalues = None         # Eigenvalues
+        self.sel_idxs = None            # Selected indexes
+        self.sel_filters = None         # Selected spatial filters
+        self.sel_patterns = None        # Selected patterns
+        self.sel_eigenvalues = None     # Selected eigenvalues
+        self.is_fitted = False
 
     def fit(self, X, y):
-        """Train Common Spatial Patterns (CSP) filters
+        """ Method to train the CSP.
 
-            Train Common Spatial Patterns (CSP) filters with support to >2
-            classes based on support multiclass CSP by means of approximate
-            joint diagonalization. In this case, the spatial filter selection
-            is achieved according to [1].
+        This code is based on [1] for the 2-class problem, and based on [2]
+        for the > 2-class problem.
 
-            Parameters
-            ----------
-            X : numpy.ndarray, [n_trials, samples, channels]
-                Epoched data of shape (n_trials, samples, channels)
+        Parameters
+        ----------
+        X : numpy.ndarray (n_epochs, n_samples, n_channels)
+            Epoched data of shape (n_epochs, n_samples, n_channels)
 
-            y : numpy.ndarray, [n_trials,]
-                Labels for epoched data of shape (n_trials,)
+        y : numpy.ndarray (n_epochs, )
+            Labels for epoched data of shape (n_epochs, )
 
-            References
-            ----------
-            [1] Grosse-Wentrup, Moritz, and Martin Buss. "Multiclass common
-            spatial patterns and information theoretic feature extraction."
-            Biomedical Engineering, IEEE Transactions on 55, no. 8 (2008):
-            1991-2000.
+        References
+        ----------
+        [1]  Blankertz, B., Tomioka, R., Lemm, S., Kawanabe, M., & Muller,
+        K. R. (2007). Optimizing spatial filters for robust EEG single-trial
+        analysis. IEEE Signal processing magazine, 25(1), 41-56.
+        [2] Grosse-Wentrup, Moritz, and Martin Buss. "Multiclass common
+        spatial patterns and information theoretic feature extraction."
+        Biomedical Engineering, IEEE Transactions on 55, no. 8 (2008):
+        1991-2000.
         """
+        # Error detection
         n_classes = np.unique(y)
+        if len(n_classes) > 2 and self.selection == "extremes":
+            raise ValueError("Cannot use 'extremes' selection if the data has "
+                             "more than 2 classes (%i classess found)!"
+                             % len(n_classes))
+
         # Covariance matrices
         cov = []
         for c in n_classes:
             cov.append(np.cov(X[y == c].reshape(-1, X.shape[-1]).T))
-        cov = np.array(cov)
-        # Classic implementation for 2-class
+        cov = np.array(cov)  # dimensions [n_classes x n_cha x n_cha]
+
+        # Classic implementation for 2 classes
         if len(n_classes) == 2:
             # Solve the eigenvalue problem
-            eigenvalues, filters = slinalg.eigh(cov[0], cov[0] + cov[1])
+            self.eigenvalues, eigenvectors = slinalg.eigh(cov[0], cov.sum(0))
 
             # Indexes for sorting eigenvectors (w)
-            ix_sorted = np.argsort(np.abs(eigenvalues - 0.5))[::-1]
-        # Implementation for >2-classes
+            if self.selection == "eigenvalues":
+                # Automatic sorting using eigenvalues
+                self.sel_idxs = np.argsort(np.abs(self.eigenvalues - 0.5))[::-1]
+                self.sel_idxs = self.sel_idxs[:self.n_filters]
+            # if self.selection == "ratio-of-means":
+            #     proj0 = [np.dot(eigenvectors.T, trial.T) for trial in X[
+            #         y == n_classes[0]]]
+            #     proj0 = np.transpose(np.array(proj0), (0, 2, 1))
+            #     # epochs x filters x channels
+            if self.selection == "extremes":
+                # Automatic selection using extremes for both classes
+                self.sel_idxs = list()
+                ids = np.arange(len(self.eigenvalues)).tolist()
+                start = False
+                while len(self.sel_idxs) < self.n_filters:
+                    if start:
+                        self.sel_idxs.append(ids.pop(0))
+                    else:
+                        self.sel_idxs.append((ids.pop(len(ids) - 1)))
+                    start = not start
+
+        # Implementation for more than 2 classes
         elif len(n_classes) > 2:
             # Approximate joint diagonalization based on jacobi angle
-            filters, d = self.adj_pham(x=cov)
+            filters, d = self._adj_pham(x=cov)
             filters = filters.T
             # Normalization
             # Mean covariance
             cmean = np.average(cov, axis=0)
             for i in range(filters.shape[1]):
                 temp = np.dot(np.dot(filters[:, i].T, cmean), filters[:, i])
                 filters[:, i] /= np.sqrt(temp)
             # We calculate the probability of each class
-            info = []
+            self.eigenvalues = []
             prob_class = [np.mean(y == c) for c in n_classes]
             for j in range(filters.shape[1]):
                 patterns, b = 0, 0
                 for i, c in enumerate(n_classes):
-                    temp = np.dot(np.dot(filters[:, j].T, cov[i]), filters[:, j])
+                    temp = np.dot(np.dot(filters[:, j].T, cov[i]),
+                                  filters[:, j])
                     patterns += prob_class[i] * np.log(np.sqrt(temp))
                     b += prob_class[i] * (temp ** 2 - 1)
                 mutual_info = - (patterns + (3.0 / 16) * (b ** 2))
-                info.append(mutual_info)
-            eigenvalues = info
-            # Indexes for sorting eigenvectors (w)
-            ix_sorted = np.argsort(info)[::-1]
+                self.eigenvalues.append(mutual_info)
+
+            # Indexes for sorting eigenvalues (w)
+            if self.selection == "eigenvalues":
+                self.sel_idxs = np.argsort(self.eigenvalues)[::-1]
+                self.sel_idxs = self.sel_idxs[:self.n_filters]
         else:
             raise ValueError("Number of classes must be  >= 2")
-        # Sort eigenvectors (w)
-        filters = filters[:, ix_sorted]
-        eigenvalues = [eigenvalues[i] for i in ix_sorted]
-        eigenvalues = np.diag(eigenvalues)
-        # Activation spatial patterns
-        # patterns = slinalg.pinv2(filters).T   # deprecated and removed in scipy 1.9.0
-        patterns = slinalg.pinv(filters).T
-
-        # Attribute storing of number of filters
-        self.filters = filters[:, :self.n_filters].T
-        self.eigenvalues = eigenvalues
-        self.patterns = patterns[:, :self.n_filters].T
+
+        # Get all the spatial filters, patterns and eigenvalues (non-sorted)
+        self.filters = eigenvectors.T
+        self.patterns = slinalg.pinv(eigenvectors)
+        self.eigenvalues = np.array(self.eigenvalues)
+
+        # Get the selected spatial filters, patterns and eigenvalues
+        if self.sel_idxs is not None:
+            self.sel_filters = self.filters[self.sel_idxs, :]
+            self.sel_patterns = self.patterns[self.sel_idxs, :]
+            self.sel_eigenvalues = self.eigenvalues[self.sel_idxs]
+        else:
+            self.sel_filters = self.filters
+            self.sel_patterns = self.patterns
+            self.sel_eigenvalues = self.eigenvalues
+        self.is_fitted = True
 
     def project(self, X):
-        """ This method projects the input data X with the spatial filters W
+        """ Projects the input data X with the selected spatial filters.
 
         Parameters
         ----------
-        X : numpy.ndarray [n_trials, samples, channels]
-            Input data (dimensions [n_trials, samples, channels])
+        X : numpy.ndarray (n_epochs, n_samples, n_channels)
+            Epoched data of shape (n_epochs, n_samples, n_channels).
 
         Returns
         -------
-        numpy.ndarray [n_trials, n_filters, samples]
-            Array with the epochs of signal projected in the CSP space
+        numpy.ndarray (n_epochs, n_filters, n_channels)
+            Array with the epochs of signal projected in the CSP space.
         """
-        if self.filters is None:
+        if len(X.shape) != 3:
+            raise Exception("X must be 3-dimensional (n_epochs x n_samples x "
+                            "n_channels!")
+        if not self.is_fitted:
             raise Exception("CSP must be fitted first")
-        return np.matmul(self.filters, X.transpose((0, 2, 1)))
 
-    def adj_pham(self, x, eps=1e-6, n_iter_max=15):
+        # Project each trial separately
+        projection = [np.dot(self.sel_filters, trial.T) for trial in X]
+        projection = np.transpose(np.array(projection), (0, 2, 1))
+        return projection
+
+    @staticmethod
+    def _adj_pham(x, eps=1e-6, n_iter_max=15):
         """Approximate joint diagonalization based on pham's algorithm.
             This is a direct implementation of the PHAM's AJD algorithm [1].
             Extracted from pyriemann module:
             http://github.com/alexandrebarachant/pyRiemann
 
             Parameters
             ----------
@@ -423,26 +504,121 @@
                     v[[ii, jj], :] = np.dot(tau, v[[ii, jj], :])
             if decr < epsilon:
                 break
         d = np.reshape(a, (n_times, -1, n_times)).transpose(1, 0, 2)
         return v, d
 
     def to_dict(self):
-        return self.__dict__
+        dict_ = copy(self.__dict__)
+        for key, value in dict_.items():
+            if isinstance(value, np.ndarray):
+                dict_[key] = value.tolist()
+        return dict_
 
     @staticmethod
     def from_dict(dict_data):
         csp = CSP()
-        csp.filters = dict_data['filters']
-        csp.eigenvalues = dict_data['eigenvalues']
-        csp.patterns = dict_data['patterns']
         csp.n_filters = dict_data['n_filters']
+        csp.selection = dict_data['selection']
+        csp.filters = np.array(dict_data['filters'])
+        csp.patterns = np.array(dict_data['patterns'])
+        csp.eigenvalues = np.array(dict_data['eigenvalues'])
+        csp.sel_idxs = np.array(dict_data['sel_idxs'])
+        csp.sel_filters = np.array(dict_data['sel_filters'])
+        csp.sel_patterns = np.array(dict_data['sel_patterns'])
+        csp.sel_eigenvalues = np.array(dict_data['sel_eigenvalues'])
         return csp
 
+    def plot(self, channel_set, figure=None, plot_filters=False,
+             plot_patterns=True, topo_settings=None, show=False,
+             plot_eig=True, only_selected=True):
+        # Error detection and initialization
+        if not plot_patterns and not plot_filters:
+            raise Exception("Cannot plot CSP if plot_filters and "
+                            "plot_patterns are both None")
+        if figure is None:
+            figure = plt.figure(figsize=(7.5, 3), dpi=300)
+        if len(channel_set.l_cha) != self.sel_filters.shape[1]:
+            raise Exception("The number of channels (%i) must be the same as "
+                            "the number of channels used to train the CSP ("
+                            "%i)" % (len(channel_set.l_cha),
+                                     self.sel_filters.shape[1]))
+        if topo_settings is None:
+            topo_settings = {
+                "head_radius": 1.0,
+                "head_line_width": 2,
+                "interp_contour_width": 1,
+                "interp_points": 500,
+            }
+        if only_selected:
+            sel_patterns = self.sel_patterns
+            sel_filters = self.sel_filters
+            sel_eigenvalues = self.sel_eigenvalues
+        else:
+            sel_patterns = self.patterns
+            sel_filters = self.filters
+            sel_eigenvalues = self.eigenvalues
 
+        # Parameters
+        n_row = 2 if plot_patterns and plot_filters else 1
+        max_f = 0
+        max_p = 0
+        for i in range(sel_filters.shape[0]):
+            if np.max(np.abs(sel_patterns[i, :])) > max_p:
+                max_p = np.max(np.abs(sel_patterns[i, :]))
+            if np.max(np.abs(sel_filters[i, :])) > max_f:
+                max_f = np.max(np.abs(sel_filters[i, :]))
+
+        # Plot filters
+        j = 0
+        if plot_filters:
+            for j in range(sel_filters.shape[0]):
+                ax = figure.add_subplot(n_row, sel_filters.shape[0], j + 1)
+                topo_settings["clim"] = (-max_f, max_f)
+                topo_settings["cmap"] = "RdBu"
+                topo = TopographicPlot(axes=ax, channel_set=channel_set,
+                                       **topo_settings)
+                topo.update(values=sel_filters[j, :])
+                ax.set_title("Filter %i" % j)
+                if plot_eig and not plot_patterns:
+                    ax.set_xlabel('Eig: %.3f' % sel_eigenvalues[j])
+                # Colorbar
+                if j == sel_filters.shape[0] - 1:
+                    divider = make_axes_locatable(ax)
+                    cax = divider.append_axes('right', size='5%', pad=0.05)
+                    cbar = figure.colorbar(
+                        topo.plot_handles["color-mesh"], cax=cax,
+                        orientation='vertical')
+            j += 1
+
+        # Plot patterns
+        if plot_patterns:
+            for i in range(sel_filters.shape[0]):
+                ax = figure.add_subplot(n_row, sel_filters.shape[0], j + i + 1)
+                topo_settings["clim"] = (-max_p, max_p)
+                topo_settings["cmap"] = "PiYG"
+                topo = TopographicPlot(axes=ax, channel_set=channel_set,
+                                       **topo_settings)
+                topo.update(values=sel_patterns[i, :])
+                ax.set_title("Pattern %i" % i)
+                if plot_eig:
+                    ax.set_xlabel('Eig: %.3f' % sel_eigenvalues[i])
+                # Colorbar
+                if i == sel_filters.shape[0] - 1:
+                    divider = make_axes_locatable(ax)
+                    cax = divider.append_axes('right', size='5%', pad=0.05)
+                    cbar = figure.colorbar(
+                        topo.plot_handles["color-mesh"], cax=cax,
+                        orientation='vertical')
+        plt.suptitle("CSP")
+
+        # Show?
+        if show:
+            plt.show()
+        return figure
 class CCA(components.ProcessingMethod):
     """
     The class CCA performs a Canonical Correlation Analysis filtering. First,
     function fit() sould be called to train the spatial filters. Then, spatial
     filters could be used to project testing data. After fit(), the following
     attributes are computed:
```

### Comparing `medusa-kernel-1.1.3/medusa/tensorflow_integration.py` & `medusa-kernel-1.2.0/medusa/tensorflow_integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-"""Created on Monday March 15 19:27:14 2021
+import os, warnings
 
-This module provides
+try:
+    import tensorflow as tf
+    import tensorflow_probability as tfp
+    os.environ["MEDUSA_EXTRAS_GPU_TF"] = "1"
+except:
+    os.environ["MEDUSA_EXTRAS_GPU_TF"] = "0"
 
-@author: Eduardo Santamaría-Vázquez
-"""
 
-import tensorflow as tf
-import os
-import warnings
+class TFExtrasNotInstalled(Exception):
+    def __init__(self):
+        super().__init__(
+            'This functionality requires GPU-TF extras. Install '
+            'medusa-kernel with GPU-TF extras with "pip install '
+            'medusa-kernel[GPU-TF]')
 
 
 class NoGPU(Exception):
     def __init__(self):
         super().__init__('No GPU available')
 
 
@@ -37,14 +43,17 @@
         Enables GPU acceleration. The function will check if this feature is
         available and select the proper device.
     device: str, optional
         Device that will be selected. Use tf.config.list_logical_devices() to
         list the current available devices.
     """
     try:
+        if os.environ.get("MEDUSA_EXTRAS_GPU_TF") != '1':
+            raise TFExtrasNotInstalled()
+
         if int(tf.__version__.split('.')[0]) < 2:
             raise ImportError('Tensorflow >= 2.0.0 is required for GPU '
                               'acceleration')
         # Get available devices
         gpus = tf.config.list_logical_devices(device_type='GPU')
         cpus = tf.config.list_logical_devices(device_type='CPU')
         if gpu_acceleration:
@@ -89,28 +98,31 @@
         print('Selected device: %s' % os.environ["MEDUSA_TF_DEVICE"])
 
     except ModuleNotFoundError:
         raise ModuleNotFoundError('Tensorflow is not installed')
 
 
 def check_tf_config(autoconfig=False):
-    """Checks if tensorflow has been configured
+    """Checks if tensorflow has been configured.
 
      Parameters
     ----------
     autoconfig: bool
         If tensorflow has not been configured and autoconfig is True,
         tensorflow is configured automatically, trying GPU first.
     """
-    check = True if os.environ.get("MEDUSA_TF_GPU_ACCELERATION") is not None \
-        else False
-    if not check and autoconfig:
-        __auto_config_tensorflow()
-        check = True if os.environ.get("MEDUSA_TF_GPU_ACCELERATION") is not \
-                        None else False
+    if os.environ.get("MEDUSA_EXTRAS_GPU_TF") == '1':
+        check = 1 if os.environ.get("MEDUSA_TF_GPU_ACCELERATION") \
+                     is not None else 0
+        if not check and autoconfig:
+            __auto_config_tensorflow()
+            check = 1 if os.environ.get("MEDUSA_TF_GPU_ACCELERATION") \
+                         is not None else 0
+    else:
+        check = -1
     return check
 
 
 def check_gpu_acceleration():
     """Checks if there is GPU acceleration available"""
     # Check configuration
     if not check_tf_config():
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `medusa-kernel-1.1.3/medusa/transforms.py` & `medusa-kernel-1.2.0/medusa/transforms.py`

 * *Files identical despite different names*

### Comparing `medusa-kernel-1.1.3/medusa_kernel.egg-info/PKG-INFO` & `medusa-kernel-1.2.0/medusa_kernel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: medusa-kernel
-Version: 1.1.3
+Version: 1.2.0
 Summary: Advanced biosignal processing toolbox
 Home-page: https://medusabci.com/
 Author: Eduardo Santamaría-Vázquez, Víctor Martínez-Cagigal, Diego Marcos-Martínez, Víctor Rodríguez-González, Sergio Pérez-Velasco
 Author-email: support@medusabci.com
 License: CC Attribution-NonCommercial-NoDerivs 2.0
 Keywords: Signal,Biosignal,EEG,BCI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
+Provides-Extra: TF
 License-File: LICENSE
 
 # MEDUSA© Kernel
 
 MEDUSA© is a software ecosystem for the development of BCIs and neuroscience experiments. It has two independent components with dfferent goals: MEDUSA© Kernel and MEDUSA© Platform. 
 
 MEDUSA© Kernel is a Python package that contains readyto- use methods to analyze brain signals, including advanced signal processing, machine learning, deep learning, and miscellaneous high-level analyses. It also includes logical functions and classes to handle different biosignals, such as electroencephalography (EEG) and magnetoencephalography (MEG), save experimental data or implement standalone processing pipelines.
```

### Comparing `medusa-kernel-1.1.3/medusa_kernel.egg-info/SOURCES.txt` & `medusa-kernel-1.2.0/medusa_kernel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 medusa/deep_learning_models.py
 medusa/emg.py
 medusa/epoching.py
 medusa/frequency_filtering.py
 medusa/nirs.py
 medusa/notify_me.py
 medusa/optimization.py
-medusa/pearson_corr_matrix.py
 medusa/performance_analysis.py
 medusa/signal_generators.py
 medusa/signal_orthogonalization.py
 medusa/spatial_filtering.py
 medusa/tensorflow_integration.py
 medusa/transforms.py
 medusa/utils.py
@@ -57,14 +56,15 @@
 medusa/meeg/eeg_standard_10-20_3D.tsv
 medusa/meeg/meeg.py
 medusa/meeg/meeg_montages.py
 medusa/plots/__init__.py
 medusa/plots/brain_plots.py
 medusa/plots/erp_plots.py
 medusa/plots/generic_plots.py
+medusa/plots/head_plots.py
 medusa/plots/mi_plots.py
 medusa/plots/optimal_subplots.py
 medusa/plots/timeplot.py
 medusa/plots/topographic_plots.py
 medusa_kernel.egg-info/PKG-INFO
 medusa_kernel.egg-info/SOURCES.txt
 medusa_kernel.egg-info/dependency_links.txt
```

### Comparing `medusa-kernel-1.1.3/setup.py` & `medusa-kernel-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
-# Just testing
-
-# read the contents of your README file
+# Read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='medusa-kernel',
     packages=find_packages(),
-    version='1.1.3',
+    version='1.2.0',
     keywords=['Signal', 'Biosignal', 'EEG', 'BCI'],
     url='https://medusabci.com/',
     author='Eduardo Santamaría-Vázquez, '
            'Víctor Martínez-Cagigal, '
            'Diego Marcos-Martínez, '
            'Víctor Rodríguez-González, '
            'Sergio Pérez-Velasco',
     author_email='support@medusabci.com',
-    license='CC Attribution-NonCommercial-NoDerivs 2.0',
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'scikit-learn',
         'statsmodels',
         'bson',
         'h5py',
         'dill',
         'tqdm',
-        'tensorflow==2.11',
-        'tensorflow-probability==0.16'
+        'statsmodels',
+        'PyQt5'
     ],
+    extras_require={
+        'TF': [
+            'tensorflow<2.11',
+            'tensorflow-probability==0.16'
+        ],
+    },
+    python_requires='>=3.8, <3.11',
+    package_data={
+        'medusa': ['meeg/*.tsv', 'local_activation/*.dll']
+    },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
-        'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3 :: Only',
     ],
     description='Advanced biosignal processing toolbox',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    package_data={
-        'medusa': ['meeg/*.tsv', 'local_activation/*.dll']
-    },
+    license='CC Attribution-NonCommercial-NoDerivs 2.0',
     license_files=('LICENSE',),
 )
```

