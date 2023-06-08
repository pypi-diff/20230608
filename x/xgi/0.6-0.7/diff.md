# Comparing `tmp/xgi-0.6.tar.gz` & `tmp/xgi-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgi-0.6.tar", last modified: Mon May 15 22:41:12 2023, max compression
+gzip compressed data, was "xgi-0.7.tar", last modified: Thu Jun  8 12:37:05 2023, max compression
```

## Comparing `xgi-0.6.tar` & `xgi-0.7.tar`

### file list

```diff
@@ -1,93 +1,108 @@
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.602030 xgi-0.6/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      539 2023-05-15 22:40:35.000000 xgi-0.6/CITATION.cff
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-05-15 22:40:35.000000 xgi-0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3123 2023-05-15 22:40:35.000000 xgi-0.6/CONTRIBUTING.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-04-14 16:11:20.000000 xgi-0.6/LICENSE.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-05-05 16:04:30.000000 xgi-0.6/MANIFEST.in
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4028 2023-05-15 22:41:12.601888 xgi-0.6/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5643 2023-05-15 22:40:35.000000 xgi-0.6/README.md
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.591589 xgi-0.6/logo/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.6/logo/logo.pdf
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.6/logo/logo.png
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.6/logo/logo.svg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3264 2023-05-15 22:40:35.000000 xgi-0.6/long_description.rst
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.6/pytest.ini
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.592731 xgi-0.6/requirements/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.6/requirements/README.md
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.6/requirements/benchmarks.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-05-15 22:40:35.000000 xgi-0.6/requirements/default.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-05-11 12:53:09.000000 xgi-0.6/requirements/developer.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       93 2023-05-15 22:40:35.000000 xgi-0.6/requirements/documentation.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.6/requirements/release.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-05-15 22:40:35.000000 xgi-0.6/requirements/test.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       58 2023-05-15 22:40:35.000000 xgi-0.6/requirements/tutorial.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-05-15 22:41:12.602071 xgi-0.6/setup.cfg
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1853 2023-05-15 22:40:35.000000 xgi-0.6/setup.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.595155 xgi-0.6/tutorials/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-05-05 16:04:30.000000 xgi-0.6/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-05-05 16:04:30.000000 xgi-0.6/tutorials/Tutorial 2 - Read and Write.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-05-05 16:04:30.000000 xgi-0.6/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2023-05-05 16:04:30.000000 xgi-0.6/tutorials/Tutorial 4 - Generative_Models.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   858870 2023-05-15 22:40:35.000000 xgi-0.6/tutorials/Tutorial 5 - Plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-05-15 22:40:35.000000 xgi-0.6/tutorials/Tutorial 6 - Statistics.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   214665 2023-05-15 22:40:35.000000 xgi-0.6/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-05-15 22:40:35.000000 xgi-0.6/tutorials/case_study_zhang2022.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   987944 2023-05-15 22:40:35.000000 xgi-0.6/tutorials/quickstart.ipynb
--rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-05-05 16:04:30.000000 xgi-0.6/tutorials/simplicial_kuramoto_example.ipynb
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.595580 xgi-0.6/xgi/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.6/xgi/__init__.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.596800 xgi-0.6/xgi/algorithms/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      169 2023-05-15 22:40:35.000000 xgi-0.6/xgi/algorithms/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4775 2023-05-15 22:40:35.000000 xgi-0.6/xgi/algorithms/assortativity.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     9335 2023-05-15 22:40:35.000000 xgi-0.6/xgi/algorithms/centrality.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7621 2023-05-15 22:40:35.000000 xgi-0.6/xgi/algorithms/clustering.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5393 2023-05-15 22:40:35.000000 xgi-0.6/xgi/algorithms/connected.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.597537 xgi-0.6/xgi/classes/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      151 2023-05-11 12:53:09.000000 xgi-0.6/xgi/classes/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    25904 2023-05-15 22:40:35.000000 xgi-0.6/xgi/classes/function.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    41486 2023-05-15 22:40:35.000000 xgi-0.6/xgi/classes/hypergraph.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2759 2023-05-15 22:40:35.000000 xgi-0.6/xgi/classes/hypergraphviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    23875 2023-05-15 22:40:35.000000 xgi-0.6/xgi/classes/reportviews.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    26648 2023-05-15 22:40:35.000000 xgi-0.6/xgi/classes/simplicialcomplex.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    22000 2023-05-15 22:40:35.000000 xgi-0.6/xgi/convert.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.597946 xgi-0.6/xgi/drawing/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-05-15 22:40:35.000000 xgi-0.6/xgi/drawing/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    44099 2023-05-15 22:40:35.000000 xgi-0.6/xgi/drawing/draw.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    15065 2023-05-15 22:40:35.000000 xgi-0.6/xgi/drawing/layout.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.598299 xgi-0.6/xgi/dynamics/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.6/xgi/dynamics/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8892 2023-05-15 22:40:35.000000 xgi-0.6/xgi/dynamics/synchronization.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.6/xgi/exception.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.599335 xgi-0.6/xgi/generators/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6310 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/classic.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1411 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/lattice.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10637 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/random.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/simple.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8505 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/simplicial_complexes.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    10058 2023-05-15 22:40:35.000000 xgi-0.6/xgi/generators/uniform.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.599840 xgi-0.6/xgi/linalg/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-05-15 22:40:35.000000 xgi-0.6/xgi/linalg/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     7002 2023-05-15 22:40:35.000000 xgi-0.6/xgi/linalg/hodge_matrix.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     8447 2023-05-15 22:40:35.000000 xgi-0.6/xgi/linalg/hypergraph_matrix.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6715 2023-05-15 22:40:35.000000 xgi-0.6/xgi/linalg/laplacian_matrix.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.600980 xgi-0.6/xgi/readwrite/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      179 2022-10-13 17:38:17.000000 xgi-0.6/xgi/readwrite/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6048 2023-05-15 22:40:35.000000 xgi-0.6/xgi/readwrite/bipartite.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.6/xgi/readwrite/edgelist.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2181 2023-05-15 22:40:35.000000 xgi-0.6/xgi/readwrite/incidence.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     1892 2023-05-15 22:40:35.000000 xgi-0.6/xgi/readwrite/json.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     5273 2023-05-15 22:40:35.000000 xgi-0.6/xgi/readwrite/xgi_data.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.601434 xgi-0.6/xgi/stats/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    17777 2023-05-15 22:40:35.000000 xgi-0.6/xgi/stats/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-05-15 22:40:35.000000 xgi-0.6/xgi/stats/edgestats.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)    12555 2023-05-15 22:40:35.000000 xgi-0.6/xgi/stats/nodestats.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.601680 xgi-0.6/xgi/utils/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.6/xgi/utils/__init__.py
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4781 2023-05-15 22:40:35.000000 xgi-0.6/xgi/utils/utilities.py
-drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-05-15 22:41:12.596193 xgi-0.6/xgi.egg-info/
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     4028 2023-05-15 22:41:12.000000 xgi-0.6/xgi.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslandry   (501) staff       (20)     2018 2023-05-15 22:41:12.000000 xgi-0.6/xgi.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-05-15 22:41:12.000000 xgi-0.6/xgi.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)      769 2023-05-15 22:41:12.000000 xgi-0.6/xgi.egg-info/requires.txt
--rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-05-15 22:41:12.000000 xgi-0.6/xgi.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.673583 xgi-0.7/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2184 2023-05-30 02:43:06.000000 xgi-0.7/CITATION.cff
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    13449 2023-05-30 02:43:06.000000 xgi-0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3092 2023-06-08 12:32:19.000000 xgi-0.7/CONTRIBUTING.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5426 2023-04-14 16:11:20.000000 xgi-0.7/LICENSE.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      373 2023-05-05 16:04:30.000000 xgi-0.7/MANIFEST.in
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4028 2023-06-08 12:37:05.673446 xgi-0.7/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5643 2023-05-30 02:43:06.000000 xgi-0.7/README.md
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.657726 xgi-0.7/logo/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2807 2022-10-13 17:38:17.000000 xgi-0.7/logo/logo.pdf
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    56414 2022-10-13 17:38:17.000000 xgi-0.7/logo/logo.png
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9082 2022-10-13 17:38:17.000000 xgi-0.7/logo/logo.svg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3264 2023-05-30 02:43:06.000000 xgi-0.7/long_description.rst
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      157 2022-10-13 17:38:17.000000 xgi-0.7/pytest.ini
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.658629 xgi-0.7/requirements/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      610 2022-10-13 17:38:17.000000 xgi-0.7/requirements/README.md
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       23 2022-11-02 17:36:41.000000 xgi-0.7/requirements/benchmarks.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       78 2023-05-30 02:43:06.000000 xgi-0.7/requirements/default.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       66 2023-05-21 19:12:05.000000 xgi-0.7/requirements/developer.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       93 2023-05-30 02:43:06.000000 xgi-0.7/requirements/documentation.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       39 2023-01-03 14:13:27.000000 xgi-0.7/requirements/release.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       27 2023-05-30 02:43:06.000000 xgi-0.7/requirements/test.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       58 2023-05-30 02:43:06.000000 xgi-0.7/requirements/tutorial.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       38 2023-06-08 12:37:05.673632 xgi-0.7/setup.cfg
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1853 2023-06-08 12:30:47.000000 xgi-0.7/setup.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.661683 xgi-0.7/tutorials/
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.663576 xgi-0.7/tutorials/.ipynb_checkpoints/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9419 2023-05-16 00:58:28.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 1 - Basic Hypergraph Functionality-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3684 2023-05-16 00:58:31.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 2 - Read and Write-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    18547 2023-05-16 00:59:22.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 3 - Basic simplicial complex usage-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7554 2023-05-16 01:02:54.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 4 - Generative_Models-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   858870 2023-05-16 01:03:14.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57344 2023-05-16 01:03:26.000000 xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 6 - Statistics-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   987717 2023-05-16 01:20:02.000000 xgi-0.7/tutorials/.ipynb_checkpoints/quickstart-checkpoint.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     9404 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3714 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 2 - Read and Write.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    18606 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7560 2023-05-16 02:41:54.000000 xgi-0.7/tutorials/Tutorial 4 - Generative_Models.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   858869 2023-06-08 12:07:46.000000 xgi-0.7/tutorials/Tutorial 5 - Plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57352 2023-05-30 02:43:06.000000 xgi-0.7/tutorials/Tutorial 6 - Statistics.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   214664 2023-06-08 12:07:46.000000 xgi-0.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   119598 2023-06-08 12:07:46.000000 xgi-0.7/tutorials/Tutorial 8 - Directed Hypergraphs.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    57003 2023-05-30 02:43:06.000000 xgi-0.7/tutorials/case_study_zhang2022.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   987944 2023-05-30 02:43:06.000000 xgi-0.7/tutorials/quickstart.ipynb
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)   150550 2023-05-05 16:04:30.000000 xgi-0.7/tutorials/simplicial_kuramoto_example.ipynb
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.664754 xgi-0.7/xgi/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      464 2022-11-02 17:36:41.000000 xgi-0.7/xgi/__init__.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.666472 xgi-0.7/xgi/algorithms/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      198 2023-05-30 02:43:06.000000 xgi-0.7/xgi/algorithms/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4776 2023-06-05 15:50:23.000000 xgi-0.7/xgi/algorithms/assortativity.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    12403 2023-06-08 12:07:46.000000 xgi-0.7/xgi/algorithms/centrality.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7654 2023-06-08 12:07:46.000000 xgi-0.7/xgi/algorithms/clustering.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     5393 2023-05-30 02:43:06.000000 xgi-0.7/xgi/algorithms/connected.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3094 2023-06-05 15:50:23.000000 xgi-0.7/xgi/algorithms/shortest_path.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.668381 xgi-0.7/xgi/classes/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      190 2023-06-01 16:27:59.000000 xgi-0.7/xgi/classes/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    27188 2023-06-05 15:50:23.000000 xgi-0.7/xgi/classes/dihypergraph.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    22417 2023-06-05 15:50:23.000000 xgi-0.7/xgi/classes/direportviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    25904 2023-06-08 12:07:46.000000 xgi-0.7/xgi/classes/function.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    41479 2023-06-01 16:27:59.000000 xgi-0.7/xgi/classes/hypergraph.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2759 2023-05-30 02:43:06.000000 xgi-0.7/xgi/classes/hypergraphviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    23879 2023-06-05 15:50:23.000000 xgi-0.7/xgi/classes/reportviews.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    26648 2023-05-30 02:43:06.000000 xgi-0.7/xgi/classes/simplicialcomplex.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    24139 2023-06-01 16:27:59.000000 xgi-0.7/xgi/convert.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.668848 xgi-0.7/xgi/drawing/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       42 2023-05-30 02:43:06.000000 xgi-0.7/xgi/drawing/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    60282 2023-06-08 12:13:47.000000 xgi-0.7/xgi/drawing/draw.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    15065 2023-05-30 02:43:06.000000 xgi-0.7/xgi/drawing/layout.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.669118 xgi-0.7/xgi/dynamics/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       61 2022-11-02 17:36:41.000000 xgi-0.7/xgi/dynamics/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8892 2023-05-30 02:43:06.000000 xgi-0.7/xgi/dynamics/synchronization.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      247 2022-10-13 17:38:17.000000 xgi-0.7/xgi/exception.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.670190 xgi-0.7/xgi/generators/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      227 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7405 2023-06-08 12:07:46.000000 xgi-0.7/xgi/generators/classic.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1411 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/lattice.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10637 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/random.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2749 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/simple.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8505 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/simplicial_complexes.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    10058 2023-05-30 02:43:06.000000 xgi-0.7/xgi/generators/uniform.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.670989 xgi-0.7/xgi/linalg/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      183 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7002 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/hodge_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8447 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/hypergraph_matrix.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6715 2023-05-30 02:43:06.000000 xgi-0.7/xgi/linalg/laplacian_matrix.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.672087 xgi-0.7/xgi/readwrite/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      215 2023-06-05 15:56:16.000000 xgi-0.7/xgi/readwrite/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     3010 2023-06-08 12:13:50.000000 xgi-0.7/xgi/readwrite/bigg_data.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6048 2023-05-30 02:43:06.000000 xgi-0.7/xgi/readwrite/bipartite.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4157 2023-03-17 19:59:22.000000 xgi-0.7/xgi/readwrite/edgelist.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2181 2023-05-30 02:43:06.000000 xgi-0.7/xgi/readwrite/incidence.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     1892 2023-05-30 02:43:06.000000 xgi-0.7/xgi/readwrite/json.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4405 2023-06-05 16:28:12.000000 xgi-0.7/xgi/readwrite/xgi_data.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.673003 xgi-0.7/xgi/stats/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    22043 2023-06-01 16:27:59.000000 xgi-0.7/xgi/stats/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8197 2023-06-05 15:50:23.000000 xgi-0.7/xgi/stats/diedgestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     8355 2023-06-05 17:51:07.000000 xgi-0.7/xgi/stats/dinodestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     6527 2023-05-30 02:43:06.000000 xgi-0.7/xgi/stats/edgestats.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)    12555 2023-05-30 14:17:43.000000 xgi-0.7/xgi/stats/nodestats.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.673244 xgi-0.7/xgi/utils/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)       49 2023-01-03 14:13:27.000000 xgi-0.7/xgi/utils/__init__.py
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     7084 2023-06-05 16:01:35.000000 xgi-0.7/xgi/utils/utilities.py
+drwxr-xr-x   0 nicholaslandry   (501) staff       (20)        0 2023-06-08 12:37:05.665632 xgi-0.7/xgi.egg-info/
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     4028 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)     2760 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        1 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)      769 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/requires.txt
+-rw-r--r--   0 nicholaslandry   (501) staff       (20)        4 2023-06-08 12:37:05.000000 xgi-0.7/xgi.egg-info/top_level.txt
```

### Comparing `xgi-0.6/CODE_OF_CONDUCT.md` & `xgi-0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `xgi-0.6/CONTRIBUTING.md` & `xgi-0.7/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 9. Update the "Current Version" section of CHANGELOG.md with overview of changes to the interface and add the usernames of all contributors.
 10. Submit Pull Request with a list of changes, links to issues that it addresses (if applicable)
 11. You may merge the Pull Request in once you have the sign-off of at least one other developer, or if you do not have permission to do that, you may request the reviewer to merge it for you.
 
 ## New Version process
 1. Make sure that the Github Actions workflow runs without any errors.
 2. Using the `github-changelog` package (a dependency in the [release](requirements/release.txt) requirements file), run `changelog -m xgi-org xgi [last release tag]` to get the merged pull requests with their links. Paste this into the changelog file under a new heading and edit to make more legible. Associate a GitHub username with each pull request.
-3. Increase the version number in [setup.py](setup.py), [conf.py](docs/source/conf.py), and [CITATION.cff](CITATION.cff) to the new version agreed upon by the core developers. The versioning scheme we use is [SemVer](http://semver.org/).
+3. Increase the version number in [setup.py](setup.py) and [conf.py](docs/source/conf.py) to the new version agreed upon by the core developers. The versioning scheme we use is [SemVer](http://semver.org/).
 4. Commit these changes.
 5. Create a new release on GitHub by selecting "Releases", then clicking "Draft a new release". Click "Choose a tag" and type "v" followed by the version number and then click "Create new tag". The release title will be this same string. Paste the contents of the CHANGELOG into the "Describe this release" field. Click "Publish release".
 6. Run `python setup.py sdist` from the main folder. This will create a zipped file to upload to PyPI and save it to the "dist" folder.
 6. Using `twine` (a dependency in the [release](requirements/release.txt) requirements file), run `twine upload dist/xgi-[version number].tar.gz`. Enter your username and password.
 4. The new version is now on PyPI.
 
 ## Attribution
```

