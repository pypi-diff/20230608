# Comparing `tmp/arvados-python-client-2.6.3.tar.gz` & `tmp/arvados-python-client-2.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-python-client-2.6.3.tar", last modified: Thu Jun  8 21:55:09 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-python-client-2.6.3rc1.tar", last modified: Thu Jun  1 21:38:11 2023, max compression
```

## Comparing `arvados-python-client-2.6.3.tar` & `arvados-python-client-2.6.3rc1.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2952 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6449 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/_normalize_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/_pycurlhelper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/_ranges.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19254 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76741 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/collection.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados/commands/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2127 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/_util.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    32047 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/arv_copy.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18836 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/federation_migrate.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13287 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23786 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/migrate19.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/run.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/commands/ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/config.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/diskcache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/http_to_keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61779 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1208 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/logging.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8235 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3751 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/timer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados/vocabulary.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2952 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2051 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      343 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/arvados_python_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-copy
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-federation-migrate
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-get
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-keepdocker
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-ls
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-migrate-docker19
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-normalize
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-put
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/bin/arv-ws
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2141 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/arvados_testutil.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/keepstub.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/manifest_examples.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:09.000000 arvados-python-client-2.6.3/tests/performance/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/performance/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/performance/performance_profiler.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/performance/test_a_sample.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/run_test_server.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/slow_test.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23177 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_copy.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_normalize.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arv_ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43528 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_benchmark_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77433 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    83499 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_keep_client.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_keep_locator.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_retry_job_helpers.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_sdk.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-06-08 21:55:03.000000 arvados-python-client-2.6.3/tests/test_vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/_normalize_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/_pycurlhelper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/_ranges.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17498 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76741 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/collection.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados/commands/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2127 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/_util.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    32047 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/arv_copy.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18836 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/federation_migrate.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13287 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23786 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/migrate19.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/run.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/commands/ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/config.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/diskcache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/http_to_keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61779 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8235 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3751 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/timer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados/vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2032 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      343 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-copy
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-federation-migrate
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-get
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-keepdocker
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-ls
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-migrate-docker19
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-normalize
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-put
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/bin/arv-ws
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2141 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/arvados_testutil.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/keepstub.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/manifest_examples.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:11.000000 arvados-python-client-2.6.3rc1/tests/performance/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/performance/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/performance/performance_profiler.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/performance/test_a_sample.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/run_test_server.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/slow_test.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21197 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_copy.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_normalize.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arv_ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43528 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_benchmark_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77433 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    83499 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_keep_client.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_keep_locator.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_retry_job_helpers.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_sdk.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-06-01 21:38:09.000000 arvados-python-client-2.6.3rc1/tests/test_vocabulary.py
```

### Comparing `arvados-python-client-2.6.3/LICENSE-2.0.txt` & `arvados-python-client-2.6.3rc1/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/PKG-INFO` & `arvados-python-client-2.6.3rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.3
+Version: 2.6.3rc1
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.3/README.rst` & `arvados-python-client-2.6.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/__init__.py` & `arvados-python-client-2.6.3rc1/arvados/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from builtins import object
 import bz2
 import fcntl
 import hashlib
 import http.client
 import httplib2
 import json
-import logging as stdliblog
+import logging
 import os
 import pprint
 import re
 import string
 import sys
 import time
 import types
@@ -29,29 +29,28 @@
     from UserDict import UserDict
 
 from .api import api, api_from_config, http_cache
 from .collection import CollectionReader, CollectionWriter, ResumableCollectionWriter
 from arvados.keep import *
 from arvados.stream import *
 from .arvfile import StreamFileReader
-from .logging import log_format, log_date_format, log_handler
 from .retry import RetryLoop
 import arvados.errors as errors
 import arvados.util as util
 
-# Override logging module pulled in via `from ... import *`
-# so users can `import arvados.logging`.
-logging = sys.modules['arvados.logging']
-
 # Set up Arvados logging based on the user's configuration.
 # All Arvados code should log under the arvados hierarchy.
-logger = stdliblog.getLogger('arvados')
+log_format = '%(asctime)s %(name)s[%(process)d] %(levelname)s: %(message)s'
+log_date_format = '%Y-%m-%d %H:%M:%S'
+log_handler = logging.StreamHandler()
+log_handler.setFormatter(logging.Formatter(log_format, log_date_format))
+logger = logging.getLogger('arvados')
 logger.addHandler(log_handler)
