# Comparing `tmp/cdlib-0.2.6.tar.gz` & `tmp/cdlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdlib-0.2.6.tar", last modified: Tue Mar  8 15:28:33 2022, max compression
+gzip compressed data, was "cdlib-0.3.0.tar", last modified: Thu Jun  8 09:23:51 2023, max compression
```

## Comparing `cdlib-0.2.6.tar` & `cdlib-0.3.0.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.903044 cdlib-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-03-08 15:28:19.000000 cdlib-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-03-08 15:28:19.000000 cdlib-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7944 2022-03-08 15:28:33.903044 cdlib-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7170 2022-03-08 15:28:19.000000 cdlib-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.891043 cdlib-0.2.6/cdlib/
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.891043 cdlib-0.2.6/cdlib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5270 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/attribute_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)    10733 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/bipartite_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)   100857 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/crisp_partition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/edge_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/algorithms/internal/
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/AGDL.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/BIGCLAM.py
--rw-r--r--   0 runner    (1001) docker     (121)     5597 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/COACH.py
--rw-r--r--   0 runner    (1001) docker     (121)    22041 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/CONGA.py
--rw-r--r--   0 runner    (1001) docker     (121)    23967 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/CONGO.py
--rw-r--r--   0 runner    (1001) docker     (121)    14836 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/DCS.py
--rw-r--r--   0 runner    (1001) docker     (121)     8951 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/DER.py
--rw-r--r--   0 runner    (1001) docker     (121)    15849 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/DPCLUS.py
--rw-r--r--   0 runner    (1001) docker     (121)     5591 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/EBGC.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/EnDNTM.py
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/FuzzyCom.py
--rw-r--r--   0 runner    (1001) docker     (121)     5175 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/GDMP2_nx.py
--rw-r--r--   0 runner    (1001) docker     (121)     8289 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/HLC.py
--rw-r--r--   0 runner    (1001) docker     (121)    17307 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/ILouvain.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/IPCA.py
--rw-r--r--   0 runner    (1001) docker     (121)     3718 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/Kcut.py
--rw-r--r--   0 runner    (1001) docker     (121)     4182 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/LAIS2_nx.py
--rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/LEMON.py
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/LPAM.py
--rw-r--r--   0 runner    (1001) docker     (121)     6237 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/LPANNI.py
--rw-r--r--   0 runner    (1001) docker     (121)    22727 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/LSWL.py
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/MCODE.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/Markov.py
--rw-r--r--   0 runner    (1001) docker     (121)    13034 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/NodePerception.py
--rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/OSSE.py
--rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/PercoMCV.py
--rw-r--r--   0 runner    (1001) docker     (121)     7341 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/RSC.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/SLPA_nx.py
--rw-r--r--   0 runner    (1001) docker     (121)    28999 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/SiblinarityAntichain.py
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/UMSTMO.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8421 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/belief_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)    10569 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/core_exp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2806 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/em.py
--rw-r--r--   0 runner    (1001) docker     (121)     4737 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/ga.py
--rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/graph_entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/headtail.py
--rw-r--r--   0 runner    (1001) docker     (121)     3961 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/lfm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5742 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/modularity_m.py
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/modularity_r.py
--rw-r--r--   0 runner    (1001) docker     (121)     9827 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/multicom.py
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/paris.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/principled.py
--rw-r--r--   0 runner    (1001) docker     (121)     6986 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/pycondor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/spectralCD.py
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/walkscan.py
--rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal/weightedCommunity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/algorithms/internal_dcd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal_dcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13960 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/internal_dcd/eTILES.py
--rw-r--r--   0 runner    (1001) docker     (121)    69458 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/overlapping_partition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/algorithms/temporal_partition.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/benchmark/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/benchmark/dynamic_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/benchmark/internal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/benchmark/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19426 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/benchmark/internal/rdyn.py
--rw-r--r--   0 runner    (1001) docker     (121)    12369 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/benchmark/internal/xmark.py
--rw-r--r--   0 runner    (1001) docker     (121)    15939 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/benchmark/static_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/classes/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/attr_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/bipartite_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/edge_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/fuzzy_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/named_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)    38635 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     9396 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/classes/temporal_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15225 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/datasets/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/ensemble/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10811 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/ensemble/bunch_executions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18822 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)     9237 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/comparisonranking.py
--rw-r--r--   0 runner    (1001) docker     (121)    43486 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/fitness.py
--rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/fitnessranking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.899043 cdlib-0.2.6/cdlib/evaluation/internal/
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/internal/TOPSIS.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4057 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/internal/link_modularity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/internal/omega.py
--rw-r--r--   0 runner    (1001) docker     (121)     4971 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/internal/onmi.py
--rw-r--r--   0 runner    (1001) docker     (121)     4001 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/evaluation/internal/statistical_ranking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.903044 cdlib-0.2.6/cdlib/readwrite/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/readwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5901 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/readwrite/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     7419 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.903044 cdlib-0.2.6/cdlib/viz/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7434 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/viz/networks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-03-08 15:28:19.000000 cdlib-0.2.6/cdlib/viz/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 15:28:33.891043 cdlib-0.2.6/cdlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7944 2022-03-08 15:28:33.000000 cdlib-0.2.6/cdlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-03-08 15:28:33.000000 cdlib-0.2.6/cdlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-08 15:28:33.000000 cdlib-0.2.6/cdlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-03-08 15:28:33.000000 cdlib-0.2.6/cdlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-08 15:28:33.000000 cdlib-0.2.6/cdlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-03-08 15:28:19.000000 cdlib-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-03-08 15:28:33.903044 cdlib-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-03-08 15:28:19.000000 cdlib-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 09:23:40.000000 cdlib-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 09:23:40.000000 cdlib-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-08 09:23:51.870546 cdlib-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-08 09:23:40.000000 cdlib-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.858546 cdlib-0.3.0/cdlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.862546 cdlib-0.3.0/cdlib/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/attribute_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/bipartite_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104945 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/crisp_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/edge_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/algorithms/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/AGDL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/BIGCLAM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/COACH.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22041 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/CONGA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/CONGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/DCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/DER.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/DPCLUS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/EBGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/EnDNTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/FuzzyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/GDMP2_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/HLC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17301 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/ILouvain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/IPCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/Kcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LAIS2_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LEMON.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LPAM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LPANNI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/LSWL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/MCODE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/Markov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/NodePerception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/OSSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/PercoMCV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/RSC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/SLPA_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29121 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/SiblinarityAntichain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/UMSTMO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/belief_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/core_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/ga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/graph_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/headtail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/lfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/modularity_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/modularity_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/multicom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/paris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/principled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/pycondor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/spectralCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/walkscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal/weightedCommunity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/algorithms/internal_dcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal_dcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/internal_dcd/eTILES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70332 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/overlapping_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/algorithms/temporal_partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/dynamic_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.866546 cdlib-0.3.0/cdlib/benchmark/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/internal/rdyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/internal/xmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/benchmark/static_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/attr_node_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/bipartite_node_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/edge_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/fuzzy_node_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/named_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38635 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/node_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/classes/temporal_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/datasets/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/ensemble/bunch_executions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/comparisonranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/fitnessranking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/evaluation/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/TOPSIS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/link_modularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/onmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/evaluation/internal/statistical_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/prompt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/readwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/readwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/readwrite/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.870546 cdlib-0.3.0/cdlib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/viz/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-08 09:23:40.000000 cdlib-0.3.0/cdlib/viz/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:23:51.862546 cdlib-0.3.0/cdlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 09:23:51.000000 cdlib-0.3.0/cdlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 09:23:40.000000 cdlib-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 09:23:51.870546 cdlib-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-08 09:23:40.000000 cdlib-0.3.0/setup.py
```

### Comparing `cdlib-0.2.6/LICENSE` & `cdlib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/PKG-INFO` & `cdlib-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: cdlib
-Version: 0.2.6
+Version: 0.3.0
 Summary: Community Discovery Library
 Home-page: https://github.com/GiulioRossetti/cdlib
 Author: Giulio Rossetti
 Author-email: giulio.rossetti@gmail.com
 License: BSD-Clause-2
 Keywords: community-discovery node-clustering edge-clustering complex-networks
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: C
+Provides-Extra: pypi
+Provides-Extra: all
 License-File: LICENSE
 