### Comparing `xgi-0.6/LICENSE.md` & `xgi-0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xgi-0.6/PKG-INFO` & `xgi-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgi
-Version: 0.6
+Version: 0.7
 Summary: XGI is a Python library for the representation
 Author: Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze
 Author-email: nicholas.landry@uvm.edu
 Project-URL: Documentation, https://xgi.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/xgi-org/xgi/issues
 Project-URL: Source, https://github.com/xgi-org/xgi
 Project-URL: PyPI, https://pypi.org/project/xgi/
```

### Comparing `xgi-0.6/README.md` & `xgi-0.7/README.md`

 * *Files identical despite different names*

### Comparing `xgi-0.6/logo/logo.pdf` & `xgi-0.7/logo/logo.pdf`

 * *Files identical despite different names*

### Comparing `xgi-0.6/logo/logo.png` & `xgi-0.7/logo/logo.png`

 * *Files identical despite different names*

### Comparing `xgi-0.6/logo/logo.svg` & `xgi-0.7/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `xgi-0.6/long_description.rst` & `xgi-0.7/long_description.rst`

 * *Files identical despite different names*

### Comparing `xgi-0.6/requirements/README.md` & `xgi-0.7/requirements/README.md`

 * *Files identical despite different names*

### Comparing `xgi-0.6/setup.py` & `xgi-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 import setuptools
 from setuptools import setup
 
-__version__ = "0.6"
+__version__ = "0.7"
 
 if sys.version_info < (3, 8):
     sys.exit("XGI requires Python 3.8 or later.")
 
 name = "xgi"
 
 version = __version__
```

### Comparing `xgi-0.6/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb` & `xgi-0.7/tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/Tutorial 2 - Read and Write.ipynb` & `xgi-0.7/tutorials/Tutorial 2 - Read and Write.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb` & `xgi-0.7/tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/Tutorial 4 - Generative_Models.ipynb` & `xgi-0.7/tutorials/Tutorial 4 - Generative_Models.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/Tutorial 5 - Plotting.ipynb` & `xgi-0.7/tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.1'}}"}*

