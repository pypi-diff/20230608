# Comparing `tmp/miplearn-0.3.0.dev0.tar.gz` & `tmp/miplearn-0.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miplearn-0.3.0.dev0.tar", last modified: Fri Mar 17 13:52:55 2023, max compression
+gzip compressed data, was "miplearn-0.3.0.dev1.tar", last modified: Wed Jun  7 15:09:31 2023, max compression
```

## Comparing `miplearn-0.3.0.dev0.tar` & `miplearn-0.3.0.dev1.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.705338 miplearn-0.3.0.dev0/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      311 2023-03-17 13:52:55.705338 miplearn-0.3.0.dev0/PKG-INFO
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.609338 miplearn-0.3.0.dev0/benchmark/
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.617338 miplearn-0.3.0.dev0/benchmark/src/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     9175 2023-03-09 17:51:38.000000 miplearn-0.3.0.dev0/benchmark/src/benchmark.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1291 2023-03-09 16:23:59.000000 miplearn-0.3.0.dev0/benchmark/src/collect.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)    12567 2023-03-09 16:33:52.000000 miplearn-0.3.0.dev0/benchmark/src/config.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      760 2022-10-26 15:57:37.000000 miplearn-0.3.0.dev0/benchmark/src/generate.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     8695 2022-10-05 14:42:10.000000 miplearn-0.3.0.dev0/benchmark/src/tmp.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.621338 miplearn-0.3.0.dev0/docs/
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.609338 miplearn-0.3.0.dev0/docs/_build/
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.609338 miplearn-0.3.0.dev0/docs/_build/dirhtml/
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.621338 miplearn-0.3.0.dev0/docs/_build/dirhtml/_static/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2023-01-03 16:17:38.000000 miplearn-0.3.0.dev0/docs/_build/dirhtml/_static/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      637 2023-03-08 18:28:13.000000 miplearn-0.3.0.dev0/docs/conf.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.625338 miplearn-0.3.0.dev0/miplearn/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2023-03-08 18:28:13.000000 miplearn-0.3.0.dev0/miplearn/__init__.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.629338 miplearn-0.3.0.dev0/miplearn/classifiers/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-07 17:15:14.000000 miplearn-0.3.0.dev0/miplearn/classifiers/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2274 2022-10-26 13:53:44.000000 miplearn-0.3.0.dev0/miplearn/classifiers/minprob.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1849 2023-01-19 17:50:00.000000 miplearn-0.3.0.dev0/miplearn/classifiers/singleclass.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.633338 miplearn-0.3.0.dev0/miplearn/collectors/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2023-03-09 15:17:18.000000 miplearn-0.3.0.dev0/miplearn/collectors/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2897 2023-03-09 17:37:04.000000 miplearn-0.3.0.dev0/miplearn/collectors/basic.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     4718 2022-10-05 14:38:42.000000 miplearn-0.3.0.dev0/miplearn/collectors/lazy.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1616 2022-10-05 14:38:42.000000 miplearn-0.3.0.dev0/miplearn/collectors/priority.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.637338 miplearn-0.3.0.dev0/miplearn/components/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-08-11 15:29:56.000000 miplearn-0.3.0.dev0/miplearn/components/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1629 2022-10-05 14:38:42.000000 miplearn-0.3.0.dev0/miplearn/components/lazy.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.645338 miplearn-0.3.0.dev0/miplearn/components/primal/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1097 2022-10-26 13:57:16.000000 miplearn-0.3.0.dev0/miplearn/components/primal/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2712 2023-03-09 17:42:30.000000 miplearn-0.3.0.dev0/miplearn/components/primal/actions.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1040 2022-10-26 15:33:29.000000 miplearn-0.3.0.dev0/miplearn/components/primal/expert.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     4870 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/miplearn/components/primal/indep.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     3293 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/miplearn/components/primal/joint.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     5997 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/miplearn/components/primal/mem.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1087 2022-10-05 14:38:42.000000 miplearn-0.3.0.dev0/miplearn/components/priority.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.653338 miplearn-0.3.0.dev0/miplearn/extractors/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     7485 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/miplearn/extractors/AlvLouWeh2017.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2022-10-06 16:50:02.000000 miplearn-0.3.0.dev0/miplearn/extractors/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      403 2023-01-03 16:16:47.000000 miplearn-0.3.0.dev0/miplearn/extractors/abstract.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      930 2023-01-11 16:15:25.000000 miplearn-0.3.0.dev0/miplearn/extractors/dummy.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2490 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/miplearn/extractors/fields.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     4409 2022-08-11 15:29:55.000000 miplearn-0.3.0.dev0/miplearn/h5.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2187 2023-03-09 17:38:40.000000 miplearn-0.3.0.dev0/miplearn/io.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1214 2022-10-25 15:53:33.000000 miplearn-0.3.0.dev0/miplearn/parallel.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.665338 miplearn-0.3.0.dev0/miplearn/problems/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-08-11 15:29:56.000000 miplearn-0.3.0.dev0/miplearn/problems/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     4498 2023-01-03 16:16:47.000000 miplearn-0.3.0.dev0/miplearn/problems/binpack.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     7405 2023-01-03 16:16:47.000000 miplearn-0.3.0.dev0/miplearn/problems/multiknapsack.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     6409 2023-01-03 16:16:47.000000 miplearn-0.3.0.dev0/miplearn/problems/pmedian.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     3995 2023-03-08 21:33:12.000000 miplearn-0.3.0.dev0/miplearn/problems/setcover.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1932 2022-10-26 15:33:29.000000 miplearn-0.3.0.dev0/miplearn/problems/setpack.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     3958 2023-03-08 19:23:31.000000 miplearn-0.3.0.dev0/miplearn/problems/stab.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     6295 2022-10-26 15:33:29.000000 miplearn-0.3.0.dev0/miplearn/problems/tsp.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     6946 2023-01-09 17:48:38.000000 miplearn-0.3.0.dev0/miplearn/problems/uc.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1618 2023-01-10 16:14:35.000000 miplearn-0.3.0.dev0/miplearn/problems/vertexcover.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.673338 miplearn-0.3.0.dev0/miplearn/solvers/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-26 15:33:09.000000 miplearn-0.3.0.dev0/miplearn/solvers/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1639 2023-03-09 16:26:09.000000 miplearn-0.3.0.dev0/miplearn/solvers/abstract.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)    10876 2023-03-09 17:48:21.000000 miplearn-0.3.0.dev0/miplearn/solvers/gurobi.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1377 2023-01-19 20:05:46.000000 miplearn-0.3.0.dev0/miplearn/solvers/learning.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)    14026 2023-03-09 22:04:45.000000 miplearn-0.3.0.dev0/miplearn/solvers/pyomo.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.625338 miplearn-0.3.0.dev0/miplearn.egg-info/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      311 2023-03-17 13:52:55.000000 miplearn-0.3.0.dev0/miplearn.egg-info/PKG-INFO
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2196 2023-03-17 13:52:55.000000 miplearn-0.3.0.dev0/miplearn.egg-info/SOURCES.txt
--rw-rw-r--   0 axavier   (1000) axavier   (1000)        1 2023-03-17 13:52:55.000000 miplearn-0.3.0.dev0/miplearn.egg-info/dependency_links.txt
--rw-rw-r--   0 axavier   (1000) axavier   (1000)       30 2023-03-17 13:52:55.000000 miplearn-0.3.0.dev0/miplearn.egg-info/top_level.txt
--rw-rw-r--   0 axavier   (1000) axavier   (1000)       38 2023-03-17 13:52:55.705338 miplearn-0.3.0.dev0/setup.cfg
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      621 2023-03-17 13:52:52.000000 miplearn-0.3.0.dev0/setup.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.677338 miplearn-0.3.0.dev0/tests/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-05 15:34:16.000000 miplearn-0.3.0.dev0/tests/__init__.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.681338 miplearn-0.3.0.dev0/tests/components/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-05 15:15:44.000000 miplearn-0.3.0.dev0/tests/components/__init__.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.685338 miplearn-0.3.0.dev0/tests/components/primal/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2022-10-05 15:15:42.000000 miplearn-0.3.0.dev0/tests/components/primal/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1096 2022-10-26 14:25:56.000000 miplearn-0.3.0.dev0/tests/components/primal/test_expert.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1857 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/tests/components/primal/test_indep.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1545 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/tests/components/primal/test_joint.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2595 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/tests/components/primal/test_mem.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      764 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/tests/conftest.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.689338 miplearn-0.3.0.dev0/tests/extractors/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-06 16:50:51.000000 miplearn-0.3.0.dev0/tests/extractors/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      691 2023-01-11 16:15:33.000000 miplearn-0.3.0.dev0/tests/extractors/test_dummy.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1076 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev0/tests/extractors/test_fields.py
-drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-03-17 13:52:55.705338 miplearn-0.3.0.dev0/tests/problems/
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-08-11 15:30:47.000000 miplearn-0.3.0.dev0/tests/problems/__init__.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1429 2022-10-26 15:16:18.000000 miplearn-0.3.0.dev0/tests/problems/test_binpack.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2057 2022-10-26 15:16:14.000000 miplearn-0.3.0.dev0/tests/problems/test_multiknapsack.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1965 2022-10-26 15:16:07.000000 miplearn-0.3.0.dev0/tests/problems/test_pmedian.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2798 2023-03-08 18:56:50.000000 miplearn-0.3.0.dev0/tests/problems/test_setcover.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      712 2022-10-26 15:15:54.000000 miplearn-0.3.0.dev0/tests/problems/test_setpack.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      963 2023-03-08 18:38:55.000000 miplearn-0.3.0.dev0/tests/problems/test_stab.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     1781 2022-10-26 15:15:29.000000 miplearn-0.3.0.dev0/tests/problems/test_tsp.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2670 2022-10-26 15:14:23.000000 miplearn-0.3.0.dev0/tests/problems/test_uc.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)      636 2023-01-10 16:14:35.000000 miplearn-0.3.0.dev0/tests/problems/test_vertexcover.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     2087 2022-08-11 15:30:47.000000 miplearn-0.3.0.dev0/tests/test_h5.py
--rw-rw-r--   0 axavier   (1000) axavier   (1000)     7081 2023-03-09 22:10:00.000000 miplearn-0.3.0.dev0/tests/test_solvers.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      286 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/PKG-INFO
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.076178 miplearn-0.3.0.dev1/benchmark/
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/benchmark/src/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     9177 2023-03-21 17:22:47.000000 miplearn-0.3.0.dev1/benchmark/src/benchmark.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1291 2023-03-09 16:23:59.000000 miplearn-0.3.0.dev1/benchmark/src/collect.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)    12567 2023-03-09 16:33:52.000000 miplearn-0.3.0.dev1/benchmark/src/config.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      776 2023-03-21 17:23:42.000000 miplearn-0.3.0.dev1/benchmark/src/generate.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     8695 2022-10-05 14:42:10.000000 miplearn-0.3.0.dev1/benchmark/src/tmp.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/docs/
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.076178 miplearn-0.3.0.dev1/docs/_build/
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.076178 miplearn-0.3.0.dev1/docs/_build/dirhtml/
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/docs/_build/dirhtml/_static/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2023-01-03 16:17:38.000000 miplearn-0.3.0.dev1/docs/_build/dirhtml/_static/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      637 2023-03-08 18:28:13.000000 miplearn-0.3.0.dev1/docs/conf.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/miplearn/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2023-03-08 18:28:13.000000 miplearn-0.3.0.dev1/miplearn/__init__.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/miplearn/classifiers/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-07 17:15:14.000000 miplearn-0.3.0.dev1/miplearn/classifiers/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2274 2022-10-26 13:53:44.000000 miplearn-0.3.0.dev1/miplearn/classifiers/minprob.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1849 2023-01-19 17:50:00.000000 miplearn-0.3.0.dev1/miplearn/classifiers/singleclass.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/miplearn/collectors/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2023-03-09 15:17:18.000000 miplearn-0.3.0.dev1/miplearn/collectors/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2881 2023-03-22 16:24:34.000000 miplearn-0.3.0.dev1/miplearn/collectors/basic.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     4728 2023-03-21 17:22:44.000000 miplearn-0.3.0.dev1/miplearn/collectors/lazy.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1634 2023-03-21 17:09:22.000000 miplearn-0.3.0.dev1/miplearn/collectors/priority.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.084178 miplearn-0.3.0.dev1/miplearn/components/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-08-11 15:29:56.000000 miplearn-0.3.0.dev1/miplearn/components/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1629 2022-10-05 14:38:42.000000 miplearn-0.3.0.dev1/miplearn/components/lazy.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.084178 miplearn-0.3.0.dev1/miplearn/components/primal/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1097 2022-10-26 13:57:16.000000 miplearn-0.3.0.dev1/miplearn/components/primal/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2664 2023-03-22 20:05:15.000000 miplearn-0.3.0.dev1/miplearn/components/primal/actions.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1040 2022-10-26 15:33:29.000000 miplearn-0.3.0.dev1/miplearn/components/primal/expert.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     4870 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/miplearn/components/primal/indep.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     3293 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/miplearn/components/primal/joint.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     5997 2023-03-22 19:51:55.000000 miplearn-0.3.0.dev1/miplearn/components/primal/mem.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1087 2022-10-05 14:38:42.000000 miplearn-0.3.0.dev1/miplearn/components/priority.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.088178 miplearn-0.3.0.dev1/miplearn/extractors/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     7485 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/miplearn/extractors/AlvLouWeh2017.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2022-10-06 16:50:02.000000 miplearn-0.3.0.dev1/miplearn/extractors/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      403 2023-01-03 16:16:47.000000 miplearn-0.3.0.dev1/miplearn/extractors/abstract.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      930 2023-01-11 16:15:25.000000 miplearn-0.3.0.dev1/miplearn/extractors/dummy.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2490 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/miplearn/extractors/fields.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     4457 2023-03-17 14:47:20.000000 miplearn-0.3.0.dev1/miplearn/h5.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2511 2023-03-22 16:23:48.000000 miplearn-0.3.0.dev1/miplearn/io.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1214 2022-10-25 15:53:33.000000 miplearn-0.3.0.dev1/miplearn/parallel.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.088178 miplearn-0.3.0.dev1/miplearn/problems/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-08-11 15:29:56.000000 miplearn-0.3.0.dev1/miplearn/problems/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     4658 2023-03-21 17:12:00.000000 miplearn-0.3.0.dev1/miplearn/problems/binpack.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     7571 2023-03-21 17:13:01.000000 miplearn-0.3.0.dev1/miplearn/problems/multiknapsack.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     6569 2023-03-21 17:12:55.000000 miplearn-0.3.0.dev1/miplearn/problems/pmedian.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     4332 2023-03-21 17:14:40.000000 miplearn-0.3.0.dev1/miplearn/problems/setcover.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2084 2023-03-21 17:15:03.000000 miplearn-0.3.0.dev1/miplearn/problems/setpack.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     4289 2023-03-21 17:15:49.000000 miplearn-0.3.0.dev1/miplearn/problems/stab.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     6465 2023-03-21 17:16:18.000000 miplearn-0.3.0.dev1/miplearn/problems/tsp.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     7113 2023-03-21 17:17:12.000000 miplearn-0.3.0.dev1/miplearn/problems/uc.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1783 2023-03-21 17:17:12.000000 miplearn-0.3.0.dev1/miplearn/problems/vertexcover.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.088178 miplearn-0.3.0.dev1/miplearn/solvers/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-26 15:33:09.000000 miplearn-0.3.0.dev1/miplearn/solvers/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1639 2023-03-09 16:26:09.000000 miplearn-0.3.0.dev1/miplearn/solvers/abstract.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)    10991 2023-03-17 18:49:55.000000 miplearn-0.3.0.dev1/miplearn/solvers/gurobi.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1600 2023-03-22 20:33:04.000000 miplearn-0.3.0.dev1/miplearn/solvers/learning.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)    14243 2023-03-22 20:38:17.000000 miplearn-0.3.0.dev1/miplearn/solvers/pyomo.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.080178 miplearn-0.3.0.dev1/miplearn.egg-info/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      286 2023-06-07 15:09:31.000000 miplearn-0.3.0.dev1/miplearn.egg-info/PKG-INFO
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2227 2023-06-07 15:09:31.000000 miplearn-0.3.0.dev1/miplearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)        1 2023-06-07 15:09:31.000000 miplearn-0.3.0.dev1/miplearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      326 2023-06-07 15:09:31.000000 miplearn-0.3.0.dev1/miplearn.egg-info/requires.txt
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)       41 2023-06-07 15:09:31.000000 miplearn-0.3.0.dev1/miplearn.egg-info/top_level.txt
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)       38 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/setup.cfg
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1282 2023-06-07 15:08:54.000000 miplearn-0.3.0.dev1/setup.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/tests/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-05 15:34:16.000000 miplearn-0.3.0.dev1/tests/__init__.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/tests/components/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-05 15:15:44.000000 miplearn-0.3.0.dev1/tests/components/__init__.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/tests/components/primal/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)        0 2022-10-05 15:15:42.000000 miplearn-0.3.0.dev1/tests/components/primal/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1096 2022-10-26 14:25:56.000000 miplearn-0.3.0.dev1/tests/components/primal/test_expert.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1857 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/tests/components/primal/test_indep.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1545 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/tests/components/primal/test_joint.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2595 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/tests/components/primal/test_mem.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      764 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/tests/conftest.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/tests/extractors/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-10-06 16:50:51.000000 miplearn-0.3.0.dev1/tests/extractors/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      691 2023-01-11 16:15:33.000000 miplearn-0.3.0.dev1/tests/extractors/test_dummy.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1076 2023-01-11 16:10:16.000000 miplearn-0.3.0.dev1/tests/extractors/test_fields.py
+drwxrwxr-x   0 axavier   (1000) axavier   (1000)        0 2023-06-07 15:09:31.092178 miplearn-0.3.0.dev1/tests/problems/
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      232 2022-08-11 15:30:47.000000 miplearn-0.3.0.dev1/tests/problems/__init__.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1429 2022-10-26 15:16:18.000000 miplearn-0.3.0.dev1/tests/problems/test_binpack.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2057 2022-10-26 15:16:14.000000 miplearn-0.3.0.dev1/tests/problems/test_multiknapsack.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1965 2022-10-26 15:16:07.000000 miplearn-0.3.0.dev1/tests/problems/test_pmedian.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2798 2023-03-08 18:56:50.000000 miplearn-0.3.0.dev1/tests/problems/test_setcover.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      712 2022-10-26 15:15:54.000000 miplearn-0.3.0.dev1/tests/problems/test_setpack.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      963 2023-03-08 18:38:55.000000 miplearn-0.3.0.dev1/tests/problems/test_stab.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     1781 2022-10-26 15:15:29.000000 miplearn-0.3.0.dev1/tests/problems/test_tsp.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2670 2022-10-26 15:14:23.000000 miplearn-0.3.0.dev1/tests/problems/test_uc.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)      636 2023-01-10 16:14:35.000000 miplearn-0.3.0.dev1/tests/problems/test_vertexcover.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     2087 2022-08-11 15:30:47.000000 miplearn-0.3.0.dev1/tests/test_h5.py
+-rw-rw-r--   0 axavier   (1000) axavier   (1000)     7031 2023-03-21 16:19:41.000000 miplearn-0.3.0.dev1/tests/test_solvers.py
```

### Comparing `miplearn-0.3.0.dev0/benchmark/src/benchmark.py` & `miplearn-0.3.0.dev1/benchmark/src/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
+import json
 import logging
