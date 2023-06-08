# Comparing `tmp/taskcluster-taskgraph-5.2.1.tar.gz` & `tmp/taskcluster-taskgraph-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-5.2.1.tar", last modified: Wed May 31 15:57:08 2023, max compression
+gzip compressed data, was "dist/taskcluster-taskgraph-5.3.0.tar", last modified: Thu Jun  8 20:00:01 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.2.1.tar` & `taskcluster-taskgraph-5.3.0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.888603 taskcluster-taskgraph-5.2.1/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/MANIFEST.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-05-31 15:57:08.888603 taskcluster-taskgraph-5.2.1/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/README.rst
--rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/pyproject.toml
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.858603 taskcluster-taskgraph-5.2.1/requirements/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      191 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/requirements/base.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)    20557 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/requirements/base.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/requirements/dev.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/requirements/dev.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/requirements/test.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8476 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/requirements/test.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-05-31 15:57:08.888603 taskcluster-taskgraph-5.2.1/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.848603 taskcluster-taskgraph-5.2.1/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.858603 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-05-31 15:57:08.000000 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3946 2023-05-31 15:57:08.000000 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-05-31 15:57:08.000000 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-05-31 15:57:08.000000 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)      215 2023-05-31 15:57:08.000000 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-05-31 15:57:08.000000 taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.858603 taskcluster-taskgraph-5.2.1/src/taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-05-31 15:55:34.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.868603 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1831 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/cancel.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9382 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/actions/util.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4583 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/config.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/filter_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15585 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4667 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/graph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.868603 taskcluster-taskgraph-5.2.1/src/taskgraph/loader/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/loader/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/loader/default.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/loader/transform.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/morph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.868603 taskcluster-taskgraph-5.2.1/src/taskgraph/optimize/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/optimize/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/parameters.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.868603 taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/hgrc
--rw-r--r--   0 ahal      (1000) ahal      (1000)    30243 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    44051 2023-05-02 13:20:13.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/run-task
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3132 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2397 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.868603 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5285 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10443 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6135 2023-05-31 13:37:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/from_deps.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.868603 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6826 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9800 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    51243 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.878603 taskcluster-taskgraph-5.2.1/src/taskgraph/util/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/archive.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      853 2023-05-31 13:37:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/hash.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/shell.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/templates.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18534 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8827 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2494 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-31 15:57:08.888603 taskcluster-taskgraph-5.2.1/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.2.1/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_actions_registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.2.1/test/test_create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_graph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/test/test_main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_morph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/test/test_optimize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_optimize_strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_parameters.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_scripts_fetch_content.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11792 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_scripts_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_transform_docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4891 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_from_deps.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_job.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_job_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_job_toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    23573 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.2.1/test/test_transforms_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_util_parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.2.1/test/test_util_python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_util_taskcluster.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_templates.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    14739 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_util_vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.1/test/test_util_verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_util_workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.1/test/test_util_yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/MANIFEST.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/README.rst
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/pyproject.toml
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/requirements/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      191 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/requirements/base.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    20557 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/requirements/base.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/requirements/dev.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/requirements/dev.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/requirements/test.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8476 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/requirements/test.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      215 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-06-08 19:59:10.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1831 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9382 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4583 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/config.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15585 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4667 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/graph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/morph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    30243 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    44960 2023-06-08 19:59:10.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3132 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2397 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5285 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10443 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/from_deps.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6826 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9800 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    51243 2023-06-08 14:51:24.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2502 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18534 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8827 2023-06-08 14:51:24.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2494 2023-06-08 14:51:24.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.3.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_actions_registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.3.0/test/test_create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_graph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/test/test_main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_morph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/test/test_optimize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_optimize_strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_parameters.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/test/test_scripts_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_transform_docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5880 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_job.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_job_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    23573 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/test/test_util_dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.3.0/test/test_util_python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_templates.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    14739 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_yaml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `taskcluster-taskgraph-5.2.1/LICENSE` & `taskcluster-taskgraph-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/PKG-INFO` & `taskcluster-taskgraph-5.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.2.1
+Version: 5.3.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.2.1/README.rst` & `taskcluster-taskgraph-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/pyproject.toml` & `taskcluster-taskgraph-5.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/requirements/base.txt` & `taskcluster-taskgraph-5.3.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/requirements/dev.txt` & `taskcluster-taskgraph-5.3.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/requirements/test.txt` & `taskcluster-taskgraph-5.3.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/setup.py` & `taskcluster-taskgraph-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.2.1
+Version: 5.3.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.2.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 test/test_transforms_from_deps.py
 test/test_transforms_job.py
 test/test_transforms_job_run_task.py
 test/test_transforms_job_toolchain.py
 test/test_transforms_notify.py
 test/test_transforms_task.py
 test/test_util_attributes.py
+test/test_util_dependencies.py
 test/test_util_docker.py
 test/test_util_memoize.py
 test/test_util_parameterization.py
 test/test_util_path.py
 test/test_util_python_path.py
 test/test_util_readonlydict.py
 test/test_util_schema.py
```

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.2.1"
+__version__ = "5.3.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/config.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/create.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/main.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/run-task`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import argparse
 import datetime
 import errno
 import io
 import json
 import os
 from pathlib import Path
