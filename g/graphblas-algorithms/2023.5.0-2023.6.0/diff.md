# Comparing `tmp/graphblas-algorithms-2023.5.0.tar.gz` & `tmp/graphblas-algorithms-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphblas-algorithms-2023.5.0.tar", last modified: Thu May  4 18:02:33 2023, max compression
+gzip compressed data, was "graphblas-algorithms-2023.6.0.tar", last modified: Thu Jun  8 21:47:54 2023, max compression
```

## Comparing `graphblas-algorithms-2023.5.0.tar` & `graphblas-algorithms-2023.6.0.tar`

### file list

```diff
@@ -1,140 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.925000 graphblas-algorithms-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.909000 graphblas-algorithms-2023.5.0/graphblas_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_bfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/degree_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/eigenvector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/katz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/connected.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/components/weakly_connected.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/dominating.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/isolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.913000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/reciprocity.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/regular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/unweighted.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/simple_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/smetric.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/structuralholes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tournament.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/breadth_first_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/triads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23245 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/digraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodeset.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.917000 graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/ego.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/degree_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/eigenvector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/katz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/connected.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/weakly_connected.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/dominating.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/generators/ego.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/isolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/reciprocity.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/regular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/unweighted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/weighted.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/simple_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/smetric.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/structuralholes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tournament.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/breadth_first_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/triads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_match_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.921000 graphblas-algorithms-2023.5.0/graphblas_algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:02:33.909000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 18:02:33.000000 graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10048 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:02:33.925000 graphblas-algorithms-2023.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:02:14.000000 graphblas-algorithms-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.046575 graphblas-algorithms-2023.6.0/graphblas_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.050575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/_bfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.050575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/degree_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/eigenvector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/katz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.050575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/community/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/community/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.050575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/components/connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/components/weakly_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/dominating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/efficiency_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.050575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/isomorphism/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/isomorphism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/isomorphism/isomorph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/link_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/link_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/lowest_common_ancestors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/operators/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/operators/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/reciprocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/regular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/unweighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/simple_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/smetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/structuralholes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/tournament.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/traversal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/traversal/breadth_first_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/triads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/digraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/nodemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/nodeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/generators/ego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.054575 graphblas-algorithms-2023.6.0/graphblas_algorithms/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/linalg/bethehessianmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/linalg/graphmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/linalg/laplacianmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/linalg/modularitymatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/degree_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/eigenvector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/katz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/community/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/community/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/components/connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/components/weakly_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/dominating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/efficiency_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/generators/ego.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/isomorphism/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/isomorphism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/isomorphism/isomorph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.058575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/linalg/bethehessianmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/linalg/graphmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/linalg/laplacianmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/linalg/modularitymatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/link_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/link_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/lowest_common_ancestors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/operators/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/operators/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/reciprocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/regular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/unweighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/weighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/simple_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/smetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/structuralholes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tournament.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/traversal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/traversal/breadth_first_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/triads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/tests/test_match_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/graphblas_algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 21:47:54.046575 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-06-08 21:47:54.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-06-08 21:47:54.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 21:47:54.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 21:47:54.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-08 21:47:54.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 21:47:54.000000 graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:47:54.062575 graphblas-algorithms-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 21:47:34.000000 graphblas-algorithms-2023.6.0/setup.py
```

### Comparing `graphblas-algorithms-2023.5.0/LICENSE` & `graphblas-algorithms-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/__init__.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import importlib.metadata
 
 from .classes import *
+from .generators import *
+from .linalg import *
 
 from .algorithms import *  # isort:skip
