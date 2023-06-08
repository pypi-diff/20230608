# Comparing `tmp/state_space_generator-0.1.7.tar.gz` & `tmp/state_space_generator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "state_space_generator-0.1.7.tar", last modified: Mon May  1 15:20:04 2023, max compression
+gzip compressed data, was "state_space_generator-0.1.8.tar", last modified: Thu Jun  8 08:03:21 2023, max compression
```

## Comparing `state_space_generator-0.1.7.tar` & `state_space_generator-0.1.8.tar`

### file list

```diff
@@ -1,712 +1,712 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.970481 state_space_generator-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 15:20:04.970481 state_space_generator-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-01 15:20:04.970481 state_space_generator-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.854480 state_space_generator-0.1.7/state_space_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.854480 state_space_generator-0.1.7/state_space_generator/scorpion/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     4831 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/build_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.858480 state_space_generator-0.1.7/state_space_generator/scorpion/driver/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/plan_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolio_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.858480 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_opt_merge_and_shrink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2014.py
--rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/returncodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/run_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/driver/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/fast-downward.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.858480 state_space_generator-0.1.7/state_space_generator/scorpion/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.858480 state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FastDownwardMacros.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindClp.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindCplex.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindOSI.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindSoplex.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.862480 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/axiom.cc
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/axiom.h
--rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/causal_graph.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/causal_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    35485 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.h
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/helper_functions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/helper_functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/max_dag.cc
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/max_dag.h
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/mutex_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/mutex_group.h
--rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/operator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/operator.h
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/planner.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/scc.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/scc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/state.cc
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/state.h
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/variable.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/variable.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.870480 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24768 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/DownwardFiles.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/abstract_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/abstract_task.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.874481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/array_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/dynamic_bitset.h
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.h
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/int_hash_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/int_packer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/int_packer.h
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/max_cliques.cc
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/max_cliques.h
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/named_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/ordered_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/priority_queues.h
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/sccs.cc
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/sccs.h
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/segmented_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/subscriber.h
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/axioms.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/axioms.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.878481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_state.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstraction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.cc
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.h
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_set.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cegar.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cegar.h
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cost_saturation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cost_saturation.h
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw.h
--rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/shortest_paths.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/shortest_paths.h
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/split_selector.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/split_selector.h
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/subtask_generators.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/subtask_generators.h
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/transition.h
--rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/transition_system.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/transition_system.h
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils_landmarks.cc
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils_landmarks.h
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/command_line.cc
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/command_line.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.890481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/diversifier.cc
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/diversifier.h
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.h
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.h
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.cc
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.h
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.h
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/plugin_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21981 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection.h
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/zero_one_cost_partitioning_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/zero_one_cost_partitioning_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_context.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_context.h
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_result.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_result.h
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator_cache.cc
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator_cache.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.890481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/const_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/const_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/g_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/g_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/max_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/max_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/plugin_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/pref_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/pref_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/sum_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/sum_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.894481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/
--rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/optional.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.894481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/
--rw-r--r--   0 runner    (1001) docker     (123)   166554 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/btree.h
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/meminfo.h
--rw-r--r--   0 runner    (1001) docker     (123)   185590 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap.h
--rw-r--r--   0 runner    (1001) docker     (123)   180847 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_base.h
--rw-r--r--   0 runner    (1001) docker     (123)    22491 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_bits.h
--rw-r--r--   0 runner    (1001) docker     (123)    28525 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_config.h
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_dump.h
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_fwd_decl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    80447 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/tree.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/tree_util.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristic.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.898481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/array_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/blind_search_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/blind_search_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_cache.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_cache.h
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/goal_count_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/goal_count_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.h
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/max_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/max_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.906481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/exploration.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/exploration.h
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark.h
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.h
--rw-r--r--   0 runner    (1001) docker     (123)    18194 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.h
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.cc
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.h
--rw-r--r--   0 runner    (1001) docker     (123)    18923 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.h
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.h
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.cc
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.h
--rw-r--r--   0 runner    (1001) docker     (123)    29003 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.h
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_graph.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.h
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/util.cc
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.906481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_internals.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_solver.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.918481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/distances.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/distances.h
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.h
--rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.h
--rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/labels.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/labels.h
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.cc
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.h
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.cc
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.cc
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.h
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.h
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.h
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.h
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.h
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy.h
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.cc
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.h
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.cc
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.h
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.cc
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.h
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.h
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_stateless.cc
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_stateless.h
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.h
--rw-r--r--   0 runner    (1001) docker     (123)    16831 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.h
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.h
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.h
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.cc
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.h
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.h
--rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.h
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/types.cc
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_list_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_list_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.922481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.cc
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.cc
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.cc
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.cc
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.h
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_cost.cc
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_cost.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.922481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/constraint_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/constraint_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.h
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.cc
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.h
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.h
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.cc
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.h
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.h
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_id.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_id.h
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/option_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/option_parser_util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.926481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/any.h
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/bounds.cc
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/bounds.h
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_printer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_printer.h
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/errors.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/errors.h
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/option_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/option_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/options.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/parse_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/plugin.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/plugin.h
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/predefinitions.h
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/raw_registry.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/raw_registry.h
--rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/registries.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/registries.h
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/type_namer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.938481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs.cc
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)    29343 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/cegar.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/cegar.h
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.cc
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.h
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/match_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/match_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.h
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.cc
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.cc
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.h
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.h
--rw-r--r--   0 runner    (1001) docker     (123)    28581 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.h
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.cc
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.h
--rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.h
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.cc
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.h
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.cc
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.h
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.h
--rw-r--r--   0 runner    (1001) docker     (123)    23231 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.h
--rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_database.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_database.h
--rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.cc
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.h
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_greedy.h
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.cc
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.h
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.cc
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.h
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_information.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_information.h
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/plugin_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/random_pattern.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/random_pattern.h
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/validation.cc
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/validation.h
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.cc
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.h
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_bitset.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_bitset.h
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_information.h
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_task_information.h
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/plan_manager.cc
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/plan_manager.h
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/planner.cc
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/plugin.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.942481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.h
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/plugin_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_function.cc
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_function.h
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.cc
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.h
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_optimizer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_optimizer.h
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/sample_based_potential_heuristics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/single_potential_heuristics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/util.cc
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.942481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/limited_pruning.cc
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/limited_pruning.h
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/null_pruning_method.cc
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/null_pruning_method.h
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets.h
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.h
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.h
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.h
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning_method.cc
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning_method.h
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engine.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engine.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.950481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/depth_first_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/depth_first_search.h
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/eager_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/eager_search.h
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/idastar_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/idastar_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterated_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterated_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/lazy_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/lazy_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_astar.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_eager.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_eager_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_eager_wastar.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_lazy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_wastar.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/search_common.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/search_common.h
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_node_info.cc
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_node_info.h
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_progress.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_space.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_space.h
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_statistics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_statistics.h
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_id.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_id.h
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_registry.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_registry.h
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_id.h
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_proxy.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_proxy.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.950481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/causal_graph.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/causal_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/sampling.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/sampling.h
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator.cc
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator.h
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.h
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/task_properties.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/task_properties.h
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.954481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.h
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/delegating_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/delegating_task.h
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.h
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.cc
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_goals_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_goals_task.h
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.h
--rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/root_task.cc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/root_task.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.958481 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/collections.h
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/countdown_timer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/countdown_timer.h
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/hash.h
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/language.h
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/markup.cc
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/markup.h
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/math.cc
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/math.h
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/memory.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/memory.h
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng.h
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng_options.cc
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng_options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/strings.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/strings.h
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system.h
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system_unix.cc
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system_unix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system_windows.cc
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system_windows.h
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/timer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/timer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/tokenizer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.962481 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/
--rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/axiom_rules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13114 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/fact_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/greedy_join.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8289 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/instantiate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6100 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/invariant_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/invariants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16121 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.966481 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/axioms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/f_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/pddl_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.966481 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/lisp_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/parsing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/pddl_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7436 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_to_prolog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.970481 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/README
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue34-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue34-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue405-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue405-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-falsegoal-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-falsegoal-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    86428 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-truegoal-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-truegoal-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue58-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue58-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue7-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue7-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    67932 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue73-domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue73-problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/sas_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/sccs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/split_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.970481 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33730 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/variable_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-01 15:19:49.000000 state_space_generator-0.1.7/state_space_generator/state_space_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:20:04.854480 state_space_generator-0.1.7/state_space_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 15:20:04.000000 state_space_generator-0.1.7/state_space_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-05-01 15:20:04.000000 state_space_generator-0.1.7/state_space_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:20:04.000000 state_space_generator-0.1.7/state_space_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:20:04.000000 state_space_generator-0.1.7/state_space_generator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 15:20:04.000000 state_space_generator-0.1.7/state_space_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.735628 state_space_generator-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-08 08:03:21.735628 state_space_generator-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 08:03:21.735628 state_space_generator-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.671628 state_space_generator-0.1.8/state_space_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.671628 state_space_generator-0.1.8/state_space_generator/scorpion/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4831 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/build_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.671628 state_space_generator-0.1.8/state_space_generator/scorpion/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19347 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/plan_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolio_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.675628 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_opt_merge_and_shrink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2014.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/returncodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/run_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/driver/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/fast-downward.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.675628 state_space_generator-0.1.8/state_space_generator/scorpion/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.675628 state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FastDownwardMacros.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindClp.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindCplex.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindOSI.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindSoplex.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.675628 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/axiom.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/axiom.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/causal_graph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/causal_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35485 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/helper_functions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/helper_functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/max_dag.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/max_dag.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/mutex_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/mutex_group.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/operator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/operator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/planner.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/scc.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/scc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/state.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/variable.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/variable.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.679628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24768 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/DownwardFiles.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/abstract_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/abstract_task.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.683628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/array_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/dynamic_bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/int_hash_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/int_packer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/int_packer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/max_cliques.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/max_cliques.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/named_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/ordered_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/priority_queues.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/sccs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/sccs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/segmented_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/subscriber.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/axioms.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/axioms.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.687628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_state.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstraction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_set.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cegar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cegar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cost_saturation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cost_saturation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/shortest_paths.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/shortest_paths.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/split_selector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/split_selector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/subtask_generators.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/subtask_generators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/transition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/transition_system.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/transition_system.h
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils_landmarks.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils_landmarks.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/command_line.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/command_line.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.691628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/diversifier.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/diversifier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/plugin_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21981 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/zero_one_cost_partitioning_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/zero_one_cost_partitioning_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_context.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_context.h
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_result.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_result.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator_cache.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator_cache.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.691628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/const_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/const_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/g_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/g_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/max_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/max_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/plugin_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/pref_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/pref_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/sum_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/sum_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.691628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/optional.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.695628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/
+-rw-r--r--   0 runner    (1001) docker     (123)   166554 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/btree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/meminfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)   185590 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)   180847 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22491 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_bits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28525 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_dump.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_fwd_decl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80447 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/tree.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/tree_util.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristic.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.695628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/array_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/blind_search_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/blind_search_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_cache.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/goal_count_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/goal_count_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13011 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/max_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/max_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.699628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/exploration.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/exploration.h
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18194 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37635 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18923 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29003 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_graph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/util.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.699628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_internals.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15578 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_solver.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_solver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.707628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/distances.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/distances.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/labels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/labels.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.h
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy.h
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.h
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_stateless.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_stateless.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16831 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.h
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.h
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/types.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_list_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_list_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.707628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_cost.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_cost.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.711628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/constraint_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/constraint_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_id.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/option_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/option_parser_util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.711628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/any.h
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/bounds.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/bounds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_printer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_printer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/errors.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/errors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/option_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/option_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/options.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/parse_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/plugin.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/plugin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/predefinitions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/raw_registry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/raw_registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/registries.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/registries.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/type_namer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.719628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29343 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/cegar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/cegar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/match_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/match_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28581 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13075 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23231 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15445 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_database.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_database.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_greedy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.h
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_information.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/plugin_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/random_pattern.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/random_pattern.h
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/validation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/validation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_bitset.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_task_information.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/plan_manager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/plan_manager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/planner.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/plugin.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.719628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.h
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/plugin_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_function.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_function.h
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_optimizer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_optimizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/sample_based_potential_heuristics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/single_potential_heuristics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/util.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.719628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/limited_pruning.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/limited_pruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/null_pruning_method.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/null_pruning_method.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning_method.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning_method.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engine.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engine.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.723628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/depth_first_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/depth_first_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/eager_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/eager_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/idastar_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/idastar_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterated_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterated_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/lazy_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/lazy_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_astar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_eager.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_eager_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_eager_wastar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_lazy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_wastar.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/search_common.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/search_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_node_info.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_node_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_progress.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_space.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_space.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_statistics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_statistics.h
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_id.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_registry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_registry.h
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_id.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_proxy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26025 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_proxy.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.727628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/causal_graph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/causal_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/sampling.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/task_properties.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/task_properties.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.727628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/delegating_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/delegating_task.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_goals_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_goals_task.h
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/root_task.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/root_task.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.727628 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/collections.h
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/countdown_timer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/countdown_timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/language.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/markup.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/markup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/math.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/memory.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng.h
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng_options.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng_options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/strings.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/strings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system_unix.cc
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system_unix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system_windows.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system_windows.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/timer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/tokenizer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.731628 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/axiom_rules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13114 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/fact_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/greedy_join.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8289 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/instantiate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6100 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/invariant_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/invariants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16121 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.731628 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/axioms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/f_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/pddl_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.731628 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/lisp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/parsing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/pddl_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7436 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_to_prolog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.731628 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/README
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue34-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue34-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue405-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue405-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-falsegoal-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-falsegoal-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    86428 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-truegoal-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-truegoal-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue58-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue58-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue7-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue7-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    67932 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue73-domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue73-problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/sas_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/sccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/split_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.735628 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33730 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/variable_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-08 08:03:11.000000 state_space_generator-0.1.8/state_space_generator/state_space_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:03:21.671628 state_space_generator-0.1.8/state_space_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-08 08:03:21.000000 state_space_generator-0.1.8/state_space_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-06-08 08:03:21.000000 state_space_generator-0.1.8/state_space_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:03:21.000000 state_space_generator-0.1.8/state_space_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:03:21.000000 state_space_generator-0.1.8/state_space_generator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 08:03:21.000000 state_space_generator-0.1.8/state_space_generator.egg-info/top_level.txt
```

### Comparing `state_space_generator-0.1.7/LICENSE.md` & `state_space_generator-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/setup.py` & `state_space_generator-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 
 class CustomBuild(build_py):
     def run(self):
         """ Builds the scorpion binaries. """
         curr_dir = os.getcwd()
         os.chdir(os.path.join(curr_dir, 'state_space_generator/scorpion'))
