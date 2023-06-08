# Comparing `tmp/bluesky-1.8.3.tar.gz` & `tmp/bluesky-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluesky-1.8.3.tar", last modified: Fri Apr  8 17:32:17 2022, max compression
+gzip compressed data, was "bluesky-1.9.0.tar", last modified: Thu Aug 11 14:59:48 2022, max compression
```

## Comparing `bluesky-1.8.3.tar` & `bluesky-1.9.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.312557 bluesky-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-04-08 17:32:06.000000 bluesky-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-04-08 17:32:06.000000 bluesky-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-04-08 17:32:17.312557 bluesky-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-04-08 17:32:06.000000 bluesky-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.312557 bluesky-1.8.3/bluesky/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-04-08 17:32:17.312557 bluesky-1.8.3/bluesky/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    29856 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/bundlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.308557 bluesky-1.8.3/bluesky/callbacks/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24903 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/best_effort.py
--rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/broker.py
--rw-r--r--   0 runner    (1001) docker     (121)    14405 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)    25192 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/mpl_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5919 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/olog.py
--rw-r--r--   0 runner    (1001) docker     (121)     8840 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/callbacks/zmq.py
--rw-r--r--   0 runner    (1001) docker     (121)     8293 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/cntx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.308557 bluesky-1.8.3/bluesky/commandline/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/commandline/zmq_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     8881 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    13115 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/magics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10649 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/object_plans.py
--rw-r--r--   0 runner    (1001) docker     (121)    18814 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/plan_patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)    28660 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/plan_stubs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/plan_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    71737 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/plans.py
--rw-r--r--   0 runner    (1001) docker     (121)    44364 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (121)     8353 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    96997 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/run_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/simulators.py
--rw-r--r--   0 runner    (1001) docker     (121)    22563 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/suspenders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.312557 bluesky-1.8.3/bluesky/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     9682 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_bec.py
--rw-r--r--   0 runner    (1001) docker     (121)    24484 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6455 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_documents.py
--rw-r--r--   0 runner    (1001) docker     (121)    18127 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)    12892 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (121)    11386 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_legacy_plans.py
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_magics.py
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_multi_runs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21149 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_new_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_olog_cb.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_persistent_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    11354 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_plan_patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)    20514 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_plans.py
--rw-r--r--   0 runner    (1001) docker     (121)     2861 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_ramp_plan.py
--rw-r--r--   0 runner    (1001) docker     (121)    45364 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_run_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)    28674 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_scientific.py
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_simple_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_simulators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_snaking.py
--rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_supplemental_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7631 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_suspenders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    18514 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_vertical_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)    11088 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.312557 bluesky-1.8.3/bluesky/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    56478 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-04-08 17:32:06.000000 bluesky-1.8.3/bluesky/utils/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 17:32:17.308557 bluesky-1.8.3/bluesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-04-08 17:32:17.000000 bluesky-1.8.3/bluesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-04-08 17:32:17.000000 bluesky-1.8.3/bluesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 17:32:17.000000 bluesky-1.8.3/bluesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-08 17:32:17.000000 bluesky-1.8.3/bluesky.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-08 17:32:17.000000 bluesky-1.8.3/bluesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-08 17:32:17.000000 bluesky-1.8.3/bluesky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-04-08 17:32:06.000000 bluesky-1.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-04-08 17:32:17.312557 bluesky-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-04-08 17:32:06.000000 bluesky-1.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68573 2022-04-08 17:32:06.000000 bluesky-1.8.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.146866 bluesky-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-08-11 14:59:39.000000 bluesky-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-11 14:59:39.000000 bluesky-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-08-11 14:59:48.146866 bluesky-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-08-11 14:59:39.000000 bluesky-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.146866 bluesky-1.9.0/bluesky/
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-11 14:59:48.146866 bluesky-1.9.0/bluesky/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32208 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/bundlers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.142866 bluesky-1.9.0/bluesky/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24904 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/best_effort.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14405 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25192 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/mpl_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5919 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/olog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8840 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11687 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/callbacks/zmq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8293 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/cntx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.142866 bluesky-1.9.0/bluesky/commandline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/commandline/zmq_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8881 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13115 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/magics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10649 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/object_plans.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18816 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/plan_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29126 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/plan_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71714 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/plans.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44362 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14349 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    99364 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/run_engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22563 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/suspenders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.146866 bluesky-1.9.0/bluesky/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9682 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_bec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24484 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7551 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18187 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12892 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11386 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_legacy_plans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_magics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_multi_runs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21176 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_new_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_olog_cb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_persistent_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11354 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_plan_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22111 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_plans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2861 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_ramp_plan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45809 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_run_engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28674 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_scientific.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_simple_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_simulators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2417 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_snaking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_supplemental_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8249 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_suspenders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19567 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_vertical_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11088 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1628 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.146866 bluesky-1.9.0/bluesky/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)    58221 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-08-11 14:59:39.000000 bluesky-1.9.0/bluesky/utils/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 14:59:48.142866 bluesky-1.9.0/bluesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-08-11 14:59:48.000000 bluesky-1.9.0/bluesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-08-11 14:59:48.000000 bluesky-1.9.0/bluesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 14:59:48.000000 bluesky-1.9.0/bluesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-11 14:59:48.000000 bluesky-1.9.0/bluesky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-08-11 14:59:48.000000 bluesky-1.9.0/bluesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-11 14:59:48.000000 bluesky-1.9.0/bluesky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-08-11 14:59:39.000000 bluesky-1.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-11 14:59:48.146866 bluesky-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-08-11 14:59:39.000000 bluesky-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68573 2022-08-11 14:59:39.000000 bluesky-1.9.0/versioneer.py
```

### Comparing `bluesky-1.8.3/LICENSE` & `bluesky-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/PKG-INFO` & `bluesky-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: bluesky
-Version: 1.8.3
+Version: 1.9.0
 Summary: Experiment specification & orchestration.
 Home-page: https://github.com/bluesky/bluesky
 Author: danielballan
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -38,9 +37,7 @@
 
 [**Bluesky Documentation**](http://blueskyproject.io/bluesky).
 
 The Bluesky Project enables experimental science at the lab-bench or facility scale. It is a collection of Python libraries that are co-developed but independently useful and may be adopted *a la carte*.
 
 [**Bluesky Project Documentation**](http://blueskyproject.io).
 
-
-
```

### Comparing `bluesky-1.8.3/README.md` & `bluesky-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/bundlers.py` & `bluesky-1.9.0/bluesky/bundlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 from collections import deque
+import inspect
 from itertools import count, tee
 import time as ttime
+from typing import Any, Deque, Dict, FrozenSet, List, Tuple
 from event_model import DocumentNames
 from .log import doc_logger
+from .protocols import (
+    T, Callback, Configurable, PartialEvent, Descriptor, Flyable,
+    HasName, Readable, Reading, Subscribable, check_supports
+)
 from .utils import (
     new_uid,
     IllegalMessageSequence,
     _rearrange_into_parallel_dicts,
     short_uid,
     Msg,
+    maybe_await,
+    maybe_collect_asset_docs,
+    maybe_update_hints,
 )
 
+ObjDict = Dict[Any, Dict[str, T]]
+
 
 class RunBundler:
     def __init__(self, md, record_interruptions, emit, emit_sync, log):
         # state stolen from the RE
         self.bundling = False  # if we are in the middle of bundling readings
         self._bundle_name = None  # name given to event descriptor
         self._run_start_uid = None  # The (future) runstart uid
-        self._objs_read = deque()  # objects read in one Event
-        self._read_cache = deque()  # cache of obj.read() in one Event
+        self._objs_read: Deque[HasName] = deque()  # objects read in one Event
+        self._read_cache: Deque[Dict[str, Reading]] = deque()  # cache of obj.read() in one Event
         self._asset_docs_cache = deque()  # cache of obj.collect_asset_docs()
-        self._describe_cache = dict()  # cache of all obj.describe() output
-        self._config_desc_cache = dict()  # " obj.describe_configuration()
-        self._config_values_cache = dict()  # " obj.read_configuration() values
-        self._config_ts_cache = dict()  # " obj.read_configuration() timestamps
+        self._describe_cache: ObjDict[Descriptor] = dict()  # cache of all obj.describe() output
+        self._config_desc_cache: ObjDict[Descriptor] = dict()  # " obj.describe_configuration()
+        self._config_values_cache: ObjDict[Any] = dict()  # " obj.read_configuration() values
+        self._config_ts_cache: ObjDict[Any] = dict()  # " obj.read_configuration() timestamps
         self._descriptors = dict()  # cache of {name: (objs_frozen_set, doc)}
+        # cache of {obj: {objs_frozen_set: (name, uid)}}
+        self._local_descriptors: Dict[Any, Dict[FrozenSet[str], Tuple[str, str]]] = dict()
         self._sequence_counters = dict()  # a seq_num counter per stream
         self._teed_sequence_counters = dict()  # for if we redo data-points
-        self._monitor_params = dict()  # cache of {obj: (cb, kwargs)}
+        self._monitor_params: Dict[Subscribable, Tuple[Callback, Dict]] = dict()  # cache of {obj: (cb, kwargs)}
         self.run_is_open = False
         self._uncollected = set()  # objects after kickoff(), before collect()
         # we expect the RE to take care of the composition
         self._md = md
         # this is state on the RE, mirror it here rather than refer to
         # the parent
         self.record_interruptions = record_interruptions
@@ -163,20 +176,24 @@
         Expected message object is::
 
             Msg('read', obj)
         """
         if self.bundling:
             obj = msg.obj
             # if the object is not in the _describe_cache, cache it
+            # Note: there is a race condition between the code here
+            # and in monitor() and collect(), so if you do them concurrently
+            # on the same device you make obj.describe() calls multiple times.
+            # As this is harmless and not an expected use case, we don't guard
+            # against it. Reading multiple devices concurrently works fine.
             if obj not in self._describe_cache:
-                # Validate that there is no data key name collision.
-                data_keys = obj.describe()
-                self._describe_cache[obj] = data_keys
-                self._config_desc_cache[obj] = obj.describe_configuration()
-                self._cache_config(obj)
+                await self._cache_describe(obj)
+            if obj not in self._config_desc_cache:
+                await self._cache_describe_config(obj)
+                await self._cache_read_config(obj)
 
             # check that current read collides with nothing else in
             # current event
             cur_keys = set(self._describe_cache[obj].keys())
             for read_obj in self._objs_read:
                 # that is, field names
                 known_keys = self._describe_cache[read_obj].keys()
@@ -192,26 +209,42 @@
 
             # Stash the results, which will be emitted the next time _save is
             # called --- or never emitted if _drop is called instead.
             self._read_cache.append(reading)
             # Ask the object for any resource or datum documents is has cached
             # and cache them as well. Likewise, these will be emitted if and
             # when _save is called.
-            if hasattr(obj, "collect_asset_docs"):
-                self._asset_docs_cache.extend(
-                    obj.collect_asset_docs(*msg.args, **msg.kwargs)
-                )
+            self._asset_docs_cache.extend(
+                maybe_collect_asset_docs(msg, obj, *msg.args, **msg.kwargs)
+            )
 
         return reading
 
-    def _cache_config(self, obj):
+    async def _cache_describe(self, obj):
+        "Read the object's describe and cache it."
+        obj = check_supports(obj, Readable)
+        self._describe_cache[obj] = await maybe_await(obj.describe())
+
+    async def _cache_describe_config(self, obj):
+        "Read the object's describe_configuration and cache it."
+        if isinstance(obj, Configurable):
+            conf_keys = await maybe_await(obj.describe_configuration())
+        else:
+            conf_keys = {}
+        self._config_desc_cache[obj] = conf_keys
+
+    async def _cache_read_config(self, obj):
         "Read the object's configuration and cache it."
+        if isinstance(obj, Configurable):
+            conf = await maybe_await(obj.read_configuration())
+        else:
+            conf = {}
         config_values = {}
         config_ts = {}
-        for key, val in obj.read_configuration().items():
+        for key, val in conf.items():
             config_values[key] = val["value"]
             config_ts[key] = val["timestamp"]
         self._config_values_cache[obj] = config_values
         self._config_ts_cache[obj] = config_ts
 
     async def monitor(self, msg):
         """
@@ -225,37 +258,41 @@
         Expected message object is::
 
             Msg('monitor', obj, **kwargs)
             Msg('monitor', obj, name='event-stream-name', **kwargs)
 
         where kwargs are passed through to ``obj.subscribe()``
         """
-        obj = msg.obj
+        obj = check_supports(msg.obj, Subscribable)
         if msg.args:
             raise ValueError(
                 "The 'monitor' Msg does not accept positional " "arguments."
             )
         kwargs = dict(msg.kwargs)
         name = kwargs.pop("name", short_uid("monitor"))
         if obj in self._monitor_params:
             raise IllegalMessageSequence(
                 "A 'monitor' message was sent for {}"
                 "which is already monitored".format(obj)
             )
         descriptor_uid = new_uid()
-        data_keys = obj.describe()
-        config = {obj.name: {"data": {}, "timestamps": {}}}
-        config[obj.name]["data_keys"] = obj.describe_configuration()
-        for key, val in obj.read_configuration().items():
-            config[obj.name]["data"][key] = val["value"]
-            config[obj.name]["timestamps"][key] = val["timestamp"]
+        if obj not in self._describe_cache:
+            await self._cache_describe(obj)
+        if obj not in self._config_desc_cache:
+            await self._cache_describe_config(obj)
+            await self._cache_read_config(obj)
+        data_keys = self._describe_cache[obj]
+        config = {obj.name: {
+            "data": self._config_values_cache[obj],
+            "timestamps": self._config_ts_cache[obj],
+            "data_keys": self._config_desc_cache[obj]
+        }}
         object_keys = {obj.name: list(data_keys)}
         hints = {}
-        if hasattr(obj, "hints"):
-            hints.update({obj.name: obj.hints})
+        maybe_update_hints(hints, obj)
         desc_doc = dict(
             run_start=self._run_start_uid,
             time=ttime.time(),
             data_keys=data_keys,
             uid=descriptor_uid,
             configuration=config,
             hints=hints,
@@ -266,30 +303,42 @@
                          "data keys %r (run_uid=%r)", name, data_keys.keys(),
                          self._run_start_uid,
                          extra={'doc_name': 'descriptor',
                                 'run_uid': self._run_start_uid,
                                 'data_keys': data_keys.keys()})
         seq_num_counter = count(1)
 
-        def emit_event(*args, **kwargs):
-            # Ignore the inputs. Use this call as a signal to call read on the
-            # object, a crude way to be sure we get all the info we need.
-            data, timestamps = _rearrange_into_parallel_dicts(obj.read())
+        def emit_event(readings: Dict[str, Reading] = None, *args, **kwargs):
+            if readings is not None:
+                # We were passed something we can use, but check no args or kwargs
+                assert not args and not kwargs, \
+                    "If subscribe callback called with readings, " \
+                    "args and kwargs are not supported."
+            else:
+                # Ignore the inputs. Use this call as a signal to call read on the
+                # object, a crude way to be sure we get all the info we need.
+                readable_obj = check_supports(obj, Readable)
+                readings = readable_obj.read()
+                assert not inspect.isawaitable(readings), \
+                    f"{readable_obj} has async read() method and the callback " \
+                    "passed to subscribe() was not called with Dict[str, Reading]"
+            data, timestamps = _rearrange_into_parallel_dicts(readings)
             doc = dict(
                 descriptor=descriptor_uid,
                 time=ttime.time(),
                 data=data,
                 timestamps=timestamps,
                 seq_num=next(seq_num_counter),
                 uid=new_uid(),
             )
             self.emit_sync(DocumentNames.event, doc)
 
         self._monitor_params[obj] = emit_event, kwargs
         await self.emit(DocumentNames.descriptor, desc_doc)
+        # TODO: deprecate **kwargs when Ophyd.v2 is available
         obj.subscribe(emit_event, **kwargs)
 
     def record_interruption(self, content):
         """
         Emit an event in the 'interruptions' event stream.
 
         If we are not inside a run or if self.record_interruptions is False,
@@ -319,15 +368,15 @@
         """
         Stop monitoring; i.e., remove the callback emitting event documents.
 
         Expected message object is::
 
             Msg('unmonitor', obj)
         """
-        obj = msg.obj
+        obj = check_supports(msg.obj, Subscribable)
         if obj not in self._monitor_params:
             raise IllegalMessageSequence(
                 f"Cannot 'unmonitor' {obj}; it is not " "being monitored."
             )
         cb, kwargs = self._monitor_params[obj]
         obj.clear_sub(cb)
         del self._monitor_params[obj]
@@ -388,24 +437,23 @@
             config = {}
             object_keys = {}
             hints = {}
             for obj in objs_read:
                 dks = self._describe_cache[obj]
                 obj_name = obj.name
                 # dks is an OrderedDict. Record that order as a list.
-                object_keys[obj.name] = list(dks)
+                object_keys[obj_name] = list(dks)
                 for field, dk in dks.items():
                     dk["object_name"] = obj_name
                 data_keys.update(dks)
                 config[obj_name] = {}
                 config[obj_name]["data"] = self._config_values_cache[obj]
                 config[obj_name]["timestamps"] = self._config_ts_cache[obj]
                 config[obj_name]["data_keys"] = self._config_desc_cache[obj]
-                if hasattr(obj, "hints"):
-                    hints[obj_name] = obj.hints
+                maybe_update_hints(hints, obj)
             descriptor_uid = new_uid()
             descriptor_doc = dict(
                 run_start=self._run_start_uid,
                 time=ttime.time(),
                 data_keys=data_keys,
                 uid=descriptor_uid,
                 configuration=config,
@@ -569,71 +617,38 @@
 
             Msg('complete', flyer, group=<GROUP>)
 
         where <GROUP> is a hashable identifier.
         """
         ...
 
-    async def collect(self, msg):
-        """
-        Collect data cached by a flyer and emit documents.
-
-        Expect message object is
-
-            Msg('collect', collect_obj)
-            Msg('collect', flyer_object, stream=True, return_payload=False)
-        """
-        collect_obj = msg.obj
-
-        if not self.run_is_open:
-            # sanity check -- 'kickoff' should catch this and make this
-            # code path impossible
-            raise IllegalMessageSequence(
-                "A 'collect' message was sent but no run is open."
-            )
-        self._uncollected.discard(collect_obj)
-
-        if hasattr(collect_obj, "collect_asset_docs"):
-            # Resource and Datum documents
-            for name, doc in collect_obj.collect_asset_docs():
-                # Add a 'run_start' field to the resource document on its way out.
-                if name == "resource":
-                    doc["run_start"] = self._run_start_uid
-                await self.emit(DocumentNames(name), doc)
-
-        collect_obj_config = {}
-        bulk_data = {}
-        local_descriptors = {}  # hashed on objs_read, not (name, objs_read)
+    async def _cache_describe_collect(self, collect_obj: Flyable):
+        "Read the object's describe_collect and cache it."
+        describe_collect = await maybe_await(collect_obj.describe_collect())
+        collect_obj_config: Dict[str, Dict[str, Any]] = {}
+        local_descriptors: Dict[FrozenSet[str], Tuple[str, str]] = {}
         # collect_obj.describe_collect() returns a dictionary like this:
         #     {name_for_desc1: data_keys_for_desc1,
         #      name_for_desc2: data_keys_for_desc2, ...}
-        for stream_name, stream_data_keys in collect_obj.describe_collect().items():
+        for stream_name, stream_data_keys in describe_collect.items():
             if stream_name not in self._descriptors:
                 # We do not have an Event Descriptor for this set.
                 descriptor_uid = new_uid()
                 # if we have not yet read the configuration, do so
                 if collect_obj.name not in collect_obj_config:
-                    _config = collect_obj_config[collect_obj.name] = {
-                        "data": {},
-                        "timestamps": {},
-                        "data_keys": {}
+                    if collect_obj not in self._config_desc_cache:
+                        await self._cache_describe_config(collect_obj)
+                        await self._cache_read_config(collect_obj)
+                    collect_obj_config[collect_obj.name] = {
+                        "data": self._config_values_cache[collect_obj],
+                        "timestamps": self._config_ts_cache[collect_obj],
+                        "data_keys": self._config_desc_cache[collect_obj]
                     }
-                    # but read_configuration is optional
-                    if hasattr(collect_obj, "read_configuration"):
-                        doc_logger.debug("reading configuration from %s", collect_obj)
-                        _config['data_keys'].update(collect_obj.describe_configuration())
-                        for config_key, config in collect_obj.read_configuration().items():
-                            _config["data"][config_key] = config["value"]
-                            _config["timestamps"][config_key] = config["timestamp"]
-                    else:
-                        doc_logger.debug("%s has no read_configuration method", collect_obj)
-
                 hints = {}
-                if hasattr(collect_obj, "hints"):
-                    hints.update({collect_obj.name: collect_obj.hints})
+                maybe_update_hints(hints, collect_obj)
                 doc = dict(
                     run_start=self._run_start_uid,
                     time=ttime.time(),
                     data_keys=stream_data_keys,
                     uid=descriptor_uid,
                     name=stream_name,
                     configuration=collect_obj_config,
@@ -656,54 +671,80 @@
                         "Mismatched objects read, "
                         "expected {!s}, "
                         "got {!s}".format(stream_data_keys, objs_read)
                     )
 
             descriptor_uid = doc["uid"]
             local_descriptors[frozenset(stream_data_keys)] = (stream_name, descriptor_uid)
+        self._local_descriptors[collect_obj] = local_descriptors
+
+    async def collect(self, msg):
+        """
+        Collect data cached by a flyer and emit documents.
+
+        Expect message object is
+
+            Msg('collect', collect_obj)
+            Msg('collect', flyer_object, stream=True, return_payload=False)
+        """
+        collect_obj = check_supports(msg.obj, Flyable)
+
+        if not self.run_is_open:
+            # sanity check -- 'kickoff' should catch this and make this
+            # code path impossible
+            raise IllegalMessageSequence(
+                "A 'collect' message was sent but no run is open."
+            )
+        self._uncollected.discard(collect_obj)
 
-            bulk_data[descriptor_uid] = []
+        # Resource and Datum documents
+        for name, doc in maybe_collect_asset_docs(msg, collect_obj):
+            # Add a 'run_start' field to the resource document on its way out.
+            if name == "resource":
+                doc["run_start"] = self._run_start_uid
+            await self.emit(DocumentNames(name), doc)
+
+        # Populate descriptors and local descriptors from describe_collect
+        # if not already called
+        if collect_obj not in self._local_descriptors:
+            await self._cache_describe_collect(collect_obj)
+        local_descriptors = self._local_descriptors[collect_obj]
 
         # If stream is True, run 'event' subscription per document.
         # If stream is False, run 'bulk_events' subscription once.
         stream = msg.kwargs.get("stream", False)
         # If True, accumulate all the Events in memory and return them at the
         # end, providing the plan access to the Events. If False, do not
         # accumulate, and return None.
         return_payload = msg.kwargs.get('return_payload', True)
         payload = []
+        bulk_data: Dict[str, List[PartialEvent]] = {}
 
         for ev in collect_obj.collect():
             if return_payload:
                 payload.append(ev)
 
             objs_read = frozenset(ev["data"])
             stream_name, descriptor_uid = local_descriptors[objs_read]
             seq_num = next(self._sequence_counters[stream_name])
-
             event_uid = new_uid()
-
-            reading = ev["data"]
-            for key in ev["data"]:
-                reading[key] = reading[key]
-            ev["data"] = reading
             ev["descriptor"] = descriptor_uid
             ev["seq_num"] = seq_num
             ev["uid"] = event_uid
 
             if stream:
                 doc_logger.debug("[event] document is emitted with data keys %r (run_uid=%r)",
                                  ev['data'].keys(), self._run_start_uid,
                                  event_uid,
                                  extra={'doc_name': 'event',
                                         'run_uid': self._run_start_uid,
                                         'data_keys': ev['data'].keys()})
                 await self.emit(DocumentNames.event, ev)
             else:
-                bulk_data[descriptor_uid].append(ev)
+                bulk_data.setdefault(descriptor_uid, []).append(ev)
 
         if not stream:
             await self.emit(DocumentNames.bulk_events, bulk_data)
             doc_logger.debug("[bulk events] document is emitted for descriptors (run_uid=%r)",
                              self._run_start_uid,
                              extra={'doc_name': 'bulk_events',
                                     'run_uid': self._run_start_uid})
@@ -732,8 +773,8 @@
         # Invalidate any event descriptors that include this object.
         # New event descriptors, with this new configuration, will
         # be created for any future event documents.
         for name in list(self._descriptors):
             obj_set, _ = self._descriptors[name]
             if obj in obj_set:
                 del self._descriptors[name]
-        self._cache_config(obj)
+        await self._cache_read_config(obj)
```

### Comparing `bluesky-1.8.3/bluesky/callbacks/__init__.py` & `bluesky-1.9.0/bluesky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/best_effort.py` & `bluesky-1.9.0/bluesky/callbacks/best_effort.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                 fig = plt.figure(fig_name)
 
             if not fig.axes:
                 if len(columns) < 5:
                     layout = (len(columns), 1)
                 else:
                     nrows = ncols = int(np.ceil(np.sqrt(len(columns))))
-                    while (nrows - 1) * ncols > len(columns):
+                    while (nrows - 1) * ncols >= len(columns):
                         nrows -= 1
                     layout = (nrows, ncols)
                 if ndims == 1:
                     share_kwargs = {'sharex': True}
                 elif ndims == 2:
                     share_kwargs = {'sharex': True, 'sharey': True}
                 else:
```

### Comparing `bluesky-1.8.3/bluesky/callbacks/broker.py` & `bluesky-1.9.0/bluesky/callbacks/broker.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/core.py` & `bluesky-1.9.0/bluesky/callbacks/core.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/fitting.py` & `bluesky-1.9.0/bluesky/callbacks/fitting.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/mpl_plotting.py` & `bluesky-1.9.0/bluesky/callbacks/mpl_plotting.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/olog.py` & `bluesky-1.9.0/bluesky/callbacks/olog.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/stream.py` & `bluesky-1.9.0/bluesky/callbacks/stream.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/callbacks/zmq.py` & `bluesky-1.9.0/bluesky/callbacks/zmq.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/cntx.py` & `bluesky-1.9.0/bluesky/cntx.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/commandline/zmq_proxy.py` & `bluesky-1.9.0/bluesky/commandline/zmq_proxy.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/examples.py` & `bluesky-1.9.0/bluesky/examples.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/interactive.py` & `bluesky-1.9.0/bluesky/interactive.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/log.py` & `bluesky-1.9.0/bluesky/log.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/magics.py` & `bluesky-1.9.0/bluesky/magics.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/object_plans.py` & `bluesky-1.9.0/bluesky/object_plans.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/plan_patterns.py` & `bluesky-1.9.0/bluesky/plan_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
                 flag = not flag
             # Now the flag is True if the motor is out of place in the list of arguments
             if flag:
                 return False
         return True
 
     # div_4 - the correct number of elements for pattern 1, div_5 - for pattern 2
-    div_4, div_5 = not(len(args) % 4), (len(args) > 4) and not((len(args) - 4) % 5)
+    div_4, div_5 = not (len(args) % 4), (len(args) > 4) and not ((len(args) - 4) % 5)
 
     # Check the number of elements in 'args'
     if not div_4 and not div_5:
         raise ValueError(f"Wrong number of elements in 'args': len(args) = {len(args)}")
 
     args_valid = False
     if div_4 and not div_5:
```

### Comparing `bluesky-1.8.3/bluesky/plan_stubs.py` & `bluesky-1.9.0/bluesky/plan_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import itertools
 import uuid
 from cycler import cycler
-from . import utils
 import operator
 from functools import reduce
 from collections.abc import Iterable
 import time
 import warnings
 
 try:
     # cytools is a drop-in replacement for toolz, implemented in Cython
     from cytools import partition
 except ImportError:
     from toolz import partition
 
-
+from .protocols import Triggerable
 from .utils import (
+    get_hinted_fields,
+    merge_cycler,
     separate_devices,
     all_safe_rewind,
     Msg,
     ensure_generator,
     short_uid as _short_uid,
 )
 
@@ -47,15 +48,15 @@
 
 
 def save():
     """
     Close a bundle of readings and emit a completed Event document.
 
     Yields
-    -------
+    ------
     msg : Msg
         Msg('save')
 
     See Also
     --------
     :func:`bluesky.plan_stubs.create`
     """
@@ -247,15 +248,15 @@
     :func:`bluesky.plan_stubs.abs_set`
     :func:`bluesky.plan_stubs.mvr`
     """
     group = group or str(uuid.uuid4())
     status_objects = []
 
     cyl = reduce(operator.add, [cycler(obj, [val]) for obj, val in partition(2, args)])
-    (step,) = utils.merge_cycler(cyl)
+    (step,) = merge_cycler(cyl)
     for obj, val in step.items():
         ret = yield Msg('set', obj, val, group=group, **kwargs)
         status_objects.append(ret)
     yield Msg('wait', None, group=group)
     return tuple(status_objects)
 
 
@@ -337,15 +338,15 @@
 
     Returns
     -------
     val : Any or None
         The "single" value of the device
 
     """
-    hints = getattr(obj, 'hints', {}).get("fields", [])
+    hints = get_hinted_fields(obj)
     if len(hints) > 1:
         msg = (
             f"Your object {obj} ({obj.name}.{getattr(obj, 'dotted_name', '')}) "
             f"has {len(hints)} items hinted ({hints}).  We do not know how to "
             "pick out a single value.  Please adjust the hinting by setting the "
             "kind of the components of this device or by reading one of its components"
         )
@@ -823,23 +824,26 @@
     return (yield Msg('open_run', **(md or {})))
 
 
 def close_run(exit_status=None, reason=None):
     """
     Mark the end of the current 'run'. Emit a RunStop document.
 
-    Yields
-    ------
-    msg : Msg
-        Msg('close_run')
+    Parameters
+    ----------
     exit_status : {None, 'success', 'abort', 'fail'}
         The exit status to report in the Stop document
     reason : str, optional
         Long-form description of why the run ended
 
+    Yields
+    ------
+    msg : Msg
+        Msg('close_run')
+
     See Also
     --------
     :func:`bluesky.plans_stubs.open_run`
     """
     return (yield Msg('close_run', exit_status=exit_status, reason=reason))
 
 
@@ -879,38 +883,55 @@
         name is 'primary'
 
     Yields
     ------
     msg : Msg
         messages to 'trigger', 'wait' and 'read'
     """
+    from .preprocessors import contingency_wrapper
     # If devices is empty, don't emit 'create'/'save' messages.
     if not devices:
         yield from null()
     devices = separate_devices(devices)  # remove redundant entries
     rewindable = all_safe_rewind(devices)  # if devices can be re-triggered
 
     def inner_trigger_and_read():
         grp = _short_uid('trigger')
         no_wait = True
         for obj in devices:
-            if hasattr(obj, 'trigger'):
+            if isinstance(obj, Triggerable):
                 no_wait = False
                 yield from trigger(obj, group=grp)
         # Skip 'wait' if none of the devices implemented a trigger method.
         if not no_wait:
             yield from wait(group=grp)
         yield from create(name)
-        ret = {}  # collect and return readings to give plan access to them
-        for obj in devices:
-            reading = (yield from read(obj))
-            if reading is not None:
-                ret.update(reading)
-        yield from save()
+
+        def read_plan():
+            ret = {}  # collect and return readings to give plan access to them
+            for obj in devices:
+                reading = (yield from read(obj))
+                if reading is not None:
+                    ret.update(reading)
+            return ret
+
+        def standard_path():
+            yield from save()
+
+        def exception_path(exp):
+            yield from drop()
+            raise exp
+
+        ret = yield from contingency_wrapper(
+            read_plan(),
+            except_plan=exception_path,
+            else_plan=standard_path
+            )
         return ret
+
     from .preprocessors import rewindable_wrapper
     return (yield from rewindable_wrapper(inner_trigger_and_read(),
                                           rewindable))
 
 
 def broadcast_msg(command, objs, *args, **kwargs):
     """
```

### Comparing `bluesky-1.8.3/bluesky/plan_tools.py` & `bluesky-1.9.0/bluesky/plan_tools.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/plans.py` & `bluesky-1.9.0/bluesky/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from cytools import partition
 except ImportError:
     from toolz import partition
 
 from . import plan_patterns
 
 from . import utils
-from .utils import Msg
+from .utils import Msg, get_hinted_fields
 
 from . import preprocessors as bpp
 from . import plan_stubs as bps
 
 
 def count(detectors, num=1, delay=None, *, per_shot=None, md=None):
     """
@@ -154,15 +154,15 @@
            'plan_pattern_args': dict(args=md_args),
            'hints': {},
            }
     _md.update(md or {})
 
     x_fields = []
     for motor in motors:
-        x_fields.extend(getattr(motor, 'hints', {}).get('fields', []))
+        x_fields.extend(get_hinted_fields(motor))
 
     default_dimensions = [(x_fields, 'primary')]
 
     default_hints = {}
     if len(x_fields) > 0:
         default_hints.update(dimensions=default_dimensions)
 
@@ -1083,15 +1083,15 @@
 
     # Give a hint that the motors all lie along the same axis
     # [(['motor1', 'motor2', ...], 'primary'), ] is 1D (this case)
     # [ ('motor1', 'primary'), ('motor2', 'primary'), ... ] is 2D for example
     # call x_fields because these are meant to be the x (independent) axis
     x_fields = []
     for motor in motors:
-        x_fields.extend(getattr(motor, 'hints', {}).get('fields', []))
+        x_fields.extend(get_hinted_fields(motor))
 
     default_dimensions = [(x_fields, 'primary')]
 
     default_hints = {}
     if len(x_fields) > 0:
         default_hints.update(dimensions=default_dimensions)
```

### Comparing `bluesky-1.8.3/bluesky/preprocessors.py` & `bluesky-1.9.0/bluesky/preprocessors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import generator_stop
 
 from collections import OrderedDict, deque, ChainMap
 from collections.abc import Iterable
 import uuid
-from .utils import (normalize_subs_input, root_ancestor,
+from .utils import (get_hinted_fields, normalize_subs_input, root_ancestor,
                     separate_devices,
                     Msg, ensure_generator, single_gen,
                     short_uid as _short_uid, make_decorator,
                     RunEngineControlException, merge_axis)
 from functools import wraps
 from .plan_stubs import (open_run, close_run, mv, pause, trigger_and_read)
 
@@ -992,15 +992,15 @@
         reading = yield Msg('read', obj)
         if reading is None:
             # this plan may be being list-ified
             print("*** all positions for {m.name} are "
                   "relative to current position ***".format(m=obj))
             cur_pos = 0
         else:
-            fields = getattr(obj, 'hints', {}).get('fields', [])
+            fields = get_hinted_fields(obj)
             if len(fields) == 1:
                 k, = fields
                 cur_pos = reading[k]['value']
             elif len(fields) == 0:
                 k = list(reading.keys())[0]
                 cur_pos = reading[k]['value']
             else:
```

### Comparing `bluesky-1.8.3/bluesky/run_engine.py` & `bluesky-1.9.0/bluesky/run_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 from datetime import datetime
 import sys
 from warnings import warn
-from inspect import Parameter, Signature
+from inspect import Parameter, Signature, iscoroutine
 from itertools import count
 from collections import deque, defaultdict, ChainMap
 from enum import Enum
 import functools
 import inspect
 from contextlib import ExitStack
 import threading
 import weakref
 from dataclasses import dataclass
 import typing
-from .bundlers import RunBundler
-from . import protocols as bs_protocols
+from .bundlers import RunBundler, maybe_await
+from .protocols import (Flyable, Movable, Pausable, Readable, Stageable,
+                        Stoppable, Triggerable, check_supports)
 
 import concurrent
 
 from event_model import DocumentNames, schema_validators
 from .log import logger, msg_logger, state_logger, ComposableLogAdapter
 from super_state_machine.machines import StateMachine
 from super_state_machine.extras import PropertyMachine
@@ -34,15 +35,15 @@
 
 from .utils import (CallbackRegistry, SigintHandler,
                     normalize_subs_input, AsyncInput,
                     NoReplayAllowed, RequestAbort, RequestStop,
                     RunEngineInterrupted, IllegalMessageSequence,
                     FailedPause, FailedStatus, InvalidCommand,
                     PlanHalt, Msg, ensure_generator, single_gen,
-                    DefaultDuringTask)
+                    DefaultDuringTask, warn_if_msg_args_or_kwargs)
 
 
 class _RunEnginePanic(Exception):
     ...
 
 
 @dataclass
@@ -322,15 +323,15 @@
 
     """
 
     _state = LoggingPropertyMachine(RunEngineStateMachine)
     _UNCACHEABLE_COMMANDS = ['pause', 'subscribe', 'unsubscribe', 'stage',
                              'unstage', 'monitor', 'unmonitor', 'open_run',
                              'close_run', 'install_suspender',
-                             'remove_suspender']
+                             'remove_suspender', '_start_suspender']
 
     @property
     def state(self):
         return self._state
 
     @property
     def deferred_pause_requested(self):
@@ -349,15 +350,16 @@
         return self._deferred_pause_requested
 
     def __init__(self, md=None, *, loop=None, preprocessors=None,
                  context_managers=None, md_validator=None,
                  scan_id_source=default_scan_id_source,
                  during_task=None, call_returns_result=False):
         if loop is None:
-            loop = get_bluesky_event_loop()
+            loop = asyncio.new_event_loop()
+            set_bluesky_event_loop(loop)
         self._th = _ensure_event_loop_running(loop)
         self._state_lock = threading.RLock()
         self._loop = loop
         if sys.version_info < (3, 8):
             self._loop_for_kwargs = {'loop': self._loop}
         else:
             self._loop_for_kwargs = {}
@@ -418,15 +420,15 @@
         if during_task is None:
             during_task = DefaultDuringTask()
         self._during_task = during_task
 
         # The RunEngine keeps track of a *lot* of state.
         # All flags and caches are defined here with a comment. Good luck.
         self._call_returns_result = call_returns_result  # should __call__ return UIDs or plan value
-        self._run_bundlers = {}  # a mapping of open run -> bundlers
+        self._run_bundlers: typing.Dict[typing.Any, RunBundler] = {}  # a mapping of open run -> bundlers
         self._metadata_per_call = {}  # for all runs generated by one __call__
         self._deferred_pause_requested = False  # pause at next 'checkpoint'
         self._exception = None  # stored and then raised in the _run loop
         self._interrupted = False  # True if paused, aborted, or failed
         self._staged = set()  # objects staged, not yet unstaged
         self._objs_seen = set()  # all objects seen
         self._movable_objs_touched = set()  # objects we moved at any point
@@ -460,15 +462,16 @@
             'trigger': self._trigger,
             'sleep': self._sleep,
             'wait': self._wait,
             'checkpoint': self._checkpoint,
             'clear_checkpoint': self._clear_checkpoint,
             'rewindable': self._rewindable,
             'pause': self._pause,
-            'resume': self._resume,
+            '_resume_from_suspender': self._resume,
+            '_start_suspender': self._start_suspender,
             'collect': self._collect,
             'kickoff': self._kickoff,
             'complete': self._complete,
             'configure': self._configure,
             'stage': self._stage,
             'unstage': self._unstage,
             'subscribe': self._subscribe,
@@ -928,16 +931,17 @@
         for current_run in self._run_bundlers.values():
             current_run.record_interruption('resume')
         new_plan = self._rewind()
         self._plan_stack.append(new_plan)
         self._response_stack.append(None)
         # Notify Devices of the resume in case they want to clean up.
         for obj in self._objs_seen:
-            if hasattr(obj, 'resume'):
-                obj.resume()
+            if isinstance(obj, Pausable):
+                fut = asyncio.run_coroutine_threadsafe(maybe_await(obj.resume()), self._loop)
+                fut.result()
         plan_return = self._resume_task()
         if self._interrupted:
             raise RunEngineInterrupted(self.pause_msg) from None
 
         if self._call_returns_result:
             run_engine_result = self._create_result(plan_return)
             return run_engine_result
@@ -1143,78 +1147,84 @@
                 self._interrupted = True
                 with self._state_lock:
                     self._exception = FailedPause()
                 was_paused = self._state == 'paused'
                 self._state = 'aborting'
                 if not was_paused:
                     self._task.cancel()
-
             if justification is not None:
-                print("Justification for this suspension:\n%s" % justification)
-            for current_run in self._run_bundlers.values():
-                current_run.record_interruption('resume')
-            # During suspend, all motors should be stopped. Call stop() on
-            # every object we ever set().
-            self._stop_movable_objects(success=True)
-            # Notify Devices of the pause in case they want to clean up.
-            for obj in self._objs_seen:
-                if hasattr(obj, 'pause'):
-                    try:
-                        obj.pause()
-                    except NoReplayAllowed:
-                        self._reset_checkpoint_state_meth()
-
-            # rewind to the last checkpoint
-            new_plan = self._rewind()
-            # queue up the cached messages
-            self._plan_stack.append(new_plan)
-            self._response_stack.append(None)
-
-            self._plan_stack.append(single_gen(
-                Msg('rewindable', None, self.rewindable)))
-            self._response_stack.append(None)
+                print(f"Justification for this suspension:\n{justification}")
 
-            # if there is a post plan add it between the wait
-            # and the cached messages
-            if post_plan is not None:
-                if callable(post_plan):
-                    post_plan = post_plan()
-                self._plan_stack.append(ensure_generator(post_plan))
-                self._response_stack.append(None)
-
-            # tell the devices they are ready to go again
-            self._plan_stack.append(single_gen(Msg('resume', None, )))
-            self._response_stack.append(None)
-
-            # add the wait on the future to the stack
-            self._plan_stack.append(single_gen(Msg('wait_for', None, [fut, ])))
+            # add starting the suspender logic to the stack
+            self._plan_stack.append(
+                single_gen(Msg('_start_suspender', None, pre_plan, post_plan, justification, fut))
+            )
             self._response_stack.append(None)
 
-            # if there is a pre plan add on top of the wait
-            if pre_plan is not None:
-                if callable(pre_plan):
-                    pre_plan = pre_plan()
-                self._plan_stack.append(ensure_generator(pre_plan))
-                self._response_stack.append(None)
-
-            self._plan_stack.append(single_gen(
-                Msg('rewindable', None, False)))
-            self._response_stack.append(None)
             # The event loop is still running. The pre_plan will be processed,
             # and then the RunEngine will be hung up on processing the
             # 'wait_for' message until `fut` is set.
             if not self._state == 'paused':
                 self._state = 'suspending'
                 # bump the _run task out of what ever it is awaiting
                 self._task.cancel()
 
         self.loop.call_soon_threadsafe(
             self.loop.create_task,
             _request_suspend(pre_plan, post_plan, justification))
 
+    async def _start_suspender(self, msg):
+        """
+        An internal message to do the initial work of starting a suspender
+        """
+        pre_plan, post_plan, justification, fut = msg.args
+        for current_run in self._run_bundlers.values():
+            current_run.record_interruption(
+                justification if justification is not None else "suspended"
+            )
+        # During suspend, all motors should be stopped. Call stop() on
+        # every object we ever set().
+        await self._stop_movable_objects(success=True)
+        # Notify Devices of the pause in case they want to clean up.
+        for obj in self._objs_seen:
+            if hasattr(obj, 'pause'):
+                try:
+                    await maybe_await(obj.pause())
+                except NoReplayAllowed:
+                    self._reset_checkpoint_state_meth()
+        # rewind to the last checkpoint
+        rewind_plan = self._rewind()
+        was_rewindable = self.rewindable
+
+        if callable(pre_plan):
+            pre_plan = pre_plan()
+        if callable(post_plan):
+            post_plan = post_plan()
+
+        def suspender_helper_inner_plan():
+            # none of this should run again.
+            yield Msg('rewindable', None, False)
+            # if there is a pre plan add on top of the wait
+            if pre_plan is not None:
+                yield from ensure_generator(pre_plan)
+            # wait for the future from the suspender to be released
+            yield Msg('wait_for', None, [fut, ])
+            # do the work we need to do to resume
+            yield Msg('_resume_from_suspender', None, )
+            # if there is a post plan, run it
+            if post_plan is not None:
+                yield from ensure_generator(post_plan)
+            # put rewindable back the way it was
+            yield Msg('rewindable', None, was_rewindable)
+            yield from rewind_plan
+
+        # add the above helper to the plan stack
+        self._plan_stack.append(suspender_helper_inner_plan())
+        self._response_stack.append(None)
+
     def abort(self, reason=''):
         """
         Stop a running or paused plan and mark it as aborted.
 
         Returns
         -------
         uids : tuple
@@ -1314,14 +1324,15 @@
         :meth:`RunEngine.abort`
         :meth:`RunEngine.stop`
         '''
         return self.__interrupter_helper(self._halt_coro())
 
     def __interrupter_helper(self, coro):
         if self.state == 'panicked':
+            coro.close()
             raise RuntimeError("The RunEngine is panicked and "
                                "cannot be recovered. "
                                "You must restart bluesky.")
 
         coro_event = threading.Event()
         task = None
 
@@ -1359,26 +1370,24 @@
         if self._call_returns_result:
             plan_return = self.NO_PLAN_RETURN
             run_engine_result = self._create_result(plan_return)
             return run_engine_result
         else:
             return tuple(self._run_start_uids)
 
-    def _stop_movable_objects(self, *, success=True):
+    async def _stop_movable_objects(self, *, success=True):
         "Call obj.stop() for all objects we have moved. Log any exceptions."
         for obj in self._movable_objs_touched:
-            try:
-                stop = obj.stop
-            except AttributeError:
-                self.log.debug("No 'stop' method available on %r", obj)
-            else:
+            if isinstance(obj, Stoppable):
                 try:
-                    stop(success=success)
+                    await maybe_await(obj.stop(success=success))
                 except Exception:
                     self.log.exception("Failed to stop %r.", obj)
+            else:
+                self.log.debug("No 'stop' method available on %r", obj)
 
     async def _run(self):
         """Pull messages from the plan, process them, send results back.
 
         Upon exit, clean up.
         - Call stop() on all objects that were 'set' or 'kickoff'.
         - Try to collect any uncollected flyers.
@@ -1422,21 +1431,21 @@
                     assert self._state == 'pausing'
                     # Remove any monitoring callbacks, but keep refs in
                     # self._monitor_params to re-instate them later.
                     for current_run in self._run_bundlers.values():
                         await current_run.suspend_monitors()
                     # During pause, all motors should be stopped. Call stop()
                     # on every object we ever set().
-                    self._stop_movable_objects(success=True)
+                    await self._stop_movable_objects(success=True)
                     # Notify Devices of the pause in case they want to
                     # clean up.
                     for obj in self._objs_seen:
-                        if hasattr(obj, 'pause'):
+                        if isinstance(obj, Pausable):
                             try:
-                                obj.pause()
+                                await maybe_await(obj.pause())
                             except NoReplayAllowed:
                                 self._reset_checkpoint_state_meth()
                     self._state = 'paused'
                     # Let RunEngine.__call__ return...
                     self._blocking_event.set()
 
                     await self._run_permit.wait()
@@ -1454,52 +1463,57 @@
                 # set resp to the sentinel so that if we fail in the sleep
                 # we do not add an extra response
                 resp = sentinel
                 try:
                     # the new response to be added
                     new_response = None
 
-                    # This 'await' must be here to ensure that
-                    # this coroutine breaks out of its current behavior
-                    # before trying to get the next message from the
-                    # top of the generator stack in case there has
-                    # been a pause requested.  Without this the next
-                    # message after the pause may be processed first
-                    # on resume (instead of the first message in
-                    # self._msg_cache).
-
-                    # This sleep has to be inside of this try block so
-                    # that any of the 'async' exceptions get thrown in the
-                    # correct place
-                    await asyncio.sleep(0, **self._loop_for_kwargs)
+                    # This 'await' must be here to ensure that this coroutine
+                    # breaks out of its current behavior before trying to get
+                    # the next message from the top of the generator stack in
+                    # case there has been a pause requested.  Without this the
+                    # next message after the pause may be processed first on
+                    # resume (instead of the first message in self._msg_cache).
+                    # This await also gives the co-routine for requesting
+                    # suspends a chance to run.
+
+                    # This sleep has to be inside of this try block so that any
+                    # of the 'async' exceptions get thrown in the correct
+                    # place.
+
+                    # If we are handling an exception, then burn through the
+                    # current plan stack before rather than allowing a pause or
+                    # suspension to try and finish firing.
+                    if stashed_exception is None:
+                        await asyncio.sleep(0, **self._loop_for_kwargs)
                     # always pop off a result, we are either sending it back in
                     # or throwing an exception in, in either case the left hand
                     # side of the yield in the plan will be moved past
                     resp = self._response_stack.pop()
                     # if any status tasks have failed, grab the exceptions.
                     # give priority to things pushed in from outside
                     with self._state_lock:
                         if self._exception is not None:
                             stashed_exception = self._exception
                             self._exception = None
                     # The case where we have a stashed exception
-                    if (stashed_exception is not None or
-                            isinstance(resp, Exception)):
+                    if (stashed_exception is not None or isinstance(resp, Exception)):
                         # throw the exception at the current plan
                         try:
-                            msg = self._plan_stack[-1].throw(
-                                stashed_exception or resp)
+                            msg = self._plan_stack[-1].throw(stashed_exception or resp)
                         except Exception as e:
                             # The current plan did not handle it,
                             # maybe the next plan (if any) would like
                             # to try
                             self._plan_stack.pop()
                             # we have killed the current plan, do not give
                             # it a new response
                             resp = sentinel
+                            # If there is at least one plan left in the stack,
+                            # stash the new exception go back to top
                             if len(self._plan_stack):
                                 stashed_exception = e
                                 continue
                             # no plans left and still an unhandled exception
                             # re-raise to exit the infinite loop
                             else:
                                 raise
@@ -1654,15 +1668,15 @@
         finally:
             if not exit_reason:
                 exit_reason = self._reason
             # Some done_callbacks may still be alive in other threads.
             # Block them from creating new 'failed status' tasks on the loop.
             self._pardon_failures.set()
             # call stop() on every movable object we ever set()
-            self._stop_movable_objects(success=True)
+            await self._stop_movable_objects(success=True)
             for current_run in self._run_bundlers.values():
                 # Clear any uncleared monitoring callbacks.
                 current_run.clear_monitors()
                 # Try to collect any flyers that were kicked off but
                 # not finished.  Some might not support partial
                 # collection. We swallow errors.
                 await current_run.backstop_collect()
@@ -1815,17 +1829,18 @@
         """
         Add a reading to the open event bundle.
 
         Expected message object is:
 
             Msg('read', obj)
         """
-        obj = msg.obj
+        obj = check_supports(msg.obj, Readable)
         # actually _read_ the object
-        ret = obj.read(*msg.args, **msg.kwargs)
+        warn_if_msg_args_or_kwargs(msg, obj.read, msg.args, msg.kwargs)
+        ret = await maybe_await(obj.read(*msg.args, **msg.kwargs))
 
         if ret is None:
             raise RuntimeError(
                 f"The read of {obj.name} returned None. "
                 "This is a bug in your object implementation, "
                 "`read` must return a dictionary.")
         run_key = msg.run
@@ -1941,27 +1956,28 @@
         try:
             current_run = self._run_bundlers[run_key]
         except KeyError as ke:
             raise IllegalMessageSequence("A 'kickoff' message was sent but no "
                                          "run is open.") from ke
 
         _, obj, args, kwargs, _ = msg
+        obj = check_supports(obj, Flyable)
         kwargs = dict(msg.kwargs)
         group = kwargs.pop("group", None)
-
+        warn_if_msg_args_or_kwargs(msg, obj.kickoff, msg.args, kwargs)
         ret = obj.kickoff(*msg.args, **kwargs)
         p_event = asyncio.Event(**self._loop_for_kwargs)
         pardon_failures = self._pardon_failures
 
         await current_run.kickoff(msg)
 
         def done_callback(status=None):
             self.log.debug(
                 "The object %r reports 'kickoff' is done " "with status %r",
-                msg.obj,
+                obj,
                 ret.success,
             )
             task = self._loop.call_soon_threadsafe(
                 self._status_object_completed, ret, p_event, pardon_failures
             )
             self._status_tasks.append(task)
 
@@ -1997,23 +2013,25 @@
         except KeyError as ke:
             raise IllegalMessageSequence("A 'complete' message was sent but no "
                                          "run is open.") from ke
 
         await current_run.complete(msg)
         kwargs = dict(msg.kwargs)
         group = kwargs.pop("group", None)
-        ret = msg.obj.complete(*msg.args, **kwargs)
+        obj = check_supports(msg.obj, Flyable)
+        warn_if_msg_args_or_kwargs(msg, obj.complete, msg.args, kwargs)
+        ret = obj.complete(*msg.args, **kwargs)
 
         p_event = asyncio.Event(**self._loop_for_kwargs)
         pardon_failures = self._pardon_failures
 
         def done_callback(status=None):
             self.log.debug(
                 "The object %r reports 'complete' is done " "with status %r",
-                msg.obj,
+                obj,
                 ret.success,
             )
             task = self._loop.call_soon_threadsafe(
                 self._status_object_completed, ret, p_event, pardon_failures
             )
             self._status_tasks.append(task)
 
@@ -2065,24 +2083,25 @@
 
         Expected message object is
 
             Msg('set', obj, *args, **kwargs)
 
         where arguments are passed through to `obj.set(*args, **kwargs)`.
         """
+        obj = check_supports(msg.obj, Movable)
         kwargs = dict(msg.kwargs)
         group = kwargs.pop('group', None)
-        self._movable_objs_touched.add(msg.obj)
-        ret = msg.obj.set(*msg.args, **kwargs)
+        self._movable_objs_touched.add(obj)
+        ret = obj.set(*msg.args, **kwargs)
         p_event = asyncio.Event(**self._loop_for_kwargs)
         pardon_failures = self._pardon_failures
 
         def done_callback(status=None):
             self.log.debug("The object %r reports set is done "
-                           "with status %r", msg.obj, ret.success)
+                           "with status %r", obj, ret.success)
             task = self._loop.call_soon_threadsafe(
                 self._status_object_completed, ret, p_event, pardon_failures)
             self._status_tasks.append(task)
 
         try:
             ret.add_callback(done_callback)
         except AttributeError:
@@ -2097,23 +2116,25 @@
         """
         Trigger a device and cache the returned status object.
 
         Expected message object is:
 
             Msg('trigger', obj)
         """
+        obj = check_supports(msg.obj, Triggerable)
         kwargs = dict(msg.kwargs)
         group = kwargs.pop('group', None)
-        ret = msg.obj.trigger(*msg.args, **kwargs)
+        warn_if_msg_args_or_kwargs(msg, obj.trigger, msg.args, kwargs)
+        ret = obj.trigger(*msg.args, **kwargs)
         p_event = asyncio.Event(**self._loop_for_kwargs)
         pardon_failures = self._pardon_failures
 
         def done_callback(status=None):
             self.log.debug("The object %r reports trigger is "
-                           "done with status %r.", msg.obj, ret.success)
+                           "done with status %r.", obj, ret.success)
             task = self._loop.call_soon_threadsafe(
                 self._status_object_completed, ret, p_event, pardon_failures)
             self._status_tasks.append(task)
 
         try:
             ret.add_callback(done_callback)
         except AttributeError:
@@ -2210,16 +2231,16 @@
         keyword arguments in the `Msg` signature
         """
         # Re-instate monitoring callbacks.
         for current_run in self._run_bundlers.values():
             await current_run.restore_monitors()
         # Notify Devices of the resume in case they want to clean up.
         for obj in self._objs_seen:
-            if hasattr(obj, 'resume'):
-                obj.resume()
+            if isinstance(obj, Pausable):
+                await maybe_await(obj.resume())
 
     async def _checkpoint(self, msg):
         """Instruct the RunEngine to create a checkpoint so that we can rewind
         to this point if necessary
 
         Expected message object is:
 
@@ -2313,15 +2334,15 @@
 
         Expected message object is:
 
             Msg('stage', object)
         """
         _, obj, args, kwargs, _ = msg
         # If an object has no 'stage' method, assume there is nothing to do.
-        if not isinstance(obj, bs_protocols.Stageable):
+        if not isinstance(obj, Stageable):
             return []
         result = obj.stage()
         self._staged.add(obj)  # add first in case of failure below
         await self._reset_checkpoint_state_coro()
         return result
 
     async def _unstage(self, msg):
@@ -2329,15 +2350,15 @@
 
         Expected message object is:
 
             Msg('unstage', object)
         """
         _, obj, args, kwargs, _ = msg
         # If an object has no 'unstage' method, assume there is nothing to do.
-        if not isinstance(obj, bs_protocols.Stageable):
+        if not isinstance(obj, Stageable):
             return []
         result = obj.unstage()
         # use `discard()` to ignore objects that are not in the staged set.
         self._staged.discard(obj)
         await self._reset_checkpoint_state_coro()
         return result
 
@@ -2345,15 +2366,16 @@
         """
         Stop a device.
 
         Expected message object is:
 
             Msg('stop', obj)
         """
-        return msg.obj.stop()  # nominally, this returns None
+        obj = check_supports(msg.obj, Stoppable)
+        return await maybe_await(obj.stop())  # nominally, this returns None
 
     async def _subscribe(self, msg):
         """
         Add a subscription after the run has started.
 
         This, like subscriptions passed to __call__, will be removed at the
         end by the RunEngine.
@@ -2594,16 +2616,41 @@
 
 _ensure_event_loop_running.loop_to_thread = weakref.WeakKeyDictionary()
 
 _bluesky_event_loop = None
 
 
 def get_bluesky_event_loop():
-    global _bluesky_event_loop
-    if _bluesky_event_loop is None:
-        _bluesky_event_loop = asyncio.new_event_loop()
     return _bluesky_event_loop
 
 
 def set_bluesky_event_loop(loop):
     global _bluesky_event_loop
     _bluesky_event_loop = loop
+
+
+def in_bluesky_event_loop() -> bool:
+    try:
+        # TODO: change to asyncio.get_running_loop() when we drop py3.6
+        loop = asyncio.get_event_loop()
+    except RuntimeError:
+        # Ok, no running loop
+        return False
+    else:
+        # Check if running loop is bluesky event loop
+        return loop is _bluesky_event_loop
+
+
+T = typing.TypeVar("T")
+
+
+def call_in_bluesky_event_loop(coro: typing.Awaitable[T], timeout: float = None) -> T:
+    if _bluesky_event_loop is None or not _bluesky_event_loop.is_running():
+        # Quell "coroutine never awaited" warnings
+        if iscoroutine(coro):
+            coro.close()
+        raise RuntimeError("Bluesky event loop not running")
+    fut = asyncio.run_coroutine_threadsafe(
+        coro,
+        loop=_bluesky_event_loop,
+    )
+    return fut.result(timeout=timeout)
```

### Comparing `bluesky-1.8.3/bluesky/simulators.py` & `bluesky-1.9.0/bluesky/simulators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from warnings import warn
+from bluesky.utils import maybe_await
 from bluesky.preprocessors import print_summary_wrapper
+from bluesky.run_engine import call_in_bluesky_event_loop, in_bluesky_event_loop
+from .protocols import Checkable
 
 
 def plot_raster_path(plan, x_motor, y_motor, ax=None, probe_size=None, lw=2):
     """Plot the raster path for this plan
 
     Parameters
     ----------
@@ -73,24 +76,32 @@
         ...
 
 
 print_summary = summarize_plan  # back-compat
 
 
 def check_limits(plan):
+    """Run check_limits_async in the RE"""
+    if in_bluesky_event_loop():
+        raise RuntimeError("Can't call check_limits() from within RE, use await check_limits_async() instead")
+    call_in_bluesky_event_loop(check_limits_async(plan))
+
+
+async def check_limits_async(plan):
     """
     Check that a plan will not move devices outside of their limits.
 
     Parameters
     ----------
     plan : iterable
         Must yield `Msg` objects
     """
     ignore = []
     for msg in plan:
-        if msg.command == 'set' and msg.obj not in ignore:
-            if hasattr(msg.obj, "check_value"):
-                msg.obj.check_value(msg.args[0])
+        obj = msg.obj
+        if msg.command == 'set' and obj not in ignore:
+            if isinstance(obj, Checkable):
+                await maybe_await(obj.check_value(msg.args[0]))
             else:
-                warn(f"{msg.obj.name} has no check_value() method"
+                warn(f"{obj.name} has no check_value() method"
                      f" to check if {msg.args[0]} is within its limits.")
-                ignore.append(msg.obj)
+                ignore.append(obj)
```

### Comparing `bluesky-1.8.3/bluesky/suspenders.py` & `bluesky-1.9.0/bluesky/suspenders.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/conftest.py` & `bluesky-1.9.0/bluesky/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import asyncio
 from distutils.version import LooseVersion
-from bluesky.run_engine import RunEngine, TransitionError
+from bluesky.run_engine import RunEngine, TransitionError, set_bluesky_event_loop
 import numpy as np
 import os
 import pytest
 
 
 @pytest.fixture(scope='function', params=[False, True])
 def RE(request):
     loop = asyncio.new_event_loop()
     loop.set_debug(True)
     RE = RunEngine({}, call_returns_result=request.param, loop=loop)
+    set_bluesky_event_loop(loop)
 
     def clean_event_loop():
         if RE.state not in ('idle', 'panicked'):
             try:
                 RE.halt()
             except TransitionError:
                 pass
@@ -54,17 +55,22 @@
                 for kwargs in datum_kwarg_gen]
 
 
 @pytest.fixture(scope='function')
 def db(request):
     """Return a data broker
     """
-    from databroker import temp
-    db = temp()
-    return db
+    try:
+        from databroker import temp
+        db = temp()
+        return db
+    except ImportError:
+        pytest.skip("Databroker v2 still missing temp.")
+    except ValueError:
+        pytest.skip("Intake is failing for unknown reasons.")
 
 
 @pytest.fixture(autouse=True)
 def cleanup_any_figures(request):
     import matplotlib.pyplot as plt
     "Close any matplotlib figures that were opened during a test."
     plt.close('all')
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_bec.py` & `bluesky-1.9.0/bluesky/tests/test_bec.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_callbacks.py` & `bluesky-1.9.0/bluesky/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_devices.py` & `bluesky-1.9.0/bluesky/tests/test_devices.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import itertools
+from time import time
+from typing import Dict, List
+from bluesky.protocols import Callback, Descriptor, Reading
 
 from bluesky.utils import ancestry, share_ancestor, separate_devices
 from bluesky.plan_stubs import trigger_and_read
 from bluesky.preprocessors import run_decorator
 from bluesky import Msg, RunEngineInterrupted
 import pytest
 from bluesky.tests import requires_ophyd, ophyd
 from .utils import DocCollector
+from unittest.mock import ANY
 
 if ophyd:
     from ophyd import Component as Cpt, Device, Signal
 
     class A(Device):
         s1 = Cpt(Signal, value=0)
         s2 = Cpt(Signal, value=0)
@@ -20,14 +24,36 @@
         a2 = Cpt(A, '')
 
     class DCM(Device):
         th = Cpt(Signal, value=0)
         x = Cpt(Signal, value=0)
 
 
+class SigNew:
+    def __init__(self, name: str) -> None:
+        self.name = name
+        self._callbacks: List[Callback] = []
+
+    def read(self) -> Dict[str, Reading]:
+        return {}
+
+    def describe(self) -> Dict[str, Descriptor]:
+        return {}
+
+    def subscribe(self, function: Callback) -> None:
+        self._callbacks.append(function)
+
+    def clear_sub(self, function: Callback) -> None:
+        self._callbacks.remove(function)
+
+    def _run_subs(self, *args, **kwargs):
+        for cb in self._callbacks:
+            cb({self.name: dict(value=0, timestamp=time())})
+
+
 @requires_ophyd
 def test_ancestry():
     b = B('', name='b')
     assert ancestry(b) == [b]
     assert ancestry(b.a1) == [b.a1, b]
     assert ancestry(b.a1.s1) == [b.a1.s1, b.a1, b]
 
@@ -52,30 +78,42 @@
     assert separate_devices([b1, b1.a1]) == [b1]
     assert separate_devices([b1.a1, b1.a2]) == [b1.a1, b1.a2]
     assert separate_devices([b1, b2.a1]) == [b1, b2.a1]
     assert separate_devices([b1.a1, b2.a2]) == [b1.a1, b2.a2]
     assert separate_devices([b1, a]) == [b1, a]
 
 
+@pytest.mark.parametrize('ophyd', ["v1", "v2"])
 @requires_ophyd
-def test_monitor(RE):
+def test_monitor(RE, ophyd):
     docs = []
 
     def collect(name, doc):
         docs.append(doc)
 
-    a = A('', name='a')
+    if ophyd == "v1":
+        sig = A('', name='a').s1
+    else:
+        sig = SigNew(name='a_s1')
 
     def plan():
         yield Msg('open_run')
-        yield Msg('monitor', a.s1)
-        a.s1._run_subs(sub_type='value')
+        yield Msg('monitor', sig)
+        sig._run_subs(sub_type='value')
         yield Msg('close_run')
     RE(plan(), collect)
     assert len(docs) == 4
+    assert docs[2] == {
+        'data': {'a_s1': 0},
+        'descriptor': ANY,
+        'seq_num': 1,
+        'time': pytest.approx(time(), rel=0.1),
+        'timestamps': {'a_s1': pytest.approx(time(), rel=0.1)},
+        'uid': ANY
+    }
 
 
 @requires_ophyd
 def test_monitor_with_pause_resume(RE):
     docs = []
 
     def collect(name, doc):
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_documents.py` & `bluesky-1.9.0/bluesky/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_examples.py` & `bluesky-1.9.0/bluesky/tests/test_examples.py`

 * *Files 13% similar despite different names*

```diff
@@ -279,28 +279,28 @@
         Msg('read', hw.motor),
         Msg('read', hw.det),
         Msg('save'),
         Msg('close_run'),
     ]
     assert RE.state == 'idle'
 
-    def local_suspend():
-        RE.request_suspend(ev.wait)
-
     def resume_cb():
         RE.loop.call_soon_threadsafe(ev.set)
 
+    def local_suspend():
+        RE.request_suspend(ev.wait)
+        # wait a second and then resume
+        threading.Timer(1, resume_cb).start()
+
     out = []
 
     def ev_cb(name, ev):
         out.append(ev)
     # trigger the suspend right after the check point
     threading.Timer(.1, local_suspend).start()
-    # wait a second and then resume
-    threading.Timer(1, resume_cb).start()
     # grab the start time
     start = ttime.time()
     # run, this will not return until it is done
     RE(test_list, {'event': ev_cb})
     # check to make sure it took long enough
     assert out[0]['time'] - start > 1.1
 
@@ -447,120 +447,120 @@
     assert seq_nums == [1, 2, 2, 3]
 
 
 def test_duplicate_keys(RE, hw):
     # two detectors, same data keys
 
     def gen():
-        yield(Msg('open_run'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('trigger', hw.det))
-        yield(Msg('trigger', hw.identical_det))
-        yield(Msg('read', hw.det))
-        yield(Msg('read', hw.identical_det))
-        yield(Msg('save'))
+        yield (Msg('open_run'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('trigger', hw.det))
+        yield (Msg('trigger', hw.identical_det))
+        yield (Msg('read', hw.det))
+        yield (Msg('read', hw.identical_det))
+        yield (Msg('save'))
 
     with pytest.raises(ValueError):
         RE(gen())
 
 
 def test_illegal_sequences(RE, hw):
     def gen1():
         # two 'create' msgs in a row
-        yield(Msg('open_run'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('close_run'))
+        yield (Msg('open_run'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('close_run'))
 
     with pytest.raises(IllegalMessageSequence):
         RE(gen1())
 
     def gen2():
         # two 'save' msgs in a row
-        yield(Msg('open_run'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('save'))
-        yield(Msg('save'))
-        yield(Msg('close_run'))
+        yield (Msg('open_run'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('save'))
+        yield (Msg('save'))
+        yield (Msg('close_run'))
 
     with pytest.raises(IllegalMessageSequence):
         RE(gen2())
 
     def gen3():
         # 'configure' after 'create', before 'save'
-        yield(Msg('open_run'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('configure', hw.motor, {}))
+        yield (Msg('open_run'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('configure', hw.motor, {}))
 
     with pytest.raises(IllegalMessageSequence):
         RE(gen3())
 
     def gen4():
         # two 'drop' msgs in a row
-        yield(Msg('open_run'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('drop'))
-        yield(Msg('drop'))
-        yield(Msg('close_run'))
+        yield (Msg('open_run'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('drop'))
+        yield (Msg('drop'))
+        yield (Msg('close_run'))
 
     with pytest.raises(IllegalMessageSequence):
         RE(gen4())
 
 
 def test_new_ev_desc(RE, hw):
     descs = []
 
     def collect_descs(name, doc):
         descs.append(doc)
 
     def gen1():
         # configure between two events -> two descs
-        yield(Msg('open_run'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('read', hw.motor))
-        yield(Msg('save'))
-        yield(Msg('configure', hw.motor, {}))
-        yield(Msg('create', name='primary'))
-        yield(Msg('read', hw.motor))
-        yield(Msg('save'))
-        yield(Msg('close_run'))
+        yield (Msg('open_run'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('read', hw.motor))
+        yield (Msg('save'))
+        yield (Msg('configure', hw.motor, {}))
+        yield (Msg('create', name='primary'))
+        yield (Msg('read', hw.motor))
+        yield (Msg('save'))
+        yield (Msg('close_run'))
 
     descs.clear()
     RE(gen1(), {'descriptor': collect_descs})
     assert len(descs) == 2
 
     def gen2():
         # configure between two events and explicitly before any events
         # -> two descs
-        yield(Msg('open_run'))
-        yield(Msg('configure', hw.motor, {}))
-        yield(Msg('create', name='primary'))
-        yield(Msg('read', hw.motor))
-        yield(Msg('save'))
-        yield(Msg('configure', hw.motor, {}))
-        yield(Msg('create', name='primary'))
-        yield(Msg('read', hw.motor))
-        yield(Msg('save'))
-        yield(Msg('close_run'))
+        yield (Msg('open_run'))
+        yield (Msg('configure', hw.motor, {}))
+        yield (Msg('create', name='primary'))
+        yield (Msg('read', hw.motor))
+        yield (Msg('save'))
+        yield (Msg('configure', hw.motor, {}))
+        yield (Msg('create', name='primary'))
+        yield (Msg('read', hw.motor))
+        yield (Msg('save'))
+        yield (Msg('close_run'))
 
     descs.clear()
     RE(gen2(), {'descriptor': collect_descs})
     assert len(descs) == 2
 
     def gen3():
         # configure once before any events -> one desc
-        yield(Msg('open_run'))
-        yield(Msg('configure', hw.motor, {}))
-        yield(Msg('create', name='primary'))
-        yield(Msg('read', hw.motor))
-        yield(Msg('save'))
-        yield(Msg('create', name='primary'))
-        yield(Msg('read', hw.motor))
-        yield(Msg('save'))
-        yield(Msg('close_run'))
+        yield (Msg('open_run'))
+        yield (Msg('configure', hw.motor, {}))
+        yield (Msg('create', name='primary'))
+        yield (Msg('read', hw.motor))
+        yield (Msg('save'))
+        yield (Msg('create', name='primary'))
+        yield (Msg('read', hw.motor))
+        yield (Msg('save'))
+        yield (Msg('close_run'))
 
     descs.clear()
     RE(gen3(), {'descriptor': collect_descs})
     assert len(descs) == 1
 
 
 def test_clear_checkpoint(RE):
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_flyer.py` & `bluesky-1.9.0/bluesky/tests/test_flyer.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
             Msg("complete", flyer, group="bar"),
             Msg("wait", group="bar"),
             Msg("collect", flyer),
             Msg("close_run"),
         ]
     )
     assert flyer.call_counts["collect"] == 4
-    assert flyer.call_counts["describe_collect"] == 4
+    assert flyer.call_counts["describe_collect"] == 1
     assert flyer.call_counts["read_configuration"] == 1
     assert flyer.call_counts["describe_configuration"] == 1
     assert flyer.call_counts["kickoff"] == 1
     assert flyer.call_counts["complete"] == 1
 
 
 class FlyerDetector(Device):
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_generators.py` & `bluesky-1.9.0/bluesky/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_logging.py` & `bluesky-1.9.0/bluesky/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_magics.py` & `bluesky-1.9.0/bluesky/tests/test_magics.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_multi_runs.py` & `bluesky-1.9.0/bluesky/tests/test_multi_runs.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_new_examples.py` & `bluesky-1.9.0/bluesky/tests/test_new_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
     strip_group(processed_plan)
     assert processed_plan == expected
 
 
 def test_descriptor_layout_from_monitor(RE, hw):
     collector = []
     det = hw.rand
+    det.start_simulation()
 
     def collect(name, doc):
         if name == 'descriptor':
             collector.append(doc)
 
     RE([Msg('open_run'),
         Msg('monitor', det, name=det.name),
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_olog_cb.py` & `bluesky-1.9.0/bluesky/tests/test_olog_cb.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_persistent_dict.py` & `bluesky-1.9.0/bluesky/tests/test_persistent_dict.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_plan_patterns.py` & `bluesky-1.9.0/bluesky/tests/test_plan_patterns.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_plans.py` & `bluesky-1.9.0/bluesky/tests/test_plans.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from distutils.version import LooseVersion
 import pytest
 import inspect
 from bluesky.tests.utils import DocCollector
 import bluesky.plans as bp
 import bluesky.plan_stubs as bps
+import bluesky.preprocessors as bpp
 import numpy as np
 import numpy.testing as npt
 import pandas as pd
 import random
 import re
 import collections
 from bluesky.tests.utils import MsgCollector
@@ -653,7 +654,63 @@
     for snake_axes in (10, 50.439, "some string"):
         with pytest.raises(ValueError,
                            match="Parameter 'snake_axes' is not iterable, boolean or None"):
             args = (hw.motor, 1, 2, 3,
                     hw.motor1, 4, 5, 6,
                     hw.motor2, 7, 8, 9)
             RE(plan([hw.det], *args, snake_axes=snake_axes))
+
+
+def test_describe_failure(RE):
+    ophyd = pytest.importorskip("ophyd")
+
+    class Aardvark(Exception):
+        # Unique exception to test behavior of describe.
+        ...
+
+    class BadSignalDescribe(ophyd.Signal):
+        def describe(self):
+            raise Aardvark("Look, an aardvark!")
+
+    class BadSignalRead(ophyd.Signal):
+        def read(self):
+            raise Aardvark("Look, the other aardvark!")
+
+    bad_signal1 = BadSignalDescribe(value=5, name="Arty")
+    bad_signal2 = BadSignalRead(value=5, name="Arty")
+    good_signal = ophyd.Signal(value=42, name='baseline')
+
+    class StreamTester:
+        def __init__(self):
+            self.event_count = 0
+            self.stream_names = set()
+
+        def __call__(self, name, doc):
+            if name == 'event':
+                self.event_count += 1
+            if name == 'descriptor':
+                self.stream_names.add(doc['name'])
+
+        def verify(self):
+            assert self.event_count == 2
+            assert self.stream_names == set(['baseline'])
+    st = StreamTester()
+    with pytest.raises(Aardvark, match="Look, an aardvark!"):
+        RE(
+            bpp.baseline_wrapper(
+                bp.count([bad_signal1]),
+                [good_signal]
+            ),
+            st
+        )
+    st.verify()
+
+    st = StreamTester()
+    with pytest.raises(Aardvark, match="Look, the other aardvark!"):
+        RE(
+            bpp.baseline_wrapper(
+                bp.count([bad_signal2]),
+                [good_signal]
+            ),
+            st
+        )
+    st.verify()
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_progress_bar.py` & `bluesky-1.9.0/bluesky/tests/test_progress_bar.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_protocols.py` & `bluesky-1.9.0/bluesky/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_ramp_plan.py` & `bluesky-1.9.0/bluesky/tests/test_ramp_plan.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_run_engine.py` & `bluesky-1.9.0/bluesky/tests/test_run_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from event_model import DocumentNames
 import threading
 import types
 import os
 import signal
 import sys
 from collections import defaultdict
@@ -268,14 +269,17 @@
 
         def describe_configuration(self):
             return {}
 
         def describe(self):
             return {}
 
+        def read(self):
+            return {}
+
         def subscribe(self, *args, **kwargs):
             pass
 
         def clear_sub(self, *args, **kwargs):
             pass
 
     dummy = Dummy('dummy')
@@ -489,22 +493,28 @@
         yield Msg('trigger', det)
 
     inps = []
     inps.append((test_plan,
                  motor,
                  UnReplayableSynGauss('det', motor, 'motor', center=0, Imax=1),
                  ['set', 'trigger', 'sleep',
-                  'rewindable', 'wait_for', 'resume', 'rewindable',
+                  "_start_suspender",
+                  'rewindable',
+                  'wait_for', "_resume_from_suspender",
+                  'rewindable',
                   'set', 'trigger']))
 
     inps.append((test_plan,
                  motor,
                  SynGauss('det', motor, 'motor', center=0, Imax=1),
                  ['set', 'trigger', 'sleep',
-                  'rewindable', 'wait_for', 'resume', 'rewindable',
+                  "_start_suspender",
+                  'rewindable',
+                  'wait_for', "_resume_from_suspender",
+                  'rewindable',
                   'set',
                   'trigger', 'sleep', 'set', 'trigger']))
 
     return pytest.mark.parametrize('plan,motor,det,msg_seq', inps)
 
 
 @_make_unrewindable_suspender_marker()
@@ -1378,24 +1388,25 @@
 
     class Detector:
         def __init__(self, name):
             self.name = name
             self.parent = None
             self.hints = {'vis': 'placeholder'}
 
-        def read(self):
+        async def read(self):
+            await asyncio.sleep(0.1)
             return {}
 
-        def describe(self):
+        async def describe(self):
             return {}
 
-        def read_configuration(self):
+        async def read_configuration(self):
             return {}
 
-        def describe_configuration(self):
+        async def describe_configuration(self):
             return {}
 
     det = Detector('det')
 
     collector = []
 
     RE(count([det]),
@@ -1659,14 +1670,17 @@
 
         def describe(self):
             return {}
 
         def read(self):
             ...
 
+        def trigger(self):
+            ...
+
     obj = Dummy('broken read')
     with pytest.raises(RuntimeError):
         RE([Msg('read', obj)])
 
 
 def test_self_describe(RE):
     def inner():
@@ -1683,9 +1697,15 @@
     class MockDevice:
         name = "mock_device"
 
         def trigger(self):
             assert threading.current_thread().name == "bluesky-run-engine"
             return Status()
 
+        def describe(self):
+            return {}
+
+        def read(self):
+            return {}
+
     d = MockDevice()
     RE([Msg("trigger", d)])
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_scans.py` & `bluesky-1.9.0/bluesky/tests/test_scans.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_scientific.py` & `bluesky-1.9.0/bluesky/tests/test_scientific.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_simple_api.py` & `bluesky-1.9.0/bluesky/tests/test_simple_api.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_simulators.py` & `bluesky-1.9.0/bluesky/tests/test_simulators.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     with pytest.warns(UserWarning):
         list(print_summary_wrapper(scan([det], motor, -1, 1, 10)))
     with pytest.warns(UserWarning):
         plan = grid_scan([det], motor1, -5, 5, 10, motor2, -7, 7, 15, True)
         plot_raster_path(plan, 'motor1', 'motor2', probe_size=.3)
 
 
-def test_check_limits(hw):
+def test_check_limits(RE, hw):
     det = hw.det
     motor = hw.motor
     # The motor object does not currently implement limits.
     # Use an assert to help us out if this changes in the future.
     assert not hasattr(motor, 'limits')
 
     # # check_limits should warn if it can't find check_value
@@ -54,13 +54,19 @@
 
     # check_limits should raise if limits are equal only if object raises
     # this object does not raise
     motor.limits = (2, 2)
     check_limits(scan([det], motor, -1, 1, 3))
 
 
+def test_check_limits_needs_RE():
+    with pytest.raises(RuntimeError) as ctx:
+        check_limits([])
+    assert str(ctx.value) == "Bluesky event loop not running"
+
+
 def test_plot_raster_path(hw):
     det = hw.det
     motor1 = hw.motor1
     motor2 = hw.motor2
     plan = grid_scan([det], motor1, -5, 5, 10, motor2, -7, 7, 15, True)
     plot_raster_path(plan, 'motor1', 'motor2', probe_size=.3)
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_snaking.py` & `bluesky-1.9.0/bluesky/tests/test_snaking.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_streams.py` & `bluesky-1.9.0/bluesky/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_supplemental_data.py` & `bluesky-1.9.0/bluesky/tests/test_supplemental_data.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_suspenders.py` & `bluesky-1.9.0/bluesky/tests/test_suspenders.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,47 +80,97 @@
 
     RE.install_suspender(susp)
     threading.Timer(1, sig.put, (0,)).start()
     RE.msg_hook = accum
     RE(scan)
 
     assert len(msg_lst) == 2
-    assert ['wait_for', 'checkpoint'] == [m[0] for m in msg_lst]
+    assert ["wait_for", "checkpoint"] == [m[0] for m in msg_lst]
 
 
-@pytest.mark.parametrize('pre_plan,post_plan,expected_list',
-                         [([Msg('null')], None,
-                           ['checkpoint', 'sleep', 'rewindable', 'null',
-                            'wait_for', 'resume', 'rewindable', 'sleep']),
-                          (None, [Msg('null')],
-                           ['checkpoint', 'sleep', 'rewindable',
-                            'wait_for', 'resume', 'null', 'rewindable',
-                            'sleep']),
-                          ([Msg('null')], [Msg('null')],
-                           ['checkpoint', 'sleep', 'rewindable', 'null',
-                            'wait_for', 'resume', 'null', 'rewindable',
-                            'sleep']),
-                          (lambda: [Msg('null')], lambda: [Msg('null')],
-                           ['checkpoint', 'sleep', 'rewindable', 'null',
-                            'wait_for', 'resume', 'null', 'rewindable',
-                            'sleep'])])
+@pytest.mark.parametrize(
+    "pre_plan,post_plan,expected_list",
+    [
+        (
+            [Msg("null")],
+            None,
+            [
+                "checkpoint",
+                "sleep",
+                "_start_suspender",
+                "rewindable",
+                "null",
+                "wait_for",
+                "_resume_from_suspender",
+                "rewindable",
+                "sleep",
+            ],
+        ),
+        (
+            None,
+            [Msg("null")],
+            [
+                "checkpoint",
+                "sleep",
+                "_start_suspender",
+                "rewindable",
+                "wait_for",
+                "_resume_from_suspender",
+                "null",
+                "rewindable",
+                "sleep",
+            ],
+        ),
+        (
+            [Msg("null")],
+            [Msg("null")],
+            [
+                "checkpoint",
+                "sleep",
+                "_start_suspender",
+                "rewindable",
+                "null",
+                "wait_for",
+                "_resume_from_suspender",
+                "null",
+                "rewindable",
+                "sleep",
+            ],
+        ),
+        (
+            lambda: [Msg("null")],
+            lambda: [Msg("null")],
+            [
+                "checkpoint",
+                "sleep",
+                "_start_suspender",
+                "rewindable",
+                "null",
+                "wait_for",
+                "_resume_from_suspender",
+                "null",
+                "rewindable",
+                "sleep",
+            ],
+        ),
+    ],
+)
 def test_pre_suspend_plan(RE, pre_plan, post_plan, expected_list, hw):
     sig = hw.bool_sig
-    scan = [Msg('checkpoint'), Msg('sleep', None, .2)]
+    scan = [Msg("checkpoint"), Msg("sleep", None, 0.2)]
     msg_lst = []
     sig.put(0)
 
     def accum(msg):
         msg_lst.append(msg)
 
-    susp = SuspendBoolHigh(sig, pre_plan=pre_plan,
-                           post_plan=post_plan)
+    susp = SuspendBoolHigh(sig, pre_plan=pre_plan, post_plan=post_plan)
 
     RE.install_suspender(susp)
-    threading.Timer(.1, sig.put, (1,)).start()
+    threading.Timer(0.1, sig.put, (1,)).start()
     threading.Timer(1, sig.put, (0,)).start()
     RE.msg_hook = accum
     RE(scan)
 
     assert len(msg_lst) == len(expected_list)
     assert expected_list == [m[0] for m in msg_lst]
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_transformer.py` & `bluesky-1.9.0/bluesky/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_utils.py` & `bluesky-1.9.0/bluesky/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pytest
 import numpy as np
 
 from functools import reduce
 import operator
 
-from bluesky.utils import ensure_generator, Msg, merge_cycler, is_movable, CallbackRegistry
+from bluesky.utils import (
+    ensure_generator, Msg, merge_cycler, is_movable, CallbackRegistry,
+    warn_if_msg_args_or_kwargs
+)
 from cycler import cycler
 
 
 def test_single_msg_to_gen():
     m = Msg('set', None, 0)
 
     m_list = [m for m in ensure_generator(m)]
@@ -432,7 +435,34 @@
     # Process the allowed signal with unassigned callback (no callbacks called,
     #   but it still works.
     cb.process("sig1")
 
     # Process the signal that is not allowed
     with pytest.raises(ValueError, match=f"Allowed signals are {allowed_sigs}"):
         cb.process("some_signal")
+
+
+def test_msg_args_kwargs_emits_warning_first_time(recwarn):
+    class MyDevice:
+        def kickoff(self, *args, **kwargs):
+            pass
+
+    device = MyDevice()
+    msg = Msg("kickoff")
+
+    assert len(recwarn) == 0
+    warn_if_msg_args_or_kwargs(msg, device.kickoff, (), {"arg": "value"})
+    assert len(recwarn) == 1
+    w = recwarn.pop(PendingDeprecationWarning)
+    assert str(w.message) == """\
+About to call kickoff() with args () and kwargs {'arg': 'value'}.
+In the future the passing of Msg.args and Msg.kwargs down to hardware from
+Msg("kickoff") may be deprecated. If you have a use case for these,
+we would like to know about it, so please open an issue at
+https://github.com/bluesky/bluesky/issues"""
+    assert len(recwarn) == 0
+    # Second time doesn't warn
+    warn_if_msg_args_or_kwargs(msg, device.kickoff, (), {"arg": "value"})
+    assert len(recwarn) == 0
+    # Called without kwargs doesn't warn
+    warn_if_msg_args_or_kwargs(msg, device.kickoff, (), {})
+    assert len(recwarn) == 0
```

### Comparing `bluesky-1.8.3/bluesky/tests/test_vertical_integration.py` & `bluesky-1.9.0/bluesky/tests/test_vertical_integration.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/test_zmq.py` & `bluesky-1.9.0/bluesky/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/tests/utils.py` & `bluesky-1.9.0/bluesky/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky/utils/__init__.py` & `bluesky-1.9.0/bluesky/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import os
 import sys
 import signal
 import operator
 import uuid
 from functools import reduce
-from typing import Any, Optional, Callable
+from typing import Any, Dict, Iterator, List, Optional, Callable
 from weakref import ref, WeakKeyDictionary
 import types
 import inspect
 from inspect import Parameter, Signature
 import itertools
 import abc
 from collections.abc import Iterable
@@ -25,14 +25,19 @@
 from tqdm.utils import _screen_shape_wrapper, _term_move_up, _unicode
 import warnings
 
 import msgpack
 import msgpack_numpy
 import zict
 
+from bluesky.protocols import (
+    T, Asset, HasParent, HasHints, Hints, Movable, Readable,
+    SyncOrAsync, WritesExternalAssets, check_supports
+)
+
 try:
     # cytools is a drop-in replacement for toolz, implemented in Cython
     from cytools import groupby
 except ImportError:
     from toolz import groupby
 
 
@@ -1385,15 +1390,15 @@
     complex_objs : List[PseudoPositioner]
         Independent objects which have interdependent children
 
     coupled : Dict[PseudoPositioner, Dict[str, List[OphydObj]]]
         Mapping of interdependent axis passed in.
     '''
     def get_parent(o):
-        return getattr(o, 'parent')
+        return check_supports(o, HasParent).parent
 
     independent_objs = set()
     maybe_coupled = set()
     complex_objs = set()
     for o in objs:
         parent = o.parent
         if hasattr(o, 'RealPosition'):
@@ -1547,15 +1552,47 @@
         # without importing anything that is not already imported.
         else:
             import matplotlib
             backend = matplotlib.get_backend().lower()
             # if with a Qt backend, do the scary thing
             if 'qt' in backend:
 
-                from matplotlib.backends.qt_compat import QtCore, QtWidgets
+                from matplotlib.backends.qt_compat import QtCore, QtWidgets, QT_API
+                import functools
+
+                @functools.lru_cache(None)
+                def _enum(name):
+                    """
+                    Between PyQt5 and PyQt6 how the various enums were accessed changed from
+                    all of the various names being in the module namespace to being nested under
+                    the Enum name.  Thus in PyQt5 we access the QSocketNotifier Type enum values as ::
+
+                        QtCore.QSocketNotifier.Read
+
+                    but in PyQt6 we use::
+
+                         QtCore.QSocketNotifier.Type.Read
+
+                    rather than have this checking inline where we use it, this function lets us do::
+
+                        _enum('QtCore.QSocketNotifier.Type').Read
+
+                    and well get the right namespace to get the Enum member from.
+
+                    We use the extra layer of indirection of `operator.attrgetter` so that
+                    multi-level names work and we can rely on the Qt compat layer to get the
+                    correct PyQt5 vs PyQt6
+
+                    This is copied from Matplotlib.
+                    """
+                    # foo.bar.Enum.Entry (PyQt6) <=> foo.bar.Entry (non-PyQt6).
+                    return operator.attrgetter(
+                        name if QT_API == 'PyQt6' else name.rpartition(".")[0]
+                    )(sys.modules[QtCore.__package__])
+
                 app = QtWidgets.QApplication.instance()
                 if app is None:
                     _qapp = app = QtWidgets.QApplication([b'bluesky'])
                 assert app is not None
                 event_loop = QtCore.QEventLoop()
 
                 def start_killer_thread():
@@ -1580,16 +1617,18 @@
                     # Updated docs:
                     # https://doc.qt.io/qt-5/unix-signals.html
                     import fcntl
                     rfd, wfd = os.pipe()
                     for fd in (rfd, wfd):
                         flags = fcntl.fcntl(fd, fcntl.F_GETFL)
                         fcntl.fcntl(fd, fcntl.F_SETFL, flags | os.O_NONBLOCK)
-                    wakeupsn = QtCore.QSocketNotifier(rfd,
-                                                      QtCore.QSocketNotifier.Read)
+                    wakeupsn = QtCore.QSocketNotifier(
+                        rfd,
+                        _enum('QtCore.QSocketNotifier.Type').Read
+                    )
                     origwakeupfd = signal.set_wakeup_fd(wfd)
 
                     def cleanup():
                         wakeupsn.setEnabled(False)
                         rfd = wakeupsn.socket()
                         wfd = signal.set_wakeup_fd(origwakeupfd)
                         os.close(int(rfd))
@@ -1644,15 +1683,18 @@
                 killer_timer = QtCore.QTimer()
                 killer_timer.setSingleShot(True)
                 killer_timer.timeout.connect(start_killer_thread)
                 killer_timer.start(0)
 
                 try:
                     sys.excepthook = my_exception_hook
-                    event_loop.exec_()
+                    (event_loop.exec()
+                     if hasattr(event_loop, "exec")
+                     else event_loop.exec_()
+                     )
                     # make sure any pending signals are processed
                     event_loop.processEvents()
                     if vals[1] is not None:
                         raise vals[1]
                 finally:
                     try:
                         cleanup()
@@ -1678,64 +1720,60 @@
     for key, payload in readings.items():
         data[key] = payload['value']
         timestamps[key] = payload['timestamp']
     return data, timestamps
 
 
 def is_movable(obj):
-    """Check if object satisfies bluesky 'movable' interface.
+    """Check if object satisfies bluesky 'Movable' and `Readable` interfaces.
 
     Parameters
     ----------
     obj : Object
         Object to test.
 
     Returns
     -------
     boolean
         True if movable, False otherwise.
     """
-    EXPECTED_ATTRS = (
-        'name',
-        'parent',
-        'read',
-        'describe',
-        'read_configuration',
-        'describe_configuration',
-        'set',
-    )
-    return all(hasattr(obj, attr) for attr in EXPECTED_ATTRS)
-
-
-class Movable(metaclass=abc.ABCMeta):
-    """
-    Abstract base class for objects that satisfy the bluesky 'movable' interface.
-
-    Examples
-    --------
-
-    .. code-block:: python
-
-        m = hw.motor
-        # We need to detect if 'm' is a motor
-        if isinstance(m, Movable):
-            print(f"The object {m.name} is a motor")
-    """
-    @classmethod
-    def __subclasshook__(cls, C):
-        # If the following condition is True, the object C is recognized
-        # to have Movable interface (e.g. a motor)
-        msg = """The Movable abstract base class is deprecated and will be removed in a future
-                 version of bluesky. Please use bluesky.utils.is_movable(obj) to test if an object
-                 satisfies the movable interface."""
-        warnings.warn(msg, DeprecationWarning)
-        EXPECTED_ATTRS = (
-            'name',
-            'parent',
-            'read',
-            'describe',
-            'read_configuration',
-            'describe_configuration',
-            'set',
-            'stop',
-        )
-        return all(hasattr(C, attr) for attr in EXPECTED_ATTRS)
+    return isinstance(obj, Movable) and isinstance(obj, Readable)
+
+
+def get_hinted_fields(obj) -> List[str]:
+    if isinstance(obj, HasHints):
+        return obj.hints.get("fields", [])
+    else:
+        return []
+
+
+already_warned = {}
+
+
+def warn_if_msg_args_or_kwargs(msg, meth, args, kwargs):
+    if args or kwargs and not already_warned.get(msg.command):
+        already_warned[msg.command] = True
+        error_msg = f"""\
+About to call {meth.__name__}() with args {args} and kwargs {kwargs}.
+In the future the passing of Msg.args and Msg.kwargs down to hardware from
+Msg("{msg.command}") may be deprecated. If you have a use case for these,
+we would like to know about it, so please open an issue at
+https://github.com/bluesky/bluesky/issues"""
+        warnings.warn(error_msg, PendingDeprecationWarning)
+
+
+def maybe_update_hints(hints: Dict[str, Hints], obj):
+    if isinstance(obj, HasHints):
+        hints[obj.name] = obj.hints
+
+
+def maybe_collect_asset_docs(msg, obj, *args, **kwargs) -> Iterator[Asset]:
+    if isinstance(obj, WritesExternalAssets):
+        warn_if_msg_args_or_kwargs(msg, obj.collect_asset_docs, args, kwargs)
+        yield from obj.collect_asset_docs(*args, **kwargs)
+
+
+async def maybe_await(ret: SyncOrAsync[T]) -> T:
+    if inspect.isawaitable(ret):
+        return await ret
+    else:
+        return ret
```

### Comparing `bluesky-1.8.3/bluesky/utils/jupyter.py` & `bluesky-1.9.0/bluesky/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/bluesky.egg-info/PKG-INFO` & `bluesky-1.9.0/bluesky.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: bluesky
-Version: 1.8.3
+Version: 1.9.0
 Summary: Experiment specification & orchestration.
 Home-page: https://github.com/bluesky/bluesky
 Author: danielballan
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -38,9 +37,7 @@
 
 [**Bluesky Documentation**](http://blueskyproject.io/bluesky).
 
 The Bluesky Project enables experimental science at the lab-bench or facility scale. It is a collection of Python libraries that are co-developed but independently useful and may be adopted *a la carte*.
 
 [**Bluesky Project Documentation**](http://blueskyproject.io).
 
-
-
```

### Comparing `bluesky-1.8.3/bluesky.egg-info/SOURCES.txt` & `bluesky-1.9.0/bluesky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/setup.py` & `bluesky-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `bluesky-1.8.3/versioneer.py` & `bluesky-1.9.0/versioneer.py`

 * *Files identical despite different names*