```diff
@@ -737,13 +737,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.11.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `xgi-0.6/tutorials/Tutorial 6 - Statistics.ipynb` & `xgi-0.7/tutorials/Tutorial 6 - Statistics.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb` & `xgi-0.7/tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'cells'": "{2: {'source': ['This is a simple example to show how the function to draw a "*

 * *            "hypergraph with hyperedges displayed as colored convex hulls work.']}}"}*

```diff
@@ -17,15 +17,15 @@
                 "import networkx as nx"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This is a simple example to show how the function to draw an hypergraph with hyperedges displayed as colored convex hulls work."
+                "This is a simple example to show how the function to draw a hypergraph with hyperedges displayed as colored convex hulls work."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
```

### Comparing `xgi-0.6/tutorials/case_study_zhang2022.ipynb` & `xgi-0.7/tutorials/case_study_zhang2022.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/quickstart.ipynb` & `xgi-0.7/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/tutorials/simplicial_kuramoto_example.ipynb` & `xgi-0.7/tutorials/simplicial_kuramoto_example.ipynb`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/algorithms/assortativity.py` & `xgi-0.7/xgi/algorithms/assortativity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Algorithms for finding the degree assortativity of a hypergraph."""
+
 import random
 from itertools import combinations
 
 import numpy as np
 
 from ..classes import is_uniform, unique_edge_sizes
 from ..exception import XGIError
```

### Comparing `xgi-0.6/xgi/algorithms/centrality.py` & `xgi-0.7/xgi/algorithms/centrality.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Algorithms for computing the centralities of nodes (and edges) in a hypergraph."""
+
 from warnings import warn
 
 import networkx as nx
 import numpy as np
 from numpy.linalg import norm
 from scipy.sparse.linalg import eigsh
 
@@ -12,14 +13,15 @@
 from ..linalg import clique_motif_matrix, incidence_matrix
 
 __all__ = [
     "clique_eigenvector_centrality",
     "h_eigenvector_centrality",
     "node_edge_centrality",
     "line_vector_centrality",
+    "katz_centrality",
 ]
 
 
 def clique_eigenvector_centrality(H, tol=1e-6):
     """Compute the clique motif eigenvector centrality of a hypergraph.
 
     Parameters
@@ -170,24 +172,24 @@
 
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest
     f : lambda function, optional
         The function f as described in Tudisco and Higham.
-        Must accept a numpy array. By default, $x^2$.
+        Must accept a numpy array. By default, :math:`f(x) = x^2`.
     g : lambda function, optional
         The function g as described in Tudisco and Higham.
-        Must accept a numpy array. By default, $\sqrt{x}$.
+        Must accept a numpy array. By default, :math`g(x) = \sqrt{x}`.
     phi : lambda function, optional
         The function phi as described in Tudisco and Higham.
-        Must accept a numpy array. By default $x^2$.
+        Must accept a numpy array. By default :math:`\phi(x) = x^2`.
     psi : lambda function, optional
         The function psi as described in Tudisco and Higham.
-        Must accept a numpy array. By default: $\sqrt{x}$.
+        Must accept a numpy array. By default: :math:`\psi(x) = \sqrt{x}`.
     max_iter : int, optional
         Number of iterations at which the algorithm terminates
         if convergence is not reached. By default, 100.
     tol : float > 0, optional
         The total allowable error in the node and edge centralities.
         By default, 1e-6.
 
@@ -247,14 +249,15 @@
     return {node_dict[n]: new_x[n] for n in node_dict}, {
         edge_dict[e]: new_y[e] for e in edge_dict
     }
 
 
 def line_vector_centrality(H):
     """The vector centrality of nodes in the line graph of the hypergraph.
+
     Parameters
     ----------
     H : Hypergraph
         The hypergraph of interest
 
     Returns
     -------
@@ -303,7 +306,100 @@
 
         c_i *= 1 / k
 
         for node in H.nodes:
             vc[node].append(c_i[node])
 
     return vc
+
+
+def katz_centrality(H, index=False, cutoff=100):
+    r"""Returns the Katz-centrality vector of a non-empty hypergraph H.
+
+    The Katz-centrality measures the relative importance of a node by counting
+    how many distinct walks start from it. The longer the walk is the smaller
+    its contribution will be (attenuation factor :math:`\alpha`).
+    Initially defined for graphs, the Katz-centrality is here generalized to
+    hypergraphs using the most basic definition of neighbors: two nodes that
+    share an hyperedge.
+
+    Parameters
+    ----------
+    H : xgi.Hypergraph
+        Hypergraph on which to compute the Katz-centralities.
+    index : bool
+        If set to `True`, will return a dictionary mapping each vector index to a
+        node. Default value is `False`.
+    cutoff : int
+        Power at which to stop the series :math:`A + \alpha A^2 + \alpha^2 A^3 + \dots`
+        Default value is 100.
+
+    Returns
+    -------
+    c : np.ndarray
+        Vector of the node centralities, sorted by the node indexes.
+    nodedict : dict
+        If index is set to True, nodedict will contain the nodes ids, keyed by
+        their indice in vector `c`.
+        Thus, `c[key]` will be the centrality of node `nodedict[key]`.
+
+    Raises
+    ------
+    XGIError
+        If the hypergraph is empty.
+
+    Notes
+    -----
+    [1] The Katz-centrality is defined as
+
+    .. math::
+        c = [(I - \alpha A^{t})^{-1} - I]{\bf 1},
+
+    where :math:`A` is the adjency matrix of the the (hyper)graph.
+    Since :math:`A^{t} = A` for undirected graphs (our case), we have:
+
+
+    .. math::
+        &[I + A + \alpha A^2 + \alpha^2 A^3 + \dots](I - \alpha A^{t})
+
+        & = [I + A + \alpha A^2 + \alpha^2 A^3 + \dots](I - \alpha A)
+
+        & = (I + A + \alpha A^2 + \alpha^2 A^3 + \dots) - A - \alpha A^2
+
+        & - \alpha^2 A^3 - \alpha^3 A^4 - \dots
+
+        & = I
+
+    And :math:`(I - \alpha A^{t})^{-1} = I + A + \alpha A^2 + \alpha^2 A^3 + \dots`
+    Thus we can use the power serie to compute the Katz-centrality.
+    [2] The Katz-centrality of isolated nodes (no hyperedges contains them) is
+    zero. The Katz-centrality of an empty hypergraph is not defined.
+
+    References
+    ----------
+    See https://en.wikipedia.org/wiki/Katz_centrality#Alpha_centrality (visited
+    May 20 2023) for a clear definition of Katz centrality.
+    """
+
+    if index:
+        A, nodedict = clique_motif_matrix(H, index=True)
+    else:
+        A = clique_motif_matrix(H, index=False)
+
+    N = len(H.nodes)
+    M = len(H.edges)
+    if N == 0:  # no nodes
+        raise XGIError("The Katz-centrality of an empty hypergraph is not defined.")
+    elif M == 0:
+        c = np.zeros(N)
+    else:  # there is at least one edge, both N and M are non-zero
+        alpha = 1 / 2**N
+        mat = A
+        for power in range(1, cutoff):
+            mat = alpha * mat.dot(A) + A
+        u = 1 / N * np.ones(N)
+        c = mat.dot(u)
+
+    if index:
+        return c, nodedict
+    else:
+        return c
```

### Comparing `xgi-0.6/xgi/algorithms/clustering.py` & `xgi-0.7/xgi/algorithms/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+"""Algorithms for computing nodal clustering coefficients."""
+
 import numpy as np
 
 from ..exception import XGIError
 from ..linalg import adjacency_matrix
 
 __all__ = [
     "clustering_coefficient",
     "local_clustering_coefficient",
     "two_node_clustering_coefficient",
 ]
 
 
 def clustering_coefficient(H):
-    """Return the clustering coefficients for
+    r"""Return the clustering coefficients for
     each node in a Hypergraph.
 
     This clustering coefficient is defined as the
     clustering coefficient of the unweighted pairwise
-    projection of the hypergraph, i.e., `num / denom`,
-    where `num` equals $A^3_{i,i}$ and `denom` equals
-    $\binom{k}{2}$.  Here $A$ is the adjacency matrix
-    of the network and $k$ is the pairwise
-    degree of $i$.
+    projection of the hypergraph, i.e.,
+    :math:`c = A^3_{i,i}/\binom{k}{2},`
+    where :math:`A` is the adjacency matrix of the network
+    and :math:`k` is the pairwise degree of :math:`i`.
 
     Parameters
     ----------
     H : Hypergraph
         Hypergraph
 
     Returns
```

### Comparing `xgi-0.6/xgi/algorithms/connected.py` & `xgi-0.7/xgi/algorithms/connected.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/classes/function.py` & `xgi-0.7/xgi/classes/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,15 +768,15 @@
     except ZeroDivisionError:
         return 0.0
 
 
 def incidence_density(H, order=None, max_order=None, ignore_singletons=False):
     r"""Density of the incidence matrix.
 
-    The incidence matrix of a hypergraph contains one row per node nad one column per
+    The incidence matrix of a hypergraph contains one row per node and one column per
     edge.  An entry is non-zero when the corresponding node is a member of the
     corresponding edge.  The density of this matrix is the number of non-zero entries
     divided by the total number of entries.
 
     Parameters
     ---------
     order : int, optional
```

### Comparing `xgi-0.6/xgi/classes/hypergraph.py` & `xgi-0.7/xgi/classes/hypergraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import defaultdict
 from collections.abc import Hashable, Iterable
 from copy import copy, deepcopy
 from itertools import count
 from warnings import warn
 
 from ..exception import IDNotFound, XGIError
-from ..utils.utilities import IDDict, update_uid_counter
+from ..utils import IDDict, update_uid_counter
 from .reportviews import EdgeView, NodeView
 
 __all__ = ["Hypergraph"]
 
 
 class Hypergraph:
     r"""A hypergraph is a collection of subsets of a set of *nodes* or *vertices*.
@@ -18,17 +18,15 @@
     A hypergraph is a pair :math:`(V, E)`, where :math:`V` is a set of elements called
     *nodes* or *vertices*, and :math:`E` is a set whose elements are subsets of
     :math:`V`, that is, each :math:`e \in E` satisfies :math:`e \subset V`.  The
     elements of :math:`E` are called *hyperedges* or simply *edges*.
 
     The Hypergraph class allows any hashable object as a node and can associate
     attributes to each node, edge, or the hypergraph itself, in the form of key/value
-    pairs.
-
-    Multiedges and self-loops are allowed.
+    pairs. In this representation, multiedges are allowed.
 
     Parameters
     ----------
     incoming_data : input hypergraph data, optional
         Data to initialize the hypergraph. If None (default), an empty
         hypergraph is created, i.e. one with no nodes or edges.
         The data can be in the following formats:
@@ -894,15 +892,15 @@
             If no edge has that ID.
 
         See Also
         --------
         remove_edges_from : Remove multiple edges.
 
         """
-        for node in self.edges.members(id):
+        for node in self._edge[id].copy():
             self._node[node].remove(id)
         del self._edge[id]
         del self._edge_attr[id]
 
     def remove_edges_from(self, ebunch):
         """Remove multiple edges.
 
@@ -918,15 +916,15 @@
 
         See Also
         --------
         remove_edge : remove a single edge.
 
         """
         for id in ebunch:
-            for node in self.edges.members(id):
+            for node in self._edge[id].copy():
                 self._node[node].remove(id)
             del self._edge[id]
             del self._edge_attr[id]
 
     def remove_node_from_edge(self, edge, node):
         """Remove a node from an existing edge.
 
@@ -992,15 +990,15 @@
             self.add_nodes_from(nodes)
         if edges:
             self.add_edges_from(edges)
 
     def clear(self, hypergraph_attr=True):
         """Remove all nodes and edges from the graph.
 
-        Also removes node and edge attribues, and optionally hypergraph attributes.
+        Also removes node and edge attributes, and optionally hypergraph attributes.
 
         Parameters
         ----------
         hypergraph_attr : bool, optional
             Whether to remove hypergraph attributes as well.
             By default, True.
```

### Comparing `xgi-0.6/xgi/classes/hypergraphviews.py` & `xgi-0.7/xgi/classes/hypergraphviews.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/classes/reportviews.py` & `xgi-0.7/xgi/classes/reportviews.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """View classes for hypergraphs.
 
 A View class allows for inspection and querying of an underlying object but does not
-allow modification.  This module provides View classes for nodes, edges, degree, and
-edge size of a hypergraph.  Views are automatically updaed when the hypergraph changes.
+allow modification.  This module provides View classes for nodes and edges of a hypergraph.
+Views are automatically updaed when the hypergraph changes.
 
 """
 
 from collections import defaultdict
 from collections.abc import Mapping, Set
 from functools import reduce
 
@@ -23,18 +23,16 @@
     """Base View class for accessing the ids (nodes or edges) of a Hypergraph.
 
     Can optionally keep track of a subset of ids.  By default all node ids or all edge
     ids are kept track of.
 
     Parameters
     ----------
-    id_dict : dict
-        The original dict this is a view of.
-    id_attrs : dict
-        The original attribute dict this is a view of.
+    network : Hypergraph or Simplicial Complex
+        The underlying network
     ids : iterable
         A subset of the keys in id_dict to keep track of.
 
     Raises
     ------
     XGIError
         If ids is not a subset of the keys of id_dict.
@@ -133,15 +131,15 @@
         ----------
         id : hashable
             node or edge ID
 
         Returns
         -------
         dict
-            Node attributes.
+            attributes associated to the ID.
 
         Raises
         ------
         XGIError
             If the id is not being kept track of by this view, or if id is not in the
             hypergraph, or if id is not hashable.
 
@@ -179,16 +177,16 @@
         return self.from_view(self, bunch)
 
     def filterby(self, stat, val, mode="eq"):
         """Filter the IDs in this view by a statistic.
 
         Parameters
         ----------
-        stat : str or :class:`xgi.stats.NodeStat`
-            `NodeStat` object, or name of a `NodeStat`.
+        stat : str or :class:`xgi.stats.NodeStat`/:class:`xgi.stats.EdgeStat`
+            `NodeStat`/`EdgeStat` object, or name of a `NodeStat`/`EdgeStat`.
         val : Any
             Value of the statistic.  Usually a single numeric value.  When mode is
             'between', must be a tuple of exactly two values.
         mode : str, optional
             How to compare each value to `val`.  Can be one of the following.
 
             * 'eq' (default): Return IDs whose value is exactly equal to `val`.
@@ -476,15 +474,15 @@
 
         Allows to create a view with the same underlying data but with a different
         bunch.
 
         Parameters
         ----------
         view : IDView
-            The view used to initialze the new object
+            The view used to initialize the new object
         bunch : iterable
             IDs the new view will keep track of
 
         Returns
         -------
         IDView
             A view that is identical to `view` but keeps track of different IDs.
@@ -499,15 +497,15 @@
         all_ids = set(view._id_dict)
         if bunch is None:
             newview._ids = all_ids
         else:
             bunch = set(bunch)
             wrong = bunch - all_ids
             if wrong:
-                raise IDNotFound(f"Nodes {wrong} not in the hypergraph")
+                raise IDNotFound(f"IDs {wrong} not in the hypergraph")
             newview._ids = bunch
         return newview
 
     def _from_iterable(self, it):
         """Construct an instance of the class from any iterable input.
 
         This overrides collections.abc.Set._from_iterable, which is in turn used to
@@ -567,15 +565,15 @@
         Raises
         ------
         XGIError
             If `n` is not hashable or if it is not in the hypergraph.
 
         """
         return (
-            {key: self._id_dict[key] for key in self}
+            {key: self._id_dict[key].copy() for key in self}
             if n is None
             else self._id_dict[n].copy()
         )
 
     def isolates(self, ignore_singletons=False):
         """Nodes that belong to no edges.
 
@@ -673,17 +671,17 @@
             If `dtype` is not dict or list
         IDNotFound
             If `e` does not exist in the hypergraph
 
         """
         if e is None:
             if dtype is dict:
-                return {key: self._id_dict[key] for key in self}
+                return {key: self._id_dict[key].copy() for key in self}
             elif dtype is list:
-                return [self._id_dict[key] for key in self]
+                return [self._id_dict[key].copy() for key in self]
             else:
                 raise XGIError(f"Unrecognized dtype {dtype}")
 
         if e not in self:
             raise IDNotFound(f'ID "{e}" not in this view')
 
         return self._id_dict[e].copy()
```

### Comparing `xgi-0.6/xgi/classes/simplicialcomplex.py` & `xgi-0.7/xgi/classes/simplicialcomplex.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/convert.py` & `xgi-0.7/xgi/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     csc_matrix,
     csr_array,
     csr_matrix,
     lil_array,
     lil_matrix,
 )
 