```

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/LICENSE.md` & `state_space_generator-0.1.8/state_space_generator/scorpion/LICENSE.md`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/README.md` & `state_space_generator-0.1.8/state_space_generator/scorpion/README.md`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/build.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/build.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/build_configs.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/build_configs.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/aliases.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/aliases.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/arguments.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/arguments.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/call.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/call.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/limits.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/limits.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/main.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/main.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/plan_manager.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/plan_manager.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolio_runner.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolio_runner.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_1.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_1.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_2.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_opt_fdss_2.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_opt_merge_and_shrink.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_opt_merge_and_shrink.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_1.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_1.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2014.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2014.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2018.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/portfolios/seq_sat_fdss_2018.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/returncodes.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/returncodes.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/run_components.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/run_components.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/tests.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/tests.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/driver/util.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/driver/util.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/CMakeLists.txt` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FastDownwardMacros.cmake` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FastDownwardMacros.cmake`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindClp.cmake` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindClp.cmake`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindCplex.cmake` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindCplex.cmake`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindOSI.cmake` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindOSI.cmake`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/cmake_modules/FindSoplex.cmake` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/cmake_modules/FindSoplex.cmake`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/CMakeLists.txt` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/README.md` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/README.md`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/axiom.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/axiom.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/axiom.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/axiom.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/causal_graph.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/causal_graph.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/causal_graph.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/causal_graph.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/h2_mutexes.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/helper_functions.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/helper_functions.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/helper_functions.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/helper_functions.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/max_dag.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/max_dag.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/mutex_group.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/mutex_group.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/mutex_group.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/mutex_group.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/operator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/operator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/operator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/operator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/planner.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/planner.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/scc.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/scc.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/scc.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/scc.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/state.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/state.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/variable.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/variable.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/preprocess_h2/variable.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/preprocess_h2/variable.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/CMakeLists.txt` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/DownwardFiles.cmake` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/DownwardFiles.cmake`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/abstract_task.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/abstract_task.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/array_pool.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/array_pool.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/dynamic_bitset.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/dynamic_bitset.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/equivalence_relation.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/int_hash_set.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/int_hash_set.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/int_packer.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/int_packer.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/int_packer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/int_packer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/max_cliques.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/max_cliques.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/max_cliques.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/max_cliques.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/named_vector.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/named_vector.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/ordered_set.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/ordered_set.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/partial_state_tree.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/priority_queues.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/priority_queues.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/sccs.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/sccs.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/sccs.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/sccs.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/segmented_vector.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/segmented_vector.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/algorithms/subscriber.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/algorithms/subscriber.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/axioms.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/axioms.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/axioms.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/axioms.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_state.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_state.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstract_state.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstract_state.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstraction.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstraction.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/abstraction.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/abstraction.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/additive_cartesian_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_heuristic_function.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_set.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_set.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cartesian_set.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cartesian_set.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cegar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cegar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cegar.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cegar.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cost_saturation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cost_saturation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/cost_saturation.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/cost_saturation.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/flaw_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/flaw_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/refinement_hierarchy.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/shortest_paths.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/shortest_paths.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/shortest_paths.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/shortest_paths.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/split_selector.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/split_selector.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/split_selector.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/split_selector.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/subtask_generators.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/subtask_generators.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/subtask_generators.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/subtask_generators.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/transition.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/transition.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/transition_system.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/transition_system.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/transition_system.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/transition_system.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/types.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/types.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils_landmarks.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils_landmarks.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cegar/utils_landmarks.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cegar/utils_landmarks.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/command_line.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/command_line.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/command_line.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/command_line.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/abstraction_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/abstraction_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/canonical_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cartesian_abstraction_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/cost_partitioning_heuristic_collection_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/diversifier.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/diversifier.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/diversifier.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/diversifier.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_abstraction.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/explicit_projection_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/greedy_order_utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_cost_partitioning_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/max_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/max_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/optimal_cost_partitioning_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_dynamic_greedy.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_greedy.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_generator_random.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/order_optimizer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/pho_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/projection_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/saturated_cost_partitioning_online_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/types.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/types.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/uniform_cost_partitioning_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/unsolvability_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/cost_saturation/zero_one_cost_partitioning_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/cost_saturation/zero_one_cost_partitioning_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_context.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_context.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_context.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_context.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_result.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_result.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluation_result.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluation_result.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluator_cache.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluator_cache.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/combining_evaluator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/const_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/const_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/const_evaluator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/const_evaluator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/g_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/g_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/max_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/max_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/pref_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/pref_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/sum_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/sum_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/evaluators/weighted_evaluator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/optional.hh` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/optional.hh`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/btree.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/btree.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/meminfo.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/meminfo.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_base.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_base.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_bits.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_bits.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_config.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_config.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_dump.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_dump.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_fwd_decl.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_fwd_decl.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/parallel_hashmap/phmap_utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/tree.hh` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/tree.hh`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/ext/tree_util.hh` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/ext/tree_util.hh`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/additive_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/array_pool.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/array_pool.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/blind_search_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/blind_search_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cea_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_cache.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_cache.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_cache.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_cache.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/cg_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/domain_transition_graph.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/ff_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/goal_count_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/goal_count_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/hm_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/lm_cut_landmarks.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/max_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/max_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/max_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/max_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/heuristics/relaxation_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/exploration.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/exploration.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/exploration.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/exploration.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_cost_assignment.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_count_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_h_m.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_merged.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_reasonable_orders_hps.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_relaxation.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_exhaust.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_rpg_sasp.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_factory_zhu_givan.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_graph.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_graph.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_graph.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_graph.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/landmark_status_manager.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/util.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/util.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/landmarks/util.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/landmarks/util.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_internals.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_internals.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_internals.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_internals.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_solver.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_solver.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/lp/lp_solver.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/lp/lp_solver.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/distances.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/distances.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/distances.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/distances.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/factored_transition_system.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/fts_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_equivalence_relation.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/label_reduction.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/labels.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/labels.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/labels.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/labels.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_algorithm.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_and_shrink_representation.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_dfp.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_goal_relevance.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_miasm_utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_single_random.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_scoring_function_total_order.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_selector_score_based_filtering.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_precomputed.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_sccs.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_factory_stateless.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_precomputed.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_sccs.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_stateless.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_strategy_stateless.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/merge_tree_factory_linear.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bisimulation.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_bucket_based.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_fh.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_random.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/shrink_strategy.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/transition_system.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/types.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/types.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/merge_and_shrink/utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/merge_and_shrink/utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_list_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_list_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/alternation_open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/best_first_open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/epsilon_greedy_open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/pareto_open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/tiebreaking_open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/open_lists/type_based_open_list.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_cost.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_cost.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/constraint_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/constraint_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/delete_relaxation_constraints.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/lm_cut_constraints.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/operator_counting_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_abstraction_constraints.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/pho_constraints.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_counting/state_equation_constraints.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/operator_id.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/operator_id.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/option_parser.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/option_parser.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/any.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/any.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_printer.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_printer.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_printer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_printer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/doc_utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/doc_utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/errors.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/errors.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/errors.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/errors.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/option_parser.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/option_parser.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/option_parser.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/option_parser.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/options.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/options.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/parse_tree.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/parse_tree.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/plugin.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/plugin.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/predefinitions.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/predefinitions.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/raw_registry.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/raw_registry.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/raw_registry.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/raw_registry.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/registries.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/registries.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/registries.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/registries.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/options/type_namer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/options/type_namer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/canonical_pdbs_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/cegar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/cegar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/cegar.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/cegar.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/dominance_pruning.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/incremental_canonical_pdbs.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/match_tree.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/match_tree.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/match_tree.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/match_tree.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_cliques.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_combo.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_disjoint_cegar.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_genetic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_hillclimbing.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_manual.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_cegar.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_multiple_random.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_generator_systematic_scp.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_collection_information.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_database.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_database.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_database.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_database.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_evaluator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_cegar.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_greedy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_greedy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_manual.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_generator_random.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_information.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_information.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pattern_information.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pattern_information.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/pdb_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/random_pattern.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/random_pattern.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/random_pattern.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/random_pattern.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/types.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/types.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/utils.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/utils.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/utils.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/utils.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/validation.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/validation.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pdbs/zero_one_pdbs_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_array.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_array.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_bitset.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_bitset.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_bitset.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_bitset.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_state_information.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_state_information.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/per_task_information.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/per_task_information.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/plan_manager.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/plan_manager.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/plan_manager.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/plan_manager.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/planner.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/planner.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/diverse_potential_heuristics.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_function.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_function.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_function.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_function.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_max_heuristic.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_optimizer.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_optimizer.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/potential_optimizer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/potential_optimizer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/sample_based_potential_heuristics.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/sample_based_potential_heuristics.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/single_potential_heuristics.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/single_potential_heuristics.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/util.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/util.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/potentials/util.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/potentials/util.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/limited_pruning.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/limited_pruning.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/limited_pruning.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/limited_pruning.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/null_pruning_method.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/null_pruning_method.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_atom_centric.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_ec.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning/stubborn_sets_simple.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning_method.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning_method.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/pruning_method.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/pruning_method.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engine.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engine.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engine.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engine.h`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class OrderedSet;
 }
 
 namespace successor_generator {
 class SuccessorGenerator;
 }
 
-enum SearchStatus {IN_PROGRESS, TIMEOUT, FAILED, SOLVED, UNSOLVABLE};
+enum SearchStatus {IN_PROGRESS, TIMEOUT, RESOURCEOUT, FAILED, SOLVED, UNSOLVABLE};
 
 class SearchEngine {
 protected:
     SearchStatus status;
     bool solution_found;
     Plan plan;
```

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/breadth_first_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/depth_first_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/depth_first_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/depth_first_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/depth_first_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/eager_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/eager_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/eager_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/eager_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/enforced_hill_climbing_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.cc`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 #include "../option_parser.h"
 #include "../plugin.h"
 
 #include "../task_utils/successor_generator.h"
 #include "../task_utils/task_properties.h"
 #include "../utils/logging.h"
+#include "../utils/countdown_timer.h"
 
 #include <algorithm>
 #include <cassert>
 
 using namespace std;
 
 namespace exhaustive_search {
@@ -50,20 +51,19 @@
     }
     atoms_file.close();
     return mapping;
 }
 
 ExhaustiveSearch::ExhaustiveSearch(const Options &opts)
     : SearchEngine(opts),
+      max_num_states(opts.get<int>("max_num_states")),
       dump_atoms_to_file(opts.get<bool>("dump_atoms")),
       dump_states_to_file(opts.get<bool>("dump_states")),
       dump_transitions_to_file(opts.get<bool>("dump_transitions")) {
     assert(cost_type == ONE);
-    states_file.open("states.txt");
-    transitions_file.open("transitions.txt");
 }
 
 void ExhaustiveSearch::initialize() {
     utils::g_log << "Dumping the reachable state space..." << endl;
     cout << "# F (fact): [fact ID] [name]" << endl;
     cout << "# G (goal state): [goal state ID] [fact ID 1] [fact ID 2] ..." << endl;
     cout << "# N (non-goal state): [non-goal state ID] [fact ID 1] [fact ID 2] ..." << endl;
@@ -76,14 +76,37 @@
     // The initial state has id 0, so we'll start there.
     current_state_id = 0;
     dump_state(initial_state);
     SearchNode node = search_space.get_node(initial_state);
     node.close();
 }
 
+void ExhaustiveSearch::search() {
+    states_file.open("states.txt");
+    transitions_file.open("transitions.txt");
+    initialize();
+    utils::CountdownTimer timer(max_time);
+    while (status == IN_PROGRESS) {
+        status = step();
+        if (timer.is_expired()) {
+            log << "Time limit reached. Abort search." << endl;
+            status = TIMEOUT;
+            break;
+        }
+        if (state_registry.size() >= max_num_states) {
+            log << "Num states limit reached. Abort search." << endl;
+            status = RESOURCEOUT;
+            break;
+        }
+    }
+    states_file.close();
+    transitions_file.close();
+    log << "Actual search time: " << timer.get_elapsed_time() << endl;
+}
+
 void ExhaustiveSearch::print_statistics() const {
     statistics.print_detailed_statistics();
     search_space.print_statistics();
 }
 
 void ExhaustiveSearch::dump_state(const State &state) {
     char state_type = (task_properties::is_goal_state(task_proxy, state)) ? 'G' : 'N';
@@ -99,16 +122,14 @@
     std::cout << ss.str() << std::endl;
     states_file << ss.str() << "\n";
 }
 
 SearchStatus ExhaustiveSearch::step() {
     if (current_state_id == static_cast<int>(state_registry.size())) {
         utils::g_log << "Finished dumping the reachable state space." << endl;
-        states_file.close();
-        transitions_file.close();
         return FAILED;
     }
 
     State s = state_registry.lookup_state(StateID(current_state_id));
     statistics.inc_expanded();
 
     /* Next time we'll look at the next state that was created in the registry.
@@ -128,14 +149,17 @@
             transitions_file << s.get_id().value << " " << succ_state.get_id().value << "\n";
         }
 
         SearchNode node = search_space.get_node(succ_state);
         if (dump_states_to_file && node.is_new()) {
             dump_state(succ_state);
             node.close();
+            if (state_registry.size() >= max_num_states) {
+                return FAILED;
+            }
         }
     }
     return IN_PROGRESS;
 }
 
 static shared_ptr<SearchEngine> _parse(OptionParser &parser) {
     parser.document_synopsis(
@@ -143,14 +167,18 @@
         "Dump the reachable state space.");
     utils::add_log_options_to_parser(parser);
 
     parser.add_option<double>(
         "max_time",
         "The timit limit in seconds for generating the state space.",
         "infinity");
+    parser.add_option<int>(
+        "max_num_states",
+        "The timit on the maximum number of states in the state space.",
+        "infinity");
 
     Options opts = parser.parse();
 
     opts.set<OperatorCost>("cost_type", ONE);
     opts.set<int>("bound", numeric_limits<int>::max());
     opts.set<bool>("dump_atoms", true);
     opts.set<bool>("dump_states", true);
```

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/exhaustive_search.h`

 * *Files 7% similar despite different names*

```diff
@@ -12,26 +12,29 @@
 namespace exhaustive_search {
 class ExhaustiveSearch : public SearchEngine {
     int current_state_id;
     std::vector<std::vector<int>> fact_mapping;
 
     void dump_state(const State &state);
 
+    int max_num_states;
     bool dump_atoms_to_file;
     bool dump_states_to_file;
     bool dump_transitions_to_file;
 
     std::ofstream states_file;
     std::ofstream transitions_file;
 
 protected:
     virtual void initialize() override;
     virtual SearchStatus step() override;
 
 public:
     explicit ExhaustiveSearch(const options::Options &opts);
 
+    virtual void search() override;
+
     virtual void print_statistics() const override;
 };
 }
 
 #endif