+import os
+import pickle
 import random
+import re
 import sys
+from contextlib import redirect_stdout
 from distutils.dir_util import mkpath
 from glob import glob
+from io import StringIO
 from os.path import dirname, exists
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from time import time
-import json
-from contextlib import redirect_stdout
-import os
-from io import StringIO
-import re
-import pickle
 
 import pandas as pd
 
+from config import challenges, methods, n_jobs, n_seeds
 from miplearn.h5 import H5File
-from miplearn.io import load, _RedirectOutput
+from miplearn.io import _RedirectOutput
 from miplearn.parallel import p_umap
 
-from config import challenges, methods, n_jobs, timelimit_benchmark, n_seeds
-
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 stdout_handler = logging.StreamHandler(sys.stdout)
 stdout_handler.setLevel(logging.ERROR)
 stdout_handler.setFormatter(logging.Formatter("[%(asctime)s] %(message)s"))
 logger.addHandler(stdout_handler)
 
@@ -57,17 +56,17 @@
         # Set up logger
         file_handler = logging.FileHandler(log_filename, mode="w")
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(logging.Formatter("[%(asctime)s] %(message)s"))
         logger.addHandler(file_handler)
 
         # Fit
-        data = sorted(glob(f"data/{challenge.name}/*.pkl.gz"))
-        h5 = [f.replace(".pkl.gz", ".h5") for f in data]
-        train_h5 = h5[: challenge.n_train]
+        data_filenames = sorted(glob(f"data/{challenge.name}/*.pkl.gz"))
+        h5_filenames = [f"{filename}.h5" for filename in data_filenames]
+        train_h5 = h5_filenames[: challenge.n_train]
         for c in method.components:
             c.fit(train_h5)
 
         # Pickle
         _write_pkl(method, pkl_filename)
 
         # Tear down logger