-from .classes import Hypergraph, SimplicialComplex, set_edge_attributes
+from .classes import DiHypergraph, Hypergraph, SimplicialComplex, set_edge_attributes
 from .exception import XGIError
-from .generators import empty_hypergraph, empty_simplicial_complex
+from .generators import empty_dihypergraph, empty_hypergraph, empty_simplicial_complex
 from .linalg import adjacency_matrix, incidence_matrix
-from .utils.utilities import dual_dict
 
 __all__ = [
     "convert_to_hypergraph",
+    "convert_to_dihypergraph",
     "convert_to_graph",
     "convert_to_simplicial_complex",
     "from_hyperedge_list",
     "to_hyperedge_list",
     "from_hyperedge_dict",
     "to_hyperedge_dict",
     "from_bipartite_pandas_dataframe",
@@ -77,14 +77,23 @@
         H = empty_hypergraph(create_using)
         H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
         ee = data.edges
         H.add_edges_from((ee.members(e), e, deepcopy(attr)) for e, attr in ee.items())
         H._hypergraph = deepcopy(data._hypergraph)
         return H
 
+    elif isinstance(data, DiHypergraph):
+        H = empty_hypergraph(create_using)
+        H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
+        ee = data.edges
+        H.add_edges_from((ee.members(e), e, deepcopy(attr)) for e, attr in ee.items())
+        H._hypergraph = deepcopy(data._hypergraph)
+        if not isinstance(create_using, DiHypergraph):
+            return H
+
     elif isinstance(data, SimplicialComplex):
         return from_max_simplices(data)
 
     elif isinstance(data, list):
         # edge list
         result = from_hyperedge_list(data, create_using)
         if not isinstance(create_using, Hypergraph):
@@ -118,14 +127,68 @@
     ):
         from_incidence_matrix(data, create_using)
 
     else:
         raise XGIError("Input data has unsupported type.")
 
 
+def convert_to_dihypergraph(data, create_using=None):
+    """Make a dihypergraph from a known data structure.
+
+    The preferred way to call this is automatically from the class constructor.
+
+    Parameters
+    ----------
+    data : object to be converted
+        Current known types are:
+         * a DiHypergraph object
+         * a SimplicialComplex object
+         * list-of-iterables
+         * dict-of-iterables
+         * Pandas DataFrame (bipartite edgelist)
+         * numpy matrix
+         * numpy ndarray
+         * scipy sparse matrix
+    create_using : Hypergraph constructor, optional (default=Hypergraph)
+        Hypergraph type to create. If hypergraph instance, then cleared before populated.
+
+    Returns
+    -------
+    Hypergraph object
+        A hypergraph constructed from the data
+
+    """
+    if data is None:
+        return empty_dihypergraph(create_using)
+
+    elif isinstance(data, DiHypergraph):
+        H = empty_dihypergraph(create_using)
+        H.add_nodes_from((n, attr) for n, attr in data.nodes.items())
+        ee = data.edges
+        H.add_edges_from((ee.dimembers(e), e, deepcopy(attr)) for e, attr in ee.items())
+        H._hypergraph = deepcopy(data._hypergraph)
+        if not isinstance(create_using, DiHypergraph):
+            return H
+
+    elif isinstance(data, list):
+        # edge list
+        result = from_hyperedge_list(data, create_using)
+        if not isinstance(create_using, DiHypergraph):
+            return result
+
+    elif isinstance(data, dict):
+        # edge dict in the form we need
+        result = from_hyperedge_dict(data, create_using)
+        if not isinstance(create_using, DiHypergraph):
+            return result
+
+    else:
+        raise XGIError("Input data has unsupported type.")
+
+
 def convert_to_graph(H):
     """Graph projection (1-skeleton) of the hypergraph H.
     Weights are not considered.
 
     Parameters
     ----------
     H : Hypergraph object
@@ -335,15 +398,14 @@
 
     See Also
     --------
     to_hyperedge_dict
 
     """
     H = empty_hypergraph(create_using)
