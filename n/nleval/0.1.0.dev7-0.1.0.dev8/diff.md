# Comparing `tmp/nleval-0.1.0.dev7.tar.gz` & `tmp/nleval-0.1.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nleval-0.1.0.dev7.tar", last modified: Sun Mar 12 23:21:38 2023, max compression
+gzip compressed data, was "nleval-0.1.0.dev8.tar", last modified: Thu Jun  8 15:53:57 2023, max compression
```

## Comparing `nleval-0.1.0.dev7.tar` & `nleval-0.1.0.dev8.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.589467 nleval-0.1.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-03-12 23:21:38.589467 nleval-0.1.0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 23:21:38.589467 nleval-0.1.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.573467 nleval-0.1.0.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/config/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/diseases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/disgenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval/data/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotation/diseases.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotation/disgenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotation/gene_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/annotation/human_phenotype_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval/data/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/experimental/alevinfry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.581467 nleval-0.1.0.dev7/src/nleval/data/network/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/biogrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/bioplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/comppi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/consensuspathdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/funcoup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/hippie.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/humanbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/humannet.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/humap.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/huri.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/omnipath.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/pcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/proteomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/signor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/network/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.581467 nleval-0.1.0.dev7/src/nleval/data/ontology/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/ontology/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/ontology/gene_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/data/ontology/mondo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.581467 nleval-0.1.0.dev7/src/nleval/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/ext/grape.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/ext/pecanpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/ext/sknetwork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.581467 nleval-0.1.0.dev7/src/nleval/feature/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/feature/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/feature/multifeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/feature/singlefeat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/graph/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    30738 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/graph/sparse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/label/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24696 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/label/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/existence_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/negative_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/nonred.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/pairwise_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/filters/value_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/label/split/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/split/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/split/holdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/label/split/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/metric/graphgym_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/metric/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/model/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model/label_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.585467 nleval-0.1.0.dev7/src/nleval/model_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model_trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model_trainer/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model_trainer/graphgym.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model_trainer/label_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/model_trainer/supervised_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.589467 nleval-0.1.0.dev7/src/nleval/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/cx_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/dataset_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/download.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16905 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/idhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10692 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/registers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/src/nleval/util/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.577467 nleval-0.1.0.dev7/src/nleval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-03-12 23:21:38.000000 nleval-0.1.0.dev7/src/nleval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-12 23:21:38.000000 nleval-0.1.0.dev7/src/nleval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 23:21:38.000000 nleval-0.1.0.dev7/src/nleval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 23:21:38.000000 nleval-0.1.0.dev7/src/nleval.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-12 23:21:38.000000 nleval-0.1.0.dev7/src/nleval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-12 23:21:38.000000 nleval-0.1.0.dev7/src/nleval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:38.589467 nleval-0.1.0.dev7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/test/test_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43111 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/test/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-12 23:21:26.000000 nleval-0.1.0.dev7/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.534527 nleval-0.1.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-06-08 15:53:57.534527 nleval-0.1.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:53:57.534527 nleval-0.1.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.518527 nleval-0.1.0.dev8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.522527 nleval-0.1.0.dev8/src/nleval/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.522527 nleval-0.1.0.dev8/src/nleval/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/config/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.522527 nleval-0.1.0.dev8/src/nleval/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.522527 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/diseases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/disgenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.526527 nleval-0.1.0.dev8/src/nleval/data/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotation/diseases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotation/disgenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotation/gene_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/annotation/human_phenotype_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.526527 nleval-0.1.0.dev8/src/nleval/data/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/experimental/alevinfry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.526527 nleval-0.1.0.dev8/src/nleval/data/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/biogrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/bioplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/comppi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/consensuspathdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/funcoup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/hippie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/humanbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/humannet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/humap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/huri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/omnipath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/pcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/proteomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/signor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/network/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.526527 nleval-0.1.0.dev8/src/nleval/data/ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/ontology/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/ontology/gene_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/data/ontology/mondo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/dataset_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/ext/grape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/ext/orbital_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/ext/pecanpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/ext/sknetwork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/feature/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/feature/multifeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/feature/singlefeat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/graph/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32294 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/graph/sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/label/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/label/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/existence_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/negative_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/nonred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/pairwise_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/filters/value_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/label/split/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/split/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/split/holdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/label/split/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/metric/graphgym_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/metric/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.530527 nleval-0.1.0.dev8/src/nleval/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model/label_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.534527 nleval-0.1.0.dev8/src/nleval/model_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model_trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model_trainer/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model_trainer/graphgym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model_trainer/label_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/model_trainer/supervised_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.534527 nleval-0.1.0.dev8/src/nleval/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/cx_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/dataset_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/download.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16905 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/idhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10692 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/registers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/src/nleval/util/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.522527 nleval-0.1.0.dev8/src/nleval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-06-08 15:53:57.000000 nleval-0.1.0.dev8/src/nleval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-08 15:53:57.000000 nleval-0.1.0.dev8/src/nleval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:53:57.000000 nleval-0.1.0.dev8/src/nleval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:53:57.000000 nleval-0.1.0.dev8/src/nleval.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-08 15:53:57.000000 nleval-0.1.0.dev8/src/nleval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 15:53:57.000000 nleval-0.1.0.dev8/src/nleval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:53:57.534527 nleval-0.1.0.dev8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/test/test_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43053 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/test/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-08 15:53:44.000000 nleval-0.1.0.dev8/test/test_wrapper.py
```

### Comparing `nleval-0.1.0.dev7/LICENSE` & `nleval-0.1.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/PKG-INFO` & `nleval-0.1.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nleval
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: A Python toolkit for biological network learning evaluation
 Author-email: Remy Liu <liurenmi@msu.edu>
 License: MIT
 Project-URL: home, https://github.com/krishnanlab/NetworkLearningEval
 Project-URL: bug-tracker, https://github.com/krishnanlab/NetworkLearningEval/issues
 Keywords: Data Processing,Gene Classification,Machine Learning,Network Biology,Network Repositories
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nleval-0.1.0.dev7/README.md` & `nleval-0.1.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/pyproject.toml` & `nleval-0.1.0.dev8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nleval"
-version = "0.1.0-dev7"
+version = "0.1.0-dev8"
 description = "A Python toolkit for biological network learning evaluation"
 readme = "README.md"
 
 authors = [
     {name = "Remy Liu", email = "liurenmi@msu.edu"},
 ]
 license = {text = "MIT"}