@@ -128,15 +127,15 @@
         logger.addHandler(file_handler)
 
         try:
             with NamedTemporaryFile() as tempfile:
                 with H5File(tempfile.name) as h5:
                     components = _read_pkl(pkl_filename).components
                     with _RedirectOutput([]):
-                        model = load(data_filename, challenge.build_model)
+                        model = challenge.build_model(data_filename)
                     model.extract_after_load(h5)
                     stats = {}
                     for comp in components:
                         comp.before_mip(h5_filename, model, stats)
                     streams = [StringIO()]
                     with _RedirectOutput(streams):
                         model.optimize()
```

### Comparing `miplearn-0.3.0.dev0/benchmark/src/collect.py` & `miplearn-0.3.0.dev1/benchmark/src/collect.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/benchmark/src/config.py` & `miplearn-0.3.0.dev1/benchmark/src/config.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/benchmark/src/generate.py` & `miplearn-0.3.0.dev1/benchmark/src/generate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from os.path import exists
 
 from config import challenges, n_jobs
-from miplearn.io import save
+from miplearn.io import write_pkl_gz
 
 if __name__ == "__main__":
     for challenge in challenges:
         if exists(f"data/{challenge.name}/"):
             print(f"Skipping data/{challenge.name}")
             continue
         print(f"\n{challenge.name}")
         data = challenge.generator.generate(challenge.n_samples)