-    H.add_nodes_from(dual_dict(d))
     H.add_edges_from((members, uid) for uid, members in d.items())
     return H
 
 
 def to_hyperedge_dict(H):
     """Outputs a hyperedge dictionary
```

### Comparing `xgi-0.6/xgi/drawing/draw.py` & `xgi-0.7/xgi/drawing/draw.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 from inspect import signature
 from itertools import combinations
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import cm
 from matplotlib.colors import LinearSegmentedColormap, ListedColormap
+from matplotlib.patches import FancyArrow
+from mpl_toolkits.mplot3d.art3d import Line3DCollection, Poly3DCollection
+from networkx import spring_layout
 from scipy.spatial import ConvexHull
 
 from .. import convert
-from ..classes import Hypergraph, SimplicialComplex, max_edge_order
+from ..classes import DiHypergraph, Hypergraph, SimplicialComplex, max_edge_order
 from ..exception import XGIError
 from ..stats import EdgeStat, NodeStat
-from .layout import barycenter_spring_layout
+from .layout import _augmented_projection, barycenter_spring_layout
 
 __all__ = [
     "draw",
     "draw_nodes",
     "draw_hyperedges",
     "draw_simplices",
     "draw_node_labels",
     "draw_hyperedge_labels",
     "draw_hypergraph_hull",
+    "draw_multilayer",
+    "draw_dihypergraph",
 ]
 
 
 def draw(
     H,
     pos=None,
     ax=None,
@@ -1268,14 +1273,448 @@
         pos,
         ax,
         node_fc,
         node_ec,
         node_lw,
         node_size,
         max_order,
+        settings,
+        node_labels,
+        **kwargs,
+    )
+
+    # compute axis limits
+    _update_lims(pos, ax)
+
+    return ax
+
+
+def draw_multilayer(
+    H,
+    pos=None,
+    ax=None,
+    node_fc="tab:blue",
+    node_ec="black",
+    node_lw=0.5,
+    node_size=5,
+    max_order=None,
+    palette="jet",
+    conn_lines=True,
+    conn_lines_style="dotted",
+    width=5,
+    height=5,
+    h_angle=10,
+    v_angle=0,
+    sep=1,
+):
+    """Draw a hypergraph or simplicial complex visualized in 3D
+    showing hyperedges/simplices of different orders on superimposed layers.
+
+    Parameters
+    ----------
+    H : Hypergraph or SimplicialComplex.
+        Higher-order network to plot.
+    pos : dict or None, optional
+        The positions of the nodes in the multilayer network. If None, a default layout will be computed using xgi.barycenter_spring_layout(). Default is None.
+    ax : matplotlib Axes3DSubplot or None, optional
+        The subplot to draw the visualization on. If None, a new subplot will be created. Default is None.
+    node_fc : color or sequence of colors, optional
+        The face color(s) of the nodes. Default is "tab:blue".
+    node_ec : color or sequence of colors, optional
+        The edge color(s) of the nodes. Default is "black".
+    node_lw : float or sequence of floats, optional
+        The linewidth(s) of the node edges. Default is 0.5.
+    node_size : scalar or array-like, optional
+        The size(s) of the nodes. Default is 5.
+    max_order : int or None, optional
+        The maximum order of hyperedges/simplices to consider for coloring. If None edges up to the maximal order are drawn. Default is None.
+    palette : str, optional
+        The name of the matplotlib color palette to use. Default is 'jet'.
+    conn_lines : bool, optional
+        Whether to draw connections between layers. Default is True.
+    conn_lines_style : str, optional
+        The linestyle of the connections between layers. Default is 'dotted'.
+    width : float, optional
+        The width of the figure in inches. Default is 5.
+    height : float, optional
+        The height of the figure in inches. Default is 5.
+    h_angle : float, optional
+        The rotation angle around the horizontal axis in degrees. Default is 10.
+    v_angle : float, optional
+        The rotation angle around the vertical axis in degrees. Default is 0.
+    sep : float, optional
+        The separation between layers. Default is 1.
+
+    Returns
+    -------
+    ax : matplotlib Axes3DSubplot
+        The subplot with the multilayer network visualization.
+    """
+
+    if pos is None:
+        pos = barycenter_spring_layout(H)
+
+    if ax is None:
+        fig, ax = plt.subplots(
+            1, 1, figsize=(width, height), dpi=600, subplot_kw={"projection": "3d"}
+        )
+
+    if max_order is None:
+        max_order = max_edge_order(H)
+
+    cmap = cm.get_cmap(palette, max_order)
+
+    xs, ys = zip(*pos.values())
+
+    for order in range(1, max_order + 1):
+        zs = [order * sep] * len(xs)
+
+        # draw lines connecting points on the different planes
+        if conn_lines and order > 1:
+            thru_nodes = H.nodes
+            lines3d_between = [
+                (list(pos[i]) + [order * sep - sep], list(pos[i]) + [order * sep])
+                for i in thru_nodes
+            ]
+            between_lines = Line3DCollection(
+                lines3d_between,
+                zorder=order,
+                color=".5",
+                alpha=0.4,
+                linestyle=conn_lines_style,
+                linewidth=1,
+            )
+            ax.add_collection3d(between_lines)
+
+        # draw the edges/simplices of given order
+        edges = H.edges.filterby("order", order).members()
+        # dyads
+        if order == 1:
+            lines3d = [
+                (list(pos[i]) + [order * sep], list(pos[j]) + [order * sep])
+                for i, j in edges
+            ]
+            line_collection = Line3DCollection(
+                lines3d,
+                zorder=order - 1,
+                color=cmap(order - 1),
+                alpha=1,
+                linewidth=0.7,
+            )
+            ax.add_collection3d(line_collection)
+        # higher-orders
+        else:
+            poly = []
+            for e in edges:
+                vertices = np.array([[xs[i - 1], ys[i - 1], zs[i - 1]] for i in e])
+                vertices = _CCW_sort(vertices)
+                poly.append(vertices)
+            poly = Poly3DCollection(
+                poly,
+                zorder=order - 1,
+                color=cmap(order - 1),
+                alpha=0.5,
+            )
+            ax.add_collection3d(poly)
+        # draw nodes
+        ax.scatter(
+            xs,
+            ys,
+            zs,
+            c=node_fc,
+            edgecolors=node_ec,
+            linewidths=node_lw,
+            marker="o",
+            alpha=1,
+            zorder=order + 1,
+            s=node_size,
+        )
+        # draw surfaces corresponding to the different orders
+        xdiff = np.max(xs) - np.min(xs)
+        ydiff = np.max(ys) - np.min(ys)
+        ymin = np.min(ys) - ydiff * 0.1
+        ymax = np.max(ys) + ydiff * 0.1
+        xmin = np.min(xs) - xdiff * 0.1 * (width / height)
+        xmax = np.max(xs) + xdiff * 0.1 * (width / height)
+        xx, yy = np.meshgrid([xmin, xmax], [ymin, ymax])
+        zz = np.zeros(xx.shape) + order * sep
+        ax.plot_surface(
+            xx,
+            yy,
+            zz,
+            color=cmap(order - 1),
+            alpha=0.1,
+            zorder=order,
+        )
+
+    ax.view_init(h_angle, v_angle)
+    ax.set_ylim(np.min(ys) - ydiff * 0.1, np.max(ys) + ydiff * 0.1)
+    ax.set_xlim(np.min(xs) - xdiff * 0.1, np.max(xs) + xdiff * 0.1)
+    ax.set_axis_off()
+
+    return ax
+
+
+def draw_dihypergraph(
+    DH,
+    ax=None,
+    lines_fc=None,
+    lines_lw=1.5,
+    line_head_width=0.05,
+    node_fc="white",
+    node_ec="black",
+    node_lw=1,
+    node_size=15,
+    edge_marker_toggle=True,
+    edge_marker_fc=None,
+    edge_marker_ec=None,
+    edge_marker="s",
+    edge_marker_lw=1,
+    edge_marker_size=15,
+    max_order=None,
+    node_labels=False,
+    hyperedge_labels=False,
+    settings=None,
+    **kwargs,
+):
+    """Draw a directed hypergraph
+
+    Parameters
+    ----------
+    DH : DirectedHypergraph
+        The directed hypergraph to draw.
+    ax : matplotlib.pyplot.axes, optional
+        Axis to draw on. If None (default), get the current axes.
+    lines_fc : str, dict, iterable, optional
+        Color of the hyperedges (lines). If str, use the same color for all hyperedges.
+        If a dict, must contain (hyperedge_id: color_str) pairs. If other iterable,
+        assume the colors are specified in the same order as the hyperedges are found
+        in DH.edges. If None (default), use the size of the hyperedges.
+    lines_lw : int, float, dict, iterable, optional
+        Line width of the hyperedges (lines). If int or float, use the same width for
+        all hyperedges. If a dict, must contain (hyperedge_id: width) pairs. If other
+        iterable, assume the widths are specified in the same order as the hyperedges
+        are found in DH.edges. By default, 1.5.
+    line_head_width : float, optional
+        Length of arrows' heads. By default, 0.05
+    node_fc : str, dict, iterable, or NodeStat, optional
+        Color of the nodes.  If str, use the same color for all nodes.  If a dict, must
+        contain (node_id: color_str) pairs.  If other iterable, assume the colors are
+        specified in the same order as the nodes are found in H.nodes. If NodeStat, use
+        the colormap specified with node_fc_cmap. By default, "white".
+    node_ec : str, dict, iterable, or NodeStat, optional
+        Color of node borders.  If str, use the same color for all nodes.  If a dict,
+        must contain (node_id: color_str) pairs.  If other iterable, assume the colors
+        are specified in the same order as the nodes are found in H.nodes. If NodeStat,
+        use the colormap specified with node_ec_cmap. By default, "black".
+    node_lw : int, float, dict, iterable, or NodeStat, optional
+        Line width of the node borders in pixels.  If int or float, use the same width
+        for all node borders.  If a dict, must contain (node_id: width) pairs.  If
+        iterable, assume the widths are specified in the same order as the nodes are
+        found in H.nodes. If NodeStat, use a monotonic linear interpolation defined
+        between min_node_lw and max_node_lw. By default, 1.
+    node_size : int, float, dict, iterable, or NodeStat, optional
+        Radius of the nodes in pixels.  If int or float, use the same radius for all
+        nodes.  If a dict, must contain (node_id: radius) pairs.  If iterable, assume
+        the radiuses are specified in the same order as the nodes are found in
+        H.nodes. If NodeStat, use a monotonic linear interpolation defined between
+        min_node_size and max_node_size. By default, 15.
+    edge_marker_toggle: bool, optional
+        If True then marker representing the hyperedges are drawn. By default True.
+    edge_marker_fc: str, dict, iterable, optional
+        Filling color of the hyperedges (markers). If str, use the same color for all hyperedges.
+        If a dict, must contain (hyperedge_id: color_str) pairs. If other iterable,
+        assume the colors are specified in the same order as the hyperedges are found
+        in DH.edges. If None (default), use the size of the hyperedges.
+    edge_marker_ec: str, dict, iterable, optional
+        Edge color of the hyperedges (markers). If str, use the same color for all hyperedges.
+        If a dict, must contain (hyperedge_id: color_str) pairs. If other iterable,
+        assume the colors are specified in the same order as the hyperedges are found
+        in DH.edges. If None (default), use the size of the hyperedges.
+    edge_marker: str, optional
+        Marker used for the hyperedges. By default 's' (square marker).
+    max_order : int, optional
+        Maximum of hyperedges to plot. If None (default), plots all orders.
+    node_labels : bool or dict, optional
+        If True, draw ids on the nodes. If a dict, must contain (node_id: label) pairs.
+        By default, False.
+    hyperedge_labels : bool or dict, optional
+        If True, draw ids on the hyperedges. If a dict, must contain (edge_id: label)
+        pairs.  By default, False.
+    **kwargs : optional args
+        Alternate default values. Values that can be overwritten are the following:
+        * min_node_size
+        * max_node_size
+        * min_node_lw
+        * max_node_lw
+        * node_fc_cmap
+        * node_ec_cmap
+        * min_lines_lw
+        * max_lines_lw
+        * lines_fc_cmap
+        * edge_fc_cmap
+        * edge_marker_fc_cmap
+        * edge_marker_ec_cmap
+
+    Returns
+    -------
+    ax : matplotlib.pyplot.axes
+
+    Raises
+    ------
+    XGIError
+        If something different than a DiHypergraph is passed.
+
+    See Also
+    --------
+    draw
+    draw_nodes
+    draw_node_labels
+
+    """
+    if not isinstance(DH, DiHypergraph):
+        raise XGIError("The input must be a DiHypergraph")
+
+    if settings is None:
+        settings = {
+            "min_node_size": 10.0,
+            "max_node_size": 30.0,
+            "min_node_lw": 1.0,
+            "max_node_lw": 5.0,
+            "node_fc_cmap": cm.Reds,
+            "node_ec_cmap": cm.Greys,
+            "min_lines_lw": 2.0,
+            "max_lines_lw": 10.0,
+            "lines_fc_cmap": cm.Blues,
+            "edge_marker_fc_cmap": cm.Blues,
+            "edge_marker_ec_cmap": cm.Greys,
+        }
+
+    settings.update(kwargs)
+
+    if ax is None:
+        ax = plt.gca()
+
+    ax.get_xaxis().set_ticks([])
+    ax.get_yaxis().set_ticks([])
+    ax.axis("off")
+
+    # convert to hypergraph in order to use the augmented projection function
+    H_conv = convert.convert_to_hypergraph(DH)
+
+    if not max_order:
+        max_order = max_edge_order(H_conv)
+
+    lines_lw = _scalar_arg_to_dict(
+        lines_lw, H_conv.edges, settings["min_lines_lw"], settings["max_lines_lw"]
+    )
+
+    if lines_fc is None:
+        lines_fc = H_conv.edges.size
+
+    lines_fc = _color_arg_to_dict(lines_fc, H_conv.edges, settings["lines_fc_cmap"])
+
+    if edge_marker_fc is None:
+        edge_marker_fc = H_conv.edges.size
+
+    edge_marker_fc = _color_arg_to_dict(
+        edge_marker_fc, H_conv.edges, settings["edge_marker_fc_cmap"]
+    )
+
+    if edge_marker_ec is None:
+        edge_marker_ec = H_conv.edges.size
+
+    edge_marker_ec = _color_arg_to_dict(
+        edge_marker_ec, H_conv.edges, settings["edge_marker_ec_cmap"]
+    )
+
+    node_size = _scalar_arg_to_dict(
+        node_size, H_conv.nodes, settings["min_node_size"], settings["max_node_size"]
+    )
+
+    G_aug = _augmented_projection(H_conv)
+    for dyad in H_conv.edges.filterby("size", 2).members():
+        index = max(G_aug.nodes) + 1
+        G_aug.add_edges_from([[list(dyad)[0], index], [list(dyad)[1], index]])
+
+    phantom_nodes = [n for n in list(G_aug.nodes) if n not in list(H_conv.nodes)]
+    pos = spring_layout(G_aug)
+
+    for id, he in DH.edges.members(dtype=dict).items():
+        d = len(he) - 1
+        # identify the center of the edge in the augemented projection
+        center = [n for n in phantom_nodes if set(G_aug.neighbors(n)) == he][0]
+        x_center, y_center = pos[center]
+        for node in DH.edges.dimembers(id)[0]:
+            x_coords = [pos[node][0], x_center]
+            y_coords = [pos[node][1], y_center]
+            line = plt.Line2D(
+                x_coords,
+                y_coords,
+                color=lines_fc[id],
+                lw=lines_lw[id],
+                zorder=max_order - d,
+            )
+            ax.add_line(line)
+        for node in DH.edges.dimembers(id)[1]:
+            dx, dy = pos[node][0] - x_center, pos[node][1] - y_center
+            # the following to avoid the point of the arrow overlapping the node
+            distance = np.hypot(dx, dy)
+            direction_vector = np.array([dx, dy]) / distance
+            shortened_distance = (
+                distance - node_size[node] * 0.003
+            )  # Calculate the shortened length
+            dx = direction_vector[0] * shortened_distance
+            dy = direction_vector[1] * shortened_distance
+            arrow = FancyArrow(
+                x_center,
+                y_center,
+                dx,
+                dy,
+                color=lines_fc[id],
+                width=lines_lw[id] * 0.001,
+                length_includes_head=True,
+                head_width=line_head_width,
+                zorder=max_order - d,
+            )
+            ax.add_patch(arrow)
+        if edge_marker_toggle:
+            ax.scatter(
+                x=x_center,
+                y=y_center,
+                marker=edge_marker,
+                s=edge_marker_size**2,
+                c=edge_marker_fc[id],
+                edgecolors=edge_marker_ec[id],
+                linewidths=edge_marker_lw,
+                zorder=max_order,
+            )
+
+    if hyperedge_labels:
+        # Get all valid keywords by inspecting the signatures of draw_node_labels
+        valid_label_kwds = signature(draw_hyperedge_labels).parameters.keys()
+        # Remove the arguments of this function (draw_networkx)
+        valid_label_kwds = valid_label_kwds - {"H", "pos", "ax", "hyperedge_labels"}
+        if any([k not in valid_label_kwds for k in kwargs]):
+            invalid_args = ", ".join([k for k in kwargs if k not in valid_label_kwds])
+            raise ValueError(f"Received invalid argument(s): {invalid_args}")
+        label_kwds = {k: v for k, v in kwargs.items() if k in valid_label_kwds}
+        if "font_size_edges" not in label_kwds:
+            label_kwds["font_size_edges"] = 6
+        draw_hyperedge_labels(H_conv, pos, hyperedge_labels, ax_edges=ax, **label_kwds)
+
+    draw_nodes(
+        H_conv,
+        pos,
+        ax,
+        node_fc,
+        node_ec,
+        node_lw,
+        node_size,
+        max_order,
         settings,
         node_labels,
         **kwargs,
     )
 
     # compute axis limits
     _update_lims(pos, ax)
```

### Comparing `xgi-0.6/xgi/drawing/layout.py` & `xgi-0.7/xgi/drawing/layout.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/dynamics/synchronization.py` & `xgi-0.7/xgi/dynamics/synchronization.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/generators/classic.py` & `xgi-0.7/xgi/generators/classic.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 """
 
 from itertools import chain, combinations
 
 __all__ = [
     "empty_hypergraph",
+    "empty_dihypergraph",
     "empty_simplicial_complex",
     "trivial_hypergraph",
     "complete_hypergraph",
 ]
 
 
 def _empty_network(create_using, default):