-from .generators import *  # isort:skip
 
 try:
     __version__ = importlib.metadata.version("graphblas-algorithms")
 except Exception as exc:  # pragma: no cover (safety)
     raise AttributeError(
         "`graphblas_algorithms.__version__` not available. This may mean "
         "graphblas-algorithms was incorrectly installed or not installed at all. "
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/__init__.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 from .cluster import *
 from .community import *
 from .components import *
 from .core import *
 from .cuts import *
 from .dag import *
 from .dominating import *
+from .efficiency_measures import *
 from .isolate import *
+from .isomorphism import *
 from .link_analysis import *
+from .lowest_common_ancestors import *
 from .operators import *
 from .reciprocity import *
 from .regular import *
 from .shortest_paths import *
 from .simple_paths import *
 from .smetric import *
 from .structuralholes import *
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_bfs.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/_bfs.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,43 +7,58 @@
 
 def _get_cutoff(n, cutoff):
     if cutoff is None or cutoff >= n:
         return n  # Everything
     return cutoff + 1  # Inclusive
 
 
-def _bfs_plain(G, source=None, target=None, *, index=None, cutoff=None):
+# Push-pull optimization is possible, but annoying to implement
+def _bfs_plain(
+    G, source=None, target=None, *, index=None, cutoff=None, transpose=False, name="bfs_plain"
+):
     if source is not None:
+        if source not in G._key_to_id:
+            raise KeyError(f"The node {source} is not in the graph")
         index = G._key_to_id[source]
     if target is not None:
+        if target not in G._key_to_id:
+            raise KeyError(f"The node {target} is not in the graph")
         dst_id = G._key_to_id[target]
     else:
         dst_id = None
     A = G.get_property("offdiag")
+    if transpose and G.is_directed():
+        A = A.T  # TODO: should we use "AT" instead?
     n = A.nrows
-    v = Vector(bool, n, name="bfs_plain")
+    v = Vector(bool, n, name=name)
     q = Vector(bool, n, name="q")
     v[index] = True
     q[index] = True
     any_pair_bool = any_pair[bool]
     cutoff = _get_cutoff(n, cutoff)
     for _i in range(1, cutoff):
         q(~v.S, replace) << any_pair_bool(q @ A)
         if q.nvals == 0:
             break
+        v(q.S) << True
         if dst_id is not None and dst_id in q:
             break
-        v(q.S) << True
     return v
 
 
-def _bfs_level(G, source, cutoff=None, *, transpose=False, dtype=int):
+def _bfs_level(G, source, target=None, *, cutoff=None, transpose=False, dtype=int):
     if dtype == bool:
         dtype = int
     index = G._key_to_id[source]
+    if target is not None:
+        if target not in G._key_to_id:
+            raise KeyError(f"The node {target} is not in the graph")
+        dst_id = G._key_to_id[target]
+    else:
+        dst_id = None
     A = G.get_property("offdiag")
     if transpose and G.is_directed():
         A = A.T  # TODO: should we use "AT" instead?
     n = A.nrows
     v = Vector(dtype, n, name="bfs_level")
     q = Vector(bool, n, name="q")
     v[index] = 0
@@ -51,18 +66,20 @@
     any_pair_bool = any_pair[bool]
     cutoff = _get_cutoff(n, cutoff)
     for i in range(1, cutoff):
         q(~v.S, replace) << any_pair_bool(q @ A)
         if q.nvals == 0:
             break
         v(q.S) << i
+        if dst_id is not None and dst_id in q:
+            break
     return v
 
 
-def _bfs_levels(G, nodes, cutoff=None, *, dtype=int):
+def _bfs_levels(G, nodes, *, cutoff=None, dtype=int):
     if dtype == bool:
         dtype = int
     A = G.get_property("offdiag")
     n = A.nrows
     if nodes is None:
         # TODO: `D = Vector.from_scalar(0, n, dtype).diag()`
         D = Vector(dtype, n, name="bfs_levels_vector")
@@ -86,15 +103,15 @@
         Q(~D.S, replace) << any_pair_bool(Q @ A)
         if Q.nvals == 0:
             break
         D(Q.S) << i
     return D
 
 
-def _bfs_parent(G, source, cutoff=None, *, target=None, transpose=False, dtype=int):
+def _bfs_parent(G, source, target=None, *, cutoff=None, transpose=False, dtype=int):
     if dtype == bool:
         dtype = int
     index = G._key_to_id[source]
     if target is not None:
         dst_id = G._key_to_id[target]
     else:
         dst_id = None
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/_helpers.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/_helpers.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/boundary.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/boundary.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/degree_alg.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/degree_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/eigenvector.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/eigenvector.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/centrality/katz.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/centrality/katz.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cluster.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/community/quality.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/community/quality.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/core.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/core.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/cuts.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/cuts.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/isolate.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/isolate.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/link_analysis/hits_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from graphblas import Matrix, Vector, binary, monoid
 from graphblas.semiring import plus_first, plus_times
 
 from graphblas_algorithms import Graph
 
 from .._helpers import is_converged
 from ..exceptions import ConvergenceFailure
@@ -109,15 +108,14 @@
     nodelist=None,
     dangling=None,
     name="google_matrix",
 ) -> Matrix:
     A = G._A
     ids = G.list_to_ids(nodelist)
     if ids is not None:
-        ids = np.array(ids, np.uint64)
         A = A[ids, ids].new(float, name=name)
     else:
         A = A.dup(float, name=name)
     N = A.nrows
     if N == 0:
         return A
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/operators/binary.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/operators/binary.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 from graphblas import Matrix, binary, dtypes, unary
 
 from ..exceptions import GraphBlasAlgorithmException
 
 __all__ = [
     "compose",
     "difference",
@@ -59,17 +58,17 @@
 
 def intersection(G, H, *, name="intersection"):
     if G.is_multigraph() != H.is_multigraph():
         raise GraphBlasAlgorithmException("All graphs must be graphs or multigraphs.")
     if G.is_multigraph():
         raise NotImplementedError("Not yet implemented for multigraphs")
     keys = sorted(G._key_to_id.keys() & H._key_to_id.keys(), key=G._key_to_id.__getitem__)
-    ids = np.array(G.list_to_ids(keys), np.uint64)
+    ids = G.list_to_ids(keys)
     A = G._A[ids, ids].new()
-    ids = np.array(H.list_to_ids(keys), np.uint64)
+    ids = H.list_to_ids(keys)
     B = H._A[ids, ids].new(dtypes.unify(A.dtype, H._A.dtype), mask=A.S, name=name)
     B << unary.one(B)
     return type(G)(B, key_to_id=dict(zip(keys, range(len(keys)))))
 
 
 def difference(G, H, *, name="difference"):
     if G.is_multigraph() != H.is_multigraph():
@@ -80,15 +79,15 @@
         raise GraphBlasAlgorithmException("Node sets of graphs not equal")
     A = G._A
     if G._key_to_id == H._key_to_id:
         B = H._A
     else:
         # Need to perform a permutation
         keys = sorted(G._key_to_id, key=G._key_to_id.__getitem__)
-        ids = np.array(H.list_to_ids(keys), np.uint64)
+        ids = H.list_to_ids(keys)
         B = H._A[ids, ids].new()
     C = unary.one(A).new(mask=~B.S, name=name)
     return type(G)(C, key_to_id=G._key_to_id)
 
 
 def symmetric_difference(G, H, *, name="symmetric_difference"):
     if G.is_multigraph() != H.is_multigraph():
@@ -99,15 +98,15 @@
         raise GraphBlasAlgorithmException("Node sets of graphs not equal")
     A = G._A
     if G._key_to_id == H._key_to_id:
         B = H._A
     else:
         # Need to perform a permutation
         keys = sorted(G._key_to_id, key=G._key_to_id.__getitem__)
-        ids = np.array(H.list_to_ids(keys), np.uint64)
+        ids = H.list_to_ids(keys)
         B = H._A[ids, ids].new()
     Mask = binary.pair[bool](A & B).new(name="mask")
     C = binary.pair(A | B, left_default=True, right_default=True).new(mask=~Mask.S, name=name)
     return type(G)(C, key_to_id=G._key_to_id)
 
 
 def compose(G, H, *, name="compose"):
@@ -117,33 +116,33 @@
         raise NotImplementedError("Not yet implemented for multigraphs")
     A = G._A
     B = H._A
     if G._key_to_id.keys() == H._key_to_id.keys():
         if G._key_to_id != H._key_to_id:
             # Need to perform a permutation
             keys = sorted(G._key_to_id, key=G._key_to_id.__getitem__)
-            ids = np.array(H.list_to_ids(keys), np.uint64)
+            ids = H.list_to_ids(keys)
             B = B[ids, ids].new()
         C = binary.second(A | B).new(name=name)
         key_to_id = G._key_to_id
     else:
         keys = sorted(G._key_to_id.keys() & H._key_to_id.keys(), key=G._key_to_id.__getitem__)
         B = H._A
         C = Matrix(
             dtypes.unify(A.dtype, B.dtype),
             A.nrows + B.nrows - len(keys),
             A.ncols + B.ncols - len(keys),
             name=name,
         )
         C[: A.nrows, : A.ncols] = A
-        ids1 = np.array(G.list_to_ids(keys), np.uint64)
-        ids2 = np.array(H.list_to_ids(keys), np.uint64)
+        ids1 = G.list_to_ids(keys)
+        ids2 = H.list_to_ids(keys)
         C[ids1, ids1] = B[ids2, ids2]
         newkeys = sorted(H._key_to_id.keys() - G._key_to_id.keys(), key=H._key_to_id.__getitem__)
-        ids = np.array(H.list_to_ids(newkeys), np.uint64)
+        ids = H.list_to_ids(newkeys)
         C[A.nrows :, A.ncols :] = B[ids, ids]
         # Now make new `key_to_id`
         ids += A.nrows
         key_to_id = dict(zip(newkeys, ids.tolist()))
         key_to_id.update(G._key_to_id)
     return type(G)(C, key_to_id=key_to_id)
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/reciprocity.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/reciprocity.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/regular.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/regular.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/dense.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/dense.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/shortest_paths/weighted.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/shortest_paths/weighted.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 import numpy as np
 from graphblas import Matrix, Vector, binary, indexunary, monoid, replace, select, unary
 from graphblas.semiring import any_pair, min_plus
 
 from .._bfs import _bfs_level, _bfs_levels, _bfs_parent, _bfs_plain
-from ..exceptions import Unbounded
+from ..exceptions import NoPath, Unbounded
 
 __all__ = [
     "single_source_bellman_ford_path_length",
     "bellman_ford_path",
+    "bellman_ford_path_length",
     "bellman_ford_path_lengths",
     "negative_edge_cycle",
 ]
 
 
-def single_source_bellman_ford_path_length(G, source, *, cutoff=None):
+def _bellman_ford_path_length(G, source, target=None, *, cutoff=None, name):
     # No need for `is_weighted=` keyword, b/c this is assumed to be weighted (I think)
-    index = G._key_to_id[source]
+    src_id = G._key_to_id[source]
+    if target is not None:
+        dst_id = G._key_to_id[target]
+    else:
+        dst_id = None
+
     if G.get_property("is_iso"):
         # If the edges are iso-valued (and positive), then we can simply do level BFS
         is_negative, iso_value = G.get_properties("has_negative_edges+ iso_value")
         if not is_negative:
             if cutoff is not None:
                 cutoff = int(cutoff // iso_value)
-            d = _bfs_level(G, source, cutoff, dtype=iso_value.dtype)
+            d = _bfs_level(G, source, target, cutoff=cutoff, dtype=iso_value.dtype)
+            if dst_id is not None:
+                d = d.get(dst_id)
+                if d is None:
+                    raise NoPath(f"node {target} not reachable from {source}")
             if iso_value != 1:
                 d *= iso_value
             return d
         # It's difficult to detect negative cycles with BFS
-        if G._A[index, index].get() is not None:
+        if G._A[src_id, src_id].get() is not None:
             raise Unbounded("Negative cycle detected.")
-        if not G.is_directed() and G._A[index, :].nvals > 0:
+        if not G.is_directed() and G._A[src_id, :].nvals > 0:
             # For undirected graphs, any negative edge is a cycle
             raise Unbounded("Negative cycle detected.")
 
     # Use `offdiag` instead of `A`, b/c self-loops don't contribute to the result,
     # and negative self-loops are easy negative cycles to avoid.
     # We check if we hit a self-loop negative cycle at the end.
-    A, has_negative_diagonal = G.get_properties("offdiag has_negative_diagonal")
+    if dst_id is None:
+        A, has_negative_diagonal = G.get_properties("offdiag has_negative_diagonal")
+    else:
+        A, is_negative, has_negative_diagonal = G.get_properties(
+            "offdiag has_negative_edges- has_negative_diagonal"
+        )
     if A.dtype == bool:
         # Should we upcast e.g. INT8 to INT64 as well?
         dtype = int
     else:
         dtype = A.dtype
     n = A.nrows
     d = Vector(dtype, n, name="single_source_bellman_ford_path_length")
-    d[index] = 0
+    d[src_id] = 0
     cur = d.dup(name="cur")
     mask = Vector(bool, n, name="mask")
     one = unary.one[bool]
     for _i in range(n - 1):
         # This is a slightly modified Bellman-Ford algorithm.
         # `cur` is the current frontier of values that improved in the previous iteration.
         # This means that in this iteration we drop values from `cur` that are not better.
@@ -62,31 +77,48 @@
 
         # Drop values from `cur` that didn't improve
         cur(mask.V, replace) << cur
         if cur.nvals == 0:
             break
         # Update `d` with values that improved
         d(cur.S) << cur
+        if dst_id is not None and not is_negative:
+            # Limit exploration if we have a target
+            cutoff = cur.get(dst_id, cutoff)
     else:
         # Check for negative cycle when for loop completes without breaking
         cur << min_plus(cur @ A)
         if cutoff is not None:
             cur << select.valuele(cur, cutoff)
         mask << binary.lt(cur & d)
-        if mask.reduce(monoid.lor):
+        if dst_id is None and mask.reduce(monoid.lor) or dst_id is not None and mask.get(dst_id):
             raise Unbounded("Negative cycle detected.")
     if has_negative_diagonal:
         # We removed diagonal entries above, so check if we visited one with a negative weight
         diag = G.get_property("diag")
         cur << select.valuelt(diag, 0)
         if any_pair(d @ cur):
             raise Unbounded("Negative cycle detected.")
+    if dst_id is not None:
+        d = d.get(dst_id)
+        if d is None:
+            raise NoPath(f"node {target} not reachable from {source}")
     return d
 
 
+def single_source_bellman_ford_path_length(
+    G, source, *, cutoff=None, name="single_source_bellman_ford_path_length"
+):
+    return _bellman_ford_path_length(G, source, cutoff=cutoff, name=name)
+
+
+def bellman_ford_path_length(G, source, target):
+    return _bellman_ford_path_length(G, source, target, name="bellman_ford_path_length")
+
+
 def bellman_ford_path_lengths(G, nodes=None, *, expand_output=False):
     """Extra parameter: expand_output
 
     Parameters
     ----------
     expand_output : bool, default False
         When False, the returned Matrix has one row per node in nodes.
@@ -181,15 +213,15 @@
 def bellman_ford_path(G, source, target):
     src_id = G._key_to_id[source]
     dst_id = G._key_to_id[target]
     if G.get_property("is_iso"):
         # If the edges are iso-valued (and positive), then we can simply do level BFS
         is_negative = G.get_property("has_negative_edges+")
         if not is_negative:
-            p = _bfs_parent(G, source, target=target)
+            p = _bfs_parent(G, source, target)
             return _reconstruct_path_from_parents(G, p, src_id, dst_id)
         raise Unbounded("Negative cycle detected.")
     A, is_negative, has_negative_diagonal = G.get_properties(
         "offdiag has_negative_edges- has_negative_diagonal"
     )
     if A.dtype == bool:
         # Should we upcast e.g. INT8 to INT64 as well?
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/simple_paths.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/simple_paths.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tests/test_cluster.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/tournament.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/tournament.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/algorithms/traversal/breadth_first_search.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/algorithms/traversal/breadth_first_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 
 
 def bfs_layers(G, sources):
     if sources in G:
         sources = [sources]
     ids = G.list_to_ids(sources)
-    if not ids:
+    if ids is None or len(ids) == 0:
         return
     A = G.get_property("offdiag")
     n = A.nrows
     v = Vector(bool, size=n, name="bfs_layers")
     q = Vector.from_coo(ids, True, size=n, name="q")
     any_pair_bool = any_pair[bool]
     yield q.dup(name="bfs_layer_0")
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_caching.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/_caching.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/_utils.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     return self.list_to_vector(nodes, size=size, name=name).S
 
 
 def list_to_ids(self, nodes):
     if nodes is None:
         return None
     key_to_id = self._key_to_id
-    return [key_to_id[key] for key in nodes]
+    return np.fromiter((key_to_id[key] for key in nodes), np.uint64)
 
 
 def list_to_keys(self, indices):
     if indices is None:
         return None
     id_to_key = self.id_to_key
     return [id_to_key[idx] for idx in indices]
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/digraph.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/digraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import defaultdict
+from copy import deepcopy
 
 import graphblas as gb
 from graphblas import Matrix, binary, replace, select, unary
 
 import graphblas_algorithms as ga
 
 from . import _utils
@@ -605,14 +606,23 @@
         A = self._A
         if reciprocal:
             B = binary.any(A & A.T).new(name=name)
         else:
             B = binary.any(A | A.T).new(name=name)
         return Graph(B, key_to_id=self._key_to_id)
 
+    def reverse(self, copy=True):
+        # We could even re-use many of the cached values
+        A = self._A.T  # This probably mostly works, but does not yet support assignment
+        if copy:
+            A = A.new()
+        rv = type(self)(A, key_to_id=self._key_to_id)
+        rv.graph.update(deepcopy(self.graph))
+        return rv
+
 
 class MultiDiGraph(DiGraph):
     def is_multigraph(self):
         return True
 
 
 __all__ = ["DiGraph", "MultiDiGraph"]
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/graph.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/graph.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodemap.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/nodemap.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/classes/nodeset.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/classes/nodeset.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/generators/ego.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/generators/ego.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/_utils.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/_utils.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/boundary.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/boundary.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/degree_alg.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/degree_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/eigenvector.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/eigenvector.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/centrality/katz.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/centrality/katz.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cluster.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/community/quality.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/community/quality.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/connected.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/components/connected.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/components/weakly_connected.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/components/weakly_connected.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/cuts.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/cuts.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/dag.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/dag.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/exception.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 try:
     import networkx as nx
 except ImportError:
 
     class NetworkXError(Exception):
         pass
 
+    class NetworkXNoPath(Exception):
+        pass
+
     class NetworkXPointlessConcept(Exception):
         pass
 
     class NetworkXUnbounded(Exception):
         pass
 
     class NodeNotFound(Exception):
@@ -16,14 +19,15 @@
 
     class PowerIterationFailedConvergence(Exception):
         pass
 
 else:
     from networkx import (
         NetworkXError,
+        NetworkXNoPath,
         NetworkXPointlessConcept,
         NetworkXUnbounded,
         NodeNotFound,
         PowerIterationFailedConvergence,
     )
 try:
     import scipy as sp
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/link_analysis/hits_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/operators/binary.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/operators/binary.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/reciprocity.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/reciprocity.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/dense.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/dense.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from graphblas_algorithms import algorithms
 from graphblas_algorithms.classes.digraph import to_graph
 
 from ..exception import NetworkXError
 
 __all__ = ["floyd_warshall", "floyd_warshall_numpy", "floyd_warshall_predecessor_and_distance"]
 
@@ -24,15 +22,15 @@
 
 
 def floyd_warshall_numpy(G, nodelist=None, weight="weight"):
     G = to_graph(G, weight=weight)
     if nodelist is not None:
         if not (len(nodelist) == len(G) == len(set(nodelist))):
             raise NetworkXError("nodelist must contain every node in G with no repeats.")
-        permutation = np.array(G.list_to_ids(nodelist), np.uint64)
+        permutation = G.list_to_ids(nodelist)
     else:
         permutation = None
     try:
         return algorithms.floyd_warshall_predecessor_and_distance(
             G, is_weighted=weight is not None, compute_predecessors=False, permutation=permutation
         )[1]
     except algorithms.exceptions.GraphBlasAlgorithmException as e:
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/unweighted.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/unweighted.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/shortest_paths/weighted.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/shortest_paths/weighted.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from graphblas_algorithms import algorithms
+from graphblas_algorithms import algorithms, exceptions
 from graphblas_algorithms.classes.digraph import to_graph
 
 from .._utils import normalize_chunksize, partition
-from ..exception import NetworkXUnbounded, NodeNotFound
+from ..exception import NetworkXNoPath, NetworkXUnbounded, NodeNotFound
 
 __all__ = [
     "all_pairs_bellman_ford_path_length",
     "bellman_ford_path",
+    "bellman_ford_path_length",
     "negative_edge_cycle",
     "single_source_bellman_ford_path_length",
 ]
 
 
 def all_pairs_bellman_ford_path_length(G, weight="weight", *, chunksize="10 MiB"):
     # Larger chunksize offers more parallelism, but uses more memory.
@@ -61,12 +62,22 @@
     G = to_graph(G, weight=weight)
     try:
         return algorithms.bellman_ford_path(G, source, target)
     except KeyError as e:
         raise NodeNotFound(*e.args) from e
 
 
+def bellman_ford_path_length(G, source, target, weight="weight"):
+    G = to_graph(G, weight=weight)
+    try:
+        return algorithms.bellman_ford_path_length(G, source, target)
+    except KeyError as e:
+        raise NodeNotFound(*e.args) from e
+    except exceptions.NoPath as e:
+        raise NetworkXNoPath(*e.args) from e
+
+
 def negative_edge_cycle(G, weight="weight", heuristic=True):
     # TODO: what if weight is a function?
     # TODO: use a heuristic to try to stop early
     G = to_graph(G, weight=weight)
     return algorithms.negative_edge_cycle(G)
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_cluster.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tests/test_utils.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/tournament.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/tournament.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from graphblas import io
-
 from graphblas_algorithms import algorithms
 from graphblas_algorithms.classes.digraph import to_directed_graph
 from graphblas_algorithms.utils import not_implemented_for
 
 from .simple_paths import is_simple_path as is_path  # noqa: F401
 
 __all__ = ["is_tournament", "score_sequence", "tournament_matrix"]
@@ -24,10 +22,9 @@
     return algorithms.score_sequence(G).tolist()
 
 
 @not_implemented_for("undirected")
 @not_implemented_for("multigraph")
 def tournament_matrix(G):
     G = to_directed_graph(G)
-    T = algorithms.tournament_matrix(G)
     # TODO: can we return a different, more native object?
-    return io.to_scipy_sparse(T)
+    return algorithms.tournament_matrix(G)
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/nxapi/traversal/breadth_first_search.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/nxapi/traversal/breadth_first_search.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_core.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms/tests/test_match_nx.py` & `graphblas-algorithms-2023.6.0/graphblas_algorithms/tests/test_match_nx.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,21 +158,28 @@
                 print(f"Remove `{name}` from `{from_}` here:")
                 for _, _, path in sorted(extra):
                     print("   ", ":".join(path.rsplit(".", 1)))
     if failing:  # pragma: no cover
         raise AssertionError
 
 
+def get_fullname(info):
+    fullname = info.fullname
+    if not fullname.endswith(f".{info.dispatchname}"):
+        fullname += f" ({info.dispatchname})"
+    return fullname
+
+
 def test_print_dispatched_not_implemented(nx_names_to_info, gb_names_to_info):
     """It may be informative to see the results from this to identify functions to implement.
 
     $ pytest -s -k test_print_dispatched_not_implemented
     """
     not_implemented = nx_names_to_info.keys() - gb_names_to_info.keys()
-    fullnames = {next(iter(nx_names_to_info[name])).fullname for name in not_implemented}
+    fullnames = {get_fullname(next(iter(nx_names_to_info[name]))) for name in not_implemented}
     print()
     print("=================================================================================")
     print("Functions dispatched in NetworkX that ARE NOT implemented in graphblas-algorithms")
     print("---------------------------------------------------------------------------------")
     for i, name in enumerate(sorted(fullnames)):
         print(i, name)
     print("=================================================================================")
@@ -180,15 +187,15 @@
 
 def test_print_dispatched_implemented(nx_names_to_info, gb_names_to_info):
     """It may be informative to see the results from this to identify implemented functions.
 
     $ pytest -s -k test_print_dispatched_implemented
     """
     implemented = nx_names_to_info.keys() & gb_names_to_info.keys()
-    fullnames = {next(iter(nx_names_to_info[name])).fullname for name in implemented}
+    fullnames = {get_fullname(next(iter(nx_names_to_info[name]))) for name in implemented}
     print()
     print("=============================================================================")
     print("Functions dispatched in NetworkX that ARE implemented in graphblas-algorithms")
     print("-----------------------------------------------------------------------------")
     for i, name in enumerate(sorted(fullnames)):
         print(i, name)
     print("=============================================================================")
```

### Comparing `graphblas-algorithms-2023.5.0/graphblas_algorithms.egg-info/SOURCES.txt` & `graphblas-algorithms-2023.6.0/graphblas_algorithms.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 graphblas_algorithms/algorithms/_helpers.py
 graphblas_algorithms/algorithms/boundary.py
 graphblas_algorithms/algorithms/cluster.py
 graphblas_algorithms/algorithms/core.py
 graphblas_algorithms/algorithms/cuts.py
 graphblas_algorithms/algorithms/dag.py
 graphblas_algorithms/algorithms/dominating.py
+graphblas_algorithms/algorithms/efficiency_measures.py
 graphblas_algorithms/algorithms/exceptions.py
 graphblas_algorithms/algorithms/isolate.py
+graphblas_algorithms/algorithms/lowest_common_ancestors.py
 graphblas_algorithms/algorithms/reciprocity.py
 graphblas_algorithms/algorithms/regular.py
 graphblas_algorithms/algorithms/simple_paths.py
 graphblas_algorithms/algorithms/smetric.py
 graphblas_algorithms/algorithms/structuralholes.py
 graphblas_algorithms/algorithms/tournament.py
 graphblas_algorithms/algorithms/triads.py
@@ -35,19 +37,22 @@
 graphblas_algorithms/algorithms/centrality/eigenvector.py
 graphblas_algorithms/algorithms/centrality/katz.py
 graphblas_algorithms/algorithms/community/__init__.py
 graphblas_algorithms/algorithms/community/quality.py
 graphblas_algorithms/algorithms/components/__init__.py
 graphblas_algorithms/algorithms/components/connected.py
 graphblas_algorithms/algorithms/components/weakly_connected.py
+graphblas_algorithms/algorithms/isomorphism/__init__.py
+graphblas_algorithms/algorithms/isomorphism/isomorph.py
 graphblas_algorithms/algorithms/link_analysis/__init__.py
 graphblas_algorithms/algorithms/link_analysis/hits_alg.py
 graphblas_algorithms/algorithms/link_analysis/pagerank_alg.py
 graphblas_algorithms/algorithms/operators/__init__.py
 graphblas_algorithms/algorithms/operators/binary.py
+graphblas_algorithms/algorithms/operators/unary.py
 graphblas_algorithms/algorithms/shortest_paths/__init__.py
 graphblas_algorithms/algorithms/shortest_paths/dense.py
 graphblas_algorithms/algorithms/shortest_paths/generic.py
 graphblas_algorithms/algorithms/shortest_paths/unweighted.py
 graphblas_algorithms/algorithms/shortest_paths/weighted.py
 graphblas_algorithms/algorithms/tests/__init__.py
 graphblas_algorithms/algorithms/tests/test_cluster.py
@@ -58,24 +63,31 @@
 graphblas_algorithms/classes/_utils.py
 graphblas_algorithms/classes/digraph.py
 graphblas_algorithms/classes/graph.py
 graphblas_algorithms/classes/nodemap.py
 graphblas_algorithms/classes/nodeset.py
 graphblas_algorithms/generators/__init__.py
 graphblas_algorithms/generators/ego.py
+graphblas_algorithms/linalg/__init__.py
+graphblas_algorithms/linalg/bethehessianmatrix.py
+graphblas_algorithms/linalg/graphmatrix.py
+graphblas_algorithms/linalg/laplacianmatrix.py
+graphblas_algorithms/linalg/modularitymatrix.py
 graphblas_algorithms/nxapi/__init__.py
 graphblas_algorithms/nxapi/_utils.py
 graphblas_algorithms/nxapi/boundary.py
 graphblas_algorithms/nxapi/cluster.py
 graphblas_algorithms/nxapi/core.py
 graphblas_algorithms/nxapi/cuts.py
 graphblas_algorithms/nxapi/dag.py
 graphblas_algorithms/nxapi/dominating.py
+graphblas_algorithms/nxapi/efficiency_measures.py
 graphblas_algorithms/nxapi/exception.py
 graphblas_algorithms/nxapi/isolate.py
+graphblas_algorithms/nxapi/lowest_common_ancestors.py
 graphblas_algorithms/nxapi/reciprocity.py
 graphblas_algorithms/nxapi/regular.py
 graphblas_algorithms/nxapi/simple_paths.py
 graphblas_algorithms/nxapi/smetric.py
 graphblas_algorithms/nxapi/structuralholes.py
 graphblas_algorithms/nxapi/tournament.py
 graphblas_algorithms/nxapi/triads.py
@@ -86,19 +98,27 @@
 graphblas_algorithms/nxapi/community/__init__.py
 graphblas_algorithms/nxapi/community/quality.py
 graphblas_algorithms/nxapi/components/__init__.py
 graphblas_algorithms/nxapi/components/connected.py
 graphblas_algorithms/nxapi/components/weakly_connected.py
 graphblas_algorithms/nxapi/generators/__init__.py
 graphblas_algorithms/nxapi/generators/ego.py
+graphblas_algorithms/nxapi/isomorphism/__init__.py
+graphblas_algorithms/nxapi/isomorphism/isomorph.py
+graphblas_algorithms/nxapi/linalg/__init__.py
+graphblas_algorithms/nxapi/linalg/bethehessianmatrix.py
+graphblas_algorithms/nxapi/linalg/graphmatrix.py
+graphblas_algorithms/nxapi/linalg/laplacianmatrix.py
+graphblas_algorithms/nxapi/linalg/modularitymatrix.py
 graphblas_algorithms/nxapi/link_analysis/__init__.py
 graphblas_algorithms/nxapi/link_analysis/hits_alg.py
 graphblas_algorithms/nxapi/link_analysis/pagerank_alg.py
 graphblas_algorithms/nxapi/operators/__init__.py
 graphblas_algorithms/nxapi/operators/binary.py
+graphblas_algorithms/nxapi/operators/unary.py
 graphblas_algorithms/nxapi/shortest_paths/__init__.py
 graphblas_algorithms/nxapi/shortest_paths/dense.py
 graphblas_algorithms/nxapi/shortest_paths/generic.py
 graphblas_algorithms/nxapi/shortest_paths/unweighted.py
 graphblas_algorithms/nxapi/shortest_paths/weighted.py
 graphblas_algorithms/nxapi/tests/__init__.py
 graphblas_algorithms/nxapi/tests/test_cluster.py
```

### Comparing `graphblas-algorithms-2023.5.0/pyproject.toml` & `graphblas-algorithms-2023.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -91,26 +91,30 @@
 # $ python -c 'import tomli ; [print(x) for x in sorted(tomli.load(open("pyproject.toml", "rb"))["tool"]["setuptools"]["packages"])]'
 packages = [
     "graphblas_algorithms",
     "graphblas_algorithms.algorithms",
     "graphblas_algorithms.algorithms.centrality",
     "graphblas_algorithms.algorithms.community",
     "graphblas_algorithms.algorithms.components",
+    "graphblas_algorithms.algorithms.isomorphism",
     "graphblas_algorithms.algorithms.link_analysis",
     "graphblas_algorithms.algorithms.operators",
     "graphblas_algorithms.algorithms.shortest_paths",
     "graphblas_algorithms.algorithms.tests",
     "graphblas_algorithms.algorithms.traversal",
     "graphblas_algorithms.classes",
     "graphblas_algorithms.generators",
+    "graphblas_algorithms.linalg",
     "graphblas_algorithms.nxapi",
     "graphblas_algorithms.nxapi.centrality",
     "graphblas_algorithms.nxapi.community",
     "graphblas_algorithms.nxapi.components",
     "graphblas_algorithms.nxapi.generators",
+    "graphblas_algorithms.nxapi.isomorphism",
+    "graphblas_algorithms.nxapi.linalg",
     "graphblas_algorithms.nxapi.link_analysis",
     "graphblas_algorithms.nxapi.operators",
     "graphblas_algorithms.nxapi.shortest_paths",
     "graphblas_algorithms.nxapi.tests",
     "graphblas_algorithms.nxapi.traversal",
     "graphblas_algorithms.tests",
     "graphblas_algorithms.utils",
@@ -227,21 +231,23 @@
     "EM",  # flake8-errmsg (Perhaps nicer, but too much work)
     "ICN",  # flake8-import-conventions (Doesn't allow "_" prefix such as `_np`)
     "PYI",  # flake8-pyi (We don't have stub files yet)
     "SLF",  # flake8-self (We can use our own private variables--sheesh!)
     "TID",  # flake8-tidy-imports (Rely on isort and our own judgement)
     "TCH",  # flake8-type-checking (Note: figure out type checking later)
     "ARG",  # flake8-unused-arguments (Sometimes helpful, but too strict)
+    "TD",  # flake8-todos (Maybe okay to add some of these)
     "ERA",  # eradicate (We like code in comments!)
     "PD",  # pandas-vet (Intended for scripts that use pandas, not libraries)
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]  # Allow unused imports (w/o defining `__all__`)
 "graphblas_algorithms/**/tests/*py" = ["S101", "T201", "D103", "D100"]  # Allow assert, print, and no docstring
+"graphblas_algorithms/interface.py" = ["PIE794"]  # Allow us to use `mod = nxapi.<module>` repeatedly
 "graphblas_algorithms/nxapi/exception.py" = ["F401"]  # Allow unused imports (w/o defining `__all__`)
 "scripts/*.py" = ["INP001", "S101", "T201"]  # Not a package, allow assert, allow print
 
 [tool.ruff.flake8-builtins]
 builtins-ignorelist = ["copyright"]
 
 [tool.ruff.flake8-pytest-style]
```