-        save(
+        write_pkl_gz(
             data,
             f"data/{challenge.name}/",
             prefix=f"{challenge.name}-",
             n_jobs=n_jobs,
         )
```

### Comparing `miplearn-0.3.0.dev0/benchmark/src/tmp.py` & `miplearn-0.3.0.dev1/benchmark/src/tmp.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/docs/conf.py` & `miplearn-0.3.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/classifiers/minprob.py` & `miplearn-0.3.0.dev1/miplearn/classifiers/minprob.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/classifiers/singleclass.py` & `miplearn-0.3.0.dev1/miplearn/classifiers/singleclass.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/collectors/basic.py` & `miplearn-0.3.0.dev1/miplearn/collectors/basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 import json
 import os
 from io import StringIO
 from os.path import exists
 from typing import Callable, List
-from math import isfinite
 
 from ..h5 import H5File
-from ..io import _RedirectOutput, load, gzip
+from ..io import _RedirectOutput, gzip, _to_h5_filename
 from ..parallel import p_umap
 
 
 class BasicCollector:
     def collect(
         self,
         filenames: List[str],
         build_model: Callable,
         n_jobs: int = 1,
         progress: bool = False,
     ) -> None:
-        def _collect(filename):
-            h5_filename = filename.replace(".pkl.gz", ".h5")
-            mps_filename = filename.replace(".pkl.gz", ".mps")
+        def _collect(data_filename):
+            h5_filename = _to_h5_filename(data_filename)
+            mps_filename = h5_filename.replace(".h5", ".mps")
 
             if exists(h5_filename):
                 # Try to read optimal solution
                 mip_var_values = None
                 try:
                     with H5File(h5_filename, "r") as h5:
                         mip_var_values = h5.get_array("mip_var_values")
@@ -41,15 +40,15 @@
                 else:
                     return
 
             with H5File(h5_filename, "w") as h5:
                 streams = [StringIO()]
                 with _RedirectOutput(streams):
                     # Load and extract static features
-                    model = load(filename, build_model)
+                    model = build_model(data_filename)
                     model.extract_after_load(h5)
 
                     # Solve LP relaxation
                     relaxed = model.relax()
                     relaxed.optimize()
                     relaxed.extract_after_lp(h5)
```

### Comparing `miplearn-0.3.0.dev0/miplearn/collectors/lazy.py` & `miplearn-0.3.0.dev1/miplearn/collectors/lazy.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from io import StringIO
 from typing import Callable
 
 import gurobipy as gp
+import numpy as np
 from gurobipy import GRB, LinExpr
 
 from ..h5 import H5File
-from ..io import _RedirectOutput, load
-
-import numpy as np
+from ..io import _RedirectOutput
 
 
 class LazyCollector:
     def __init__(
         self,
         min_constrs: int = 100_000,
         time_limit: float = 900,
     ) -> None:
         self.min_constrs = min_constrs
         self.time_limit = time_limit
 
-    def collect(self, data: str, build_model: Callable, tol: float = 1e-6) -> None:
-        h5_filename = data.replace(".pkl.gz", ".h5")
+    def collect(
+        self, data_filename: str, build_model: Callable, tol: float = 1e-6
+    ) -> None:
+        h5_filename = f"{data_filename}.h5"
         with H5File(h5_filename, "r+") as h5:
             streams = [StringIO()]
             lazy = None
             with _RedirectOutput(streams):
                 slacks = h5.get_array("mip_constr_slacks")
                 assert slacks is not None
 
@@ -36,15 +37,15 @@
                 if len(slacks) < self.min_constrs:
                     print("Problem is too small. Skipping.")
                     h5.put_array("mip_constr_lazy", np.zeros(len(slacks)))
                     return
 
                 # Load model
                 print("Loading model...")
-                model = load(data, build_model)
+                model = build_model(data_filename)
                 model.params.LazyConstraints = True
                 model.params.timeLimit = self.time_limit
                 gp_constrs = np.array(model.getConstrs())
                 gp_vars = np.array(model.getVars())
 
                 # Load constraints
                 lhs = h5.get_sparse("static_constr_lhs")
```

### Comparing `miplearn-0.3.0.dev0/miplearn/collectors/priority.py` & `miplearn-0.3.0.dev1/miplearn/collectors/priority.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         print_interval: int = 1,
         node_limit: int = 500,
     ) -> None:
         self.time_limit = time_limit
         self.print_interval = print_interval
         self.node_limit = node_limit
 