@@ -22,15 +23,15 @@
     --------
     empty_hypergraph
     empty_simplicial_complex
 
     """
     if create_using is None:
         H = default()
-    elif hasattr(create_using, "_node"):
+    elif hasattr(create_using, "_node") or hasattr(create_using, "_node_in"):
         # create_using is a Hypergraph object
         create_using.clear()
         H = create_using
     else:
         # try create_using as constructor
         H = create_using()
     return H
@@ -71,14 +72,53 @@
     import xgi
 
     if default is None:
         default = xgi.Hypergraph
     return _empty_network(create_using, default)
 
 
+def empty_dihypergraph(create_using=None, default=None):
+    """Returns the empty dihypergraph with zero nodes and edges.
+
+    Parameters
+    ----------
+    create_using : DiHypergraph Instance, Constructor or None
+        If None, use the `default` constructor.
+        If a constructor, call it to create an empty dihypergraph.
+    default : DiHypergraph constructor (default None)
+        The constructor to use if create_using is None.
+        If None, then xgi.Hypergraph is used.
+
+    Returns
+    -------
+    Hypergraph object
+        An empty hypergraph
+
+    See also
+    --------
+    empty_simplicial_complex
+    trivial_hypergraph
+
+    Examples
+    --------
+    >>> import xgi
+    >>> H = xgi.empty_dihypergraph()
+    >>> H.num_nodes, H.num_edges
+    (0, 0)
+
+    """
+    # this import needs to happen when the function runs, not when the module is first
+    # imported, to avoid circular imports
+    import xgi
+
+    if default is None:
+        default = xgi.DiHypergraph
+    return _empty_network(create_using, default)
+
+
 def empty_simplicial_complex(create_using=None, default=None):
     """Returns the empty simplicial complex with zero nodes and simplices.
 
     Parameters
     ----------
     create_using : SimplicialComplex Instance, Constructor or None
         If None, use the `default` constructor.