-logger.setLevel(stdliblog.DEBUG if config.get('ARVADOS_DEBUG')
-                else stdliblog.WARNING)
+logger.setLevel(logging.DEBUG if config.get('ARVADOS_DEBUG')
+                else logging.WARNING)
 
 def task_set_output(self, s, num_retries=5):
     for tries_left in RetryLoop(num_retries=num_retries, backoff_start=0):
         try:
             return api('v1').job_tasks().update(
                 uuid=self['uuid'],
                 body={
```

### Comparing `arvados-python-client-2.6.3/arvados/_normalize_stream.py` & `arvados-python-client-2.6.3rc1/arvados/_normalize_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/_pycurlhelper.py` & `arvados-python-client-2.6.3rc1/arvados/_pycurlhelper.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/_ranges.py` & `arvados-python-client-2.6.3rc1/arvados/_ranges.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/api.py` & `arvados-python-client-2.6.3rc1/arvados/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,31 +19,28 @@
 import json
 import logging
 import os
 import re
 import socket
 import ssl
 import sys
-import threading
 import time
 import types
 
 import apiclient
 import apiclient.http
 from apiclient import discovery as apiclient_discovery
 from apiclient import errors as apiclient_errors
 from . import config
 from . import errors
 from . import retry
 from . import util
 from . import cache
-from .logging import GoogleHTTPClientFilter, log_handler
 
 _logger = logging.getLogger('arvados.api')
-_googleapiclient_log_lock = threading.Lock()
 
 MAX_IDLE_CONNECTION_DURATION = 30
 
 # These constants supported our own retry logic that we've since removed in
 # favor of using googleapiclient's num_retries. They're kept here purely for
 # API compatibility, but set to 0 to indicate no retries happen.
 RETRY_DELAY_INITIAL = 0
@@ -251,52 +248,22 @@
             cache=http_cache('discovery') if cache else None,
             disable_ssl_certificate_validation=bool(insecure),
         )
     if http.timeout is None:
         http.timeout = timeout
     http = _patch_http_request(http, token, num_retries)
 
-    # The first time a client is instantiated, temporarily route
-    # googleapiclient.http retry logs if they're not already. These are
-    # important because temporary problems fetching the discovery document
-    # can cause clients to appear to hang early. This can be removed after
-    # we have a more general story for handling googleapiclient logs (#20521).
-    client_logger = logging.getLogger('googleapiclient.http')
-    # "first time a client is instantiated" = thread that acquires this lock
-    # It is never released.
-    # googleapiclient sets up its own NullHandler so we detect if logging is
-    # configured by looking for a real handler anywhere in the hierarchy.
-    client_logger_unconfigured = _googleapiclient_log_lock.acquire(blocking=False) and all(
-        isinstance(handler, logging.NullHandler)
-        for logger_name in ['', 'googleapiclient', 'googleapiclient.http']
-        for handler in logging.getLogger(logger_name).handlers
+    svc = apiclient_discovery.build(
+        'arvados', version,
+        cache_discovery=False,
+        discoveryServiceUrl=discoveryServiceUrl,
+        http=http,
+        num_retries=num_retries,
+        **kwargs,
     )
-    if client_logger_unconfigured:
-        client_level = client_logger.level
-        client_filter = GoogleHTTPClientFilter()
-        client_logger.addFilter(client_filter)
-        client_logger.addHandler(log_handler)
-        if logging.NOTSET < client_level < client_filter.retry_levelno:
-            client_logger.setLevel(client_level)
-        else:
-            client_logger.setLevel(client_filter.retry_levelno)
-    try:
-        svc = apiclient_discovery.build(
-            'arvados', version,
-            cache_discovery=False,
-            discoveryServiceUrl=discoveryServiceUrl,
-            http=http,
-            num_retries=num_retries,
-            **kwargs,
-        )
-    finally:
-        if client_logger_unconfigured:
-            client_logger.removeHandler(log_handler)
-            client_logger.removeFilter(client_filter)
-            client_logger.setLevel(client_level)
     svc.api_token = token
     svc.insecure = insecure
     svc.request_id = request_id
     svc.config = lambda: util.get_config_once(svc)
     svc.vocabulary = lambda: util.get_vocabulary_once(svc)
     svc.close_connections = types.MethodType(_close_connections, svc)
     http.max_request_size = svc._rootDesc.get('maxRequestSize', 0)
```

### Comparing `arvados-python-client-2.6.3/arvados/arvfile.py` & `arvados-python-client-2.6.3rc1/arvados/arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/cache.py` & `arvados-python-client-2.6.3rc1/arvados/cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/collection.py` & `arvados-python-client-2.6.3rc1/arvados/collection.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/_util.py` & `arvados-python-client-2.6.3rc1/arvados/commands/_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/arv_copy.py` & `arvados-python-client-2.6.3rc1/arvados/commands/arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/federation_migrate.py` & `arvados-python-client-2.6.3rc1/arvados/commands/federation_migrate.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/get.py` & `arvados-python-client-2.6.3rc1/arvados/commands/get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/keepdocker.py` & `arvados-python-client-2.6.3rc1/arvados/commands/keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/ls.py` & `arvados-python-client-2.6.3rc1/arvados/commands/ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/migrate19.py` & `arvados-python-client-2.6.3rc1/arvados/commands/migrate19.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/put.py` & `arvados-python-client-2.6.3rc1/arvados/commands/put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/run.py` & `arvados-python-client-2.6.3rc1/arvados/commands/run.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/commands/ws.py` & `arvados-python-client-2.6.3rc1/arvados/commands/ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/config.py` & `arvados-python-client-2.6.3rc1/arvados/config.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/crunch.py` & `arvados-python-client-2.6.3rc1/arvados/crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/diskcache.py` & `arvados-python-client-2.6.3rc1/arvados/diskcache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/errors.py` & `arvados-python-client-2.6.3rc1/arvados/errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/events.py` & `arvados-python-client-2.6.3rc1/arvados/events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/http_to_keep.py` & `arvados-python-client-2.6.3rc1/arvados/http_to_keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/keep.py` & `arvados-python-client-2.6.3rc1/arvados/keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/retry.py` & `arvados-python-client-2.6.3rc1/arvados/retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/safeapi.py` & `arvados-python-client-2.6.3rc1/arvados/safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/stream.py` & `arvados-python-client-2.6.3rc1/arvados/stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/timer.py` & `arvados-python-client-2.6.3rc1/arvados/timer.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/util.py` & `arvados-python-client-2.6.3rc1/arvados/util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados/vocabulary.py` & `arvados-python-client-2.6.3rc1/arvados/vocabulary.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/arvados_python_client.egg-info/PKG-INFO` & `arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.3
+Version: 2.6.3rc1
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.3/arvados_python_client.egg-info/SOURCES.txt` & `arvados-python-client-2.6.3rc1/arvados_python_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 arvados/config.py
 arvados/crunch.py
 arvados/diskcache.py
 arvados/errors.py
 arvados/events.py
 arvados/http_to_keep.py
 arvados/keep.py
-arvados/logging.py
 arvados/retry.py
 arvados/safeapi.py
 arvados/stream.py
 arvados/timer.py
 arvados/util.py
 arvados/vocabulary.py
 arvados/commands/__init__.py
```

### Comparing `arvados-python-client-2.6.3/arvados_version.py` & `arvados-python-client-2.6.3rc1/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/bin/arv-normalize` & `arvados-python-client-2.6.3rc1/bin/arv-normalize`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/setup.py` & `arvados-python-client-2.6.3rc1/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/arvados_testutil.py` & `arvados-python-client-2.6.3rc1/tests/arvados_testutil.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/keepstub.py` & `arvados-python-client-2.6.3rc1/tests/keepstub.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/manifest_examples.py` & `arvados-python-client-2.6.3rc1/tests/manifest_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/performance/performance_profiler.py` & `arvados-python-client-2.6.3rc1/tests/performance/performance_profiler.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/run_test_server.py` & `arvados-python-client-2.6.3rc1/tests/run_test_server.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_api.py` & `arvados-python-client-2.6.3rc1/tests/test_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from builtins import range
 import arvados
 import collections
 import contextlib
 import httplib2
 import itertools
 import json
-import logging
 import mimetypes
 import os
 import socket
 import string
 import sys
 import unittest
 import urllib.parse as urlparse
@@ -26,18 +25,16 @@
 from apiclient import errors as apiclient_errors
 from apiclient import http as apiclient_http
 from arvados.api import (
     api_client,
     normalize_api_kwargs,
     api_kwargs_from_config,
     OrderedJsonModel,
-    _googleapiclient_log_lock,
 )
 from .arvados_testutil import fake_httplib2_response, mock_api_responses, queue_with
-import httplib2.error
 
 if not mimetypes.inited:
     mimetypes.init()
 
 class ArvadosApiTest(run_test_server.TestCaseWithServers):
     MAIN_SERVER = {}
     ERROR_HEADERS = {'Content-Type': mimetypes.types_map['.json']}
@@ -390,54 +387,14 @@
         ]:
             with self.subTest(f"api_client fails with {arg_index}={arg_value!r}"), \
                  self.assertRaises(apiclient_errors.UnknownApiNameOrVersion):
                 args = list(all_args)
                 args[arg_index] = arg_value
                 api_client(*args, insecure=True)
 
-    def test_initial_retry_logs(self):
-        try:
-            _googleapiclient_log_lock.release()
-        except RuntimeError:
-            # Lock was never acquired - that's the state we want anyway
-            pass
-        real_logger = logging.getLogger('googleapiclient.http')
-        mock_logger = mock.Mock(wraps=real_logger)
-        mock_logger.handlers = logging.getLogger('googleapiclient').handlers
-        mock_logger.level = logging.NOTSET
-        with mock.patch('logging.getLogger', return_value=mock_logger), \
-             mock.patch('time.sleep'), \
-             self.assertLogs(real_logger, 'INFO') as actual_logs:
-            try:
-                api_client('v1', 'https://test.invalid/', 'NoToken', num_retries=1)
-            except httplib2.error.ServerNotFoundError:
-                pass
-        mock_logger.addFilter.assert_called()
-        mock_logger.addHandler.assert_called()
-        mock_logger.setLevel.assert_called()
-        mock_logger.removeHandler.assert_called()
-        mock_logger.removeFilter.assert_called()
-        self.assertRegex(actual_logs.output[0], r'^INFO:googleapiclient\.http:Sleeping \d')
-
-    def test_configured_logger_untouched(self):
-        real_logger = logging.getLogger('googleapiclient.http')
-        mock_logger = mock.Mock(wraps=real_logger)
-        mock_logger.handlers = logging.getLogger().handlers
-        with mock.patch('logging.getLogger', return_value=mock_logger), \
-             mock.patch('time.sleep'):
-            try:
-                api_client('v1', 'https://test.invalid/', 'NoToken', num_retries=1)
-            except httplib2.error.ServerNotFoundError:
-                pass
-        mock_logger.addFilter.assert_not_called()
-        mock_logger.addHandler.assert_not_called()
-        mock_logger.setLevel.assert_not_called()
-        mock_logger.removeHandler.assert_not_called()
-        mock_logger.removeFilter.assert_not_called()
-
 
 class ConstructNumRetriesTestCase(unittest.TestCase):
     @staticmethod
     def _fake_retry_request(http, num_retries, req_type, sleep, rand, uri, method, *args, **kwargs):
         return http.request(uri, method, *args, **kwargs)
 
     @contextlib.contextmanager
```

### Comparing `arvados-python-client-2.6.3/tests/test_arv_copy.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arv_get.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arv_keepdocker.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arv_ls.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arv_normalize.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_normalize.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arv_put.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arv_ws.py` & `arvados-python-client-2.6.3rc1/tests/test_arv_ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_arvfile.py` & `arvados-python-client-2.6.3rc1/tests/test_arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_benchmark_collections.py` & `arvados-python-client-2.6.3rc1/tests/test_benchmark_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_cache.py` & `arvados-python-client-2.6.3rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_collections.py` & `arvados-python-client-2.6.3rc1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_crunch.py` & `arvados-python-client-2.6.3rc1/tests/test_crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_errors.py` & `arvados-python-client-2.6.3rc1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_events.py` & `arvados-python-client-2.6.3rc1/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_http.py` & `arvados-python-client-2.6.3rc1/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_keep_client.py` & `arvados-python-client-2.6.3rc1/tests/test_keep_client.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_keep_locator.py` & `arvados-python-client-2.6.3rc1/tests/test_keep_locator.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_retry.py` & `arvados-python-client-2.6.3rc1/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_retry_job_helpers.py` & `arvados-python-client-2.6.3rc1/tests/test_retry_job_helpers.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_safeapi.py` & `arvados-python-client-2.6.3rc1/tests/test_safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_sdk.py` & `arvados-python-client-2.6.3rc1/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_stream.py` & `arvados-python-client-2.6.3rc1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_util.py` & `arvados-python-client-2.6.3rc1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.3/tests/test_vocabulary.py` & `arvados-python-client-2.6.3rc1/tests/test_vocabulary.py`

 * *Files identical despite different names*