```

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/idastar_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/idastar_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/idastar_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/idastar_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterated_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterated_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterated_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterated_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/iterative_deepening_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/lazy_search.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/lazy_search.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/lazy_search.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/lazy_search.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_astar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_astar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_eager.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_eager.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_eager_greedy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_eager_greedy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_eager_wastar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_eager_wastar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_lazy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_lazy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_greedy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_greedy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_wastar.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/plugin_lazy_wastar.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/search_common.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/search_common.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_engines/search_common.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_engines/search_common.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_node_info.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_node_info.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_progress.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_progress.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_progress.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_progress.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_space.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_space.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_space.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_space.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_statistics.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_statistics.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/search_statistics.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/search_statistics.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_id.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_id.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_registry.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_registry.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/state_registry.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/state_registry.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_id.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_id.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_proxy.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_proxy.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_proxy.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_proxy.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/causal_graph.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/causal_graph.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/causal_graph.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/causal_graph.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/incremental_successor_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/sampling.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/sampling.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/sampling.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/sampling.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/successor_generator_internals.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/task_properties.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/task_properties.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/task_properties.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/task_properties.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/task_utils/variable_order_finder.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/cost_adapted_task.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/delegating_task.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/delegating_task.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/delegating_task.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/delegating_task.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/domain_abstracted_task_factory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_goals_task.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_goals_task.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/modified_operator_costs_task.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/tasks/root_task.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/tasks/root_task.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/collections.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/collections.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/countdown_timer.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/countdown_timer.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/hash.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/hash.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/logging.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/logging.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/logging.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/logging.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/markup.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/markup.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/markup.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/markup.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/math.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/math.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/math.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/math.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/memory.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/memory.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/memory.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/memory.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng_options.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng_options.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/rng_options.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/rng_options.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/strings.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/strings.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/strings.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/strings.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system_unix.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system_unix.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/system_windows.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/system_windows.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/timer.cc` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/timer.cc`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/timer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/timer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/search/utils/tokenizer.h` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/search/utils/tokenizer.h`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/axiom_rules.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/axiom_rules.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/build_model.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/build_model.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/constraints.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/constraints.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/fact_groups.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/fact_groups.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/graph.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/graph.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/greedy_join.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/greedy_join.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/instantiate.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/instantiate.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/invariant_finder.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/invariant_finder.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/invariants.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/invariants.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/normalize.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/normalize.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/options.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/options.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/__init__.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/__init__.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/actions.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/actions.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/axioms.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/axioms.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/conditions.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/conditions.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/effects.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/effects.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/f_expression.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/f_expression.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/functions.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/functions.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/pddl_types.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/pddl_types.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl/tasks.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl/tasks.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/lisp_parser.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/lisp_parser.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/parsing_functions.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/parsing_functions.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_parser/pddl_file.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_parser/pddl_file.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/pddl_to_prolog.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/pddl_to_prolog.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue34-domain.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue34-domain.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue34-problem.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue34-problem.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue405-domain.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue405-domain.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-domain.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-domain.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-problem.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue49-orig-problem.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue58-domain.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue58-domain.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue7-domain.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue7-domain.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue7-problem.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue7-problem.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue73-domain.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue73-domain.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/regression-tests/issue73-problem.pddl` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/regression-tests/issue73-problem.pddl`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/sas_tasks.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/sas_tasks.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/sccs.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/sccs.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/simplify.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/simplify.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/split_rules.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/split_rules.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tests/test_normalization.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tests/test_scripts.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/timers.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/timers.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/tools.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/tools.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/translate.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/translate.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/scorpion/src/translate/variable_order.py` & `state_space_generator-0.1.8/state_space_generator/scorpion/src/translate/variable_order.py`

 * *Files identical despite different names*