@@ -111,15 +151,15 @@
 
     if default is None:
         default = xgi.SimplicialComplex
     return _empty_network(create_using, default)
 
 
 def trivial_hypergraph(n=1, create_using=None, default=None):
-    """Returns a hypergraph with `n` node and zero edges.
+    """Returns a hypergraph with `n` nodes and zero edges.
 
     Parameters
     ----------
     n : int, optional
         Number of nodes (default is 1)
     create_using : Hypergraph Instance, Constructor or None
         If None, use the `default` constructor.
```

### Comparing `xgi-0.6/xgi/generators/lattice.py` & `xgi-0.7/xgi/generators/lattice.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/generators/random.py` & `xgi-0.7/xgi/generators/random.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/generators/simple.py` & `xgi-0.7/xgi/generators/simple.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/generators/simplicial_complexes.py` & `xgi-0.7/xgi/generators/simplicial_complexes.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/generators/uniform.py` & `xgi-0.7/xgi/generators/uniform.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/linalg/hodge_matrix.py` & `xgi-0.7/xgi/linalg/hodge_matrix.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/linalg/hypergraph_matrix.py` & `xgi-0.7/xgi/linalg/hypergraph_matrix.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/linalg/laplacian_matrix.py` & `xgi-0.7/xgi/linalg/laplacian_matrix.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/readwrite/bipartite.py` & `xgi-0.7/xgi/readwrite/bipartite.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/readwrite/edgelist.py` & `xgi-0.7/xgi/readwrite/edgelist.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/readwrite/incidence.py` & `xgi-0.7/xgi/readwrite/incidence.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/readwrite/json.py` & `xgi-0.7/xgi/readwrite/json.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/readwrite/xgi_data.py` & `xgi-0.7/xgi/readwrite/xgi_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Load a data set from the xgi-data repository or a local file."""
 import json
 import os
-from functools import lru_cache
 from warnings import warn
 
-import requests
-
 from .. import convert
 from ..exception import XGIError
+from ..utils import request_json_from_url, request_json_from_url_cached
 
 __all__ = ["load_xgi_data", "download_xgi_data"]
 
 
 def load_xgi_data(
     dataset=None,
     cache=True,
@@ -21,47 +19,52 @@
     edgetype=None,
     max_order=None,
 ):
     """Load a data set from the xgi-data repository or a local file.
 
     Parameters
     ----------
-    dataset : str, default: None
+    dataset : str, optional
         Dataset name. Valid options are the top-level tags of the
-        index.json file in the xgi-data repository. If None, prints
+        index.json file in the xgi-data repository. If None (default), prints
         the list of available datasets.
     cache : bool, optional
-        Whether to cache the input data
+        Whether to cache the input data, by default True.
     read : bool, optional
         If read==True, search for a local copy of the data set. Use the local
-        copy if it exists, otherwise use the  xgi-data repository.
+        copy if it exists, otherwise use the xgi-data repository.
+        By default, False.
     path : str, optional
         Path to a local copy of the data set
     nodetype : type, optional
-        Type to cast the node ID to
+        Type to cast the node ID to, by default None.
     edgetype : type, optional
-        Type to cast the edge ID to
+        Type to cast the edge ID to, by default None.
     max_order: int, optional
-        Maximum order of edges to add to the hypergraph
+        Maximum order of edges to add to the hypergraph, by default None.
 
     Returns
     -------
     Hypergraph
         The loaded hypergraph.
 
     Raises
     ------
     XGIError
        The specified dataset does not exist.
     """
+    index_url = (
+        "https://gitlab.com/complexgroupinteractions/"
+        "xgi-data/-/raw/main/index.json?inline=false"
+    )
 
     # If no dataset is specified, print a list of the available datasets.
     if dataset is None:
-        index_url = "https://gitlab.com/complexgroupinteractions/xgi-data/-/raw/main/index.json?inline=false"
-        index_data = _request_json_from_url(index_url)
+
+        index_data = request_json_from_url(index_url)
         print("Available datasets are the following:")
         print(*index_data, sep="\n")
         return
 
     if read:
         cfp = os.path.join(path, dataset + ".json")
         if os.path.exists(cfp):
@@ -72,18 +75,15 @@
             )
         else:
             warn(
                 f"No local copy was found at {cfp}. The data is requested "
                 "from the xgi-data repository instead. To download a local "
                 "copy, use `download_xgi_data`."
             )
-    if cache:
-        data = _request_from_xgi_data_cached(dataset)
-    else:
-        data = _request_from_xgi_data(dataset)
+    data = _request_from_xgi_data(dataset, cache=cache)
 
     return convert.dict_to_hypergraph(
         data, nodetype=nodetype, edgetype=edgetype, max_order=max_order
     )
 
 
 def download_xgi_data(dataset, path=""):
@@ -102,23 +102,25 @@
 
     jsondata = _request_from_xgi_data(dataset)
     jsonfile = open(os.path.join(path, dataset + ".json"), "w")
     json.dump(jsondata, jsonfile)
     jsonfile.close()
 
 
-def _request_from_xgi_data(dataset=None):
+def _request_from_xgi_data(dataset=None, cache=True):
     """Request a dataset from xgi-data.
 
     Parameters
     ----------
-    dataset : str, default: None
+    dataset : str, optional
         Dataset name. Valid options are the top-level tags of the
         index.json file in the xgi-data repository. If None, prints
         the list of available datasets.
+    cache : bool, optional
+        Whether or not to cache the output
 
     Returns
     -------
     Data
         The requested data loaded from a json file.
 
     Raises
@@ -126,73 +128,24 @@
     XGIError
         If the HTTP request is not successful or the dataset does not exist.
 
     See also
     ---------
     load_xgi_data
     """
+    index_url = (
+        "https://gitlab.com/complexgroupinteractions/"
+        "xgi-data/-/raw/main/index.json?inline=false"
+    )
 
-    index_url = "https://gitlab.com/complexgroupinteractions/xgi-data/-/raw/main/index.json?inline=false"
-    index_data = _request_json_from_url(index_url)
+    index_data = request_json_from_url(index_url)
 
     key = dataset.lower()
     if key not in index_data:
         print("Valid dataset names:")
         print(*index_data, sep="\n")
         raise XGIError("Must choose a valid dataset name!")
 
-    return _request_json_from_url(index_data[key]["url"])
-
-
-@lru_cache(maxsize=None)
-def _request_from_xgi_data_cached(dataset):
-    """Request a dataset from xgi-data and cache the result.
-
-    Wraps `_request_from_xgi_data` in an lru_cache decorator.
-
-    Parameters
-    ----------
-    dataset : str
-        Dataset name. Valid options are the top-level tags of the
-        index.json file in the xgi-data repository.
-
-    Returns
-    -------
-    Data
-        The requested data loaded from a json file.
-
-    See also
-    ---------
-    load_xgi_data
-    """
-
-    return _request_from_xgi_data(dataset)
-
-
-def _request_json_from_url(url):
-    """HTTP request json file and return as dict.
-
-    Parameters
-    ----------
-    url : str
-        The url where the json file is located.
-
-    Returns
-    -------
-    dict
-        A dictionary of the JSON requested.
-
-    Raises
-    ------
-    XGIError
-        If the connection fails or if there is a bad HTTP request.
-    """
-
-    try:
-        r = requests.get(url)
-    except requests.ConnectionError:
-        raise XGIError("Connection Error!")
-
-    if r.ok:
-        return r.json()
+    if cache:
+        return request_json_from_url_cached(index_data[key]["url"])
     else:
-        raise XGIError(f"Error: HTTP response {r.status_code}")
+        return request_json_from_url(index_data[key]["url"])
```

### Comparing `xgi-0.6/xgi/stats/__init__.py` & `xgi-0.7/xgi/stats/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,17 +46,24 @@
 
 import numpy as np
 import pandas as pd
 from scipy.stats import moment as spmoment
 
 from xgi.exception import IDNotFound
 
-from . import edgestats, nodestats
+from . import edgestats, diedgestats, dinodestats, nodestats
 
-__all__ = ["nodestat_func", "edgestat_func", "dispatch_stat", "dispatch_many_stats"]
+__all__ = [
+    "nodestat_func",
+    "edgestat_func",
+    "dinodestat_func",
+    "diedgestat_func",
+    "dispatch_stat",
+    "dispatch_many_stats",
+]
 
 
 class IDStat:
     """Mapping between nodes or edges and a quantity or property."""
 
     def __init__(self, network, view, func, args=None, kwargs=None):
         self.view = view
@@ -204,24 +211,44 @@
     `NodeStat` objects represent a mapping that assigns a value to each node in a
     network.  For more details, see the `tutorial
     <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
 
+class DiNodeStat(IDStat):
+    """An arbitrary node-quantity mapping.
+
+    `NodeStat` objects represent a mapping that assigns a value to each node in a
+    network.  For more details, see the `tutorial
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+
+    """
+
+
 class EdgeStat(IDStat):
     """An arbitrary edge-quantity mapping.
 
     `EdgeStat` objects represent a mapping that assigns a value to each edge in a
     network.  For more details, see the `tutorial
     <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
 
+class DiEdgeStat(IDStat):
+    """An arbitrary edge-quantity mapping.
+
+    `EdgeStat` objects represent a mapping that assigns a value to each edge in a
+    network.  For more details, see the `tutorial
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+
+    """
+
+
 class MultiIDStat(IDStat):
     """Multiple mappings."""
 
     statsclass = None
     """IDStat subclass to use."""
 
     statsmodule = None