+import platform
 import re
 import shutil
 import signal
 import socket
 import stat
 import subprocess
 import time
@@ -650,14 +651,32 @@
     # Unlike base_ref just above, there is no need to checkout the revision:
     # it's immediately available after the fetch.
     if base_rev and base_rev != NULL_REVISION:
         args = ["git", "fetch", "origin", base_rev]
 
         retry_required_command(b"vcs", args, cwd=destination_path, extra_env=env)
 
+    # If a ref was provided, it might be tag, so we need to make sure we fetch
+    # those. This is explicitly only done when base and head repo match,
+    # because it is the only scenario where tags could be present. (PRs, for
+    # example, always include an explicit rev.) Failure to do this could result
+    # in not having a tag, or worse: having an outdated version of one.
+    # `--force` is needed to be able to update an existing tag.
+    if ref and base_repo == head_repo:
+        args = [
+            "git",
+            "fetch",
+            "--tags",
+            "--force",
+            base_repo,
+            ref,
+        ]
+
+        retry_required_command(b"vcs", args, cwd=destination_path, extra_env=env)
+
     # If a ref isn't provided, we fetch all refs from head_repo, which may be slow
     args = [
         "git",
         "fetch",
         "--no-tags",
         head_repo,
         ref if ref else "+refs/heads/*:refs/remotes/work/*",
@@ -1049,21 +1068,28 @@
                 break
             print_line(prefix, data)
 
     monitor_process = Thread(target=capture_output)
     monitor_process.start()
     return process
 
+def _display_python_version():
+    print_line(
+        b"setup",
+        b"Python version: "+ bytes(platform.python_version(), 'utf-8')
+    )
+
 
 def main(args):
     os.environ["TASK_WORKDIR"] = os.getcwd()
     print_line(
         b"setup",
         b"run-task started in %s\n" % os.environ["TASK_WORKDIR"].encode("utf-8"),
     )
+    _display_python_version()
     running_as_root = IS_POSIX and os.getuid() == 0
 
     # Arguments up to '--' are ours. After are for the main task
     # to be executed.
     try:
         i = args.index("--")
         our_args = args[0:i]
```

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/task.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/from_deps.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 These transforms are useful when follow-up tasks are needed for some
 indeterminate subset of existing tasks. For example, running a signing task
 after each build task, whatever builds may exist.
 """
 from copy import deepcopy
 from textwrap import dedent
 
-from voluptuous import ALLOW_EXTRA, Any, Optional, Required
+from voluptuous import Any, Extra, Optional, Required
 
 from taskgraph.transforms.base import TransformSequence
 from taskgraph.util.attributes import attrmatch
 from taskgraph.util.dependencies import GROUP_BY_MAP
 from taskgraph.util.schema import Schema
 
 FROM_DEPS_SCHEMA = Schema(
@@ -66,17 +66,27 @@
                     """
                 If True, copy attributes from the dependency matching the
                 first kind in the `kinds` list (whether specified explicitly
                 or taken from `kind-dependencies`).
                 """.lstrip()
                 ),
             ): bool,
-        }
+            Optional(
+                "unique-kinds",
+                description=dedent(
+                    """
+                If true (the default), there must be only a single unique task
+                for each kind in a dependency group. Setting this to false
+                disables that requirement.
+                """.lstrip()
+                ),
+            ): bool,
+        },
+        Extra: object,
     },
-    extra=ALLOW_EXTRA,
 )
 """Schema for from_deps transforms."""
 
 transforms = TransformSequence()
 transforms.add_validate(FROM_DEPS_SCHEMA)
 
 
@@ -133,24 +143,27 @@
             groups = func(config, deps, arg)
         else:
             func = GROUP_BY_MAP[group_by]
             groups = func(config, deps)
 
         # Split the task, one per group.
         copy_attributes = from_deps.get("copy-attributes", False)
+        unique_kinds = from_deps.get("unique-kinds", True)
         for group in groups:
             # Verify there is only one task per kind in each group.
             group_kinds = {t.kind for t in group}
-            if len(group_kinds) < len(group):
+            if unique_kinds and len(group_kinds) < len(group):
                 raise Exception(
                     "The from_deps transforms only allow a single task per kind in a group!"
                 )
 
             new_task = deepcopy(task)
-            new_task["dependencies"] = {dep.kind: dep.label for dep in group}
+            new_task["dependencies"] = {
+                dep.kind if unique_kinds else dep.label: dep.label for dep in group
+            }
 
             # Set name and copy attributes from the primary kind.
             for kind in kinds:
                 if kind in group_kinds:
                     primary_kind = kind
                     break
             else:
```

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.3.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.3.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_actions_registry.py` & `taskcluster-taskgraph-5.3.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_create.py` & `taskcluster-taskgraph-5.3.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_decision.py` & `taskcluster-taskgraph-5.3.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_files_changed.py` & `taskcluster-taskgraph-5.3.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_generator.py` & `taskcluster-taskgraph-5.3.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_graph.py` & `taskcluster-taskgraph-5.3.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_main.py` & `taskcluster-taskgraph-5.3.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_morph.py` & `taskcluster-taskgraph-5.3.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_optimize.py` & `taskcluster-taskgraph-5.3.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.3.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_parameters.py` & `taskcluster-taskgraph-5.3.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.3.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.3.0/test/test_scripts_run_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -377,7 +377,22 @@
             base_ref="mybranch",
             base_rev=mock_git_repo["main"],
             ref=mock_git_repo["branch"],
             commit=mock_git_repo["branch"],
             ssh_key_file=None,
             ssh_known_hosts_file=None,
         )