### Comparing `state_space_generator-0.1.7/state_space_generator/state_space_generator.py` & `state_space_generator-0.1.8/state_space_generator/state_space_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import subprocess
 from pathlib import Path
 
 HERE = Path(__file__).resolve().parent
 
-def build_callstring(max_time: float):
+def build_callstring(max_time: float, max_num_states: int):
     result = "dump_reachable_search_space("
     if max_time is not None:
-        result += f"max_time={max_time}"
+        result += f"max_time={max_time},"
+    if max_num_states is not None:
+        result += f"max_num_states={max_num_states},"
     result +=  ")"
     return result
 
-def generate_state_space(domain: str, problem: str, max_time: str = None):
+def generate_state_space(domain: str, problem: str, max_time: str = None, max_num_states: int=None):
     command = [
         "python3",
         Path(HERE / 'scorpion/fast-downward.py').resolve(),
         "--keep-sas-file",
         Path(domain).resolve(),
         Path(problem).resolve(),
         "--translate-options",
         "--dump-static-predicates",
         "--dump-predicates",
         "--dump-constants",
         "--dump-static-atoms",
         "--dump-goal-atoms",
         "--search-options",
         "--search",
-        build_callstring(max_time)]
+        build_callstring(max_time, max_num_states)]
     print(f'Executing "{" ".join(map(str, command))}"')
     with open("run.log", "w") as file:
         subprocess.run(command, stdout=file,text=True)
 
 # for debugging purposes
 # python3 ./fast-downward.py ../../domain.pddl ../../p-1-0.pddl --translate-options --dump-static-predicates --dump-predicates --dump-constants --dump-static-atoms --dump-goal-atoms --search-options --search "dump_reachable_search_space(max_time=0)"
```

### Comparing `state_space_generator-0.1.7/state_space_generator.egg-info/SOURCES.txt` & `state_space_generator-0.1.8/state_space_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