-    def collect(self, data: str, _: Callable) -> None:
-        basename = data.replace(".pkl.gz", "")
+    def collect(self, data_filename: str, _: Callable) -> None:
+        basename = data_filename.replace(".pkl.gz", "")
         env = os.environ.copy()
         env["JULIA_NUM_THREADS"] = "1"
         ret = subprocess.run(
             [
                 "julia",
                 "--project=.",
                 "-e",
```

### Comparing `miplearn-0.3.0.dev0/miplearn/components/lazy.py` & `miplearn-0.3.0.dev1/miplearn/components/lazy.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/components/primal/__init__.py` & `miplearn-0.3.0.dev1/miplearn/components/primal/__init__.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/components/primal/actions.py` & `miplearn-0.3.0.dev1/miplearn/components/primal/actions.py`

 * *Files 22% similar despite different names*

```diff
@@ -80,14 +80,14 @@
 
         constr_rhs += len(constr_vars) * self.tol
         logger.info(
             f"Adding proximity constraint (tol={self.tol}, nz={len(constr_vars)})..."
         )
 
         model.add_constrs(
-            var_names=np.array(constr_vars),
-            constrs_lhs=np.array([constr_lhs]),
-            constrs_sense=np.array(["<"], dtype="S"),
-            constrs_rhs=np.array([constr_rhs]),
+            np.array(constr_vars),
+            np.array([constr_lhs]),
+            np.array(["<"], dtype="S"),
+            np.array([constr_rhs]),
         )
         if stats is not None:
             stats["Heuristic"] = True
```

### Comparing `miplearn-0.3.0.dev0/miplearn/components/primal/expert.py` & `miplearn-0.3.0.dev1/miplearn/components/primal/expert.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/components/primal/indep.py` & `miplearn-0.3.0.dev1/miplearn/components/primal/indep.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/components/primal/joint.py` & `miplearn-0.3.0.dev1/miplearn/components/primal/joint.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/components/primal/mem.py` & `miplearn-0.3.0.dev1/miplearn/components/primal/mem.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/components/priority.py` & `miplearn-0.3.0.dev1/miplearn/components/priority.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/extractors/AlvLouWeh2017.py` & `miplearn-0.3.0.dev1/miplearn/extractors/AlvLouWeh2017.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/extractors/dummy.py` & `miplearn-0.3.0.dev1/miplearn/extractors/dummy.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/extractors/fields.py` & `miplearn-0.3.0.dev1/miplearn/extractors/fields.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/h5.py` & `miplearn-0.3.0.dev1/miplearn/h5.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 
     def put_bytes(self, key: str, value: Bytes) -> None:
         assert isinstance(
             value, (bytes, bytearray)
         ), f"bytes expected; found: {value.__class__}"  # type: ignore
         self.put_array(key, np.frombuffer(value, dtype="uint8"))
 
+    def close(self):
+        self.file.close()
+
     def __enter__(self) -> "H5File":
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
```

### Comparing `miplearn-0.3.0.dev0/miplearn/io.py` & `miplearn-0.3.0.dev1/miplearn/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         _value: Any,
         _traceback: Any,
     ) -> None:
         sys.stdout = self._original_stdout
         sys.stderr = self._original_stderr
 
 
-def save(
+def write_pkl_gz(
     objs: List[Any],
     dirname: str,
     prefix: str = "",
     n_jobs: int = 1,
     progress: bool = False,
 ) -> List[str]:
     filenames = [f"{dirname}/{prefix}{i:05d}.pkl.gz" for i in range(len(objs))]
@@ -53,29 +53,40 @@
     def _process(i: int) -> None:
         filename = filenames[i]
         obj = objs[i]
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         with GzipFile(filename, "wb") as file:
             pickle.dump(obj, cast(IO[bytes], file))
 
-    p_umap(
-        _process,
-        range(len(objs)),
-        smoothing=0,
-        num_cpus=n_jobs,
-        maxtasksperchild=None,
-        disable=not progress,
-    )
+    if n_jobs > 1:
+        p_umap(
+            _process,
+            range(len(objs)),
+            smoothing=0,
+            num_cpus=n_jobs,
+            maxtasksperchild=None,
+            disable=not progress,
+        )
+    else:
+        for i in range(len(objs)):
+            _process(i)
     return filenames
 
 
-def load(filename: str, build_model: Callable) -> Any:
-    with GzipFile(filename, "rb") as file:
-        data = pickle.load(cast(IO[bytes], file))
-        return build_model(data)
-
-
 def gzip(filename: str) -> None:
     with open(filename, "rb") as input_file:
         with GzipFile(f"{filename}.gz", "wb") as output_file:
             shutil.copyfileobj(input_file, output_file)
     os.remove(filename)
+
+
+def read_pkl_gz(filename: str) -> Any:
+    with GzipFile(filename, "rb") as file:
+        return pickle.load(cast(IO[bytes], file))
+
+
+def _to_h5_filename(data_filename: str) -> str:
+    output = f"{data_filename}.h5"
+    output = output.replace(".pkl.gz.h5", ".h5")
+    output = output.replace(".pkl.h5", ".h5")
+    output = output.replace(".jld2.h5", ".h5")
+    return output
```

### Comparing `miplearn-0.3.0.dev0/miplearn/parallel.py` & `miplearn-0.3.0.dev1/miplearn/parallel.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/binpack.py` & `miplearn-0.3.0.dev1/miplearn/problems/binpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import gurobipy as gp
 import numpy as np
 from gurobipy import GRB, quicksum
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 
 
 @dataclass
 class BinPackData:
     """Data for the bin packing problem.
 
@@ -104,16 +105,20 @@
             sizes = sizes * self.sizes_jitter.rvs(n)
             capacity = capacity * self.capacity_jitter.rvs()
             return BinPackData(sizes.round(2), capacity.round(2))
 
         return [_sample() for n in range(n_samples)]
 
 
-def build_binpack_model(data: BinPackData) -> GurobiModel:
+def build_binpack_model(data: Union[str, BinPackData]) -> GurobiModel:
     """Converts bin packing problem data into a concrete Gurobipy model."""
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, BinPackData)
+
     model = gp.Model()
     n = data.sizes.shape[0]
 
     # Var: Use bin
     y = model.addVars(n, name="y", vtype=GRB.BINARY)
 
     # Var: Assign item to bin
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/multiknapsack.py` & `miplearn-0.3.0.dev1/miplearn/problems/multiknapsack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import gurobipy as gp
 import numpy as np
 from gurobipy import GRB
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 
 
 @dataclass
 class MultiKnapsackData:
     """Data for the multi-dimensional knapsack problem
 
@@ -169,16 +170,20 @@
                 b = b.round()
                 w = w.round()
             return MultiKnapsackData(p, b, w)
 
         return [_sample() for _ in range(n_samples)]
 
 
-def build_multiknapsack_model(data: MultiKnapsackData) -> GurobiModel:
+def build_multiknapsack_model(data: Union[str, MultiKnapsackData]) -> GurobiModel:
     """Converts multi-knapsack problem data into a concrete Gurobipy model."""
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, MultiKnapsackData)
+
     model = gp.Model()
     m, n = data.weights.shape
     x = model.addMVar(n, vtype=GRB.BINARY, name="x")
     model.addConstr(data.weights @ x <= data.capacities)
     model.setObjective(-data.prices @ x)
     model.update()
     return GurobiModel(model)
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/pmedian.py` & `miplearn-0.3.0.dev1/miplearn/problems/pmedian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import gurobipy as gp
 import numpy as np
 from gurobipy import quicksum, GRB
 from scipy.spatial.distance import pdist, squareform
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 
 
 @dataclass
 class PMedianData:
     """Data for the capacitated p-median problem
 
@@ -136,16 +137,20 @@
                 self.ref_data = data
 
             return data
 
         return [_sample() for _ in range(n_samples)]
 
 
-def build_pmedian_model(data: PMedianData) -> GurobiModel:
+def build_pmedian_model(data: Union[str, PMedianData]) -> GurobiModel:
     """Converts capacitated p-median data into a concrete Gurobipy model."""
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, PMedianData)
+
     model = gp.Model()
     n = len(data.demands)
 
     # Decision variables
     x = model.addVars(n, n, vtype=GRB.BINARY, name="x")
     y = model.addVars(n, vtype=GRB.BINARY, name="y")
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/setcover.py` & `miplearn-0.3.0.dev1/miplearn/problems/setcover.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List
+from typing import List, Union
 
 import gurobipy as gp
 import numpy as np
 import pyomo.environ as pe
 from gurobipy.gurobipy import GRB
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 from miplearn.solvers.pyomo import PyomoModel
 
 
 @dataclass
 class SetCoverData:
     costs: np.ndarray
@@ -77,34 +78,43 @@
                 costs=costs.round(2),
                 incidence_matrix=incidence_matrix,
             )
 
         return [_sample() for _ in range(n_samples)]
 
 
-def build_setcover_model_gurobipy(data: SetCoverData) -> GurobiModel:
+def build_setcover_model_gurobipy(data: Union[str, SetCoverData]) -> GurobiModel:
+    data = _read_setcover_data(data)
     (n_elements, n_sets) = data.incidence_matrix.shape
     model = gp.Model()
     x = model.addMVar(n_sets, vtype=GRB.BINARY, name="x")
     model.addConstr(data.incidence_matrix @ x >= np.ones(n_elements), name="eqs")
     model.setObjective(data.costs @ x)
     model.update()
     return GurobiModel(model)
 
 
 def build_setcover_model_pyomo(
-    data: SetCoverData,
+    data: Union[str, SetCoverData],
     solver="gurobi_persistent",
 ) -> PyomoModel:
+    data = _read_setcover_data(data)
     (n_elements, n_sets) = data.incidence_matrix.shape
     model = pe.ConcreteModel()
     model.sets = pe.Set(initialize=range(n_sets))
     model.x = pe.Var(model.sets, domain=pe.Boolean, name="x")
     model.eqs = pe.Constraint(pe.Any)
     for i in range(n_elements):
         model.eqs[i] = (
             sum(data.incidence_matrix[i, j] * model.x[j] for j in range(n_sets)) >= 1
         )
     model.obj = pe.Objective(
         expr=sum(data.costs[j] * model.x[j] for j in range(n_sets))
     )
     return PyomoModel(model, solver)
+
+
+def _read_setcover_data(data: Union[str, SetCoverData]) -> SetCoverData:
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, SetCoverData)
+    return data
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/setpack.py` & `miplearn-0.3.0.dev1/miplearn/problems/setpack.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List
+from typing import List, Union
 
 import gurobipy as gp
 import numpy as np
 from gurobipy.gurobipy import GRB
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
 from .setcover import SetCoverGenerator
 from miplearn.solvers.gurobi import GurobiModel
+from ..io import read_pkl_gz
 
 
 @dataclass
 class SetPackData:
     costs: np.ndarray
     incidence_matrix: np.ndarray
 
@@ -48,15 +49,18 @@
                 s.costs,
                 s.incidence_matrix,
             )
             for s in self.gen.generate(n_samples)
         ]
 
 
-def build_setpack_model(data: SetPackData) -> GurobiModel:
+def build_setpack_model(data: Union[str, SetPackData]) -> GurobiModel:
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, SetPackData)
     (n_elements, n_sets) = data.incidence_matrix.shape
     model = gp.Model()
     x = model.addMVar(n_sets, vtype=GRB.BINARY, name="x")
     model.addConstr(data.incidence_matrix @ x <= np.ones(n_elements))
     model.setObjective(-data.costs @ x)
     model.update()
     return GurobiModel(model)
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/stab.py` & `miplearn-0.3.0.dev1/miplearn/problems/stab.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List
+from typing import List, Union
 
 import gurobipy as gp
 import networkx as nx
 import numpy as np
 import pyomo.environ as pe
 from gurobipy import GRB, quicksum
 from networkx import Graph
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 from miplearn.solvers.pyomo import PyomoModel
 
 
 @dataclass
 class MaxWeightStableSetData:
     graph: Graph
@@ -78,29 +79,38 @@
         return [_sample() for _ in range(n_samples)]
 
     def _generate_graph(self) -> Graph:
         return nx.generators.random_graphs.binomial_graph(self.n.rvs(), self.p.rvs())
 
 
 def build_stab_model_gurobipy(data: MaxWeightStableSetData) -> GurobiModel:
+    data = _read_stab_data(data)
     model = gp.Model()
     nodes = list(data.graph.nodes)
     x = model.addVars(nodes, vtype=GRB.BINARY, name="x")
     model.setObjective(quicksum(-data.weights[i] * x[i] for i in nodes))
     for clique in nx.find_cliques(data.graph):
         model.addConstr(quicksum(x[i] for i in clique) <= 1)
     model.update()
     return GurobiModel(model)
 
 
 def build_stab_model_pyomo(
     data: MaxWeightStableSetData,
     solver="gurobi_persistent",
 ) -> PyomoModel:
+    data = _read_stab_data(data)
     model = pe.ConcreteModel()
     nodes = pe.Set(initialize=list(data.graph.nodes))
     model.x = pe.Var(nodes, domain=pe.Boolean, name="x")
     model.obj = pe.Objective(expr=sum([-data.weights[i] * model.x[i] for i in nodes]))
     model.clique_eqs = pe.ConstraintList()
     for clique in nx.find_cliques(data.graph):
         model.clique_eqs.add(expr=sum(model.x[i] for i in clique) <= 1)
     return PyomoModel(model, solver)
+
+
+def _read_stab_data(data: Union[str, MaxWeightStableSetData]) -> MaxWeightStableSetData:
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, MaxWeightStableSetData)
+    return data
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/tsp.py` & `miplearn-0.3.0.dev1/miplearn/problems/tsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List, Tuple, Optional, Any
+from typing import List, Tuple, Optional, Any, Union
 
 import gurobipy as gp
 import networkx as nx
 import numpy as np
 from gurobipy import quicksum, GRB, tuplelist
 from scipy.spatial.distance import pdist, squareform
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 import logging
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class TravelingSalesmanData:
@@ -107,15 +108,19 @@
 
     def _generate_cities(self) -> Tuple[int, np.ndarray]:
         n = self.n.rvs()
         cities = np.array([(self.x.rvs(), self.y.rvs()) for _ in range(n)])
         return n, cities
 
 
-def build_tsp_model(data: TravelingSalesmanData) -> GurobiModel:
+def build_tsp_model(data: Union[str, TravelingSalesmanData]) -> GurobiModel:
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, TravelingSalesmanData)
+
     edges = tuplelist(
         (i, j) for i in range(data.n_cities) for j in range(i + 1, data.n_cities)
     )
     model = gp.Model()
 
     # Decision variables
     x = model.addVars(edges, vtype=GRB.BINARY, name="x")
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/uc.py` & `miplearn-0.3.0.dev1/miplearn/problems/uc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
 from math import pi
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import gurobipy as gp
 import numpy as np
 from gurobipy import GRB, quicksum
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
+from miplearn.io import read_pkl_gz
 from miplearn.solvers.gurobi import GurobiModel
 
 
 @dataclass
 class UnitCommitmentData:
     demand: np.ndarray
     min_power: np.ndarray
@@ -107,23 +108,27 @@
                 self.ref_data = data
 
             return data
 
         return [_sample() for _ in range(n_samples)]
 
 
-def build_uc_model(data: UnitCommitmentData) -> GurobiModel:
+def build_uc_model(data: Union[str, UnitCommitmentData]) -> GurobiModel:
     """
     Models the unit commitment problem according to equations (1)-(5) of:
 
         Bendotti, P., Fouilhoux, P. & Rottner, C. The min-up/min-down unit
         commitment polytope. J Comb Optim 36, 1024-1058 (2018).
         https://doi.org/10.1007/s10878-018-0273-y
 
     """
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, UnitCommitmentData)
+
     T = len(data.demand)
     G = len(data.min_power)
     D = data.demand
     Pmin, Pmax = data.min_power, data.max_power
     L = data.min_uptime
     l = data.min_downtime
```

### Comparing `miplearn-0.3.0.dev0/miplearn/problems/vertexcover.py` & `miplearn-0.3.0.dev1/miplearn/problems/vertexcover.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 
 from dataclasses import dataclass
-from typing import List
+from typing import List, Union
 
 import gurobipy as gp
 import numpy as np
 from gurobipy import GRB, quicksum
 from networkx import Graph
 from scipy.stats import uniform, randint
 from scipy.stats.distributions import rv_frozen
 
 from .stab import MaxWeightStableSetGenerator
 from miplearn.solvers.gurobi import GurobiModel
+from ..io import read_pkl_gz
 
 
 @dataclass
 class MinWeightVertexCoverData:
     graph: Graph
     weights: np.ndarray
 
@@ -35,15 +36,18 @@
     def generate(self, n_samples: int) -> List[MinWeightVertexCoverData]:
         return [
             MinWeightVertexCoverData(s.graph, s.weights)
             for s in self._generator.generate(n_samples)
         ]
 
 
-def build_vertexcover_model(data: MinWeightVertexCoverData) -> GurobiModel:
+def build_vertexcover_model(data: Union[str, MinWeightVertexCoverData]) -> GurobiModel:
+    if isinstance(data, str):
+        data = read_pkl_gz(data)
+    assert isinstance(data, MinWeightVertexCoverData)
     model = gp.Model()
     nodes = list(data.graph.nodes)
     x = model.addVars(nodes, vtype=GRB.BINARY, name="x")
     model.setObjective(quicksum(data.weights[i] * x[i] for i in nodes))
     for (v1, v2) in data.graph.edges:
         model.addConstr(x[v1] + x[v2] >= 1)
     model.update()
```

### Comparing `miplearn-0.3.0.dev0/miplearn/solvers/abstract.py` & `miplearn-0.3.0.dev1/miplearn/solvers/abstract.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/miplearn/solvers/gurobi.py` & `miplearn-0.3.0.dev1/miplearn/solvers/gurobi.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         gp_constrs = self.inner.getConstrs()
         h5.put_array(
             "mip_var_values",
             np.array(self.inner.getAttr("x", gp_vars), dtype=float),
         )
         h5.put_array(
             "mip_constr_slacks",
-            np.array(self.inner.getAttr("slack", gp_constrs), dtype=float),
+            np.abs(np.array(self.inner.getAttr("slack", gp_constrs), dtype=float)),
         )
         h5.put_scalar("mip_obj_value", self.inner.objVal)
         h5.put_scalar("mip_obj_bound", self.inner.objBound)
         try:
             h5.put_scalar("mip_gap", self.inner.mipGap)
         except AttributeError:
             pass
@@ -268,20 +268,23 @@
                 dtype="S",
             ),
         )
         for (h5_field, gp_field) in {
             "lp_constr_dual_values": "pi",
             "lp_constr_sa_rhs_up": "saRhsUp",
             "lp_constr_sa_rhs_down": "saRhsLow",
-            "lp_constr_slacks": "slack",
         }.items():
             h5.put_array(
                 h5_field,
                 np.array(self.inner.getAttr(gp_field, gp_constrs), dtype=float),
             )
+        h5.put_array(
+            "lp_constr_slacks",
+            np.abs(np.array(self.inner.getAttr("slack", gp_constrs), dtype=float)),
+        )
 
     def _extract_after_mip_solution_pool(self, h5: H5File) -> None:
         gp_vars = self.inner.getVars()
         pool_var_values = []
         pool_obj_values = []
         for i in range(self.inner.SolCount):
             self.inner.params.SolutionNumber = i
```

### Comparing `miplearn-0.3.0.dev0/miplearn/solvers/learning.py` & `miplearn-0.3.0.dev1/miplearn/solvers/learning.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #  MIPLearn: Extensible Framework for Learning-Enhanced Mixed-Integer Optimization
 #  Copyright (C) 2020-2022, UChicago Argonne, LLC. All rights reserved.
 #  Released under the modified BSD license. See COPYING.md for more details.
 from os.path import exists
-from typing import List, Any
+from tempfile import NamedTemporaryFile
+from typing import List, Any, Union
 
 from miplearn.h5 import H5File
-from miplearn.io import load
+from miplearn.io import _to_h5_filename
+from miplearn.solvers.abstract import AbstractModel
 
 
 class LearningSolver:
     def __init__(self, components: List[Any], skip_lp=False):
         self.components = components
         self.skip_lp = skip_lp
 
-    def fit(self, train_filenames):
-        train_h5 = [f.replace(".pkl.gz", ".h5") for f in train_filenames]
+    def fit(self, data_filenames):
+        h5_filenames = [_to_h5_filename(f) for f in data_filenames]
         for comp in self.components:
-            comp.fit(train_h5)
+            comp.fit(h5_filenames)
 
-    def optimize(self, data_filename, build_model):
+    def optimize(self, model: Union[str, AbstractModel], build_model=None):
+        if isinstance(model, str):
+            h5_filename = _to_h5_filename(model)
+            assert build_model is not None
+            model = build_model(model)
+        else:
+            h5_filename = NamedTemporaryFile().name
         stats = {}
-        h5_filename = data_filename.replace(".pkl.gz", ".h5")
         mode = "r+" if exists(h5_filename) else "w"
         with H5File(h5_filename, mode) as h5:
-            model = load(data_filename, build_model)
             model.extract_after_load(h5)
             if not self.skip_lp:
                 relaxed = model.relax()
                 relaxed.optimize()
                 relaxed.extract_after_lp(h5)
             for comp in self.components:
                 comp.before_mip(h5_filename, model, stats)
             model.optimize()
             model.extract_after_mip(h5)
 
-        model.optimize()
         return stats
```

### Comparing `miplearn-0.3.0.dev0/miplearn/solvers/pyomo.py` & `miplearn-0.3.0.dev1/miplearn/solvers/pyomo.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,56 +13,56 @@
 
 from miplearn.h5 import H5File
 from miplearn.solvers.abstract import AbstractModel
 import pyomo.environ as pe
 
 
 class PyomoModel(AbstractModel):
-    def __init__(self, model: pe.ConcreteModel, solver_name: str):
-        self.model = model
+    def __init__(self, model: pe.ConcreteModel, solver_name: str = "gurobi_persistent"):
+        self.inner = model
         self.solver_name = solver_name
         self.solver = pe.SolverFactory(solver_name)
         self.is_persistent = hasattr(self.solver, "set_instance")
         if self.is_persistent:
             self.solver.set_instance(model)
         self.results = None
         self._is_warm_start_available = False
-        if not hasattr(self.model, "dual"):
-            self.model.dual = Suffix(direction=Suffix.IMPORT)
-            self.model.rc = Suffix(direction=Suffix.IMPORT)
-            self.model.slack = Suffix(direction=Suffix.IMPORT)
+        if not hasattr(self.inner, "dual"):
+            self.inner.dual = Suffix(direction=Suffix.IMPORT)
+            self.inner.rc = Suffix(direction=Suffix.IMPORT)
+            self.inner.slack = Suffix(direction=Suffix.IMPORT)
 
     def add_constrs(
         self,
         var_names: np.ndarray,
         constrs_lhs: np.ndarray,
         constrs_sense: np.ndarray,
         constrs_rhs: np.ndarray,
         stats: Optional[Dict] = None,
     ) -> None:
         variables = self._var_names_to_vars(var_names)
-        if not hasattr(self.model, "added_eqs"):
-            self.model.added_eqs = pe.ConstraintList()
+        if not hasattr(self.inner, "added_eqs"):
+            self.inner.added_eqs = pe.ConstraintList()
         for i in range(len(constrs_sense)):
             lhs = sum([variables[j] * constrs_lhs[i, j] for j in range(len(variables))])
             sense = constrs_sense[i]
             rhs = constrs_rhs[i]
             if sense == b"=":
-                eq = self.model.added_eqs.add(lhs == rhs)
+                eq = self.inner.added_eqs.add(lhs == rhs)
             elif sense == b"<":
-                eq = self.model.added_eqs.add(lhs <= rhs)
+                eq = self.inner.added_eqs.add(lhs <= rhs)
             elif sense == b">":
-                eq = self.model.added_eqs.add(lhs >= rhs)
+                eq = self.inner.added_eqs.add(lhs >= rhs)
             else:
                 raise Exception(f"Unknown sense: {sense}")
             self.solver.add_constraint(eq)
 
     def _var_names_to_vars(self, var_names):
         varname_to_var = {}
-        for var in self.model.component_objects(Var):
+        for var in self.inner.component_objects(Var):
             for idx in var:
                 v = var[idx]
                 varname_to_var[v.name] = var[idx]
         return [varname_to_var[var_name.decode()] for var_name in var_names]
 
     def extract_after_load(self, h5: H5File) -> None:
         self._extract_after_load_vars(h5)
@@ -102,32 +102,32 @@
         self,
         var_names: np.ndarray,
         var_values: np.ndarray,
         stats: Optional[Dict] = None,
     ) -> None:
         variables = self._var_names_to_vars(var_names)
         for (var, val) in zip(variables, var_values):
-            var.fix(val)
-            self.solver.update_var(var)
+            if np.isfinite(val):
+                var.fix(val)
+                self.solver.update_var(var)
 
     def optimize(self) -> None:
         if self.is_persistent:
             self.results = self.solver.solve(
                 tee=True,
                 warmstart=self._is_warm_start_available,
             )
         else:
             self.results = self.solver.solve(
-                self.model,
+                self.inner,
                 tee=True,
             )
-            print(self.results)
 
     def relax(self) -> "AbstractModel":
-        relaxed = self.model.clone()
+        relaxed = self.inner.clone()
         for var in relaxed.component_objects(Var):
             for idx in var:
                 if var[idx].domain == pyomo.core.base.set_types.Binary:
                     lb, ub = var[idx].bounds
                     var[idx].setlb(lb)
                     var[idx].setub(ub)
                     var[idx].domain = pyomo.core.base.set_types.Reals
@@ -142,33 +142,34 @@
         assert len(var_values.shape) == 2
         (n_starts, n_vars) = var_values.shape
         assert len(var_names.shape) == 1
         assert var_names.shape[0] == n_vars
         assert n_starts == 1, "Pyomo does not support multiple warm starts"
         variables = self._var_names_to_vars(var_names)
         for (var, val) in zip(variables, var_values[0, :]):
-            var.value = val
+            if np.isfinite(val):
+                var.value = val
         self._is_warm_start_available = True
 
     def _extract_after_load_vars(self, h5):
         names: List[str] = []
         types: List[str] = []
         upper_bounds: List[float] = []
         lower_bounds: List[float] = []
         obj_coeffs: List[float] = []
 
         obj = None
         obj_offset = 0.0
         obj_count = 0
-        for obj in self.model.component_objects(Objective):
+        for obj in self.inner.component_objects(Objective):
             obj, obj_offset = self._parse_pyomo_expr(obj.expr)
             obj_count += 1
         assert obj_count == 1, f"One objective function expected; found {obj_count}"
 
-        for (i, var) in enumerate(self.model.component_objects(pyomo.core.Var)):
+        for (i, var) in enumerate(self.inner.component_objects(pyomo.core.Var)):
             for idx in var:
                 v = var[idx]
 
                 # Variable name
                 if idx is None:
                     names.append(var.name)
                 else:
@@ -186,14 +187,18 @@
                 ]:
                     types.append("C")
                 else:
                     raise Exception(f"unknown variable domain: {v.domain}")
 
                 # Variable upper/lower bounds
                 lb, ub = v.bounds
+                if lb is None:
+                    lb = -float("inf")
+                if ub is None:
+                    ub = float("Inf")
                 upper_bounds.append(float(ub))
                 lower_bounds.append(float(lb))
 
                 # Objective coefficients
                 if v.name in obj:
                     obj_coeffs.append(obj[v.name])
                 else:
@@ -211,15 +216,15 @@
         rhs: List[float] = []
         senses: List[str] = []
         lhs_row: List[int] = []
         lhs_col: List[int] = []
         lhs_data: List[float] = []
 
         varname_to_idx = {}
-        for var in self.model.component_objects(Var):
+        for var in self.inner.component_objects(Var):
             for idx in var:
                 varname = var.name
                 if idx is not None:
                     varname = var[idx].name
                 varname_to_idx[varname] = len(varname_to_idx)
 
         def _parse_constraint(c: pe.Constraint, row: int) -> None:
@@ -258,15 +263,15 @@
                 lhs_col.append(varname_to_idx[expr.name])
                 lhs_data.append(1.0)
             else:
                 raise Exception(f"Unknown expression type: {expr.__class__.__name__}")
 
         curr_row = 0
         for (i, constr) in enumerate(
-            self.model.component_objects(pyomo.core.Constraint)
+            self.inner.component_objects(pyomo.core.Constraint)
         ):
             if len(constr) > 0:
                 for idx in constr:
                     names.append(constr[idx].name)
                     _parse_constraint(constr[idx], curr_row)
                     curr_row += 1
             else:
@@ -279,47 +284,47 @@
         h5.put_array("static_constr_names", np.array(names, dtype="S"))
         h5.put_array("static_constr_rhs", np.array(rhs))
         h5.put_array("static_constr_sense", np.array(senses, dtype="S"))
 
     def _extract_after_lp_vars(self, h5):
         rc = []
         values = []
-        for var in self.model.component_objects(Var):
+        for var in self.inner.component_objects(Var):
             for idx in var:
                 v = var[idx]
-                rc.append(self.model.rc[v])
+                rc.append(self.inner.rc[v])
                 values.append(v.value)
         h5.put_array("lp_var_reduced_costs", np.array(rc))
         h5.put_array("lp_var_values", np.array(values))
 
     def _extract_after_lp_constrs(self, h5):
         dual = []
         slacks = []
-        for constr in self.model.component_objects(pyomo.core.Constraint):
+        for constr in self.inner.component_objects(pyomo.core.Constraint):
             for idx in constr:
                 c = constr[idx]
-                dual.append(self.model.dual[c])
-                slacks.append(self.model.slack[c])
+                dual.append(self.inner.dual[c])
+                slacks.append(abs(self.inner.slack[c]))
         h5.put_array("lp_constr_dual_values", np.array(dual))
         h5.put_array("lp_constr_slacks", np.array(slacks))
 
     def _extract_after_mip_vars(self, h5):
         values = []
-        for var in self.model.component_objects(Var):
+        for var in self.inner.component_objects(Var):
             for idx in var:
                 v = var[idx]
                 values.append(v.value)
         h5.put_array("mip_var_values", np.array(values))
 
     def _extract_after_mip_constrs(self, h5):
         slacks = []
-        for constr in self.model.component_objects(pyomo.core.Constraint):
+        for constr in self.inner.component_objects(pyomo.core.Constraint):
             for idx in constr:
                 c = constr[idx]
-                slacks.append(self.model.slack[c])
+                slacks.append(abs(self.inner.slack[c]))
         h5.put_array("mip_constr_slacks", np.array(slacks))
 
     def _parse_pyomo_expr(self, expr: Any):
         lhs = {}
         offset = 0.0
         if isinstance(expr, SumExpression):
             for term in expr._args_:
@@ -344,18 +349,18 @@
                 return 0
             else:
                 return float("inf")
         else:
             return abs(zp - zd) / abs(zp)
 
     def _get_sense(self):
-        for obj in self.model.component_objects(Objective):
+        for obj in self.inner.component_objects(Objective):
             sense = obj.sense
             if sense == pyomo.core.kernel.objective.minimize:
                 return "min"
             elif sense == pyomo.core.kernel.objective.maximize:
                 return "max"
             else:
                 raise Exception(f"Unknown sense: ${sense}")
 
     def write(self, filename: str) -> None:
-        self.model.write(filename, io_options={"symbolic_solver_labels": True})
+        self.inner.write(filename, io_options={"symbolic_solver_labels": True})
```

### Comparing `miplearn-0.3.0.dev0/miplearn.egg-info/SOURCES.txt` & `miplearn-0.3.0.dev1/miplearn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 miplearn/__init__.py
 miplearn/h5.py
 miplearn/io.py
 miplearn/parallel.py
 miplearn.egg-info/PKG-INFO
 miplearn.egg-info/SOURCES.txt
 miplearn.egg-info/dependency_links.txt
+miplearn.egg-info/requires.txt
 miplearn.egg-info/top_level.txt
 miplearn/classifiers/__init__.py
 miplearn/classifiers/minprob.py
 miplearn/classifiers/singleclass.py
 miplearn/collectors/__init__.py
 miplearn/collectors/basic.py
 miplearn/collectors/lazy.py
```

### Comparing `miplearn-0.3.0.dev0/tests/components/primal/test_expert.py` & `miplearn-0.3.0.dev1/tests/components/primal/test_expert.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/components/primal/test_indep.py` & `miplearn-0.3.0.dev1/tests/components/primal/test_indep.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/components/primal/test_joint.py` & `miplearn-0.3.0.dev1/tests/components/primal/test_joint.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/components/primal/test_mem.py` & `miplearn-0.3.0.dev1/tests/components/primal/test_mem.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/conftest.py` & `miplearn-0.3.0.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/extractors/test_dummy.py` & `miplearn-0.3.0.dev1/tests/extractors/test_dummy.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/extractors/test_fields.py` & `miplearn-0.3.0.dev1/tests/extractors/test_fields.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_binpack.py` & `miplearn-0.3.0.dev1/tests/problems/test_binpack.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_multiknapsack.py` & `miplearn-0.3.0.dev1/tests/problems/test_multiknapsack.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_pmedian.py` & `miplearn-0.3.0.dev1/tests/problems/test_pmedian.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_setcover.py` & `miplearn-0.3.0.dev1/tests/problems/test_setcover.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_setpack.py` & `miplearn-0.3.0.dev1/tests/problems/test_setpack.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_stab.py` & `miplearn-0.3.0.dev1/tests/problems/test_stab.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_tsp.py` & `miplearn-0.3.0.dev1/tests/problems/test_tsp.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_uc.py` & `miplearn-0.3.0.dev1/tests/problems/test_uc.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/problems/test_vertexcover.py` & `miplearn-0.3.0.dev1/tests/problems/test_vertexcover.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/test_h5.py` & `miplearn-0.3.0.dev1/tests/test_h5.py`

 * *Files identical despite different names*

### Comparing `miplearn-0.3.0.dev0/tests/test_solvers.py` & `miplearn-0.3.0.dev1/tests/test_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             test_array("static_var_types", [b"B", b"B", b"B", b"B", b"B"])
             test_array("static_var_upper_bounds", [1.0, 1.0, 1.0, 1.0, 1.0])
 
             relaxed = model.relax()
             relaxed.optimize()
             relaxed.extract_after_lp(h5)
             test_array("lp_constr_dual_values", [0, 5, 6])
-            test_array("lp_constr_slacks", [-1, 0, 0])
+            test_array("lp_constr_slacks", [1, 0, 0])
             test_scalar("lp_obj_value", 11.0)
             test_array("lp_var_reduced_costs", [0.0, 5.0, 6.0, 0.0, 2.0])
             test_array("lp_var_values", [1.0, 0.0, 0.0, 1.0, 0.0])
             if model._supports_basis_status:
                 test_array("lp_var_basis_status", [b"B", b"L", b"L", b"B", b"L"])
                 test_array("lp_constr_basis_status", [b"B", b"N", b"N"])
             if model._supports_sensitivity_analysis:
@@ -117,15 +117,15 @@
                 test_array("lp_var_sa_lb_down", [-inf, 0.0, 0.0, -inf, 0.0])
             lp_wallclock_time = h5.get_scalar("lp_wallclock_time")
             assert lp_wallclock_time is not None
             assert lp_wallclock_time >= 0
 
             model.optimize()
             model.extract_after_mip(h5)
-            test_array("mip_constr_slacks", [-1, 0, 0])
+            test_array("mip_constr_slacks", [1, 0, 0])
             test_array("mip_var_values", [1.0, 0.0, 0.0, 1.0, 0.0])
             test_scalar("mip_gap", 0)
             test_scalar("mip_obj_bound", 11.0)
             test_scalar("mip_obj_value", 11.0)
             mip_wallclock_time = h5.get_scalar("mip_wallclock_time")
             assert mip_wallclock_time is not None
             assert mip_wallclock_time > 0
@@ -143,18 +143,18 @@
                 assert pool_var_values.shape == (n_sols, 5)
 
 
 def _test_add_constr(model: AbstractModel):
     with NamedTemporaryFile() as tempfile:
         with H5File(tempfile.name) as h5:
             model.add_constrs(
-                var_names=np.array([b"x[2]", b"x[3]"], dtype="S"),
-                constrs_lhs=np.array([[0, 1], [1, 0]]),
-                constrs_sense=np.array(["=", "="], dtype="S"),
-                constrs_rhs=np.array([0, 0]),
+                np.array([b"x[2]", b"x[3]"], dtype="S"),
+                np.array([[0, 1], [1, 0]]),
+                np.array(["=", "="], dtype="S"),
+                np.array([0, 0]),
             )
             model.optimize()
             model.extract_after_mip(h5)
             assert h5.get_array("mip_var_values").tolist() == [1, 0, 0, 0, 1]
 
 
 def _test_fix_vars(model: AbstractModel):
```