-# CDlib - Community Discovery Library
+# CDlib - Community Detection Library
 [![codecov](https://codecov.io/gh/GiulioRossetti/cdlib/branch/master/graph/badge.svg?token=3YJOEVK02B)](https://codecov.io/gh/GiulioRossetti/cdlib)
 [![Build](https://github.com/GiulioRossetti/cdlib/actions/workflows/python-package.yml/badge.svg)](https://github.com/GiulioRossetti/cdlib/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/cdlib/badge/?version=latest)](http://cdlib.readthedocs.io/en/latest/?badge=latest)
 [![CodeQL](https://github.com/GiulioRossetti/cdlib/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/GiulioRossetti/cdlib/actions/workflows/codeql-analysis.yml)
-[![Updates](https://pyup.io/repos/github/GiulioRossetti/cdlib/shield.svg)](https://pyup.io/repos/github/GiulioRossetti/cdlib/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/GiulioRossetti/nclib.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/GiulioRossetti/nclib/context:python)
 [![pyversions](https://img.shields.io/pypi/pyversions/cdlib.svg)](https://badge.fury.io/py/cdlib)
 [![PyPI version](https://badge.fury.io/py/cdlib.svg)](https://badge.fury.io/py/cdlib)
 [![Anaconda-Server Badge](https://anaconda.org/giuliorossetti/cdlib/badges/version.svg)](https://anaconda.org/giuliorossetti/cdlib)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/cdlib/month)](https://pepy.tech/project/cdlib)
 [![Downloads](https://pepy.tech/badge/cdlib)](https://pepy.tech/project/cdlib)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4575156.svg)](https://doi.org/10.5281/zenodo.4575156)
 [![SBD++](https://img.shields.io/badge/Available%20on-SoBigData%2B%2B-green)](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853)
 
 
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/_CDlib_.svg?style=social&label=Follow%20%40_CDlib_)](https://twitter.com/_CDlib_)
 
-<!---
-[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FGiulioRossetti%2Fcdlib.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FGiulioRossetti%2Fcdlib?ref=badge_shield)
---->
 
-``CDlib`` is a meta-library for community discovery in complex networks: it implements algorithms, clustering fitness functions as well as visualization facilities.
+
+``CDlib`` is a meta-library for community detection in complex networks: it implements algorithms, clustering fitness functions as well as visualization facilities.
 
 
 ``CDlib`` is designed around the ``networkx`` python library: however, when needed, it takes care to automatically convert (from and to) ``igraph`` object so to provide an abstraction on specific algorithm implementations to the final user.
 
 ``CDlib`` provides a standardized input/output facilities for several Community Discovery algorithms: whenever possible, to guarantee literature coherent results, implementations of CD algorithms are inherited from their original projects (acknowledged on the [documentation](https://cdlib.readthedocs.io)).
 
 
@@ -79,40 +76,48 @@
 Alternatively use pip
 ```bash
 pip install cdlib
 ```
 
 or conda
 ```bash
+conda create -n cdlib python=3.9
 conda config --add channels giuliorossetti
 conda config --add channels conda-forge
 conda install cdlib
 ```
 
 ### Optional Dependencies (pip package)
-``CDlib`` relies on a few packages calling C code that can be cumbersome to install on Windows machines: to address such issue, the default installation does not try to install set up such requirements.
+To simplify the installation process, the default installation does not include optional dependencies (e.g., ``graph-tool``). If you need them, you can install them manually or run the following command:
 
-Such a choice has been made to allow (even) non *unix user to install the library and get access to its core functionalities. 
+```bash
+pip install cdlib[C]
+```
 
-To integrate the standard installation with you can either:
+This option, safe for *nix users, will install all those optional dependencies that require C code compilation.
 
-- (Windows) manually install the optional packages (versions details are specified in ``requirements_optional.txt``) following the original projects guidelines, or
-- (Linux/OSX) run the command:
+```bash
+pip install cdlib[pypi]
+```
+
+This option will install all those optional dependencies that are not available on conda/conda-forge.
 
 ```bash
-pip install cdlib[C]
+pip install cdlib[all]
 ```
 
-Such caveat will install everything that can be easily automated under Linux/OSX. 
+This option will install all optional dependencies accessible with the flag ``C`` and ``pypi``.
 
 #### (Advanced) 
 
-##### Graph-tool
-The only optional dependency that will remain unsatisfied following the previous procedures will be ``graph-tool`` (used to add SBM models). 
-If you need it up and running, refer to the official [documentation](https://git.skewed.de/count0/graph-tool/wikis/installation-instructions) and install the conda-forge version of the package.
+Due to some strict requirements, the installation of a subset of optional dependencies is left outside the previous procedures.
+
+##### graph-tool
+``CDlib`` integrates the support for SBM models offered by ``graph-tool``.
+To install it refer to the official [documentation](https://git.skewed.de/count0/graph-tool/wikis/installation-instructions) and install the conda-forge version of the package (or the deb version if in a *nix system).
 
 ##### ASLPAw
 
 Since its 2.1.0 release ``ASLPAw`` relies on ``gmpy2`` whose installation through pip is not easy to automatize due to some C dependencies.
 To address such issue test the following recipe:
 
 ```bash
@@ -120,15 +125,15 @@
 pip install shuffle_graph>=2.1.0 similarity-index-of-label-graph>=2.0.1 ASLPAw>=2.1.0
 ```
 
 In case this does not solve the issue, please refer to the official ``gmpy2`` [installation](https://gmpy2.readthedocs.io/en/latest/intro.html#installation) instructions.
 
 ### Optional Dependencies (Conda package)
 
-``CDlib`` relies on a few packages not available through conda: to install it please use pip:
+``CDlib`` relies on a few packages not available through conda: to install them please use pip.
 
 ```bash
 pip install pycombo
 pip install GraphRicciCurvature
 
 conda install gmpy2 
 pip install shuffle_graph>=2.1.0 similarity-index-of-label-graph>=2.0.1 ASLPAw>=2.1.0
@@ -144,9 +149,7 @@
 If you like to include your model in CDlib feel free to fork the project, open an issue and contact us.
 
 ### How to contribute to this project?
 
 Contributing is good, doing it correctly is better! Check out our [rules](https://github.com/GiulioRossetti/cdlib/blob/master/.github/CONTRIBUTING.md), issue a proper [pull request](https://github.com/GiulioRossetti/cdlib/blob/master/.github/PULL_REQUEST_TEMPLATE.md) /[bug report](https://github.com/GiulioRossetti/cdlib/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) / [feature request](https://github.com/GiulioRossetti/cdlib/blob/master/.github/ISSUE_TEMPLATE/feature_request.md).
 
 We are a welcoming community... just follow the [Code of Conduct](https://github.com/GiulioRossetti/cdlib/blob/master/.github/CODE_OF_CONDUCT.md).
-
-
```

### Comparing `cdlib-0.2.6/README.md` & `cdlib-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-# CDlib - Community Discovery Library
+# CDlib - Community Detection Library
 [![codecov](https://codecov.io/gh/GiulioRossetti/cdlib/branch/master/graph/badge.svg?token=3YJOEVK02B)](https://codecov.io/gh/GiulioRossetti/cdlib)
 [![Build](https://github.com/GiulioRossetti/cdlib/actions/workflows/python-package.yml/badge.svg)](https://github.com/GiulioRossetti/cdlib/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/cdlib/badge/?version=latest)](http://cdlib.readthedocs.io/en/latest/?badge=latest)
 [![CodeQL](https://github.com/GiulioRossetti/cdlib/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/GiulioRossetti/cdlib/actions/workflows/codeql-analysis.yml)
-[![Updates](https://pyup.io/repos/github/GiulioRossetti/cdlib/shield.svg)](https://pyup.io/repos/github/GiulioRossetti/cdlib/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/GiulioRossetti/nclib.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/GiulioRossetti/nclib/context:python)
 [![pyversions](https://img.shields.io/pypi/pyversions/cdlib.svg)](https://badge.fury.io/py/cdlib)
 [![PyPI version](https://badge.fury.io/py/cdlib.svg)](https://badge.fury.io/py/cdlib)
 [![Anaconda-Server Badge](https://anaconda.org/giuliorossetti/cdlib/badges/version.svg)](https://anaconda.org/giuliorossetti/cdlib)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/cdlib/month)](https://pepy.tech/project/cdlib)
 [![Downloads](https://pepy.tech/badge/cdlib)](https://pepy.tech/project/cdlib)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4575156.svg)](https://doi.org/10.5281/zenodo.4575156)
 [![SBD++](https://img.shields.io/badge/Available%20on-SoBigData%2B%2B-green)](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853)
 
 
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/_CDlib_.svg?style=social&label=Follow%20%40_CDlib_)](https://twitter.com/_CDlib_)
 
-<!---
-[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FGiulioRossetti%2Fcdlib.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FGiulioRossetti%2Fcdlib?ref=badge_shield)
---->
 
-``CDlib`` is a meta-library for community discovery in complex networks: it implements algorithms, clustering fitness functions as well as visualization facilities.
+
+``CDlib`` is a meta-library for community detection in complex networks: it implements algorithms, clustering fitness functions as well as visualization facilities.
 
 
 ``CDlib`` is designed around the ``networkx`` python library: however, when needed, it takes care to automatically convert (from and to) ``igraph`` object so to provide an abstraction on specific algorithm implementations to the final user.
 
 ``CDlib`` provides a standardized input/output facilities for several Community Discovery algorithms: whenever possible, to guarantee literature coherent results, implementations of CD algorithms are inherited from their original projects (acknowledged on the [documentation](https://cdlib.readthedocs.io)).
 
 
@@ -57,40 +53,48 @@
 Alternatively use pip
 ```bash
 pip install cdlib
 ```
 
 or conda
 ```bash
+conda create -n cdlib python=3.9
 conda config --add channels giuliorossetti
 conda config --add channels conda-forge
 conda install cdlib
 ```
 
 ### Optional Dependencies (pip package)
-``CDlib`` relies on a few packages calling C code that can be cumbersome to install on Windows machines: to address such issue, the default installation does not try to install set up such requirements.
+To simplify the installation process, the default installation does not include optional dependencies (e.g., ``graph-tool``). If you need them, you can install them manually or run the following command:
 
-Such a choice has been made to allow (even) non *unix user to install the library and get access to its core functionalities. 
+```bash
+pip install cdlib[C]
+```
 
-To integrate the standard installation with you can either:
+This option, safe for *nix users, will install all those optional dependencies that require C code compilation.
 
-- (Windows) manually install the optional packages (versions details are specified in ``requirements_optional.txt``) following the original projects guidelines, or
-- (Linux/OSX) run the command:
+```bash
+pip install cdlib[pypi]
+```
+
+This option will install all those optional dependencies that are not available on conda/conda-forge.
 
 ```bash
-pip install cdlib[C]
+pip install cdlib[all]
 ```
 
-Such caveat will install everything that can be easily automated under Linux/OSX. 
+This option will install all optional dependencies accessible with the flag ``C`` and ``pypi``.
 
 #### (Advanced) 
 
-##### Graph-tool
-The only optional dependency that will remain unsatisfied following the previous procedures will be ``graph-tool`` (used to add SBM models). 
-If you need it up and running, refer to the official [documentation](https://git.skewed.de/count0/graph-tool/wikis/installation-instructions) and install the conda-forge version of the package.
+Due to some strict requirements, the installation of a subset of optional dependencies is left outside the previous procedures.
+
+##### graph-tool
+``CDlib`` integrates the support for SBM models offered by ``graph-tool``.
+To install it refer to the official [documentation](https://git.skewed.de/count0/graph-tool/wikis/installation-instructions) and install the conda-forge version of the package (or the deb version if in a *nix system).
 
 ##### ASLPAw
 
 Since its 2.1.0 release ``ASLPAw`` relies on ``gmpy2`` whose installation through pip is not easy to automatize due to some C dependencies.
 To address such issue test the following recipe:
 
 ```bash
@@ -98,15 +102,15 @@
 pip install shuffle_graph>=2.1.0 similarity-index-of-label-graph>=2.0.1 ASLPAw>=2.1.0
 ```
 
 In case this does not solve the issue, please refer to the official ``gmpy2`` [installation](https://gmpy2.readthedocs.io/en/latest/intro.html#installation) instructions.
 
 ### Optional Dependencies (Conda package)
 
-``CDlib`` relies on a few packages not available through conda: to install it please use pip:
+``CDlib`` relies on a few packages not available through conda: to install them please use pip.
 
 ```bash
 pip install pycombo
 pip install GraphRicciCurvature
 
 conda install gmpy2 
 pip install shuffle_graph>=2.1.0 similarity-index-of-label-graph>=2.0.1 ASLPAw>=2.1.0
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/attribute_clustering.py` & `cdlib-0.3.0/cdlib/algorithms/attribute_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,34 +60,34 @@
 
     .. note:: Reference implementation: https://github.com/GiulioRossetti/Eva/tree/master/Eva
     """
 
     g = convert_graph_formats(g_original, nx.Graph)
     nx.set_node_attributes(g, labels)
 
+    mapping = dict(zip(g, range(0, len(g))))
+    rev_map = {v: k for k, v in mapping.items()}
+    relabel_g = nx.relabel_nodes(g, mapping)
+
     coms, coms_labels = Eva.eva_best_partition(
-        g, weight=weight, resolution=resolution, alpha=alpha
+        relabel_g, weight=weight, resolution=resolution, alpha=alpha
     )
 
     # Reshaping the results
     coms_to_node = defaultdict(list)
     for n, c in coms.items():
-        coms_to_node[c].append(n)
+        coms_to_node[c].append(rev_map[n])
 
     coms_eva = [list(c) for c in coms_to_node.values()]
     return AttrNodeClustering(
         coms_eva,
         g_original,
         "Eva",
         coms_labels,
-        method_parameters={
-            "weight": weight,
-            "resolution": resolution,
-            "alpha": alpha,
-        },
+        method_parameters={"weight": weight, "resolution": resolution, "alpha": alpha},
     )
 
 
 def ilouvain(g_original: object, labels: dict) -> AttrNodeClustering:
     """
     The I-Louvain algorithm extends the Louvain approach in order to deal only with the scalar attributes of the nodes.
     It optimizes Newman's modularity combined with an entropy measure.
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/bipartite_clustering.py` & `cdlib-0.3.0/cdlib/algorithms/bipartite_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from cdlib import BiNodeClustering
 import networkx as nx
 from cdlib.utils import convert_graph_formats
 from collections import defaultdict
 from cdlib.algorithms.internal.pycondor import condor_object, initial_community, brim
+from cdlib.prompt_utils import report_missing_packages, prompt_import_failure
 
 missing_packages = set()
 
 try:
     import infomap as imp
 except ModuleNotFoundError:
     missing_packages.add("infomap")
     imp = None
+except Exception as exception:
+    prompt_import_failure("infomap", exception)
 
 try:
     from wurlitzer import pipes
 except ModuleNotFoundError:
     missing_packages.add("wurlitzer")
     pipes = None
 
@@ -25,19 +28,15 @@
 
 try:
     import leidenalg
 except ModuleNotFoundError:
     missing_packages.add("leidenalg")
     leidenalg = None
 
-if len(missing_packages) > 0:
-    print(
-        "Note: to be able to use all bipartite methods, you need to install some additional packages: ",
-        missing_packages,
-    )
+report_missing_packages(missing_packages)
 
 __all__ = ["bimlpa", "CPM_Bipartite", "infomap_bipartite", "condor"]
 
 
 def bimlpa(g_original: object, theta: float = 0.3, lambd: int = 7) -> BiNodeClustering:
     """
     BiMLPA is designed to detect the many-to-many correspondence community in bipartite networks using multi-label propagation algorithm.
@@ -47,15 +46,15 @@
 
     ========== ======== ======== =========
     Undirected Directed Weighted Bipartite
     ========== ======== ======== =========
     Yes        No       No       Yes
     ========== ======== ======== =========
 
-    :param g_original: a networkx/igraph object
+    :param g_original: a networkx/igraph object (instance of igraph.Graph or nx.Graph).
     :param theta: Label weights threshold. Default 0.3.
     :param lambd: The max number of labels. Default 7.
     :return: BiNodeClustering object
 
 
     :Example:
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/crisp_partition.py` & `cdlib-0.3.0/cdlib/algorithms/crisp_partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import sys
 import numpy as np
 from typing import Callable
 from copy import deepcopy
 from cdlib.algorithms.internal import DER
 
-# import community as louvain_modularity
 from community import community_louvain
+
 from collections import defaultdict
 from cdlib import NodeClustering, FuzzyNodeClustering
+
+# from cdlib.algorithms.internal.Bayan import bayan_alg
 from cdlib.algorithms.internal.belief_prop import detect_belief_communities
 from cdlib.algorithms.internal.em import EM_nx
 from cdlib.algorithms.internal.scan import SCAN_nx
 from cdlib.algorithms.internal.GDMP2_nx import GDMP2
 from cdlib.algorithms.internal.AGDL import Agdl
 from cdlib.algorithms.internal.FuzzyCom import fuzzy_comm
-from cdlib.algorithms.internal.Markov import markov
 from cdlib.algorithms.internal.ga import ga_community_detection
 from cdlib.algorithms.internal.SiblinarityAntichain import (
     matrix_node_recursive_antichain_partition,
 )
 from cdlib.algorithms.internal.LSWL import (
     LSWLCommunityDiscovery_offline,
     LSWLPlusCommunityDetection,
@@ -29,19 +30,22 @@
 from cdlib.algorithms.internal.modularity_r import ModularityRCommunityDiscovery
 from cdlib.algorithms.internal.headtail import HeadTail
 from cdlib.algorithms.internal.Kcut import kcut_exec
 from cdlib.algorithms.internal.paris import paris as paris_alg, paris_best_clustering
 from cdlib.algorithms.internal.principled import principled
 from cdlib.algorithms.internal.MCODE import m_code
 from cdlib.algorithms.internal.RSC import rsc_evaluate_graph
+from cdlib.prompt_utils import report_missing_packages, prompt_import_failure
+
 import warnings
 
 import markov_clustering as mc
-from chinese_whispers import chinese_whispers as cw
-from chinese_whispers import aggregate_clusters
+
+# from chinese_whispers import chinese_whispers as cw
+# from chinese_whispers import aggregate_clusters
 from thresholdclustering.thresholdclustering import best_partition as th_best_partition
 import networkx as nx
 
 from cdlib.utils import (
     convert_graph_formats,
     __from_nx_to_graph_tool,
     affiliations2nodesets,
@@ -51,14 +55,16 @@
 missing_packages = set()
 
 try:
     import infomap as imp
 except ModuleNotFoundError:
     missing_packages.add("infomap")
     imp = None
+except Exception as exception:
+    prompt_import_failure("infomap", exception)
 
 try:
     from wurlitzer import pipes
 except ModuleNotFoundError:
     missing_packages.add("wurlitzer")
     pipes = None
 
@@ -76,24 +82,27 @@
 try:
     import graph_tool.all as gt
 except ModuleNotFoundError:
     missing_packages.add("graph_tool")
     gt = None
 
 try:
-    import karateclub
+    import bayanpy as by
 except ModuleNotFoundError:
-    missing_packages.add("karateclub")
+    missing_packages.add("bayanpy")
+    by = None
 
+# try:
+#    import karateclub
+# except ModuleNotFoundError:
+#    missing_packages.add("karateclub")
+
+
+report_missing_packages(missing_packages)
 
-if len(missing_packages) > 0:
-    print(
-        "Note: to be able to use all crisp methods, you need to install some additional packages: ",
-        missing_packages,
-    )
 
 try:
     from GraphRicciCurvature.OllivierRicci import OllivierRicci
 except ModuleNotFoundError:
     OllivierRicci = None
 
 try:
@@ -122,35 +131,36 @@
     "spinglass",
     "eigenvector",
     "agdl",
     "frc_fgsn",
     "sbm_dl",
     "sbm_dl_nested",
     "markov_clustering",
-    "edmot",
-    "chinesewhispers",
+    # "edmot",
+    # "chinesewhispers",
     "siblinarity_antichain",
     "ga",
     "belief",
     "threshold_clustering",
     "lswl_plus",
     "lswl",
     "mod_m",
     "mod_r",
     "head_tail",
     "kcut",
-    "gemsec",
-    "scd",
+    # "gemsec",
+    # "scd",
     "pycombo",
     "paris",
     "principled_clustering",
     "ricci_community",
     "spectral",
     "mcode",
     "r_spectral_clustering",
+    "bayan",
 ]
 
 
 def girvan_newman(g_original: object, level: int) -> NodeClustering:
     """
     The Girvan–Newman algorithm detects communities by progressively removing edges from the original graph.
     The algorithm removes the "most valuable" edge, traditionally the edge with the highest betweenness centrality, at each step. As the graph breaks down into pieces, the tightly knit community structure is exposed and the result can be depicted as a dendrogram.
@@ -338,29 +348,30 @@
         communities,
         g_original,
         "GDMP2",
         method_parameters={"min_threshold": min_threshold},
     )
 
 
-def spinglass(g_original: object) -> NodeClustering:
+def spinglass(g_original: object, spins: int = 25) -> NodeClustering:
     """
     Spinglass relies on an analogy between a very popular statistical mechanic model called Potts spin glass, and the community structure.
     It applies the simulated annealing optimization technique on this model to optimize the modularity.
 
 
     **Supported Graph Types**
 
     ========== ======== ========
     Undirected Directed Weighted
     ========== ======== ========
     Yes        No       No
     ========== ======== ========
 
     :param g_original: a networkx/igraph object
+    :param spins: the number of spins to use. This is the upper limit for the number of communities. It is not a problem to supply a (reasonably) big number here, in which case some spin states will be unpopulated.
     :return: NodeClustering object
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.karate_club_graph()
@@ -372,15 +383,15 @@
     """
     if ig is None:
         raise ModuleNotFoundError(
             "Optional dependency not satisfied: install igraph to use the selected feature."
         )
 
     g = convert_graph_formats(g_original, ig.Graph)
-    coms = g.community_spinglass()
+    coms = g.community_spinglass(spins=spins)
     communities = []
 
     for c in coms:
         communities.append([g.vs[x]["name"] for x in c])
 
     return NodeClustering(
         communities, g_original, "Spinglass", method_parameters={"": ""}
@@ -1038,14 +1049,15 @@
 
 
 def infomap(g_original: object, flags: str = "") -> NodeClustering:
     """
     Infomap is based on ideas of information theory.
     The algorithm uses the probability flow of random walks on a network as a proxy for information flows in the real system and it decomposes the network into modules by compressing a description of the probability flow.
 
+    NB: in case the Infomap package is not installed/installable (e.g., on M1 silicon Macs), the implementation used is the one from the igraph library.
 
     **Supported Graph Types**
 
     ========== ======== ========
     Undirected Directed Weighted
     ========== ======== ========
     Yes        Yes      Yes
@@ -1066,22 +1078,34 @@
 
     Rosvall M, Bergstrom CT (2008) `Maps of random walks on complex networks reveal community structure. <https://www.pnas.org/content/105/4/1118/>`_ Proc Natl Acad SciUSA 105(4):1118–1123
 
     .. note:: Reference implementation: https://pypi.org/project/infomap/
 
     .. note:: Infomap Python API documentation: https://mapequation.github.io/infomap/python/
     """
+
     global imp, pipes
     if imp is None:
         try:
             import infomap as imp
         except ModuleNotFoundError:
-            raise ModuleNotFoundError(
-                "Optional dependency not satisfied: install infomap to use the selected feature."
+            g = convert_graph_formats(g_original, ig.Graph)
+            coms = g.community_infomap()
+
+            communities = []
+
+            for c in coms:
+                communities.append([g.vs[x]["name"] for x in c])
+
+            return NodeClustering(
+                communities, g_original, "Infomap", method_parameters={"igraph": True}
             )
+            # raise ModuleNotFoundError(
+            #    "Optional dependency not satisfied: install infomap to use the selected feature."
+            # )
     if pipes is None:
         try:
             from wurlitzer import pipes
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
                 "Optional dependency not satisfied: install package wurlitzer to use infomap."
             )
@@ -1400,15 +1424,15 @@
 
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.karate_club_graph()
-    >>> coms = principled_clustering(G, 3)
+    >>> coms = algorithms.principled_clustering(G, 3)
 
 
     :References:
 
     B Ball, B., & E JNewman, M. (2011). An efficient and principled method for detecting communities in networks. Physical ReviewE, 84, 036103.
 
     .. note:: Reference implementation: https://github.com/Zabot/principled_clustering
@@ -1459,15 +1483,15 @@
 
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.karate_club_graph()
-    >>> coms = sbm_dl(G)
+    >>> coms = algorithms.sbm_dl(G)
 
 
     :References:
 
     Tiago P. Peixoto, “Efficient Monte Carlo and greedy heuristic for the inference of stochastic block models”, Phys. Rev. E 89, 012804 (2014), DOI: 10.1103/PhysRevE.89.012804 [sci-hub, @tor], arXiv: 1310.4378.
 
     .. note:: Implementation from graph-tool library, please report to https://graph-tool.skewed.de for details
@@ -1515,15 +1539,15 @@
 
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
     >>> G = nx.karate_club_graph()
-    >>> coms = sbm_dl(G)
+    >>> coms = algorithms.sbm_dl(G)
 
 
     :References:
 
     Tiago P. Peixoto, “Hierarchical block structures and high-resolution model selection in large networks”, Physical Review X 4.1 (2014): 011047
 
     .. note:: Implementation from graph-tool library, please report to https://graph-tool.skewed.de for details
@@ -1549,20 +1573,15 @@
 
     level0 = state.get_levels()[0]
 
     affiliations = level0.get_blocks().get_array()
     affiliations = {label_map[i]: affiliations[i] for i in range(len(affiliations))}
     coms = affiliations2nodesets(affiliations)
     coms = [list(v) for k, v in coms.items()]
-    return NodeClustering(
-        coms,
-        g_original,
-        "SBM_nested",
-        method_parameters={},
-    )
+    return NodeClustering(coms, g_original, "SBM_nested", method_parameters={})
 
 
 def markov_clustering(
     g_original: object,
     expansion: int = 2,
     inflation: int = 2,
     loop_value: int = 1,
@@ -1612,17 +1631,17 @@
     .. note:: Reference implementation: https://github.com/GuyAllard/markov_clustering
     """
 
     g = convert_graph_formats(g_original, nx.Graph)
     g, maps = nx_node_integer_mapping(g)
 
     if maps is not None:
-        matrix = nx.to_scipy_sparse_matrix(g, nodelist=range(len(maps)))
+        matrix = nx.to_scipy_sparse_array(g, nodelist=range(len(maps)))
     else:
-        matrix = nx.to_scipy_sparse_matrix(g)
+        matrix = nx.to_scipy_sparse_array(g)
 
     result = mc.run_mcl(
         matrix,
         expansion=expansion,
         inflation=inflation,
         loop_value=loop_value,
         iterations=iterations,
@@ -1653,140 +1672,140 @@
             "pruning_threshold": pruning_threshold,
             "pruning_frequency": pruning_frequency,
             "convergence_check_frequency": convergence_check_frequency,
         },
     )
 
 
-def chinesewhispers(
-    g_original: object, weighting: str = "top", iterations: int = 20, seed: int = None
-) -> NodeClustering:
-    """
-
-    Fuzzy graph clustering that (i) creates an intermediate representation of the input graph, which reflects the “ambiguity” of its nodes,
-    and (ii) uses hard clustering to discover crisp clusters in such “disambiguated” intermediate graph.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       Yes
-    ========== ======== ========
-
-    :param g_original:
-    :param weighting: edge weighing schemas. Available modalities: ['top', 'lin', 'log']
-    :param iterations: number of iterations
-    :param seed: random seed
-    :return: NodeClustering object
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.chinesewhispers(G)
-
-    :References:
-
-    Biemann, Chris. 2006. Chinese Whispers: An Efficient Graph Clustering Algorithm and Its Application to Natural Language Processing Problems. In Proceedings of the First Workshop on Graph Based Methods for Natural Language Processing, TextGraphs-1, pages 73–80, Association for Computational Linguistics, New York, NY, USA.
-
-    .. note:: Reference implementation: https://github.com/nlpub/chinese-whispers-python
-    """
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    g, maps = nx_node_integer_mapping(g)
-
-    cw(g, weighting=weighting, iterations=iterations, seed=seed)
-
-    coms = []
-    if maps is not None:
-        for _, cluster in sorted(
-            aggregate_clusters(g).items(), key=lambda e: len(e[1]), reverse=True
-        ):
-            coms.append([maps[n] for n in cluster])
-
-        nx.relabel_nodes(g, maps, False)
-    else:
-        for _, cluster in sorted(
-            aggregate_clusters(g).items(), key=lambda e: len(e[1]), reverse=True
-        ):
-            coms.append(list(cluster))
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "Chinese Whispers",
-        method_parameters={"weighting": weighting, "iterations": iterations},
-    )
-
-
-def edmot(
-    g_original: object, component_count: int = 2, cutoff: int = 10
-) -> NodeClustering:
-    """
-    The algorithm first creates the graph of higher order motifs. This graph is clustered by the Louvain method.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param component_count: Number of extracted motif hypergraph components. Default is 2.
-    :param cutoff: Motif edge cut-off value. Default is 10.
-    :return: NodeClustering object
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.edmot(G, max_loop=1000)
-
-    :References:
-
-    Li, Pei-Zhen, et al. "EdMot: An Edge Enhancement Approach for Motif-aware Community Detection." Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining. 2019.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    global karateclub
-
-    if "karateclub" not in sys.modules:
-        try:
-            import karateclub
-        except ModuleNotFoundError:
-            raise ModuleNotFoundError(
-                "Optional dependency not satisfied: install karateclub to use the selected feature."
-            )
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.EdMot(component_count=2, cutoff=10)
-
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "EdMot",
-        method_parameters={"component_count": component_count, "cutoff": cutoff},
-    )
+# def chinesewhispers(
+#     g_original: object, weighting: str = "top", iterations: int = 20, seed: int = None
+# ) -> NodeClustering:
+#     """
+#
+#     Fuzzy graph clustering that (i) creates an intermediate representation of the input graph, which reflects the “ambiguity” of its nodes,
+#     and (ii) uses hard clustering to discover crisp clusters in such “disambiguated” intermediate graph.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       Yes
+#     ========== ======== ========
+#
+#     :param g_original:
+#     :param weighting: edge weighing schemas. Available modalities: ['top', 'lin', 'log']
+#     :param iterations: number of iterations
+#     :param seed: random seed
+#     :return: NodeClustering object
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.chinesewhispers(G)
+#
+#     :References:
+#
+#     Biemann, Chris. 2006. Chinese Whispers: An Efficient Graph Clustering Algorithm and Its Application to Natural Language Processing Problems. In Proceedings of the First Workshop on Graph Based Methods for Natural Language Processing, TextGraphs-1, pages 73–80, Association for Computational Linguistics, New York, NY, USA.
+#
+#     .. note:: Reference implementation: https://github.com/nlpub/chinese-whispers-python
+#     """
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     g, maps = nx_node_integer_mapping(g)
+#
+#     cw(g, weighting=weighting, iterations=iterations, seed=seed)
+#
+#     coms = []
+#     if maps is not None:
+#         for _, cluster in sorted(
+#             aggregate_clusters(g).items(), key=lambda e: len(e[1]), reverse=True
+#         ):
+#             coms.append([maps[n] for n in cluster])
+#
+#         nx.relabel_nodes(g, maps, False)
+#     else:
+#         for _, cluster in sorted(
+#             aggregate_clusters(g).items(), key=lambda e: len(e[1]), reverse=True
+#         ):
+#             coms.append(list(cluster))
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "Chinese Whispers",
+#         method_parameters={"weighting": weighting, "iterations": iterations},
+#     )
+
+
+# def edmot(
+#     g_original: object, component_count: int = 2, cutoff: int = 10
+# ) -> NodeClustering:
+#     """
+#     The algorithm first creates the graph of higher order motifs. This graph is clustered by the Louvain method.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param component_count: Number of extracted motif hypergraph components. Default is 2.
+#     :param cutoff: Motif edge cut-off value. Default is 10.
+#     :return: NodeClustering object
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.edmot(G)
+#
+#     :References:
+#
+#     Li, Pei-Zhen, et al. "EdMot: An Edge Enhancement Approach for Motif-aware Community Detection." Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining. 2019.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     #global karateclub
+#
+#     if "karateclub" not in sys.modules:
+#         try:
+#             import karateclub
+#         except ModuleNotFoundError:
+#             raise ModuleNotFoundError(
+#                 "Optional dependency not satisfied: install karateclub to use the selected feature."
+#             )
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.EdMot(component_count=2, cutoff=10)
+#
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "EdMot",
+#         method_parameters={"component_count": component_count, "cutoff": cutoff},
+#     )
 
 
 def siblinarity_antichain(
     g_original: object,
     forwards_backwards_on: bool = True,
     backwards_forwards_on: bool = False,
     Lambda: int = 1,
@@ -2291,15 +2310,15 @@
     :param head_tail_ratio: head/tail division rule. Float in [0,1], dafault 0.4.
     :return: NodeClustering object
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
-    >>> G = nx.head_tail()
+    >>> G = nx.karate_club_graph()
     >>> coms = algorithms.head_tail(G, head_tail_ratio=0.8)
 
     :References:
 
     Jiang B. and Ding M. (2015), Defining least community as a homogeneous group in complex networks, Physica A, 428, 154-160.
 
     .. note:: Reference implementation: https://github.com/dingmartin/HeadTailCommunityDetection
@@ -2335,16 +2354,16 @@
     :param kmax: maximum value of k, dafault 4.
     :return: NodeClustering object
 
     :Example:
 
     >>> from cdlib import algorithms
     >>> import networkx as nx
-    >>> G = nx.head_tail()
-    >>> coms = algorithms.kcut(G, head_tail_ratio=0.8)
+    >>> G = nx.karate_club_graph()
+    >>> coms = algorithms.kcut(G, kmax=4)
 
     :References:
 
     Ruan, Jianhua, and Weixiong Zhang. "An efficient spectral algorithm for network community discovery and its applications to biological and social networks." Seventh IEEE International Conference on Data Mining (ICDM 2007). IEEE, 2007.
 
     .. note:: Reference implementation: https://github.com/hmliangliang/kcut-algorithm
 
@@ -2352,181 +2371,181 @@
 
     g = convert_graph_formats(g_original, nx.Graph)
     coms = kcut_exec(g, kmax)
 
     return NodeClustering(coms, g_original, "Kcut", method_parameters={"kmax": kmax})
 
 
-def gemsec(
-    g_original: object,
-    walk_number: int = 5,
-    walk_length: int = 80,
-    dimensions: int = 32,
-    negative_samples: int = 5,
-    window_size: int = 5,
-    learning_rate: float = 0.1,
-    clusters: int = 10,
-    gamma: float = 0.1,
-    seed: int = 42,
-) -> NodeClustering:
-    """
-    The procedure uses random walks to approximate the pointwise mutual information matrix obtained by pooling normalized adjacency matrix powers.
-    This matrix is decomposed by an approximate factorization technique which is combined with a k-means like clustering cost.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        Yes      No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param walk_number: Number of random walks. Default is 5.
-    :param walk_length: Length of random walks. Default is 80.
-    :param dimensions: Dimensionality of embedding. Default is 32.
-    :param negative_samples: Number of negative samples. Default is 5.
-    :param window_size: Matrix power order. Default is 5.
-    :param learning_rate: Gradient descent learning rate. Default is 0.1.
-    :param clusters: Number of cluster centers. Default is 10.
-    :param gamma: Clustering cost weight coefficient. Default is 0.1.
-    :param seed: Random seed value. Default is 42.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.gemsec(G)
-
-    :References:
-
-    Rozemberczki, B., Davies, R., Sarkar, R., & Sutton, C. (2019, August). Gemsec: Graph embedding with self clustering. In Proceedings of the 2019 IEEE/ACM international conference on advances in social networks analysis and mining (pp. 65-72).
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    global karateclub
-    if "karateclub" not in sys.modules:
-        try:
-            import karateclub
-        except ModuleNotFoundError:
-            raise ModuleNotFoundError(
-                "Optional dependency not satisfied: install karateclub to use the selected feature."
-            )
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.GEMSEC(
-        walk_number=walk_number,
-        walk_length=walk_length,
-        dimensions=dimensions,
-        negative_samples=negative_samples,
-        window_size=window_size,
-        learning_rate=learning_rate,
-        clusters=clusters,
-        gamma=gamma,
-        seed=seed,
-    )
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "GEMSEC",
-        method_parameters={
-            "walk_number": walk_number,
-            "walk_length": walk_length,
-            "dimensions": dimensions,
-            "negative_samples": negative_samples,
-            "window_size": window_size,
-            "learning_rate": learning_rate,
-            "clusters": clusters,
-            "gamma": gamma,
-            "seed": seed,
-        },
-        overlap=False,
-    )
-
-
-def scd(
-    g_original: object, iterations: int = 25, eps: float = 1e-06, seed: int = 42
-) -> NodeClustering:
-    """
-    The procedure greedily optimizes the approximate weighted community clustering metric.
-    First, clusters are built around highly clustered nodes. Second, we refine the initial partition by using the approximate WCC.
-    These refinements happen for the whole vertex set.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param iterations: Refinemeent iterations. Default is 25.
-    :param eps: Epsilon score for zero division correction. Default is 10**-6.
-    :param seed: Random seed value. Default is 42.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.scd(G)
-
-    :References:
-
-    Prat-Pérez, A., Dominguez-Sal, D., & Larriba-Pey, J. L. (2014, April). High quality, scalable and parallel community detection for large real graphs. In Proceedings of the 23rd international conference on World wide web (pp. 225-236).
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    global karateclub
-
-    if "karateclub" not in sys.modules:
-        try:
-            import karateclub
-        except ModuleNotFoundError:
-            raise ModuleNotFoundError(
-                "Optional dependency not satisfied: install karateclub to use the selected feature."
-            )
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.SCD(iterations=iterations, eps=eps, seed=seed)
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "SCD",
-        method_parameters={"iterations": iterations, "eps": eps, "seed": seed},
-        overlap=False,
-    )
+# def gemsec(
+#     g_original: object,
+#     walk_number: int = 5,
+#     walk_length: int = 80,
+#     dimensions: int = 32,
+#     negative_samples: int = 5,
+#     window_size: int = 5,
+#     learning_rate: float = 0.1,
+#     clusters: int = 10,
+#     gamma: float = 0.1,
+#     seed: int = 42,
+# ) -> NodeClustering:
+#     """
+#     The procedure uses random walks to approximate the pointwise mutual information matrix obtained by pooling normalized adjacency matrix powers.
+#     This matrix is decomposed by an approximate factorization technique which is combined with a k-means like clustering cost.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        Yes      No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param walk_number: Number of random walks. Default is 5.
+#     :param walk_length: Length of random walks. Default is 80.
+#     :param dimensions: Dimensionality of embedding. Default is 32.
+#     :param negative_samples: Number of negative samples. Default is 5.
+#     :param window_size: Matrix power order. Default is 5.
+#     :param learning_rate: Gradient descent learning rate. Default is 0.1.
+#     :param clusters: Number of cluster centers. Default is 10.
+#     :param gamma: Clustering cost weight coefficient. Default is 0.1.
+#     :param seed: Random seed value. Default is 42.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.gemsec(G)
+#
+#     :References:
+#
+#     Rozemberczki, B., Davies, R., Sarkar, R., & Sutton, C. (2019, August). Gemsec: Graph embedding with self clustering. In Proceedings of the 2019 IEEE/ACM international conference on advances in social networks analysis and mining (pp. 65-72).
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     global karateclub
+#     if "karateclub" not in sys.modules:
+#         try:
+#             import karateclub
+#         except ModuleNotFoundError:
+#             raise ModuleNotFoundError(
+#                 "Optional dependency not satisfied: install karateclub to use the selected feature."
+#             )
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.GEMSEC(
+#         walk_number=walk_number,
+#         walk_length=walk_length,
+#         dimensions=dimensions,
+#         negative_samples=negative_samples,
+#         window_size=window_size,
+#         learning_rate=learning_rate,
+#         clusters=clusters,
+#         gamma=gamma,
+#         seed=seed,
+#     )
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "GEMSEC",
+#         method_parameters={
+#             "walk_number": walk_number,
+#             "walk_length": walk_length,
+#             "dimensions": dimensions,
+#             "negative_samples": negative_samples,
+#             "window_size": window_size,
+#             "learning_rate": learning_rate,
+#             "clusters": clusters,
+#             "gamma": gamma,
+#             "seed": seed,
+#         },
+#         overlap=False,
+#     )
+
+
+# def scd(
+#     g_original: object, iterations: int = 25, eps: float = 1e-06, seed: int = 42
+# ) -> NodeClustering:
+#     """
+#     The procedure greedily optimizes the approximate weighted community clustering metric.
+#     First, clusters are built around highly clustered nodes. Second, we refine the initial partition by using the approximate WCC.
+#     These refinements happen for the whole vertex set.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param iterations: Refinemeent iterations. Default is 25.
+#     :param eps: Epsilon score for zero division correction. Default is 10**-6.
+#     :param seed: Random seed value. Default is 42.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.scd(G)
+#
+#     :References:
+#
+#     Prat-Pérez, A., Dominguez-Sal, D., & Larriba-Pey, J. L. (2014, April). High quality, scalable and parallel community detection for large real graphs. In Proceedings of the 23rd international conference on World wide web (pp. 225-236).
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     global karateclub
+#
+#     if "karateclub" not in sys.modules:
+#         try:
+#             import karateclub
+#         except ModuleNotFoundError:
+#             raise ModuleNotFoundError(
+#                 "Optional dependency not satisfied: install karateclub to use the selected feature."
+#             )
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.SCD(iterations=iterations, eps=eps, seed=seed)
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "SCD",
+#         method_parameters={"iterations": iterations, "eps": eps, "seed": seed},
+#         overlap=False,
+#     )
 
 
 def pycombo(
     g_original: object,
     weight: str = "weight",
     max_communities: int = None,
     modularity_resolution: float = 1.0,
@@ -2770,17 +2789,15 @@
             "projection_on_smaller_class": projection_on_smaller_class,
         },
         overlap=False,
     )
 
 
 def mcode(
-    g_original: object,
-    weights: str = None,
-    weight_threshold: float = 0.2,
+    g_original: object, weights: str = None, weight_threshold: float = 0.2
 ) -> NodeClustering:
     """
     MCODE is the earliest seed-growth method for predicting protein complexes from PPI networks. MCODE works in two steps:
 
     1. vertex weighting, and
     2. molecular complex prediction.
 
@@ -2814,35 +2831,29 @@
 
     Bader, G.D., Hogue, C.W. 2003. An automated method for ﬁnding molecular complexes in large protein interaction networks. BMC Bioinformatics 4, 2.
 
     .. note:: Reference Implementation: https://github.com/trueprice/python-graph-clustering
     """
 
     g = convert_graph_formats(g_original, nx.Graph)
-    clustering = m_code(
-        g,
-        weights=weights,
-        weight_threshold=weight_threshold,
-    )
+    clustering = m_code(g, weights=weights, weight_threshold=weight_threshold)
 
     return NodeClustering(
         clustering,
         g_original,
         "mcode",
-        method_parameters={
-            "weight_threshold": weight_threshold,
-        },
+        method_parameters={"weight_threshold": weight_threshold},
         overlap=False,
     )
 
 
 def r_spectral_clustering(
     g_original: object,
     n_clusters: int = 2,
-    method: str = "regularized",
+    method: str = "vanilla",
     percentile: int = None,
 ) -> NodeClustering:
     """
     Spectral clustering partitions the nodes of a graph into groups based upon the eigenvectors of the graph Laplacian.
     Despite the claims of spectral clustering being “popular”, in applied research using graph data, spectral clustering (without regularization) often returns a partition of the nodes that is uninteresting, typically finding a large cluster that contains most of the data and many smaller clusters, each with only a few nodes.
     This method allows to compute spectral clustering with/withouth different regualarization functions designed to address such a limitation.
 
@@ -2898,7 +2909,73 @@
         method_parameters={
             "n_clusters": n_clusters,
             "method": method,
             "percentile": percentile,
         },
         overlap=False,
     )
+
+
+def bayan(
+    g_original: object,
+    threshold: float = 0.001,
+    time_allowed: int = 60,
+    resolution: float = 1,
+) -> NodeClustering:
+    """
+    The Bayan algorithm is community detection method that is capable of providing a globally optimal solution to the modularity maximization problem.
+    Bayan can also be implemented such that it provides an approximation of the maximum modularity with a guarantee of proximity.
+    This algorithm is theoretically grounded by the Integer Programming (IP) formulation of the modularity maximization problem and relies on an exact branch-and-cut scheme for solving the NP-complete optimization problem to global optimality.
+
+    The algorithm is integrated as an *optional* feature in CDlib due to its dependency on the Gurobi solver.
+    For a detailed description on how to satisfy such a dependency please refer to the instructions provided in the official documentation: https://github.com/saref/bayan
+
+    **Supported Graph Types**
+
+    ========== ======== ========
+    Undirected Directed Weighted
+    ========== ======== ========
+    Yes        No       Yes
+    ========== ======== ========
+
+    :param g_original: a networkx/igraph object
+    :param threshold: Threshold is the minimum optimality gap that Bayan should execute till. In the above example if Bayan finds a solution with modularity within 0.001 of the optimal solution, it will return that solution.
+    :param time_allowed: Time allowed is the maximum time in seconds that Bayan should execute for.
+    :param resolution: Resolution is the resolution parameter of the modularity function.
+    :return: NodeClustering object
+
+    :Example:
+
+    >>> from cdlib import algorithms
+    >>> import networkx as nx
+    >>> G = nx.karate_club_graph()
+    >>> com = algorithms.bayan(G)
+
+    :References:
+
+    Aref, Samin, Hriday Chheda, and Mahdi Mostajabdaveh. "The Bayan Algorithm: Detecting Communities in Networks Through Exact and Approximate Optimization of Modularity." arXiv preprint arXiv:2209.04562 (2022).
+    """
+
+    if by is None:
+        raise Exception(
+            "===================================================== \n"
+            "The bayan algorithm seems not to be installed (or incorrectly installed). \n"
+            "Please resolve with: pip install bayanpy"
+        )
+
+    g = convert_graph_formats(g_original, nx.Graph)
+
+    _, _, community, _, _ = by.bayan(
+        g, threshold=threshold, time_allowed=time_allowed, resolution=resolution
+    )
+
+    return NodeClustering(
+        community,
+        g_original,
+        "Bayan",
+        method_parameters={
+            "threshold": threshold,
+            "time_allowed": time_allowed,
+            "resolution": resolution,
+        },
+        overlap=False,
+    )
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/edge_clustering.py` & `cdlib-0.3.0/cdlib/algorithms/edge_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/AGDL.py` & `cdlib-0.3.0/cdlib/algorithms/internal/AGDL.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 import networkx as nx
 
 
 def __knn(k, x):
     from sklearn.neighbors import NearestNeighbors
 
     neigh = NearestNeighbors(k + 1, metric="euclidean", n_jobs=-1).fit(x)
-    k_neighbors = neigh.kneighbors(
-        x,
-        k + 1,
-    )
+    k_neighbors = neigh.kneighbors(x, k + 1)
     distance = np.array(k_neighbors[0][:, 1:])
     indices = np.array(k_neighbors[1][:, 1:])
     return distance, indices
 
 
 def __w_matrix(distance, indices, ks, a=10):
     n = len(distance)
@@ -74,17 +71,17 @@
             ji = np.ix_(vc[j], vc[i])
 
             w_ij, w_ji = w[ij], w[ji]
             ci, cj = len(vc[i]), len(vc[j])
 
             ones_i = np.ones((ci, 1))
             ones_j = np.ones((cj, 1))
-            affinity[i][j] = (1 / ci ** 2) * np.transpose(ones_i).dot(w_ij).dot(
+            affinity[i][j] = (1 / ci**2) * np.transpose(ones_i).dot(w_ij).dot(
                 w_ji
-            ).dot(ones_i) + (1 / cj ** 2) * np.transpose(ones_j).dot(w_ji).dot(
+            ).dot(ones_i) + (1 / cj**2) * np.transpose(ones_j).dot(w_ji).dot(
                 w_ij
             ).dot(
                 ones_j
             )
             affinity[j][i] = affinity[i][j]
     return affinity
 
@@ -94,16 +91,16 @@
     ji = np.ix_(c2, c1)
 
     w_ij, w_ji = w[ij], w[ji]
     ci, cj = len(c1), len(c2)
 
     ones_i = np.ones((ci, 1))
     ones_j = np.ones((cj, 1))
-    affinity = (1 / ci ** 2) * np.transpose(ones_i).dot(w_ij).dot(w_ji).dot(ones_i) + (
-        1 / cj ** 2
+    affinity = (1 / ci**2) * np.transpose(ones_i).dot(w_ij).dot(w_ji).dot(ones_i) + (
+        1 / cj**2
     ) * np.transpose(ones_j).dot(w_ji).dot(w_ij).dot(ones_j)
     return affinity[0, 0]
 
 
 def __get_neighbor(vc, kc, w):
     ns, as_ = [], []
     A = __get_affinity_matrix(vc, w)
@@ -128,15 +125,17 @@
     # convert distance to similarity
     similarity, _ = __w_matrix(distance, indices, ks, a)
     g = nx.from_numpy_matrix(similarity, create_using=nx.DiGraph)
     return g
 
 
 def Agdl(g, target_cluster_num, kc):
-    similarity = nx.to_numpy_matrix(g)
+    similarity = np.asmatrix(
+        nx.to_numpy_array(g)
+    )  # , **kwargs)) #nx.to_numpy_matrix(g)
     # Using k0grpha to initilize cluster
 
     cluster = __k0graph(similarity)
 
     neighbor_set, affinity_set = __get_neighbor(cluster, kc, similarity)
     current_cluster_num = len(cluster)
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/BIGCLAM.py` & `cdlib-0.3.0/cdlib/algorithms/internal/BIGCLAM.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/COACH.py` & `cdlib-0.3.0/cdlib/algorithms/internal/COACH.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Author: True Price <jtprice@cs.unc.edu>
 
 # A core-attachment based method to detect protein complexes in PPI networks
 # Wu, Li, Kwoh, Ng (2009)
 # http://www.biomedcentral.com/1471-2105/10/169
 
 from collections import defaultdict
-from itertools import combinations
 import functools
 
 
 # return average degree and density for a graph
 def __graph_stats(graph):
     avg_deg = sum(len(n) for n in graph.values()) / float(len(graph))
     density = avg_deg / (len(graph) - 1)
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/CONGA.py` & `cdlib-0.3.0/cdlib/algorithms/internal/CONGA.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/CONGO.py` & `cdlib-0.3.0/cdlib/algorithms/internal/CONGO.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/DCS.py` & `cdlib-0.3.0/cdlib/algorithms/internal/DCS.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/DER.py` & `cdlib-0.3.0/cdlib/algorithms/internal/DER.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/DPCLUS.py` & `cdlib-0.3.0/cdlib/algorithms/internal/DPCLUS.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/EBGC.py` & `cdlib-0.3.0/cdlib/algorithms/internal/EBGC.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import numpy as np
 import networkx as nx
 import matplotlib.pyplot as plt
-import random
 from queue import Queue
-from collections import defaultdict
-
-# from dgl.data import LegacyTUDataset
 
 
 class EBGC:
     def __init__(self):
         self.g = None
         self.adj = None
         self.node_num = None
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/EnDNTM.py` & `cdlib-0.3.0/cdlib/algorithms/internal/EnDNTM.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import networkx as nx
-import random
 from networkx.algorithms import community as com
-import random
 import collections
 
 
 def __bfs(graph, root, epsilon):
     seen, queue, distance = {root}, collections.deque([root]), 1
     while queue:
         parent = queue.popleft()
@@ -16,15 +14,15 @@
                     queue.append(child)
         distance += 1
     return seen
 
 
 def endntm_evalFuction(graph, clusters_list, etha=0.5):
     mod = com.modularity(graph, clusters_list)
-    coverage = nx.algorithms.community.quality.coverage(graph, clusters_list)
+    coverage = nx.algorithms.community.partition_quality(graph, clusters_list)[0]
     val = (1 - etha) * coverage + etha * mod
     return val
 
 
 def endntm_find_overlap_cluster(graph, clusters_list, epsilon):
 
     node_cluster_dic = {}
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/FuzzyCom.py` & `cdlib-0.3.0/cdlib/algorithms/internal/FuzzyCom.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,22 +58,19 @@
     :param graph: networkx graph
     :param theta:
     :param eps:
     :param r:
     :return:
     """
 
-    adjacency_mat = nx.to_numpy_matrix(graph)
+    adjacency_mat = np.asmatrix(nx.to_numpy_array(graph))
 
     theta_cores = []
     num_vertices = adjacency_mat.shape[0]
 
-    # Fuzzy granule initialization
-    # gran = [i for i in range(num_vertices)]
-
     # Calculate distance between all vertices
     dist = list(nx.all_pairs_shortest_path_length(graph))
 
     # Membership values between all nodes
     fuzz_d = np.zeros(shape=adjacency_mat.shape).astype(float)
     for i in range(num_vertices):
         nid, n_dist = dist[i]
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/GDMP2_nx.py` & `cdlib-0.3.0/cdlib/algorithms/internal/GDMP2_nx.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,22 +107,26 @@
 
     A = nx.adjacency_matrix(graph)
     adj_matrix = A.todense()
 
     M = np.zeros(adj_matrix.shape)
 
     row, col = adj_matrix.shape
-
     # Building similarity function matrix, ie, Cosine Function matrix of all Column Vectors
 
     for x in range(0, row):
+        x1 = adj_matrix[:, x]
         for y in range(x, col):
-            M[x][y] = 1 - scipy.spatial.distance.cosine(
-                adj_matrix[:, x], adj_matrix[:, y]
-            )
+            y1 = adj_matrix[:, y]
+            try:
+                M[x][y] = 1 - scipy.spatial.distance.cosine(x1, y1)
+            except ValueError:
+                x1 = np.ndarray(x1.flatten())[0]
+                y1 = np.ndarray(y1.flatten())[0]
+                M[x][y] = 1 - scipy.spatial.distance.cosine(x1, y1)
 
     tuples = []
     # On basis of zero graph
     min_value = 1 if min(graph.nodes()) > 0 else 0
 
     # Considering only non zero values
     for (x, y), value in np.ndenumerate(M):
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/HLC.py` & `cdlib-0.3.0/cdlib/algorithms/internal/HLC.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/ILouvain.py` & `cdlib-0.3.0/cdlib/algorithms/internal/ILouvain.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,21 +135,21 @@
 
         return out
 
     def calculateGiniMatrixInitial(self):
         giniMatrix = {}
         for v1 in self.graph:
             giniMatrix[self.authorIndex[v1]] = {}
-        np.zeros(self.nbVertices ** 2).reshape((self.nbVertices, self.nbVertices))
+        np.zeros(self.nbVertices**2).reshape((self.nbVertices, self.nbVertices))
         for v1 in self.graph:
             for v2 in self.graph:
                 d = (
                     -1
                     * self.dist(self.authorIndex[v1], self.authorIndex[v2])
-                    / self.nbVertices ** 2
+                    / self.nbVertices**2
                 )
                 giniMatrix[self.authorIndex[v1]][self.authorIndex[v2]] = d
                 giniMatrix[self.authorIndex[v2]][self.authorIndex[v1]] = d
         """
         print "Calculating Gini Matrix Initial"
         Y = pdist(self.attributes, 'sqeuclidean')
         print "division"
@@ -292,15 +292,15 @@
                 # For the attributes
                 if giniMatrix is not None:
                     weight = giniMatrix[node][neighbor]
                 else:
                     weight = (
                         -1
                         * self.dist(self.authorIndex[node], self.authorIndex[neighbor])
-                        / self.nbVertices ** 2
+                        / self.nbVertices**2
                     )
                     weights[neighborcom][1] = weights[neighborcom][1] + weight
         return weights
 
     def __remove(self, node, com, weight, status):
         status.degrees[com] = status.degrees.get(com, 0.0) - status.gdegrees.get(
             node, 0.0
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/IPCA.py` & `cdlib-0.3.0/cdlib/algorithms/internal/IPCA.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/Kcut.py` & `cdlib-0.3.0/cdlib/algorithms/internal/Kcut.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/LAIS2_nx.py` & `cdlib-0.3.0/cdlib/algorithms/internal/LAIS2_nx.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/LEMON.py` & `cdlib-0.3.0/cdlib/algorithms/internal/LEMON.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/LPAM.py` & `cdlib-0.3.0/cdlib/algorithms/internal/LPAM.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
                 if d_i != 0 and d_j != 0:
                     s_ij = r_ij - (1 / d_i) - (1 / d_j)
                     w_ij = A[i, j]
                     w_ii = A[i, i]
                     w_jj = A[j, j]
                     u_ij = (
                         ((2 * w_ij) / (d_i * d_j))
-                        - (w_ii / (d_i ** 2))
-                        - (w_jj / (d_j ** 2))
+                        - (w_ii / (d_i**2))
+                        - (w_jj / (d_j**2))
                     )
                     C_AMP[i, j] = s_ij + u_ij
                     C_AMP[j, i] = s_ij + u_ij
                 else:
                     C_AMP[i, j] = np.NaN
                     C_AMP[j, i] = np.NaN
         return C_AMP
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/LPANNI.py` & `cdlib-0.3.0/cdlib/algorithms/internal/LPANNI.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/LSWL.py` & `cdlib-0.3.0/cdlib/algorithms/internal/LSWL.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import networkx as nx
-import os.path
 import time
 from copy import deepcopy
 import random
 
 
 class LSWLCommunityDiscovery(object):
     minimum_improvement = 0.000001
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/MCODE.py` & `cdlib-0.3.0/cdlib/algorithms/internal/MCODE.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/Markov.py` & `cdlib-0.3.0/cdlib/algorithms/internal/Markov.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/NodePerception.py` & `cdlib-0.3.0/cdlib/algorithms/internal/NodePerception.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/OSSE.py` & `cdlib-0.3.0/cdlib/algorithms/internal/OSSE.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     community = list()
 
     for s in seed:
         r[s] = 1.0 / (len(seed) * 1.0)
 
     pr_eps = 1.0 / max(10.0 * targetvol, 100.0)
     maxsteps = 1.0 / (pr_eps * (1.0 - alpha))
-    maxsteps = min(maxsteps, 0.5 * (2.0 ** 32 - 1.0))
+    maxsteps = min(maxsteps, 0.5 * (2.0**32 - 1.0))
 
     nsteps = compute_local_pagerank(G, r, p, alpha, pr_eps, int(maxsteps), q)
     if nsteps == 0:
         p = r
 
     # Scale the probabilities by their degree
     for node, pr in p.items():
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/PercoMCV.py` & `cdlib-0.3.0/cdlib/algorithms/internal/PercoMCV.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 #       this code is used, this way will allow us to know the evolution of our proposed algorithm. Injoy              #
 #                                   Contact us: contact@abil.ac.cd - University of Kinshasa                           #
 #######################################################################################################################
 
 from collections import defaultdict
 import networkx as nx
 
-# First step
-# computation of k-clique percolation algorithm
-# with k = 4
-
 
 def __k_clique_communities(g, cliques=None):
     if cliques is None:
         cliques = nx.find_cliques(g)
     cliques = [frozenset(c) for c in cliques if len(c) >= 4]
 
     # First index which nodes are in which cliques
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/RSC.py` & `cdlib-0.3.0/cdlib/algorithms/internal/RSC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import warnings
 import networkx as nx
 import numpy as np
-import scipy
 
 warnings.filterwarnings("ignore")
 
 """
 Reconstructing [1]
 [1] Understanding Regularized Spectral Clustering via Graph Conductance Yilin Zhang, Karl Rohe: NIPS'18
 https://arxiv.org/pdf/1806.01468.pdf
@@ -146,22 +145,20 @@
     # Experiment only on undirected graphs
     if graph.is_directed():
         graph = graph.to_undirected()
 
     # Before computing anything, largest connected component identified and used
     graph = graph.subgraph(max(nx.connected_components(graph), key=len)).copy()
 
-    adj_matrix = nx.to_scipy_sparse_matrix(graph, format="csr")
+    adj_matrix = nx.to_scipy_sparse_array(graph, format="csr")
 
     if method == "sklearn_spectral_embedding":
-        (
-            labels,
-            num_iterations,
-            smallest_cluster_size,
-        ) = __sklearn_spectral_clustering(adj_matrix, n_clusters)
+        (labels, num_iterations, smallest_cluster_size) = __sklearn_spectral_clustering(
+            adj_matrix, n_clusters
+        )
 
     elif method == "sklearn_kmeans":
         labels, num_iterations, smallest_cluster_size = __sklearn_kmeans(
             adj_matrix, n_clusters
         )
 
     elif method == "vanilla":
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/SLPA_nx.py` & `cdlib-0.3.0/cdlib/algorithms/internal/SLPA_nx.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/SiblinarityAntichain.py` & `cdlib-0.3.0/cdlib/algorithms/internal/SiblinarityAntichain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jun 20 12:52:55 2018
 @author: Vaiva & Tim
 """
 
-from collections import defaultdict
-import itertools
+
 import numpy as np
 import random
 import itertools
-import math
 import networkx as nx
 import scipy.sparse as sparse
 
 __authors__ = ["Vaiva Vasiliauskaite", "T.S. Evans"]
 __all__ = ["matrix_node_recursive_antichain_partition"]
 
 
@@ -46,17 +44,22 @@
 
     # class variables
     def __init__(self, node_id_dict, similarity_matrix, Lambda, with_replacement):
         # Initial Quality Measures
         self.similarity_matrix = similarity_matrix
         self.node_id_dict = node_id_dict
         self.strength = similarity_matrix.sum(axis=0)
-        self.strength = {
-            n: self.strength[0, node_id_dict[n]] for n in node_id_dict.keys()
-        }  # sum over rows?
+        try:
+            self.strength = {
+                n: self.strength[node_id_dict[n]] for n in node_id_dict.keys()
+            }  # sum over rows?
+        except IndexError:
+            self.strength = {
+                n: self.strength[0, node_id_dict[n]] for n in node_id_dict.keys()
+            }
         self.total_weight = similarity_matrix.sum()  # /2
         self.Lambda = Lambda
         self.with_replacement = with_replacement
 
     def delta_strength_quality_unnormalised(self, partition1, partition2):
         """
         Using in-strength null model calculate the change in unnormalised quality if two partitions are combined.
@@ -476,17 +479,18 @@
     target_nodes - list of nodes
 
     Return
     ------
     True - if nodes in source_nodes and target_nodes form a weakly_connected subgraph
     False - if not
     """
-    source_nodes_id, target_nodes_id = [nodedict[s] for s in source_nodes], [
-        nodedict[t] for t in target_nodes
-    ]
+    source_nodes_id, target_nodes_id = (
+        [nodedict[s] for s in source_nodes],
+        [nodedict[t] for t in target_nodes],
+    )
 
     for s, t in itertools.product(source_nodes_id, target_nodes_id):
         if path_matrix[s, t] == 1 or path_matrix[t, s] == 1:
             return True
     return False
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/UMSTMO.py` & `cdlib-0.3.0/cdlib/algorithms/internal/UMSTMO.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import networkx as nx
-import itertools
 
 parent = dict()
 rank = dict()
 
 
 def __make_set(vertice):
     parent[vertice] = vertice
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/belief_prop.py` & `cdlib-0.3.0/cdlib/algorithms/internal/belief_prop.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/core_exp.py` & `cdlib-0.3.0/cdlib/algorithms/internal/core_exp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Aug 12 09:14:20 2020
 @author: saipr
 """
-import pandas as pd
 import networkx as nx
 import numpy as np
-import matplotlib.pyplot as plt
-from networkx import community as c
-import community as com
-import itertools
-import random
-from random import sample
-from networkx import algorithms as al
 
 
 # --------------------Methods in Core Expansion--------------------------------#
 
 # Managing method to call everything as need be
 def findCommunities(g, tol=0.0005):
     # assign all the edges their neighborhoodOverlap
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/em.py` & `cdlib-0.3.0/cdlib/algorithms/internal/em.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             for g in range(self.k):
                 x = self.pi[g]
                 for j in self.g.neighbors(i):
                     x *= self.theta[g][j]
                 q[i].append(x)
                 norm += x
             for g in range(self.k):
-                q[i][g] /= norm
+                q[i][g] /= (norm + 1e-10)  # tolerance adjustment
 
     def m_step(self, q):
         for g in range(self.k):
             sum1 = 0.0
             sum3 = 0.0
             for i in range(self.n):
                 sum1 += q[i][g]
@@ -43,15 +43,15 @@
                 sum3 += q[i][g] * len(list(self.g.neighbors(i)))
             self.pi[g] = sum1 / self.n  # update pi
             for i in range(self.n):
                 self.theta[g][i] /= sum3  # norm
 
     def execute(self):
         # initial parameters
-        X = [1.0 + random.random() for i in range(self.k)]
+        X = [1.0 + random.random() for _ in range(self.k)]
         norm = sum(X)
         self.pi = [x / norm for x in X]
 
         for i in range(self.k):
             Y = [1.0 + random.random() for j in range(self.n)]
             norm = sum(Y)
             self.theta.append([y / norm for y in Y])
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/ga.py` & `cdlib-0.3.0/cdlib/algorithms/internal/ga.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             for j in s:
                 submatrix[i][j] = matrix[i][j]
         M = 0
         v = 0
         for row in list(s):
             row_mean = np.sum(submatrix[row]) / len(s)
             v += np.sum(submatrix[row])
-            M += (row_mean ** r) / len(s)
+            M += (row_mean**r) / len(s)
         CS += M * v
     return CS
 
 
 def __roulette_selection(df_elites):
     prob = np.random.random_sample()
     sum_cs = np.sum(df_elites["community_score"])
@@ -138,15 +138,19 @@
 
 def __mutation(chrom, Adj, mutation_rate):
     if np.random.random_sample() < mutation_rate:
         chrom = chrom
         neighbor = []
         while len(neighbor) < 2:
             mutant = np.random.randint(1, len(chrom))
-            row = Adj[mutant].toarray()[0]
+            if not isinstance(Adj, np.ndarray):
+                Adj = Adj.toarray()
+            # Adj = Adj.toarray()
+            # print(type(Adj), Adj, Adj[mutant])
+            row = Adj[mutant]
             neighbor = [i for i in range(len(row)) if row[i] == 1]
             if len(neighbor) > 1:
                 neighbor.remove(chrom[mutant])
                 to_change = int(np.floor(np.random.random_sample() * (len(neighbor))))
                 chrom[mutant] = neighbor[to_change]
                 neighbor.append(chrom[mutant])
     return chrom
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/graph_entropy.py` & `cdlib-0.3.0/cdlib/algorithms/internal/graph_entropy.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/headtail.py` & `cdlib-0.3.0/cdlib/algorithms/internal/headtail.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import networkx as nx
-import timeit
 import numpy as np
 
 
 def __HeadTailCommunityDetection(G, finaledgelist, head_tail_ratio=0.6):
 
     H = nx.connected_components(G)
 
     for s in H:
         subgraph = nx.subgraph(G, s)
-        result = nx.edge_betweenness(subgraph, normalized=False)
+        result = nx.algorithms.edge_betweenness_centrality(subgraph, normalized=False)
         edges = list(result.keys())
         values = list(result.values())
         mean = np.mean(values)
         edgelist = []
         edgetemp = subgraph.edges()
         if len(edgetemp) <= 2:
             for edge in edgetemp:
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/lfm.py` & `cdlib-0.3.0/cdlib/algorithms/internal/lfm.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/modularity_m.py` & `cdlib-0.3.0/cdlib/algorithms/internal/modularity_m.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import networkx as nx
-
-import time
 from random import random, shuffle
 
 
 class ModularityMCommunityDiscovery:
     def __init__(self, graph):
         self.graph = graph
         self.starting_node = None
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/modularity_r.py` & `cdlib-0.3.0/cdlib/algorithms/internal/modularity_r.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import networkx as nx
-
-import time
 from random import random
 
 
 class ModularityRCommunityDiscovery(object):
     minimum_improvement = 0.000001
 
     def __init__(self, graph):
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/multicom.py` & `cdlib-0.3.0/cdlib/algorithms/internal/multicom.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/paris.py` & `cdlib-0.3.0/cdlib/algorithms/internal/paris.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/principled.py` & `cdlib-0.3.0/cdlib/algorithms/internal/principled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import math
 import random
-import sys
 import operator
 from collections import defaultdict
 
 
 def principled(g, cluster_count):
 
     clusters = range(cluster_count)
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/pycondor.py` & `cdlib-0.3.0/cdlib/algorithms/internal/pycondor.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/scan.py` & `cdlib-0.3.0/cdlib/algorithms/internal/scan.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/spectralCD.py` & `cdlib-0.3.0/cdlib/algorithms/internal/spectralCD.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/walkscan.py` & `cdlib-0.3.0/cdlib/algorithms/internal/walkscan.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal/weightedCommunity.py` & `cdlib-0.3.0/cdlib/algorithms/internal/weightedCommunity.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/internal_dcd/eTILES.py` & `cdlib-0.3.0/cdlib/algorithms/internal_dcd/eTILES.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/algorithms/overlapping_partition.py` & `cdlib-0.3.0/cdlib/algorithms/overlapping_partition.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from cdlib.algorithms.internal.CONGA import Conga_
 from cdlib.algorithms.internal.LAIS2_nx import LAIS2
 from cdlib.algorithms.internal.lfm import LFM_nx
 from cdlib.algorithms.internal import LEMON
 from cdlib.algorithms.internal.SLPA_nx import slpa_nx
 from cdlib.algorithms.internal.multicom import MultiCom
 from cdlib.algorithms.internal.PercoMCV import percoMVC
-from cdlib.algorithms.internal.LPAM import LPAM
 from cdlib.algorithms.internal.core_exp import findCommunities as core_exp_find
 from cdlib.algorithms.internal.weightedCommunity import weightedCommunity
 from cdlib.algorithms.internal.LPANNI import LPANNI, GraphGenerator
 from cdlib.algorithms.internal.DCS import main_dcs
 from cdlib.algorithms.internal.UMSTMO import UMSTMO
 from cdlib.algorithms.internal.walkscan import WalkSCAN
 from cdlib.algorithms.internal.IPCA import i_pca
@@ -28,36 +27,38 @@
 from cdlib.algorithms.internal.COACH import co_ach
 from cdlib.algorithms.internal.graph_entropy import graphentropy
 from cdlib.algorithms.internal.EBGC import EBGC
 from cdlib.algorithms.internal.EnDNTM import (
     endntm_find_overlap_cluster,
     endntm_evalFuction,
 )
+from cdlib.prompt_utils import report_missing_packages
+
 import warnings
 
 missing_packages = set()
 
 
-def __try_load_karate(init=False):
-    global karateclub
-    if init == True or "karateclub" not in sys.modules:
-        try:
-            import karateclub
-
-        except ModuleNotFoundError:
-            if not init:
-                raise ModuleNotFoundError(
-                    "Optional dependency not satisfied: install karateclub to use the selected feature."
-                )
-
-
-__try_load_karate(init=True)
-if "karateclub" not in sys.modules:
-    karateclub = None
-    missing_packages.add("karateclub")
+# def __try_load_karate(init=False):
+#     global karateclub
+#     if init == True or "karateclub" not in sys.modules:
+#         try:
+#             import karateclub
+#
+#         except ModuleNotFoundError:
+#             if not init:
+#                 raise ModuleNotFoundError(
+#                     "Optional dependency not satisfied: install karateclub to use the selected feature."
+#                 )
+#
+#
+# __try_load_karate(init=True)
+# if "karateclub" not in sys.modules:
+#     karateclub = None
+#     missing_packages.add("karateclub")
 
 
 try:
     import igraph as ig
 except ModuleNotFoundError:
     ig = None
 try:
@@ -67,19 +68,22 @@
 
 try:
     from ASLPAw_package import ASLPAw
 except ModuleNotFoundError:
     ASLPAw = None
     missing_packages.add("ASLPAw")
 
-if len(missing_packages) > 0:
-    print(
-        "Note: to be able to use all overlapping methods, you need to install some additional packages: ",
-        missing_packages,
-    )
+try:
+    import pyclustering
+    from cdlib.algorithms.internal.LPAM import LPAM
+except ModuleNotFoundError:
+    LPAM = None
+    missing_packages.add("pyclustering")
+
+report_missing_packages(missing_packages)
 
 __all__ = [
     "ego_networks",
     "demon",
     "angel",
     "node_perception",
     "overlapping_seed_set_expansion",
@@ -87,28 +91,28 @@
     "lfm",
     "lais2",
     "congo",
     "conga",
     "lemon",
     "slpa",
     "multicom",
-    "big_clam",
-    "danmf",
-    "egonet_splitter",
-    "nnsed",
-    "mnmf",
+    # "big_clam",
+    # "danmf",
+    # "egonet_splitter",
+    # "nnsed",
+    # "mnmf",
     "aslpaw",
     "percomvc",
     "wCommunity",
     "core_expansion",
     "lpanni",
     "lpam",
     "dcs",
     "umstmo",
-    "symmnmf",
+    # "symmnmf",
     "walkscan",
     "endntm",
     "ipca",
     "dpclus",
     "coach",
     "graph_entropy",
     "ebgc",
@@ -661,15 +665,15 @@
     if ig is None:
         raise ModuleNotFoundError(
             "Optional dependency not satisfied: install igraph to use the selected feature."
         )
 
     g = convert_graph_formats(g_original, ig.Graph)
 
-    communities = Conga_(g, number_communities=3)
+    communities = Conga_(g, number_communities=number_communities)
     coms = []
     for c in communities:
         coms.append([g.vs[x]["name"] for x in c])
 
     return NodeClustering(
         coms,
         g_original,
@@ -865,369 +869,369 @@
         g_original,
         "Multicom",
         method_parameters={"seeds": seed_node},
         overlap=True,
     )
 
 
-def big_clam(
-    g_original: object,
-    dimensions: int = 8,
-    iterations: int = 50,
-    learning_rate: float = 0.005,
-) -> NodeClustering:
-    """
-    BigClam is an overlapping community detection method that scales to large networks.
-    The procedure uses gradient ascent to create an embedding which is used for deciding the node-cluster affiliations.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param dimensions: Number of embedding dimensions. Default 8.
-    :param iterations: Number of training iterations. Default 50.
-    :param learning_rate: Gradient ascent learning rate. Default is 0.005.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.big_clam(G)
-
-    :References:
-
-    Yang, Jaewon, and Jure Leskovec. "Overlapping community detection at scale: a nonnegative matrix factorization approach." Proceedings of the sixth ACM international conference on Web search and data mining. 2013.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    __try_load_karate()
-    g = convert_graph_formats(g_original, nx.Graph)
-
-    model = karateclub.BigClam(
-        dimensions=dimensions, iterations=iterations, learning_rate=learning_rate
-    )
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "BigClam",
-        method_parameters={
-            "dimensions": dimensions,
-            "iterations": iterations,
-            "learning_rate": learning_rate,
-        },
-        overlap=True,
-    )
-
-
-def danmf(
-    g_original: object,
-    layers: tuple = (32, 8),
-    pre_iterations: int = 100,
-    iterations: int = 100,
-    seed: int = 42,
-    lamb: float = 0.01,
-) -> NodeClustering:
-    """
-    The procedure uses telescopic non-negative matrix factorization in order to learn a cluster memmbership distribution over nodes. The method can be used in an overlapping and non-overlapping way.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       Yes
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param layers: Autoencoder layer sizes in a list of integers. Default [32, 8].
-    :param pre_iterations: Number of pre-training epochs. Default 100.
-    :param iterations: Number of training epochs. Default 100.
-    :param seed: Random seed for weight initializations. Default 42.
-    :param lamb: Regularization parameter. Default 0.01.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.danmf(G)
-
-    :References:
-
-    Ye, Fanghua, Chuan Chen, and Zibin Zheng. "Deep autoencoder-like nonnegative matrix factorization for community detection." Proceedings of the 27th ACM International Conference on Information and Knowledge Management. 2018.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-
-    __try_load_karate()
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.DANMF(layers, pre_iterations, iterations, seed, lamb)
-
-    mapping = {node: i for i, node in enumerate(g.nodes())}
-    rev = {i: node for node, i in mapping.items()}
-    H = nx.relabel_nodes(g, mapping)
-
-    model.fit(H)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(rev[n])
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "DANMF",
-        method_parameters={
-            "layers": layers,
-            "pre_iteration": pre_iterations,
-            "iterations": iterations,
-            "seed": seed,
-            "lamb": lamb,
-        },
-        overlap=True,
-    )
-
-
-def egonet_splitter(g_original: object, resolution: float = 1.0) -> NodeClustering:
-    """
-    The method first creates the egonets of nodes. A persona-graph is created which is clustered by the Louvain method.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param resolution: Resolution parameter of Python Louvain. Default 1.0.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.egonet_splitter(G)
-
-    :References:
-
-    Epasto, Alessandro, Silvio Lattanzi, and Renato Paes Leme. "Ego-splitting framework: From non-overlapping to overlapping clusters." Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining. 2017.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    __try_load_karate()
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.EgoNetSplitter(resolution=resolution)
-
-    mapping = {node: i for i, node in enumerate(g.nodes())}
-    rev = {i: node for node, i in mapping.items()}
-    H = nx.relabel_nodes(g, mapping)
-
-    model.fit(H)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, cs in members.items():
-        for c in cs:
-            coms_to_node[c].append(rev[n])
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "EgoNetSplitter",
-        method_parameters={"resolution": resolution},
-        overlap=True,
-    )
-
-
-def nnsed(
-    g_original: object, dimensions: int = 32, iterations: int = 10, seed: int = 42
-) -> NodeClustering:
-    """
-    The procedure uses non-negative matrix factorization in order to learn an unnormalized cluster membership distribution over nodes. The method can be used in an overlapping and non-overlapping way.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param dimensions: Embedding layer size. Default is 32.
-    :param iterations: Number of training epochs. Default 10.
-    :param seed:  Random seed for weight initializations. Default 42.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.nnsed(G)
-
-    :References:
-
-    Sun, Bing-Jie, et al. "A non-negative symmetric encoder-decoder approach for community detection." Proceedings of the 2017 ACM on Conference on Information and Knowledge Management. 2017.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-
-    __try_load_karate()
-
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.NNSED(dimensions=dimensions, iterations=iterations, seed=seed)
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "NNSED",
-        method_parameters={
-            "dimension": dimensions,
-            "iterations": iterations,
-            "seed": seed,
-        },
-        overlap=True,
-    )
-
-
-def mnmf(
-    g_original: object,
-    dimensions: int = 128,
-    clusters: int = 10,
-    lambd: float = 0.2,
-    alpha: float = 0.05,
-    beta: float = 0.05,
-    iterations: int = 200,
-    lower_control: float = 1e-15,
-    eta: float = 5.0,
-) -> NodeClustering:
-    """
-    The procedure uses joint non-negative matrix factorization with modularity based regul;arization in order to learn a cluster memmbership distribution over nodes.
-    The method can be used in an overlapping and non-overlapping way.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param dimensions: Number of dimensions. Default is 128.
-    :param clusters: Number of clusters. Default is 10.
-    :param lambd: KKT penalty. Default is 0.2
-    :param alpha: Clustering penalty. Default is 0.05.
-    :param beta: Modularity regularization penalty. Default is 0.05.
-    :param iterations:  Number of power iterations. Default is 200.
-    :param lower_control: Floating point overflow control. Default is 10**-15.
-    :param eta: Similarity mixing parameter. Default is 5.0.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.mnmf(G)
-
-    :References:
-
-    Wang, Xiao, et al. "Community preserving network embedding." Thirty-first AAAI conference on artificial intelligence. 2017.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    __try_load_karate()
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.MNMF(
-        dimensions=dimensions,
-        clusters=clusters,
-        lambd=lambd,
-        alpha=alpha,
-        beta=beta,
-        iterations=iterations,
-        lower_control=lower_control,
-        eta=eta,
-    )
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "MNMF",
-        method_parameters={
-            "dimension": dimensions,
-            "clusters": clusters,
-            "lambd": lambd,
-            "alpha": alpha,
-            "beta": beta,
-            "iterations": iterations,
-            "lower_control": lower_control,
-            "eta": eta,
-        },
-        overlap=True,
-    )
+# def big_clam(
+#     g_original: object,
+#     dimensions: int = 8,
+#     iterations: int = 50,
+#     learning_rate: float = 0.005,
+# ) -> NodeClustering:
+#     """
+#     BigClam is an overlapping community detection method that scales to large networks.
+#     The procedure uses gradient ascent to create an embedding which is used for deciding the node-cluster affiliations.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param dimensions: Number of embedding dimensions. Default 8.
+#     :param iterations: Number of training iterations. Default 50.
+#     :param learning_rate: Gradient ascent learning rate. Default is 0.005.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.big_clam(G)
+#
+#     :References:
+#
+#     Yang, Jaewon, and Jure Leskovec. "Overlapping community detection at scale: a nonnegative matrix factorization approach." Proceedings of the sixth ACM international conference on Web search and data mining. 2013.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     __try_load_karate()
+#     g = convert_graph_formats(g_original, nx.Graph)
+#
+#     model = karateclub.BigClam(
+#         dimensions=dimensions, iterations=iterations, learning_rate=learning_rate
+#     )
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "BigClam",
+#         method_parameters={
+#             "dimensions": dimensions,
+#             "iterations": iterations,
+#             "learning_rate": learning_rate,
+#         },
+#         overlap=True,
+#     )
+
+
+# def danmf(
+#     g_original: object,
+#     layers: tuple = (32, 8),
+#     pre_iterations: int = 100,
+#     iterations: int = 100,
+#     seed: int = 42,
+#     lamb: float = 0.01,
+# ) -> NodeClustering:
+#     """
+#     The procedure uses telescopic non-negative matrix factorization in order to learn a cluster memmbership distribution over nodes. The method can be used in an overlapping and non-overlapping way.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       Yes
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param layers: Autoencoder layer sizes in a list of integers. Default [32, 8].
+#     :param pre_iterations: Number of pre-training epochs. Default 100.
+#     :param iterations: Number of training epochs. Default 100.
+#     :param seed: Random seed for weight initializations. Default 42.
+#     :param lamb: Regularization parameter. Default 0.01.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.danmf(G)
+#
+#     :References:
+#
+#     Ye, Fanghua, Chuan Chen, and Zibin Zheng. "Deep autoencoder-like nonnegative matrix factorization for community detection." Proceedings of the 27th ACM International Conference on Information and Knowledge Management. 2018.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#
+#     __try_load_karate()
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.DANMF(layers, pre_iterations, iterations, seed, lamb)
+#
+#     mapping = {node: i for i, node in enumerate(g.nodes())}
+#     rev = {i: node for node, i in mapping.items()}
+#     H = nx.relabel_nodes(g, mapping)
+#
+#     model.fit(H)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(rev[n])
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "DANMF",
+#         method_parameters={
+#             "layers": layers,
+#             "pre_iteration": pre_iterations,
+#             "iterations": iterations,
+#             "seed": seed,
+#             "lamb": lamb,
+#         },
+#         overlap=True,
+#     )
+
+
+# def egonet_splitter(g_original: object, resolution: float = 1.0) -> NodeClustering:
+#     """
+#     The method first creates the egonets of nodes. A persona-graph is created which is clustered by the Louvain method.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param resolution: Resolution parameter of Python Louvain. Default 1.0.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.egonet_splitter(G)
+#
+#     :References:
+#
+#     Epasto, Alessandro, Silvio Lattanzi, and Renato Paes Leme. "Ego-splitting framework: From non-overlapping to overlapping clusters." Proceedings of the 23rd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining. 2017.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     __try_load_karate()
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.EgoNetSplitter(resolution=resolution)
+#
+#     mapping = {node: i for i, node in enumerate(g.nodes())}
+#     rev = {i: node for node, i in mapping.items()}
+#     H = nx.relabel_nodes(g, mapping)
+#
+#     model.fit(H)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, cs in members.items():
+#         for c in cs:
+#             coms_to_node[c].append(rev[n])
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "EgoNetSplitter",
+#         method_parameters={"resolution": resolution},
+#         overlap=True,
+#     )
+
+
+# def nnsed(
+#     g_original: object, dimensions: int = 32, iterations: int = 10, seed: int = 42
+# ) -> NodeClustering:
+#     """
+#     The procedure uses non-negative matrix factorization in order to learn an unnormalized cluster membership distribution over nodes. The method can be used in an overlapping and non-overlapping way.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param dimensions: Embedding layer size. Default is 32.
+#     :param iterations: Number of training epochs. Default 10.
+#     :param seed:  Random seed for weight initializations. Default 42.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.nnsed(G)
+#
+#     :References:
+#
+#     Sun, Bing-Jie, et al. "A non-negative symmetric encoder-decoder approach for community detection." Proceedings of the 2017 ACM on Conference on Information and Knowledge Management. 2017.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#
+#     __try_load_karate()
+#
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.NNSED(dimensions=dimensions, iterations=iterations, seed=seed)
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "NNSED",
+#         method_parameters={
+#             "dimension": dimensions,
+#             "iterations": iterations,
+#             "seed": seed,
+#         },
+#         overlap=True,
+#     )
+
+
+# def mnmf(
+#     g_original: object,
+#     dimensions: int = 128,
+#     clusters: int = 10,
+#     lambd: float = 0.2,
+#     alpha: float = 0.05,
+#     beta: float = 0.05,
+#     iterations: int = 200,
+#     lower_control: float = 1e-15,
+#     eta: float = 5.0,
+# ) -> NodeClustering:
+#     """
+#     The procedure uses joint non-negative matrix factorization with modularity based regul;arization in order to learn a cluster memmbership distribution over nodes.
+#     The method can be used in an overlapping and non-overlapping way.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param dimensions: Number of dimensions. Default is 128.
+#     :param clusters: Number of clusters. Default is 10.
+#     :param lambd: KKT penalty. Default is 0.2
+#     :param alpha: Clustering penalty. Default is 0.05.
+#     :param beta: Modularity regularization penalty. Default is 0.05.
+#     :param iterations:  Number of power iterations. Default is 200.
+#     :param lower_control: Floating point overflow control. Default is 10**-15.
+#     :param eta: Similarity mixing parameter. Default is 5.0.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.mnmf(G)
+#
+#     :References:
+#
+#     Wang, Xiao, et al. "Community preserving network embedding." Thirty-first AAAI conference on artificial intelligence. 2017.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     __try_load_karate()
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.MNMF(
+#         dimensions=dimensions,
+#         clusters=clusters,
+#         lambd=lambd,
+#         alpha=alpha,
+#         beta=beta,
+#         iterations=iterations,
+#         lower_control=lower_control,
+#         eta=eta,
+#     )
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "MNMF",
+#         method_parameters={
+#             "dimension": dimensions,
+#             "clusters": clusters,
+#             "lambd": lambd,
+#             "alpha": alpha,
+#             "beta": beta,
+#             "iterations": iterations,
+#             "lower_control": lower_control,
+#             "eta": eta,
+#         },
+#         overlap=True,
+#     )
 
 
 def aslpaw(g_original: object) -> NodeClustering:
     """
     ASLPAw can be used for disjoint and overlapping community detection and works on weighted/unweighted and directed/undirected networks.
     ASLPAw is adaptive with virtually no configuration parameters.
 
@@ -1517,14 +1521,19 @@
     >>> coms = algorithms.lpam(G, k=2, threshold=0.4, distance = "amp")
 
     :References:
 
     Alexander Ponomarenko, Leonidas Pitsoulis, Marat Shamshetdinov. "Link Partitioning Around Medoids". https://arxiv.org/abs/1907.08731
 
     """
+    if LPAM is None:
+        raise ModuleNotFoundError(
+            "Optional dependency not satisfied: install pyclustering (pip install pyclustering). Not available in CDlib Conda-based installation."
+        )
+
     g = convert_graph_formats(g_original, nx.Graph)
     return LPAM(graph=g, k=k, threshold=threshold, distance=distance, seed=seed)
 
 
 def dcs(g_original: object) -> NodeClustering:
     """
     Divide and Conquer Strategy
@@ -1595,82 +1604,82 @@
     g = convert_graph_formats(g_original, nx.Graph)
     communities = UMSTMO(g)
     return NodeClustering(
         communities, g_original, "UMSTMO", method_parameters={}, overlap=True
     )
 
 
-def symmnmf(
-    g_original: object,
-    dimensions: int = 32,
-    iterations: int = 200,
-    rho: float = 100.0,
-    seed: int = 42,
-) -> NodeClustering:
-    """
-    The procedure decomposed the second power od the normalized adjacency matrix with an ADMM based non-negative matrix factorization based technique.
-    This results in a node embedding and each node is associated with an embedding factor in the created latent space.
-
-
-    **Supported Graph Types**
-
-    ========== ======== ========
-    Undirected Directed Weighted
-    ========== ======== ========
-    Yes        No       No
-    ========== ======== ========
-
-    :param g_original: a networkx/igraph object
-    :param dimensions: Number of dimensions. Default is 32.
-    :param iterations:  Number of power iterations. Default is 200.
-    :param rho: Regularization tuning parameter. Default is 100.0.
-    :param seed: Random seed value. Default is 42.
-    :return: NodeClustering object
-
-
-    :Example:
-
-    >>> from cdlib import algorithms
-    >>> import networkx as nx
-    >>> G = nx.karate_club_graph()
-    >>> coms = algorithms.symmnmf(G)
-
-    :References:
-
-    Kuang, Da, Chris Ding, and Haesun Park. "Symmetric nonnegative matrix factorization for graph clustering." Proceedings of the 2012 SIAM international conference on data mining. Society for Industrial and Applied Mathematics, 2012.
-
-    .. note:: Reference implementation: https://karateclub.readthedocs.io/
-    """
-    __try_load_karate()
-    g = convert_graph_formats(g_original, nx.Graph)
-    model = karateclub.SymmNMF(
-        dimensions=dimensions, iterations=iterations, rho=rho, seed=seed
-    )
-    model.fit(g)
-    members = model.get_memberships()
-
-    # Reshaping the results
-    coms_to_node = defaultdict(list)
-    for n, c in members.items():
-        coms_to_node[c].append(n)
-
-    coms = [list(c) for c in coms_to_node.values()]
-
-    return NodeClustering(
-        coms,
-        g_original,
-        "SymmNMF",
-        method_parameters={
-            "dimension": dimensions,
-            "iterations": iterations,
-            "rho": rho,
-            "seed": seed,
-        },
-        overlap=True,
-    )
+# def symmnmf(
+#     g_original: object,
+#     dimensions: int = 32,
+#     iterations: int = 200,
+#     rho: float = 100.0,
+#     seed: int = 42,
+# ) -> NodeClustering:
+#     """
+#     The procedure decomposed the second power od the normalized adjacency matrix with an ADMM based non-negative matrix factorization based technique.
+#     This results in a node embedding and each node is associated with an embedding factor in the created latent space.
+#
+#
+#     **Supported Graph Types**
+#
+#     ========== ======== ========
+#     Undirected Directed Weighted
+#     ========== ======== ========
+#     Yes        No       No
+#     ========== ======== ========
+#
+#     :param g_original: a networkx/igraph object
+#     :param dimensions: Number of dimensions. Default is 32.
+#     :param iterations:  Number of power iterations. Default is 200.
+#     :param rho: Regularization tuning parameter. Default is 100.0.
+#     :param seed: Random seed value. Default is 42.
+#     :return: NodeClustering object
+#
+#
+#     :Example:
+#
+#     >>> from cdlib import algorithms
+#     >>> import networkx as nx
+#     >>> G = nx.karate_club_graph()
+#     >>> coms = algorithms.symmnmf(G)
+#
+#     :References:
+#
+#     Kuang, Da, Chris Ding, and Haesun Park. "Symmetric nonnegative matrix factorization for graph clustering." Proceedings of the 2012 SIAM international conference on data mining. Society for Industrial and Applied Mathematics, 2012.
+#
+#     .. note:: Reference implementation: https://karateclub.readthedocs.io/
+#     """
+#     __try_load_karate()
+#     g = convert_graph_formats(g_original, nx.Graph)
+#     model = karateclub.SymmNMF(
+#         dimensions=dimensions, iterations=iterations, rho=rho, seed=seed
+#     )
+#     model.fit(g)
+#     members = model.get_memberships()
+#
+#     # Reshaping the results
+#     coms_to_node = defaultdict(list)
+#     for n, c in members.items():
+#         coms_to_node[c].append(n)
+#
+#     coms = [list(c) for c in coms_to_node.values()]
+#
+#     return NodeClustering(
+#         coms,
+#         g_original,
+#         "SymmNMF",
+#         method_parameters={
+#             "dimension": dimensions,
+#             "iterations": iterations,
+#             "rho": rho,
+#             "seed": seed,
+#         },
+#         overlap=True,
+#     )
 
 
 def walkscan(
     g_original: object,
     nb_steps: int = 2,
     eps: float = 0.1,
     min_samples: int = 3,
@@ -1803,19 +1812,15 @@
             "clusterings": [clustering.method_name for clustering in clusterings],
             "epsilon": epsilon,
         },
         overlap=True,
     )
 
 
-def ipca(
-    g_original: object,
-    weights: str = None,
-    t_in: float = 0.5,
-) -> NodeClustering:
+def ipca(g_original: object, weights: str = None, t_in: float = 0.5) -> NodeClustering:
     """
     IPCA was introduced by Li et al. (2008) as a modiﬁed version of DPClus.
     In contrast to DPClus, this method focuses on the maintaining the diameter of a cluster, deﬁned as the maximum shortest distance between all pairs of vertices, rather than its density.
     In doing so, the seed growth aspect of IPCA emphasizes structural closeness of a predicted protein complex, as well as structural connectivity.
 
     Like DPClus, IPCA computes local vertex and edge weights by counting the number of common neighbors shared between two vertices.
     However, IPCA calculates these values only once at the beginning of the algorithm, rather than updating them every time a discovered cluster is removed from the graph.
@@ -1848,28 +1853,18 @@
     Li, M., Chen, J., Wang, J., Hu, B., Chen, G. 2008. Modifying the DPClus algorithm for identifying protein complexes based on new topological structures. BMC Bioinformatics 9, 398.
 
 
     .. note:: Reference Implementation: https://github.com/trueprice/python-graph-clustering
     """
 
     g = convert_graph_formats(g_original, nx.Graph)
-    clustering = i_pca(
-        g,
-        weights=weights,
-        t_in=t_in,
-    )
+    clustering = i_pca(g, weights=weights, t_in=t_in)
 
     return NodeClustering(
-        clustering,
-        g_original,
-        "ipca",
-        method_parameters={
-            "t_in": t_in,
-        },
-        overlap=True,
+        clustering, g_original, "ipca", method_parameters={"t_in": t_in}, overlap=True
     )
 
 
 def dpclus(
     g_original: object,
     weights: str = None,
     d_threshold: float = 0.9,
@@ -1990,18 +1985,15 @@
             "affinity_threshold": affinity_threshold,
             "closeness_threshold": closeness_threshold,
         },
         overlap=True,
     )
 
 
-def graph_entropy(
-    g_original: object,
-    weights: str = None,
-) -> NodeClustering:
+def graph_entropy(g_original: object, weights: str = None) -> NodeClustering:
     """
     This method takes advantage of the use of entropy with regard to information theory.
     Entropy is a measure of uncertainty involved in a random variable.
 
     This approach uses a new deﬁnition, Graph Entropy, as a measure of structural complexity in a graph.
     This algorithm incorporates a seed-growth technique.
     Unlike the other seed-growth style methods, however, the graph entropy approach does not require any predetermined threshold because it searches for an optimal solution by minimizing graph entropy.
@@ -2040,19 +2032,15 @@
     .. note:: Reference Implementation: https://github.com/trueprice/python-graph-clustering
     """
 
     g = convert_graph_formats(g_original, nx.Graph)
     clustering = graphentropy(g, weight=weights)
 
     return NodeClustering(
-        clustering,
-        g_original,
-        "graph_entropy",
-        method_parameters={},
-        overlap=True,
+        clustering, g_original, "graph_entropy", method_parameters={}, overlap=True
     )
 
 
 def ebgc(
     g_original: object,
 ) -> NodeClustering:
     """
@@ -2097,13 +2085,9 @@
     clustering = defaultdict(list)
     for idn, v in enumerate(node_labels):
         clustering[v].append(reverse_map[idn])
 
     clustering = [c for c in clustering.values()]
 
     return NodeClustering(
-        clustering,
-        g_original,
-        "ebgc",
-        method_parameters={},
-        overlap=True,
+        clustering, g_original, "ebgc", method_parameters={}, overlap=True
     )
```

### Comparing `cdlib-0.2.6/cdlib/algorithms/temporal_partition.py` & `cdlib-0.3.0/cdlib/algorithms/temporal_partition.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/benchmark/dynamic_benchmark.py` & `cdlib-0.3.0/cdlib/benchmark/dynamic_benchmark.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/benchmark/internal/rdyn.py` & `cdlib-0.3.0/cdlib/benchmark/internal/rdyn.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/benchmark/internal/xmark.py` & `cdlib-0.3.0/cdlib/benchmark/internal/xmark.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/benchmark/static_benchmark.py` & `cdlib-0.3.0/cdlib/benchmark/static_benchmark.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/attr_node_clustering.py` & `cdlib-0.3.0/cdlib/classes/attr_node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/bipartite_node_clustering.py` & `cdlib-0.3.0/cdlib/classes/bipartite_node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/clustering.py` & `cdlib-0.3.0/cdlib/classes/clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/edge_clustering.py` & `cdlib-0.3.0/cdlib/classes/edge_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/fuzzy_node_clustering.py` & `cdlib-0.3.0/cdlib/classes/fuzzy_node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/named_clustering.py` & `cdlib-0.3.0/cdlib/classes/named_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/node_clustering.py` & `cdlib-0.3.0/cdlib/classes/node_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/classes/temporal_clustering.py` & `cdlib-0.3.0/cdlib/classes/temporal_clustering.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/datasets/remote.py` & `cdlib-0.3.0/cdlib/datasets/remote.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/ensemble/bunch_executions.py` & `cdlib-0.3.0/cdlib/ensemble/bunch_executions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 import networkx as nx
 import numpy as np
 import cdlib
 from typing import Callable
 
 __all__ = [
     "BoolParameter",
+    "CategoricalParameter",
     "Parameter",
     "grid_execution",
     "grid_search",
     "pool",
     "pool_grid_filter",
     "random_search",
 ]
 
 Parameter = namedtuple("Parameter", "name start end step")
 Parameter.__new__.__defaults__ = (None,) * len(Parameter._fields)
 
 BoolParameter = namedtuple("BoolParameter", "name value")
 BoolParameter.__new__.__defaults__ = (None,) * len(BoolParameter._fields)
 
+CategoricalParameter = namedtuple("CategoricalParameter", "name values")
+CategoricalParameter.__new__.__defaults__ = (None,) * len(CategoricalParameter._fields)
+
 
 def __generate_ranges(parameter: tuple) -> list:
     """
 
     :param parameter:
     :return:
     """
@@ -41,14 +45,18 @@
                 values.append((parameter.name, actual))
 
     elif isinstance(parameter, BoolParameter):
         if parameter.value is None:
             values = [(parameter.name, True), (parameter.name, False)]
         else:
             values = [(parameter.name, parameter.value)]
+
+    elif isinstance(parameter, CategoricalParameter):
+        values = [(parameter.name, v) for v in parameter.values]
+
     else:
         raise ValueError(
             "parameter should be either an instance of Parameter or of BoolParameter"
         )
     return values
```

### Comparing `cdlib-0.2.6/cdlib/evaluation/comparison.py` & `cdlib-0.3.0/cdlib/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/evaluation/comparisonranking.py` & `cdlib-0.3.0/cdlib/evaluation/comparisonranking.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/evaluation/fitness.py` & `cdlib-0.3.0/cdlib/evaluation/fitness.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/evaluation/fitnessranking.py` & `cdlib-0.3.0/cdlib/evaluation/fitnessranking.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/evaluation/internal/TOPSIS.py` & `cdlib-0.3.0/cdlib/evaluation/internal/TOPSIS.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def norm(x, y):
     """normalization function; x is the array with the
     performances and y is the normalization method.
     For vector input 'v' and for linear 'l'
     """
 
     if y == "v":
-        k = np.array(np.cumsum(x ** 2, 0))
+        k = np.array(np.cumsum(x**2, 0))
         z = np.array(
             [
                 [
                     round(x[i, j] / np.sqrt(k[x.shape[0] - 1, j]), 3)
                     for j in range(x.shape[1])
                 ]
                 for i in range(x.shape[0])
```

### Comparing `cdlib-0.2.6/cdlib/evaluation/internal/link_modularity.py` & `cdlib-0.3.0/cdlib/evaluation/internal/link_modularity.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/evaluation/internal/omega.py` & `cdlib-0.3.0/cdlib/evaluation/internal/omega.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         obs = sum(A[j] / N for j in range(min(J, K) + 1))
         return J, K, N, obs, tuples1, tuples2
 
     @staticmethod
     def __expected(J, K, N, tuples1, tuples2):
         N1 = Counter(tuples1.values())
         N2 = Counter(tuples2.values())
-        exp = sum((N1[j] * N2[j]) / (N ** 2) for j in range(min(J, K) + 1))
+        exp = sum((N1[j] * N2[j]) / (N**2) for j in range(min(J, K) + 1))
         return exp
 
     @staticmethod
     def __calc_omega(obs, exp):
         if exp == obs == 1:
             return 1.0
         else:
```

### Comparing `cdlib-0.2.6/cdlib/evaluation/internal/onmi.py` & `cdlib-0.3.0/cdlib/evaluation/internal/onmi.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/evaluation/internal/statistical_ranking.py` & `cdlib-0.3.0/cdlib/evaluation/internal/statistical_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     rankings_avg = [np.mean([case[j] for case in rankings]) for j in range(k)]
     rankings_cmp = [
         r / np.lib.scimath.sqrt(k * (k + 1) / (6.0 * n)) for r in rankings_avg
     ]
 
     chi2 = ((12 * n) / float((k * (k + 1)))) * (
-        (sum(r ** 2 for r in rankings_avg)) - ((k * (k + 1) ** 2) / float(4))
+        (sum(r**2 for r in rankings_avg)) - ((k * (k + 1) ** 2) / float(4))
     )
     iman_davenport = ((n - 1) * chi2) / float((n * (k - 1) - chi2))
 
     p_value = 1 - sp.stats.f.cdf(iman_davenport, k - 1, (k - 1) * (n - 1))
 
     return iman_davenport, p_value, rankings_avg, rankings_cmp
```

### Comparing `cdlib-0.2.6/cdlib/readwrite/io.py` & `cdlib-0.3.0/cdlib/readwrite/io.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/utils.py` & `cdlib-0.3.0/cdlib/utils.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/viz/networks.py` & `cdlib-0.3.0/cdlib/viz/networks.py`

 * *Files identical despite different names*

### Comparing `cdlib-0.2.6/cdlib/viz/plots.py` & `cdlib-0.3.0/cdlib/viz/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     forDF = []
     for c in clusterings:
         cID = c.get_description()
         for c2 in clusterings:
             c2ID = c2.get_description()
             forDF.append([cID, c2ID, scoring(c, c2).score])
     df = pd.DataFrame(columns=["com1", "com2", "score"], data=forDF)
-    df = df.pivot("com1", "com2", "score")
+    df = df.pivot(index="com1", columns="com2", values="score")
     return sns.clustermap(df)
 
 
 def plot_com_stat(
     com_clusters: list, com_fitness: Callable[[object, object, bool], object]
 ) -> object:
     """
@@ -69,15 +69,15 @@
     allVals = []
     allNames = []
     for c in com_clusters:
         prop = com_fitness(c.graph, c, summary=False)
         allVals += prop
         allNames += [c.get_description()] * len(prop)
 
-    ax = sns.violinplot(allNames, allVals, cut=0, saturation=0.5, palette="Set3")
+    ax = sns.violinplot(x=allNames, y=allVals, cut=0, saturation=0.5, palette="Set3")
     for tick in ax.get_xticklabels():
         tick.set_rotation(90)
 
     plt.ylabel("%s" % com_fitness.__name__)
     plt.xlabel("Algorithm")
     plt.tight_layout()
```

### Comparing `cdlib-0.2.6/cdlib.egg-info/PKG-INFO` & `cdlib-0.3.0/cdlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 Metadata-Version: 2.1
 Name: cdlib
-Version: 0.2.6
+Version: 0.3.0
 Summary: Community Discovery Library
 Home-page: https://github.com/GiulioRossetti/cdlib
 Author: Giulio Rossetti
 Author-email: giulio.rossetti@gmail.com
 License: BSD-Clause-2
 Keywords: community-discovery node-clustering edge-clustering complex-networks
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: C
+Provides-Extra: pypi
+Provides-Extra: all
 License-File: LICENSE
 
-# CDlib - Community Discovery Library
+# CDlib - Community Detection Library
 [![codecov](https://codecov.io/gh/GiulioRossetti/cdlib/branch/master/graph/badge.svg?token=3YJOEVK02B)](https://codecov.io/gh/GiulioRossetti/cdlib)
 [![Build](https://github.com/GiulioRossetti/cdlib/actions/workflows/python-package.yml/badge.svg)](https://github.com/GiulioRossetti/cdlib/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/cdlib/badge/?version=latest)](http://cdlib.readthedocs.io/en/latest/?badge=latest)
 [![CodeQL](https://github.com/GiulioRossetti/cdlib/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/GiulioRossetti/cdlib/actions/workflows/codeql-analysis.yml)
-[![Updates](https://pyup.io/repos/github/GiulioRossetti/cdlib/shield.svg)](https://pyup.io/repos/github/GiulioRossetti/cdlib/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/GiulioRossetti/nclib.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/GiulioRossetti/nclib/context:python)
 [![pyversions](https://img.shields.io/pypi/pyversions/cdlib.svg)](https://badge.fury.io/py/cdlib)
 [![PyPI version](https://badge.fury.io/py/cdlib.svg)](https://badge.fury.io/py/cdlib)
 [![Anaconda-Server Badge](https://anaconda.org/giuliorossetti/cdlib/badges/version.svg)](https://anaconda.org/giuliorossetti/cdlib)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Downloads](https://pepy.tech/badge/cdlib/month)](https://pepy.tech/project/cdlib)
 [![Downloads](https://pepy.tech/badge/cdlib)](https://pepy.tech/project/cdlib)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4575156.svg)](https://doi.org/10.5281/zenodo.4575156)
 [![SBD++](https://img.shields.io/badge/Available%20on-SoBigData%2B%2B-green)](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853)
 
 
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/_CDlib_.svg?style=social&label=Follow%20%40_CDlib_)](https://twitter.com/_CDlib_)
 
-<!---
-[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2FGiulioRossetti%2Fcdlib.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2FGiulioRossetti%2Fcdlib?ref=badge_shield)
---->
 
-``CDlib`` is a meta-library for community discovery in complex networks: it implements algorithms, clustering fitness functions as well as visualization facilities.
+
+``CDlib`` is a meta-library for community detection in complex networks: it implements algorithms, clustering fitness functions as well as visualization facilities.
 
 
 ``CDlib`` is designed around the ``networkx`` python library: however, when needed, it takes care to automatically convert (from and to) ``igraph`` object so to provide an abstraction on specific algorithm implementations to the final user.
 
 ``CDlib`` provides a standardized input/output facilities for several Community Discovery algorithms: whenever possible, to guarantee literature coherent results, implementations of CD algorithms are inherited from their original projects (acknowledged on the [documentation](https://cdlib.readthedocs.io)).
 
 
@@ -79,40 +76,48 @@
 Alternatively use pip
 ```bash
 pip install cdlib
 ```
 
 or conda
 ```bash
+conda create -n cdlib python=3.9
 conda config --add channels giuliorossetti
 conda config --add channels conda-forge
 conda install cdlib
 ```
 
 ### Optional Dependencies (pip package)
-``CDlib`` relies on a few packages calling C code that can be cumbersome to install on Windows machines: to address such issue, the default installation does not try to install set up such requirements.
+To simplify the installation process, the default installation does not include optional dependencies (e.g., ``graph-tool``). If you need them, you can install them manually or run the following command:
 
-Such a choice has been made to allow (even) non *unix user to install the library and get access to its core functionalities. 
+```bash
+pip install cdlib[C]
+```
 
-To integrate the standard installation with you can either:
+This option, safe for *nix users, will install all those optional dependencies that require C code compilation.
 
-- (Windows) manually install the optional packages (versions details are specified in ``requirements_optional.txt``) following the original projects guidelines, or
-- (Linux/OSX) run the command:
+```bash
+pip install cdlib[pypi]
+```
+
+This option will install all those optional dependencies that are not available on conda/conda-forge.
 
 ```bash
-pip install cdlib[C]
+pip install cdlib[all]
 ```
 
-Such caveat will install everything that can be easily automated under Linux/OSX. 
+This option will install all optional dependencies accessible with the flag ``C`` and ``pypi``.
 
 #### (Advanced) 
 
-##### Graph-tool
-The only optional dependency that will remain unsatisfied following the previous procedures will be ``graph-tool`` (used to add SBM models). 
-If you need it up and running, refer to the official [documentation](https://git.skewed.de/count0/graph-tool/wikis/installation-instructions) and install the conda-forge version of the package.
+Due to some strict requirements, the installation of a subset of optional dependencies is left outside the previous procedures.
+
+##### graph-tool
+``CDlib`` integrates the support for SBM models offered by ``graph-tool``.
+To install it refer to the official [documentation](https://git.skewed.de/count0/graph-tool/wikis/installation-instructions) and install the conda-forge version of the package (or the deb version if in a *nix system).
 
 ##### ASLPAw
 
 Since its 2.1.0 release ``ASLPAw`` relies on ``gmpy2`` whose installation through pip is not easy to automatize due to some C dependencies.
 To address such issue test the following recipe:
 
 ```bash
@@ -120,15 +125,15 @@
 pip install shuffle_graph>=2.1.0 similarity-index-of-label-graph>=2.0.1 ASLPAw>=2.1.0
 ```
 
 In case this does not solve the issue, please refer to the official ``gmpy2`` [installation](https://gmpy2.readthedocs.io/en/latest/intro.html#installation) instructions.
 
 ### Optional Dependencies (Conda package)
 
-``CDlib`` relies on a few packages not available through conda: to install it please use pip:
+``CDlib`` relies on a few packages not available through conda: to install them please use pip.
 
 ```bash
 pip install pycombo
 pip install GraphRicciCurvature
 
 conda install gmpy2 
 pip install shuffle_graph>=2.1.0 similarity-index-of-label-graph>=2.0.1 ASLPAw>=2.1.0
@@ -144,9 +149,7 @@
 If you like to include your model in CDlib feel free to fork the project, open an issue and contact us.
 
 ### How to contribute to this project?
 
 Contributing is good, doing it correctly is better! Check out our [rules](https://github.com/GiulioRossetti/cdlib/blob/master/.github/CONTRIBUTING.md), issue a proper [pull request](https://github.com/GiulioRossetti/cdlib/blob/master/.github/PULL_REQUEST_TEMPLATE.md) /[bug report](https://github.com/GiulioRossetti/cdlib/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) / [feature request](https://github.com/GiulioRossetti/cdlib/blob/master/.github/ISSUE_TEMPLATE/feature_request.md).
 
 We are a welcoming community... just follow the [Code of Conduct](https://github.com/GiulioRossetti/cdlib/blob/master/.github/CODE_OF_CONDUCT.md).
-
-
```

### Comparing `cdlib-0.2.6/cdlib.egg-info/SOURCES.txt` & `cdlib-0.3.0/cdlib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 cdlib/__init__.py
+cdlib/prompt_utils.py
 cdlib/utils.py
 cdlib.egg-info/PKG-INFO
 cdlib.egg-info/SOURCES.txt
 cdlib.egg-info/dependency_links.txt
 cdlib.egg-info/requires.txt
 cdlib.egg-info/top_level.txt
 cdlib/algorithms/__init__.py
```

### Comparing `cdlib-0.2.6/setup.py` & `cdlib-0.3.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,77 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__author__ = 'Giulio Rossetti'
+__author__ = "Giulio Rossetti"
 __license__ = "BSD-2-Clause"
 __email__ = "giulio.rossetti@gmail.com"
 
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
+with open(path.join(here, "requirements.txt"), encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 
-setup(name='cdlib',
-      version='0.2.6',
-      license='BSD-Clause-2',
-      description='Community Discovery Library',
-      url='https://github.com/GiulioRossetti/cdlib',
-      author='Giulio Rossetti',
-      author_email='giulio.rossetti@gmail.com',
-      classifiers=[
-          # How mature is this project? Common values are
-          #   3 - Alpha
-          #   4 - Beta
-          #   5 - Production/Stable
-          'Development Status :: 4 - Beta',
-
-          # Indicate who your project is intended for
-          'Intended Audience :: Developers',
-          'Topic :: Software Development :: Build Tools',
-
-          # Pick your license as you wish (should match "license" above)
-          'License :: OSI Approved :: BSD License',
-
-          "Operating System :: POSIX :: Other",
-          "Operating System :: MacOS",
-
-          # Specify the Python versions you support here. In particular, ensure
-          # that you indicate whether you support Python 2, Python 3 or both.
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 3'
-      ],
-      keywords='community-discovery node-clustering edge-clustering complex-networks',
-      install_requires=requirements,
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      extras_require={
-        'C':  ["infomap>=1.3.0", "wurlitzer>=1.0.2", "GraphRicciCurvature", "networkit", "pycombo","leidenalg","karateclub"],
-      },
-      packages=find_packages(exclude=["*.test", "*.test.*", "test.*", "test", "cdlib.test", "cdlib.test.*"]),
-      )
+setup(
+    name="cdlib",
+    version="0.3.0",
+    license="BSD-Clause-2",
+    description="Community Discovery Library",
+    url="https://github.com/GiulioRossetti/cdlib",
+    author="Giulio Rossetti",
+    author_email="giulio.rossetti@gmail.com",
+    classifiers=[
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        "Development Status :: 4 - Beta",
+        # Indicate who your project is intended for
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        # Pick your license as you wish (should match "license" above)
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: POSIX :: Other",
+        "Operating System :: MacOS",
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+    ],
+    keywords="community-discovery node-clustering edge-clustering complex-networks",
+    install_requires=requirements,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    extras_require={
+        "C": [
+            "infomap>=1.3.0",
+            "wurlitzer>=1.0.2",
+            "GraphRicciCurvature",
+            "networkit",
+            "pycombo",
+            "leidenalg"
+        ],
+        "pypi": [
+            "bayanpy",
+            "pyclustering"
+        ],
+        "all": [
+            "infomap>=1.3.0",
+            "wurlitzer>=1.0.2",
+            "GraphRicciCurvature",
+            "networkit",
+            "pycombo",
+            "leidenalg",
+            "bayanpy",
+            "pyclustering"
+        ]
+    },
+    packages=find_packages(
+        exclude=["*.test", "*.test.*", "test.*", "test", "cdlib.test", "cdlib.test.*"]
+    ),
+)
```