+
+
+def test_display_python_version_should_output_python_versions_title(
+    run_task_mod, capsys
+):
+    run_task_mod._display_python_version()
+
+    assert ("Python version:" in capsys.readouterr().out) is True
+
+
+def test_display_python_version_should_output_python_versions(run_task_mod, capsys):
+    run_task_mod._display_python_version()
+
+    output = capsys.readouterr().out
+    assert ("Python version: 3." in output) or ("Python version: 2." in output) is True
```

### Comparing `taskcluster-taskgraph-5.2.1/test/test_target_tasks.py` & `taskcluster-taskgraph-5.3.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_taskgraph.py` & `taskcluster-taskgraph-5.3.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transform_docker_image.py` & `taskcluster-taskgraph-5.3.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_base.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_from_deps.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,23 @@
     assert tasks[1]["attributes"] == {"primary-kind-dependency": "foo"}
 
 
 def assert_group_by_attribute_dupe(e):
     handle_exception(e, exc=Exception)
 
 
+def assert_group_by_attribute_dupe_allowed(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 2
+    assert tasks[0]["dependencies"] == {"a": "a"}
+    assert tasks[0]["attributes"] == {"primary-kind-dependency": "foo"}
+    assert tasks[1]["dependencies"] == {"b": "b", "c": "c"}
+    assert tasks[1]["attributes"] == {"primary-kind-dependency": "foo"}
+
+
 def assert_copy_attributes(tasks):
     handle_exception(tasks)
     assert len(tasks) == 1
 
     task = tasks[0]
     assert task["attributes"] == {
         "build-type": "win",
@@ -130,14 +139,32 @@
             },
             id="group_by_attribute_dupe",
         ),
         pytest.param(
             # task
             {
                 "from-deps": {
+                    "unique-kinds": False,
+                    "group-by": {"attribute": "build-type"},
+                }
+            },
+            # kind config
+            None,
+            # deps
+            {
+                "a": make_task("a", attributes={"build-type": "linux"}, kind="foo"),
+                "b": make_task("b", attributes={"build-type": "win"}, kind="foo"),
+                "c": make_task("c", attributes={"build-type": "win"}, kind="foo"),
+            },
+            id="group_by_attribute_dupe_allowed",
+        ),
+        pytest.param(
+            # task
+            {
+                "from-deps": {
                     "group-by": {"attribute": "build-type"},
                     "copy-attributes": True,
                 }
             },
             # kind config
             None,
             # deps
```

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_job.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_transforms_task.py` & `taskcluster-taskgraph-5.3.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_attributes.py` & `taskcluster-taskgraph-5.3.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_docker.py` & `taskcluster-taskgraph-5.3.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_memoize.py` & `taskcluster-taskgraph-5.3.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.3.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_path.py` & `taskcluster-taskgraph-5.3.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_python_path.py` & `taskcluster-taskgraph-5.3.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.3.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_schema.py` & `taskcluster-taskgraph-5.3.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.3.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_templates.py` & `taskcluster-taskgraph-5.3.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_time.py` & `taskcluster-taskgraph-5.3.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.3.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_vcs.py` & `taskcluster-taskgraph-5.3.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_verify.py` & `taskcluster-taskgraph-5.3.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.3.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.2.1/test/test_util_yaml.py` & `taskcluster-taskgraph-5.3.0/test/test_util_yaml.py`

 * *Files identical despite different names*