@@ -396,37 +423,71 @@
 
     """
 
     statsclass = NodeStat
     statsmodule = nodestats
 
 
+class MultiDiNodeStat(MultiIDStat):
+    """Multiple node-quantity mappings.
+
+    For more details, see the `tutorial
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+
+    """
+
+    statsclass = DiNodeStat
+    statsmodule = dinodestats
+
+
 class MultiEdgeStat(MultiIDStat):
     """Multiple edge-quantity mappings.
 
     For more details, see the `tutorial
     <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
 
     """
 
     statsclass = EdgeStat
     statsmodule = edgestats
 
 
+class MultiDiEdgeStat(MultiIDStat):
+    """Multiple edge-quantity mappings.
+
+    For more details, see the `tutorial
+    <https://github.com/xgi-org/xgi/blob/main/tutorials/Tutorial%206%20-%20Statistics.ipynb>`_.
+
+    """
+
+    statsclass = DiEdgeStat
+    statsmodule = diedgestats
+
+
 _dispatch_data = {
     "node": {
         "module": nodestats,
         "statclass": NodeStat,
         "multistatclass": MultiNodeStat,
     },
+    "dinode": {
+        "module": dinodestats,
+        "statclass": DiNodeStat,
+        "multistatclass": MultiDiNodeStat,
+    },
     "edge": {
         "module": edgestats,
         "statclass": EdgeStat,
         "multistatclass": MultiEdgeStat,
     },
+    "diedge": {
+        "module": diedgestats,
+        "statclass": DiEdgeStat,
+        "multistatclass": MultiDiEdgeStat,
+    },
 }
 
 
 def dispatch_stat(kind, net, view, name):
     try:
         func = getattr(_dispatch_data[kind]["module"], name)
     except AttributeError as e:
@@ -529,14 +590,74 @@
     ...     return {n: 10 * net.degree(n) for n in bunch}
 
     """
     setattr(nodestats, func.__name__, func)
     return func
 
 
+def dinodestat_func(func):
+    """Decorator that allows arbitrary functions to behave like :class:`DiNodeStat` objects.
+
+    Works identically to :func:`nodestat`.  For extended documentation, see
+    :func:`nodestat_func`.
+
+    Parameters
+    ----------
+    func : callable
+        Function or callable with signature `func(net, bunch)`, where `net` is the
+        network and `bunch` is an iterable of edges in `net`.  The call `func(net,
+        bunch)` must return a dict with pairs of the form `(edge: value)` where `edge`
+        is in `bunch` and `value` is the value of the statistic at `edge`.
+
+    Returns
+    -------
+    callable
+        The decorated callable unmodified, after registering it in the `stats` framework.
+
+    See Also
+    --------
+    :func:`nodestat_func`
+    :func:`edgestat_func`
+    :func:`diedgestat_func`
+
+    """
+    setattr(dinodestats, func.__name__, func)
+    return func
+
+
+def edgestat_func(func):
+    """Decorator that allows arbitrary functions to behave like :class:`EdgeStat` objects.
+
+    Works identically to :func:`nodestat`.  For extended documentation, see
+    :func:`nodestat_func`.
+
+    Parameters
+    ----------
+    func : callable
+        Function or callable with signature `func(net, bunch)`, where `net` is the
+        network and `bunch` is an iterable of edges in `net`.  The call `func(net,
+        bunch)` must return a dict with pairs of the form `(edge: value)` where `edge`
+        is in `bunch` and `value` is the value of the statistic at `edge`.
+
+    Returns
+    -------
+    callable
+        The decorated callable unmodified, after registering it in the `stats` framework.
+
+    See Also
+    --------
+    :func:`nodestat_func`
+    :func:`edgestat_func`
+    :func:`diedgestat_func`
+
+    """
+    setattr(dinodestats, func.__name__, func)
+    return func
+
+
 def edgestat_func(func):
     """Decorate arbitrary functions to behave like :class:`EdgeStat` objects.
 
     Works identically to :func:`nodestat`.  For extended documentation, see
     :func:`nodestat_func`.
 
     Parameters
@@ -556,7 +677,37 @@
     See Also
     --------
     :func:`nodestat_func`
 
     """
     setattr(edgestats, func.__name__, func)
     return func
+
+
+def diedgestat_func(func):
+    """Decorator that allows arbitrary functions to behave like :class:`DiEdgeStat` objects.
+
+    Works identically to :func:`nodestat`.  For extended documentation, see
+    :func:`nodestat_func`.
+
+    Parameters
+    ----------
+    func : callable
+        Function or callable with signature `func(net, bunch)`, where `net` is the
+        network and `bunch` is an iterable of edges in `net`.  The call `func(net,
+        bunch)` must return a dict with pairs of the form `(edge: value)` where `edge`
+        is in `bunch` and `value` is the value of the statistic at `edge`.
+
+    Returns
+    -------
+    callable
+        The decorated callable unmodified, after registering it in the `stats` framework.
+
+    See Also
+    --------
+    :func:`nodestat_func`
+    :func:`dinodestat_func`
+    :func:`diedgestat_func`
+
+    """
+    setattr(diedgestats, func.__name__, func)
+    return func
```

### Comparing `xgi-0.6/xgi/stats/edgestats.py` & `xgi-0.7/xgi/stats/edgestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi/stats/nodestats.py` & `xgi-0.7/xgi/stats/nodestats.py`

 * *Files identical despite different names*

### Comparing `xgi-0.6/xgi.egg-info/PKG-INFO` & `xgi-0.7/xgi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgi
-Version: 0.6
+Version: 0.7
 Summary: XGI is a Python library for the representation
 Author: Nicholas Landry, Leo Torres, Maxime Lucas, Iacopo Iacopini, Giovanni Petri, Alice Patania, and Alice Schwarze
 Author-email: nicholas.landry@uvm.edu
 Project-URL: Documentation, https://xgi.readthedocs.io/en/latest/
 Project-URL: Bug Reports, https://github.com/xgi-org/xgi/issues
 Project-URL: Source, https://github.com/xgi-org/xgi
 Project-URL: PyPI, https://pypi.org/project/xgi/
```

### Comparing `xgi-0.6/xgi.egg-info/SOURCES.txt` & `xgi-0.7/xgi.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,31 +21,42 @@
 tutorials/Tutorial 1 - Basic Hypergraph Functionality.ipynb
 tutorials/Tutorial 2 - Read and Write.ipynb
 tutorials/Tutorial 3 - Basic simplicial complex usage.ipynb
 tutorials/Tutorial 4 - Generative_Models.ipynb
 tutorials/Tutorial 5 - Plotting.ipynb
 tutorials/Tutorial 6 - Statistics.ipynb
 tutorials/Tutorial 7 - Convex hulls hypergraph plotting.ipynb
+tutorials/Tutorial 8 - Directed Hypergraphs.ipynb
 tutorials/case_study_zhang2022.ipynb
 tutorials/quickstart.ipynb
 tutorials/simplicial_kuramoto_example.ipynb
+tutorials/.ipynb_checkpoints/Tutorial 1 - Basic Hypergraph Functionality-checkpoint.ipynb
+tutorials/.ipynb_checkpoints/Tutorial 2 - Read and Write-checkpoint.ipynb
+tutorials/.ipynb_checkpoints/Tutorial 3 - Basic simplicial complex usage-checkpoint.ipynb
+tutorials/.ipynb_checkpoints/Tutorial 4 - Generative_Models-checkpoint.ipynb
+tutorials/.ipynb_checkpoints/Tutorial 5 - Plotting-checkpoint.ipynb
+tutorials/.ipynb_checkpoints/Tutorial 6 - Statistics-checkpoint.ipynb
+tutorials/.ipynb_checkpoints/quickstart-checkpoint.ipynb
 xgi/__init__.py
 xgi/convert.py
 xgi/exception.py
 xgi.egg-info/PKG-INFO
 xgi.egg-info/SOURCES.txt
 xgi.egg-info/dependency_links.txt
 xgi.egg-info/requires.txt
 xgi.egg-info/top_level.txt
 xgi/algorithms/__init__.py
 xgi/algorithms/assortativity.py
 xgi/algorithms/centrality.py
 xgi/algorithms/clustering.py
 xgi/algorithms/connected.py
+xgi/algorithms/shortest_path.py
 xgi/classes/__init__.py
+xgi/classes/dihypergraph.py
+xgi/classes/direportviews.py
 xgi/classes/function.py
 xgi/classes/hypergraph.py
 xgi/classes/hypergraphviews.py
 xgi/classes/reportviews.py
 xgi/classes/simplicialcomplex.py
 xgi/drawing/__init__.py
 xgi/drawing/draw.py
@@ -60,17 +71,20 @@
 xgi/generators/simplicial_complexes.py
 xgi/generators/uniform.py
 xgi/linalg/__init__.py
 xgi/linalg/hodge_matrix.py
 xgi/linalg/hypergraph_matrix.py
 xgi/linalg/laplacian_matrix.py
 xgi/readwrite/__init__.py
+xgi/readwrite/bigg_data.py
 xgi/readwrite/bipartite.py
 xgi/readwrite/edgelist.py
 xgi/readwrite/incidence.py
 xgi/readwrite/json.py
 xgi/readwrite/xgi_data.py
 xgi/stats/__init__.py
+xgi/stats/diedgestats.py
+xgi/stats/dinodestats.py
 xgi/stats/edgestats.py
 xgi/stats/nodestats.py
 xgi/utils/__init__.py
 xgi/utils/utilities.py
```

### Comparing `xgi-0.6/xgi.egg-info/requires.txt` & `xgi-0.7/xgi.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 scipy>=1.8
 pandas>=1.3
 networkx>=2.7
 requests>=2.0
 matplotlib>=3.4
 
 [all]
+pytest-cov>=4.0
+github-changelog
 pytest>=7.2
-asv>=0.5
-matplotlib>=3.3
-isort==5.10.1
+pillow>=8.2
 black[jupyter]==22.3.0
-jupyter>=1.0
+sphinx-rtd-theme>=1.2
+asv>=0.5
 hypernetx>=1.0
-twine>=3.4
-sphinx~=6.0
-pytest-cov>=4.0
+ipython<=8.12.0
+numpydoc>=1.1
+pylint>=2.10
 seaborn>=0.10
-pillow>=8.2
+matplotlib>=3.3
+sphinx~=6.0
+twine>=3.4
 pre-commit>=2.12
-pylint>=2.10
-github-changelog
-sphinx-rtd-theme>=1.2
 sphinx_copybutton
-numpydoc>=1.1
-ipython<=8.12.0
+isort==5.10.1
+jupyter>=1.0
 wheel>=0.36
 
 [benchmarks]
 hypernetx>=1.0
 asv>=0.5
 
 [developer]
```