@@ -29,18 +29,19 @@
     "Gene Classification",
     "Machine Learning",
     "Network Biology",
     "Network Repositories",
 ]
 
 dependencies = [
-    "matplotlib<3.7",  # https://github.com/scverse/scanpy/issues/2411
+    "matplotlib",
     "mygene",
     "ndex2",
     "numpy>=1.20.0",
+    "pyOpenSSL>=23.1.1",
     "pyyaml",
     "scikit-learn>=1.0.0",
     "scipy",
     "tqdm",
 ]
 
 [project.urls]
@@ -73,14 +74,16 @@
 pyroe = [
     "pyroe",
     "scanpy",
 ]
 ext = [
     "grape",
     "pecanpy",
+    "scikit-network",
+    "networkx",
 ]
 full = ["nleval[pyroe,ext]"]
 
 [tool.setuptools]
 license-files = ["LICENSE"]
 zip-safe = false
 include-package-data = true
```

### Comparing `nleval-0.1.0.dev7/src/nleval/config/__init__.py` & `nleval-0.1.0.dev8/src/nleval/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/config/logger_config.py` & `nleval-0.1.0.dev8/src/nleval/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/__init__.py` & `nleval-0.1.0.dev8/src/nleval/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/__init__.py` & `nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/__init__.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/base.py` & `nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/diseases.py` & `nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/diseases.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/disgenet.py` & `nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/disgenet.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/go.py` & `nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/go.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotated_ontology/hpo.py` & `nleval-0.1.0.dev8/src/nleval/data/annotated_ontology/hpo.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotation/base.py` & `nleval-0.1.0.dev8/src/nleval/data/annotation/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotation/diseases.py` & `nleval-0.1.0.dev8/src/nleval/data/annotation/diseases.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotation/disgenet.py` & `nleval-0.1.0.dev8/src/nleval/data/annotation/disgenet.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotation/gene_ontology.py` & `nleval-0.1.0.dev8/src/nleval/data/annotation/gene_ontology.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/annotation/human_phenotype_ontology.py` & `nleval-0.1.0.dev8/src/nleval/data/annotation/human_phenotype_ontology.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/base.py` & `nleval-0.1.0.dev8/src/nleval/data/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/experimental/alevinfry.py` & `nleval-0.1.0.dev8/src/nleval/data/experimental/alevinfry.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/__init__.py` & `nleval-0.1.0.dev8/src/nleval/data/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/base.py` & `nleval-0.1.0.dev8/src/nleval/data/network/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/biogrid.py` & `nleval-0.1.0.dev8/src/nleval/data/network/biogrid.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/bioplex.py` & `nleval-0.1.0.dev8/src/nleval/data/network/bioplex.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/comppi.py` & `nleval-0.1.0.dev8/src/nleval/data/network/comppi.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/consensuspathdb.py` & `nleval-0.1.0.dev8/src/nleval/data/network/consensuspathdb.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/funcoup.py` & `nleval-0.1.0.dev8/src/nleval/data/network/funcoup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 class FunCoup(BaseNDExData):
     """The FunCoup funcional association network.
 
     The edge weights are PFC values, which is a probabilistic estimation about
     whether a pair of genes are functionally coupled.
 
-
     https://funcoup5.scilifelab.se/help/#Citation
 
     """
 
     cx_uuid = "172990f7-102f-11ec-b666-0ac135e8bacf"
 
     def __init__(
```

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/hippie.py` & `nleval-0.1.0.dev8/src/nleval/data/network/hippie.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/humanbase.py` & `nleval-0.1.0.dev8/src/nleval/data/network/humanbase.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/humannet.py` & `nleval-0.1.0.dev8/src/nleval/data/network/humannet.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/humap.py` & `nleval-0.1.0.dev8/src/nleval/data/network/humap.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/huri.py` & `nleval-0.1.0.dev8/src/nleval/data/network/huri.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/omnipath.py` & `nleval-0.1.0.dev8/src/nleval/data/network/omnipath.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/pcnet.py` & `nleval-0.1.0.dev8/src/nleval/data/network/pcnet.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/proteomehd.py` & `nleval-0.1.0.dev8/src/nleval/data/network/proteomehd.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/signor.py` & `nleval-0.1.0.dev8/src/nleval/data/network/signor.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/network/string.py` & `nleval-0.1.0.dev8/src/nleval/data/network/string.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/data/ontology/base.py` & `nleval-0.1.0.dev8/src/nleval/data/ontology/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/dataset.py` & `nleval-0.1.0.dev8/src/nleval/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         else:
             self.y, self.masks = label.split(
                 splitter,
                 target_ids=tuple(self.idmap.lst),
                 **split_kwargs,
             )
 
+        # TODO: replace consider_negative option in label.split with this
+        _, self.y_mask = label.get_y(
+            target_ids=tuple(self.idmap.lst),
+            return_y_mask=True,
+        )
+
     @property
     def idmap(self) -> IDmap:
         """Map instance IDs to indexes."""
         return self._idmap
 
     @property
     def size(self) -> int:
@@ -83,23 +89,33 @@
         elif feature is not None:
             self._idmap = feature.idmap.copy()
         else:
             raise ValueError("Must specify either graph or feature.")
 
     @property
     def y(self) -> Optional[np.ndarray]:
-        return self._y
+        return getattr(self, "_y", None)
 
     @y.setter
     def y(self, y: Optional[np.ndarray]):
         if y is not None and y.shape[0] != self.size:
             raise ValueError(f"Incorrect shape {y.shape=}")
         self._y = y
 
     @property
+    def y_mask(self) -> Optional[np.ndarray]:
+        return getattr(self, "_y_mask", None)
+
+    @y_mask.setter
+    def y_mask(self, y_mask: Optional[np.ndarray]):
+        if y_mask is not None and y_mask.shape[0] != self.size:
+            raise ValueError(f"Incorrect shape {y_mask.shape=}")
+        self._y_mask = y_mask
+
+    @property
     def dual(self):
         return self._dual
 
     @dual.setter
     def dual(self, dual):
         if dual:
             if not isinstance(self.features, MultiFeatureVec):
@@ -256,17 +272,29 @@
         data = Data(
             num_nodes=num_nodes,
             edge_index=edge_index,
             edge_weight=edge_weight,
             x=x,
         )
 
+        if self.graph is not None:
+            data.node_ids = list(self.graph.node_ids)
+
+        if self.label is not None:
+            data.task_ids = list(self.label.label_ids)
+
+        # Label (true) matrix
         if self.y is not None:
             data.y = torch.FloatTensor(self.y)
 
+        # Label mask (negative selection) matrix
+        if self.y_mask is not None:
+            data.y_mask = torch.BoolTensor(self.y_mask)
+
+        # Split mask matrix
         if self.masks is not None:
             data.masks = []
             for mask_name, mask in self.masks.items():
                 data.masks.append(attrname := mask_name + mask_suffix)
                 setattr(data, attrname, torch.BoolTensor(mask))
 
         data.to(device)
```

### Comparing `nleval-0.1.0.dev7/src/nleval/exception.py` & `nleval-0.1.0.dev8/src/nleval/exception.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/ext/grape.py` & `nleval-0.1.0.dev8/src/nleval/ext/grape.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/ext/pecanpy.py` & `nleval-0.1.0.dev8/src/nleval/ext/pecanpy.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/ext/sknetwork.py` & `nleval-0.1.0.dev8/src/nleval/ext/sknetwork.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/feature/base.py` & `nleval-0.1.0.dev8/src/nleval/feature/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def isempty(self) -> bool:
         """Check if the object is empty."""
         return self.idmap.size == 0
 
     @property
     def dim(self):
-        """int: dimension of feature vectors."""
+        """Int: dimension of feature vectors."""
         return self._dim
 
     @dim.setter
     def dim(self, d):
         checkers.checkNullableType("d", INT_TYPE, d)
         if d is not None:
             if d < 1:
```

### Comparing `nleval-0.1.0.dev7/src/nleval/feature/multifeat.py` & `nleval-0.1.0.dev8/src/nleval/feature/multifeat.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/feature/singlefeat.py` & `nleval-0.1.0.dev8/src/nleval/feature/singlefeat.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/graph/base.py` & `nleval-0.1.0.dev8/src/nleval/graph/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,24 +199,24 @@
     @property
     def num_nodes(self) -> int:
         """Return the number of nodes in the graph indicated by the ID map."""
         return self.idmap.size
 
     @property
     def size(self):
-        """int: number of nodes in graph."""
+        """Int: number of nodes in graph."""
         return self.num_nodes
 
     @property
     def num_edges(self) -> int:
-        """int: Number of edges."""
+        """Int: Number of edges."""
         raise NotImplementedError
 
     def isempty(self):
-        """bool: true if graph is empty, indicated by empty idmap."""
+        """Bool: true if graph is empty, indicated by empty idmap."""
         return not self.size
 
     def induced_subgraph(self, node_ids: List[str]):
         """Return a subgraph induced by a subset of nodes."""
         raise NotImplementedError
 
     def connected_components(self) -> List[List[str]]:
```

### Comparing `nleval-0.1.0.dev7/src/nleval/graph/dense.py` & `nleval-0.1.0.dev8/src/nleval/graph/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         if isinstance(key, slice):
             raise NotImplementedError
         idx = self.idmap[key]
         return self.mat[idx]
 
     @property
     def num_edges(self) -> int:
-        """int: Number of edges."""
+        """Int: Number of edges."""
         return (self.mat != 0).sum()
 
     @property
     def norm_mat(self):
         """Column normalized adjacency matrix."""
         if self._norm_mat is None:
             self._norm_mat = self._mat / self._mat.sum(axis=0)
```

### Comparing `nleval-0.1.0.dev7/src/nleval/graph/ontology.py` & `nleval-0.1.0.dev8/src/nleval/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/graph/sparse.py` & `nleval-0.1.0.dev8/src/nleval/graph/sparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,35 +45,35 @@
     @property
     def edge_data(self) -> EdgeData:
         """:obj:`list` of :obj:`dict`: adjacency list data."""
         return self._edge_data
 
     @property
     def weighted(self):
-        """bool: Whether weights (3rd column in edgelist) are available."""
+        """Bool: Whether weights (3rd column in edgelist) are available."""
         return self._weighted
 
     @property
     def directed(self):
-        """bool: Indicate whether edges are directed or not."""
+        """Bool: Indicate whether edges are directed or not."""
         return self._directed
 
     @weighted.setter
     def weighted(self, val):
         checkers.checkType("weighted", bool, val)
         self._weighted = val
 
     @directed.setter
     def directed(self, val):
         checkers.checkType("directed", bool, val)
         self._directed = val
 
     @property
     def num_edges(self) -> int:
-        """int: Number of edges."""
+        """Int: Number of edges."""
         return sum(len(nbrs) for nbrs in self.edge_data)
 
     def __getitem__(self, key: Union[str, List[str]]):
         """Return slices of constructed adjacency matrix.
 
         Args:
             key(str): key of ID
@@ -867,7 +867,43 @@
         """
         self._remove_edge(node_id1, node_id2, self.edge_data)
         self._remove_edge(node_id2, node_id1, self.rev_edge_data)
 
     def connected_components(self):
         """Find connected components."""
         raise NotImplementedError
+
+    def to_undirected_sparse_graph(self, reduction="none", **kwargs):
+        """Turn the directed sparse graph into an undirected sparse graph.
+
+        Args:
+            reduction: Type of edge weight reduction to use when directed edges
+                from both directions (source->target and target->source) are
+                present. By default, no reduction will be used, which raises
+                a ValueError exception in the presence of bidirectionarl edges.
+                Other avialble reduction strategies are: "mean" and "max".
+
+        """
+        g = SparseGraph(weighted=self.weighted, directed=False, **kwargs)
+
+        # Iterate over each node and combine edges from both directions
+        for out_nbrs, in_nbrs in zip(self._edge_data, self._rev_edge_data):
+            new_edge_data = {**out_nbrs, **in_nbrs}
+
+            # Handle bidirectional edges
+            if common_nbrs_set := set(out_nbrs) & set(in_nbrs):
+                if reduction == "mean":
+                    common_nbrs = {
+                        i: (out_nbrs[i] + in_nbrs[i]) / 2 for i in common_nbrs_set
+                    }
+                elif reduction == "max":
+                    common_nbrs = {
+                        i: max(out_nbrs[i], in_nbrs[i]) for i in common_nbrs_set
+                    }
+                else:
+                    raise ValueError(f"Conflicting nbrs:\n{out_nbrs=}\n{in_nbrs=}")
+                new_edge_data.update(common_nbrs)
+            g._edge_data.append(new_edge_data)
+
+        g.idmap = self.idmap
+
+        return g
```

### Comparing `nleval-0.1.0.dev7/src/nleval/label/collection.py` & `nleval-0.1.0.dev8/src/nleval/label/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import pandas as pd
 
 from nleval.exception import IDExistsError
 from nleval.graph import OntologyGraph
 from nleval.label.filters.base import BaseFilter
-from nleval.typing import Dict, Iterator, List, Optional, Set, Splitter, Tuple
+from nleval.typing import Dict, Iterator, List, Optional, Set, Splitter, Tuple, Union
 from nleval.util import checkers, idhandler
 
 
 class LabelsetCollection(idhandler.IDprop):
     """Collection of labelsets.
 
     This class is used for managing collection of labelsets.
@@ -279,45 +279,55 @@
                 )
         self.set_property(label_id, "Negative", set(lst))
 
     def get_y(
         self,
         target_ids: Tuple[str, ...],
         labelset_name: Optional[str] = None,
-    ) -> np.ndarray:
+        return_y_mask: bool = False,
+    ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
         """Return the y matrix.
 
         Args:
             target_ids: Tuple of entity ids used to order the rows.
             labelset_name: A specific labelset to use, if not set, use all the
                 labelests (default: :obj:`None`).
+            return_y_mask: If set to :obj:`True`, then additionally return
+                a mask indicating the positive and negative entries. In other
+                words, the neutrals, or exmaples whose labels are not
+                confidently known as positives or negatives, are deselected in
+                the mask.
 
         """
         # TODO: Clean up this, reduce redundancy with split
         target_idmap = {j: i for i, j in enumerate(target_ids)}
         entity_idmap = {j: i for i, j in enumerate(self.entity_ids)}
+        # NOTE: Assume target_ids contains all of self.entity_ids
         to_target_idx = np.array([target_idmap[i] for i in self.entity_ids])
 
-        if labelset_name is None:
-            labelsets = list(map(self.get_labelset, self.label_ids))
-            y = np.zeros((len(self.entity_ids), len(labelsets)), dtype=bool)
-            for i, labelset in enumerate(labelsets):
-                y[list(map(entity_idmap.get, labelset)), i] = True
-        else:
-            labelset = self.get_labelset(labelset_name)
-            y = np.zeros(len(self.entity_ids), dtype=bool)
-            y[list(map(entity_idmap.get, labelset))] = True
-
-        if labelset_name is not None or len(y.shape) == 1:
-            y_out = np.zeros(len(target_ids), dtype=bool)
-        else:
-            y_out = np.zeros((len(target_ids), y.shape[1]), dtype=bool)
+        names = self.label_ids if labelset_name is None else [labelset_name]
+        y = np.zeros((len(self.entity_ids), len(names)), dtype=bool)
+        y_mask = np.zeros_like(y)
+        for i, name in enumerate(names):
+            positives = self.get_labelset(name)
+            pos_idxs = list(map(entity_idmap.get, positives))
+            y[pos_idxs, i] = y_mask[pos_idxs, i] = True
+
+            negatives = self.get_negative(name)
+            neg_idxs = list(map(entity_idmap.get, negatives))
+            y_mask[neg_idxs, i] = True
+
+        # Align ids with target ids
+        y_out = np.zeros((len(target_ids), y.shape[1]), dtype=bool)
+        y_mask_out = np.zeros_like(y_out)
+
         y_out[to_target_idx] = y
+        y_mask_out[to_target_idx] = y_mask
 
-        return y_out
+        return y_out if not return_y_mask else (y_out, y_mask_out)
 
     @lru_cache  # noqa: B019
     def split(  # TODO: Reduce cyclic complexity..
         self,
         splitter: Splitter,
         target_ids: Optional[Tuple[str, ...]] = None,
         labelset_name: Optional[str] = None,
```

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/__init__.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/base.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/existence_filter.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/existence_filter.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/negative_generator.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/negative_generator.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/nonred.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/nonred.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from nleval.typing import List, Set, Tuple
 
 
 class LabelsetNonRedFilter(BaseFilter):
     """Filter out redundant labelsets in a labelset collection.
 
     The detailed procedure can be found in the supplementary data of
-    https://doi.org/10.1093/bioinformatics/btaa150 In brief, given a labelset
+    https://doi.org/10.1093/bioinformatics/btaa150
+    In brief, given a labelset
     collection, a graph of labelsets if first constructed based on the
     redundancy score function of interest. Here, we use the combination of
     Jaccard index and overlap coefficient. Then, for each connected component in
     this graph, retreieve representative labelsets according to the sum of the
     proportions of genes in a geneset that is contained in any other gene sets
     within that component.
```

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/pairwise_filter.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/pairwise_filter.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/range_filter.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/filters/value_filter.py` & `nleval-0.1.0.dev8/src/nleval/label/filters/value_filter.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/split/base.py` & `nleval-0.1.0.dev8/src/nleval/label/split/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/split/holdout.py` & `nleval-0.1.0.dev8/src/nleval/label/split/holdout.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/label/split/partition.py` & `nleval-0.1.0.dev8/src/nleval/label/split/partition.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/metric/graphgym_metric.py` & `nleval-0.1.0.dev8/src/nleval/metric/graphgym_metric.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/metric/standard.py` & `nleval-0.1.0.dev8/src/nleval/metric/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 """Standard metric extending those available in sklearn."""
 from functools import wraps
 
 import numpy as np
 import sklearn.metrics
 
+from nleval.typing import Optional
+
 
 def wrap_metric(metric_func):
     """Wrap metric function with common processing steps.
 
     - Skip computation if None
     - Perturn reduction when calculating metrics in a multi-class setting
 
     """
 
     @wraps(metric_func)
-    def wrapped(y_true, y_pred, reduce="mean"):
+    def wrapped(
+        y_true: np.ndarray,
+        y_pred: np.ndarray,
+        reduce: str = "mean",
+        y_mask: Optional[np.ndarray] = None,
+    ):
         """Metric function with common processing steps.
 
         Args:
             y_true: True label.
             y_pred: Predicted values.
             reduce: Reduction strategy to use when y_true and y_pred are
                 2-dimensional, with examples along the rows and label-class
                 along the columns. Accepted options: ['none', 'mean', 'median']
+            y_mask: Mask inidicating which entries should be considered as
+                either positives or negatives when calculating the metric. In
+                other words, we ignore the neutrals in the calculation.
 
         """
         if reduce not in ["none", "mean", "median"]:
             raise ValueError(f"Unknown reduce option {reduce!r}")
 
         if _skip(y_true, y_pred):
             return np.nan
 
+        if y_mask is None:
+            y_mask = np.ones_like(y_true, dtype=bool)
+
         if len(y_true.shape) == 1 or y_true.shape[1] == 1:
-            return metric_func(y_true, y_pred)
+            return metric_func(y_true[y_mask], y_pred[y_mask])
         else:
-            scores = [metric_func(i, j) for i, j in zip(y_true.T, y_pred.T)]
+            scores = [
+                metric_func(i[m], j[m]) for i, j, m in zip(y_true.T, y_pred.T, y_mask.T)
+            ]
 
             if reduce == "none":
                 score = np.array(scores)
             elif reduce == "mean":
                 score = np.mean(scores)
             elif reduce == "median":
                 score = np.median(scores)
             else:
-                raise ValueError("This should never happen")
+                raise ValueError(
+                    f"Unknown reduce option {reduce!r}, this should have been "
+                    "caught earlier. Please fix.",
+                )
 
             return score
 
     return wrapped
 
 
 def _skip(y_true, y_predict):
```

### Comparing `nleval-0.1.0.dev7/src/nleval/model/label_propagation.py` & `nleval-0.1.0.dev8/src/nleval/model/label_propagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         """
         super().__init__(tol=tol, max_iter=max_iter, warn=warn)
         self.beta = beta
 
     @property
     def beta(self) -> float:
-        """float: restart parameter."""
+        """Float: restart parameter."""
         return self._beta
 
     @beta.setter
     def beta(self, beta: float):
         checkValuePositive("beta", beta)
         if not 0 <= beta <= 1:
             raise ValueError(
```

### Comparing `nleval-0.1.0.dev7/src/nleval/model_trainer/base.py` & `nleval-0.1.0.dev8/src/nleval/model_trainer/base.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/model_trainer/gnn.py` & `nleval-0.1.0.dev8/src/nleval/model_trainer/gnn.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,35 @@
         val_on: str = "val",
         mask_suffix: str = "_mask",
         device: str = "cpu",
         metric_best: Optional[str] = None,
         lr: float = 0.01,
         epochs: int = 100,
         eval_steps: int = 10,
+        use_negative: bool = False,
         log_level: LogLevel = "INFO",
         log_path: Optional[str] = None,
     ):
         """Initialize GNNTrainer.
 
         Args:
             val_on (str): Validation mask name (default: :obj:`"train"`).
             device (str): Training device (default: :obj:`"cpu"`).
             metric_best (str): Metric used for determining the best model
                 (default: :obj:`None`).
                 if set to True (default: :obj:`False`)
             lr (float): Learning rate (default: :obj:`0.01`)
             epochs (int): Total epochs (default: :obj:`100`)
             eval_steps (int): Interval for evaluation (default: :obj:`10`)
+            use_negative: If set to True, then try to restrict calculation of
+                the loss function to only the positive and negative examples,
+                and exclude those that are neutral. This will be indicated in
+                the :obj:`y_mask` attribute of the data object, where the
+                entries corresponding to positives or negatives are set to
+                :obj:`True`.
 
         """
         super().__init__(
             metrics,
             train_on=train_on,
             log_level=log_level,
             log_path=log_path,
@@ -45,19 +52,20 @@
 
         self.val_on = val_on
         self.mask_suffix = mask_suffix
         self.metric_best = metric_best
         self.lr = lr
         self.epochs = epochs
         self.eval_steps = eval_steps
+        self.use_negative = use_negative
         self.device = device
 
     @property
     def metric_best(self):
-        """str: Metric used for determining the best model."""
+        """Str: Metric used for determining the best model."""
         return self._metric_best
 
     @metric_best.setter
     def metric_best(self, metric_best):
         """Setter for :attr:`metric_best`.
 
         Raises:
@@ -138,20 +146,28 @@
         Do not take into account of edge weights/attrs.
 
     """
 
     def train_epoch(self, model, data, split_idx, optimizer):
         """Train a single epoch."""
         model.train()
-        criterion = torch.nn.BCEWithLogitsLoss()
-        optimizer.zero_grad()
+        criterion = torch.nn.BCEWithLogitsLoss(reduction="none")
 
         train_mask = data[self.train_on + self.mask_suffix][:, split_idx]
         out = model(data.x, data.edge_index)
         loss = criterion(out[train_mask], data.y[train_mask])
+
+        y_mask = data.y_mask[train_mask]
+        if self.use_negative:
+            # Average of column(task)-wise mean
+            loss = (loss / y_mask.float().sum(0))[y_mask].sum()
+        else:
+            loss = loss.mean()
+
+        optimizer.zero_grad()
         loss.backward()
         optimizer.step()
 
         return loss.item()
 
     @torch.no_grad()
     def evaluate(self, model, data, split_idx):
@@ -160,16 +176,17 @@
         y_pred = model(data.x, data.edge_index).detach().cpu().numpy()
         y_true = data.y.detach().cpu().numpy()
 
         results = {}
         for metric_name, metric_func in self.metrics.items():
             for mask_name in data.masks:
                 mask = data[mask_name][:, split_idx].detach().cpu().numpy()
+                y_mask = data.y_mask[mask].detach().cpu().numpy()
                 score_name = f"{mask_name.split(self.mask_suffix)[0]}_{metric_name}"
-                score = metric_func(y_true[mask], y_pred[mask])
+                score = metric_func(y_true[mask], y_pred[mask], y_mask=y_mask)
                 results[score_name] = score
 
         results["time_per_epoch"] = self._elapse() / self.eval_steps
 
         return results
 
     def train(self, model, dataset, split_idx: int = 0):
```

### Comparing `nleval-0.1.0.dev7/src/nleval/model_trainer/graphgym.py` & `nleval-0.1.0.dev8/src/nleval/model_trainer/graphgym.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/model_trainer/label_propagation.py` & `nleval-0.1.0.dev8/src/nleval/model_trainer/label_propagation.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/model_trainer/supervised_learning.py` & `nleval-0.1.0.dev8/src/nleval/model_trainer/supervised_learning.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/typing.py` & `nleval-0.1.0.dev8/src/nleval/typing.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/checkers.py` & `nleval-0.1.0.dev8/src/nleval/util/checkers.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/converter.py` & `nleval-0.1.0.dev8/src/nleval/util/converter.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/cx_explorer.py` & `nleval-0.1.0.dev8/src/nleval/util/cx_explorer.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/deprecated.py` & `nleval-0.1.0.dev8/src/nleval/util/deprecated.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/download.py` & `nleval-0.1.0.dev8/src/nleval/util/download.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/idhandler.py` & `nleval-0.1.0.dev8/src/nleval/util/idhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         maniputation on data, use `.add_id()` or `.pop_id()` to modify data
 
         """
         return self._lst.copy()
 
     @property
     def size(self):
-        """int: number of IDs in list."""
+        """Int: number of IDs in list."""
         return len(self._lst)
 
     def copy(self):
         """Return a deepcopy of self."""
         return deepcopy(self)
 
     def isempty(self):
```

### Comparing `nleval-0.1.0.dev7/src/nleval/util/logger.py` & `nleval-0.1.0.dev8/src/nleval/util/logger.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/parallel.py` & `nleval-0.1.0.dev8/src/nleval/util/parallel.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval/util/registers.py` & `nleval-0.1.0.dev8/src/nleval/util/registers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import typing
+
 from nleval.typing import Optional, Type
 
 
+@typing.no_type_check  # issue with Type
 def overload_class(
     BaseClass: Type,
     suffix: str,
     /,
     sep: str = "_",
     docstring: Optional[str] = None,
     **overload_init_kwargs,
```

### Comparing `nleval-0.1.0.dev7/src/nleval/util/timer.py` & `nleval-0.1.0.dev8/src/nleval/util/timer.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/src/nleval.egg-info/PKG-INFO` & `nleval-0.1.0.dev8/src/nleval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nleval
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: A Python toolkit for biological network learning evaluation
 Author-email: Remy Liu <liurenmi@msu.edu>
 License: MIT
 Project-URL: home, https://github.com/krishnanlab/NetworkLearningEval
 Project-URL: bug-tracker, https://github.com/krishnanlab/NetworkLearningEval/issues
 Keywords: Data Processing,Gene Classification,Machine Learning,Network Biology,Network Repositories
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nleval-0.1.0.dev7/src/nleval.egg-info/SOURCES.txt` & `nleval-0.1.0.dev8/src/nleval.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/nleval/__init__.py
 src/nleval/dataset.py
+src/nleval/dataset_pyg.py
 src/nleval/exception.py
 src/nleval/typing.py
 src/nleval.egg-info/PKG-INFO
 src/nleval.egg-info/SOURCES.txt
 src/nleval.egg-info/dependency_links.txt
 src/nleval.egg-info/not-zip-safe
 src/nleval.egg-info/requires.txt
@@ -49,14 +50,15 @@
 src/nleval/data/network/string.py
 src/nleval/data/ontology/__init__.py
 src/nleval/data/ontology/base.py
 src/nleval/data/ontology/gene_ontology.py
 src/nleval/data/ontology/mondo.py
 src/nleval/ext/__init__.py
 src/nleval/ext/grape.py
+src/nleval/ext/orbital_features.py
 src/nleval/ext/pecanpy.py
 src/nleval/ext/sknetwork.py
 src/nleval/feature/__init__.py
 src/nleval/feature/base.py
 src/nleval/feature/multifeat.py
 src/nleval/feature/singlefeat.py
 src/nleval/graph/__init__.py
```

### Comparing `nleval-0.1.0.dev7/test/test_data.py` & `nleval-0.1.0.dev8/test/test_data.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/test/test_dataset.py` & `nleval-0.1.0.dev8/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/test/test_graph.py` & `nleval-0.1.0.dev8/test/test_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -754,15 +754,15 @@
 
 class TestDenseGraph(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.case = test_case1()
 
     def check_graph(self, graph):
-        """compare graph with data, true if identical."""
+        """Compare graph with data, true if identical."""
         mat = self.case.data_mat[:, 1:]
         IDlst = [str(int(i)) for i in self.case.data_mat[:, 0]]
         for idx1, node_id1 in enumerate(IDlst):
             for idx2, node_id2 in enumerate(IDlst):
                 with self.subTest(
                     idx1=idx1,
                     idx2=idx2,
@@ -1116,23 +1116,15 @@
 
         subgraph_exclusive = graph.restrict_to_branch("d", inclusive=False)
         self.assertEqual(sorted(subgraph_exclusive.node_ids), ["e", "f"])
 
         self.assertRaises(IDNotExistError, graph.restrict_to_branch, "g")
 
     def test_read_obo(self):
-        r"""
-
-               a
-        /      |       \
-        b      c (x, y)  d
-        |       \      /
-        e [z]       f
-
-        """
+        r"""A /      |       \ b      c (x, y)  d |       \      / e [z]       f."""
         obo_path = osp.join(SAMPLE_DATA_DIR, "toy_ontology.obo")
         with self.subTest(xref_prefix=None):
             # Do not capture xref when xref_prefix is unset
             graph = OntologyGraph()
             out = graph.read_obo(obo_path)
 
             self.assertEqual(
```

### Comparing `nleval-0.1.0.dev7/test/test_metric.py` & `nleval-0.1.0.dev8/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/test/test_model.py` & `nleval-0.1.0.dev8/test/test_model.py`

 * *Files identical despite different names*

### Comparing `nleval-0.1.0.dev7/test/test_wrapper.py` & `nleval-0.1.0.dev8/test/test_wrapper.py`

 * *Files identical despite different names*

