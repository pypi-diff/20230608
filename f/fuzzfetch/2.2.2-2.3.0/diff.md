# Comparing `tmp/fuzzfetch-2.2.2.tar.gz` & `tmp/fuzzfetch-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzfetch-2.2.2.tar", last modified: Thu Dec  1 23:32:48 2022, max compression
+gzip compressed data, was "fuzzfetch-2.3.0.tar", last modified: Thu Jun  8 15:57:44 2023, max compression
```

## Comparing `fuzzfetch-2.2.2.tar` & `fuzzfetch-2.3.0.tar`

### file list

```diff
@@ -1,1359 +1,1359 @@
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)       55 2022-03-28 16:09:31.000000 fuzzfetch-2.2.2/.codecov.yml
--rw-r--r--   0 jkratzer  (1000) jkratzer  (1000)      386 2019-12-06 00:16:58.000000 fuzzfetch-2.2.2/.gitignore
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1784 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/.pre-commit-config.yaml
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     3530 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/.taskcluster.yml
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      689 2021-05-07 13:25:16.000000 fuzzfetch-2.2.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    15550 2021-05-07 13:25:16.000000 fuzzfetch-2.2.2/LICENSE.md
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     5422 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/PKG-INFO
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4501 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/README.md
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      891 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/pyproject.toml
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1171 2022-12-01 23:32:48.185680 fuzzfetch-2.2.2/setup.cfg
--rwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)      370 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/setup.py
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/src/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.977683 fuzzfetch-2.2.2/src/fuzzfetch/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      586 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/__init__.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      266 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/__main__.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     9531 2022-12-01 23:29:31.000000 fuzzfetch-2.2.2/src/fuzzfetch/args.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    32112 2022-12-01 23:29:31.000000 fuzzfetch-2.2.2/src/fuzzfetch/core.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     2886 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/download.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      358 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/errors.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     5631 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/extract.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    13235 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/models.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     2685 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/src/fuzzfetch/path.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)        0 2021-08-03 17:51:00.000000 fuzzfetch-2.2.2/src/fuzzfetch/py.typed
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.981683 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     5422 2022-12-01 23:32:47.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/PKG-INFO
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    74557 2022-12-01 23:32:47.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/SOURCES.txt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)        1 2022-12-01 23:32:47.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/dependency_links.txt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)       53 2022-12-01 23:32:47.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/entry_points.txt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)        1 2020-12-16 16:11:12.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/not-zip-safe
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)       82 2022-12-01 23:32:47.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/requires.txt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)       10 2022-12-01 23:32:47.000000 fuzzfetch-2.2.2/src/fuzzfetch.egg-info/top_level.txt
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.981683 fuzzfetch-2.2.2/tests/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     3880 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/conftest.py
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.993682 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      522 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.06
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      522 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.09
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      693 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.04
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      693 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.08
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)       23 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.09
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1035 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.04
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      864 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.10
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      693 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.18
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      522 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.21
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      185 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2020.06.06
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2020.06.09
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2021.06.04
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2021.06.08
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)       23 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2021.06.09
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.08.04
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.08.10
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.11.18
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      341 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.11.21
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      349 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr102.pushdate.2022.11.17
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      339 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr102.shippable.2022.11.17
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    24654 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.04
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    30219 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.08
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    26721 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.08.10
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    22269 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.18
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    14796 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.21
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      317 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2021.06.04
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      317 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2021.06.08
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      317 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2022.08.10
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      317 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2022.11.18
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      317 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2022.11.21
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      188 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      193 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      201 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      190 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      205 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-nyx-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      201 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      198 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      201 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      193 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      197 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-valgrind-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      210 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      207 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      191 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      202 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      199 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      202 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.sm-linux64-fuzzilli-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      188 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-aarch64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      191 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      199 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-fuzzing-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      182 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      188 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.mobile.android-api-16-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      201 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.mobile.android-x86-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      224 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.04.20210604102111.mobile.android-api-16-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      221 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-ccov-fuzzing-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-ccov-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      218 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      226 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-fuzzing-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      221 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      225 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-valgrind-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      219 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      224 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.win64-aarch64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      219 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.win64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.mobile.android-x86-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608091819.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608155750.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      208 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.08.04.20220804043413.firefox.linux64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.08.10.20220810043040.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      224 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win32-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win64-ccov-fuzzing-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      210 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win64-ccov-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      224 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      238 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.21.20221121093640.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      235 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.21.20221121093640.firefox.macosx64-aarch64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.23d50b5617def9d4152023fd98210c0a9723e3c0.firefox.linux64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      231 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.24938c537a55f9db3913072d33b178b210e7d6b5.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      242 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      239 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win32-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      242 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win64-ccov-fuzzing-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      225 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win64-ccov-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      239 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      239 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.61484a56d30a2bbc5a3d6903e6258ae3acd714bf.mobile.android-api-16-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      231 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      236 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      244 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-ccov-fuzzing-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-ccov-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      233 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      244 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      241 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      244 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-fuzzing-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      231 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      236 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      240 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-valgrind-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      234 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      245 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      239 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-aarch64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      237 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      234 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      231 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      244 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-x86-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      231 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.c48baf52b5d666a2c67cf9e47ec408cf7e1c3281.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.c48baf52b5d666a2c67cf9e47ec408cf7e1c3281.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      253 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.ec2ad590b1485ab7d895d3d8ba9434739f8dd603.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      250 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.ec2ad590b1485ab7d895d3d8ba9434739f8dd603.firefox.macosx64-aarch64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      209 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2020.06.09.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.04.latest.mobile.android-api-16-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      207 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      209 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      210 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.win64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      207 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      216 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.mobile.android-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.mobile.android-x86-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.mobile.android-x86_64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      207 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2022.08.10.latest.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      218 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2022.11.18.latest.firefox.macosx64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      198 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      207 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      199 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      196 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      205 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-api-16-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      201 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86_64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      250 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.macosx64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      247 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.61484a56d30a2bbc5a3d6903e6258ae3acd714bf.mobile.android-api-16-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      239 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      242 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      239 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      248 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      244 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-x86-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      247 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-x86_64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      192 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      189 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      200 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      197 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      190 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      201 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      198 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      220 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      217 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      228 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      225 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      218 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      226 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      235 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      232 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      243 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      240 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      233 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      244 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      241 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      228 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      206 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      208 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      209 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      206 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      206 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      197 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      198 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      238 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      241 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      238 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      176 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      175 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      181 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      178 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      189 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      186 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      189 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      181 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      185 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-valgrind-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      198 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      179 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      190 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      176 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-aarch64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      176 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.mobile.android-api-16-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      189 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.mobile.android-x86-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      209 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      206 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      217 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      214 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      217 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-fuzzing-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      209 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      207 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      218 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.win64-aarch64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      217 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.mobile.android-x86-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608003958.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608075328.mobile.android-api-16-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      213 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608152401.firefox.linux64-valgrind-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.08.10.20220810000056.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      203 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.linux64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.win32-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.win64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      215 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118145344.firefox.linux-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      212 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118145344.firefox.linux-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      226 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.21.20221121064514.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      223 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.21.20221121064514.firefox.macosx64-aarch64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      217 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.0547f30d952e6c2114c016931d22e674ddf979b2.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      218 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.06759ac6f0a0520ad12fdb1bd15153d0dad3d4ce.firefox.linux64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      225 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.07465e448535839fec01901d138272da43c65419.firefox.win64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      226 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.07465e448535839fec01901d138272da43c65419.mobile.android-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      224 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.1ce3156a65999be49e3e7a09063095a33c8419c9.firefox.linux64-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      222 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.1ce3156a65999be49e3e7a09063095a33c8419c9.firefox.macosx64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      219 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.1ce3156a65999be49e3e7a09063095a33c8419c9.firefox.win64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      228 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.3de9c0f587a7c4bfd19e837c7b4061397d587788.firefox.linux64-valgrind-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.5aa051db918dab86c02e777058919783d750851d.firefox.linux-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.5aa051db918dab86c02e777058919783d750851d.firefox.linux-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      217 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.703dfca614b098dfe633c167400f87a56d8ab24a.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      232 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.linux64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.linux64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      232 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.linux64-fuzzing-tsan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      233 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.macosx64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.win64-aarch64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.8031852ced6910fac9ab16c1f002bdd61ff7a3b2.mobile.android-api-16-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      241 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.9791bdb6208f5f9b69e7bab87c45f358312ed06e.firefox.macosx64-aarch64-fuzzing-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      238 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.9791bdb6208f5f9b69e7bab87c45f358312ed06e.firefox.macosx64-aarch64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      224 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ba61ef86b157c63050d313a12b7bd40d1ed44435.firefox.linux64-asan-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      221 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.d6ee22ff0b33856f73a467af9c60088311b77c0c.firefox.linux64-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      219 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e18b328a3bd5837ed932e0934d3976f8131b094f.firefox.linux-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e72dcb1faf05191e689ef94b756ffcda514f2531.firefox.macosx64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e72dcb1faf05191e689ef94b756ffcda514f2531.firefox.win32-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e72dcb1faf05191e689ef94b756ffcda514f2531.firefox.win64-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      225 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.f33d0ad1e90da6318f81a62d66edc9bc43384699.mobile.android-api-16-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      219 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.f56f27ff9c0fb3c901be7f8661358c4e3ed18cf8.firefox.win32-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      232 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.fb147ea9f80500e2191ad6489de2a8f082919bc6.mobile.android-x86-fuzzing-debug
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      203 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.04.latest.mobile.android-api-16-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      197 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      198 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      203 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.win64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      204 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.mobile.android-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      200 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.mobile.android-x86-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      203 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.mobile.android-x86_64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2022.08.10.latest.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      206 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2022.11.18.latest.firefox.macosx64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      186 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      195 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      187 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win32-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      192 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      184 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      193 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      192 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-api-16-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      189 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      192 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86_64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      227 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.07465e448535839fec01901d138272da43c65419.firefox.linux-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      232 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.4119fae76a8f8c4d613ce6fd491c514b525b9b05.mobile.android-x86-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      235 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.4119fae76a8f8c4d613ce6fd491c514b525b9b05.mobile.android-x86_64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      230 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.703dfca614b098dfe633c167400f87a56d8ab24a.firefox.macosx64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      238 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.7b5b77dd3f3faa76362dd0dea4cf961cd75d374c.firefox.macosx64-aarch64-opt
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      229 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.fc3b84c96d35d6e0a6a98ffa81e660e88b511e3a.firefox.linux64-opt
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4185 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1174 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      917 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1067 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.909684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    14322 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.085681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      930 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      961 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4565 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1033 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      919 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    11538 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1067 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6248 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1064 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4568 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.089681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      991 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      993 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7734 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      871 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      968 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6773 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      669 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4565 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1033 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      919 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.093681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6608 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      697 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7295 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      952 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      923 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4573 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.097681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1003 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      993 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    13811 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      926 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      955 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.101681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1087 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      913 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7689 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1048 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      965 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.913684 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    14054 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      955 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1075 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      913 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.105681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1181 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      912 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1388 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      990 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      959 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      974 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4573 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      999 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      996 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.109681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4017 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4552 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1264 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      966 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6248 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1206 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      966 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7687 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1017 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.113681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     5438 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      975 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1001 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8176 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1051 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1184 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      969 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4565 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1021 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      919 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.117681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      963 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      971 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    14027 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      950 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      954 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    11148 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      694 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      952 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7295 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      952 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      923 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.121681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7689 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      954 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      909 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7687 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      935 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1418 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      100 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      912 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7513 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      952 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      904 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.125681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8172 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.917683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      909 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7687 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      947 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7674 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1076 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      906 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6934 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.129681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      665 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7307 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      839 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      879 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1181 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      912 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      945 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      970 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6248 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1056 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.133681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7674 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1186 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      962 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4394 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      987 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      996 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    13892 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      935 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      963 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    11538 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.137681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1067 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7878 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1390 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      991 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1334 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      968 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1176 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      966 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.141681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      957 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      969 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    11538 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1055 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      955 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.921683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7878 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1402 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      991 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1067 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.145681 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1244 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      970 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8176 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1051 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8592 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      967 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1001 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1181 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      971 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7687 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      935 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.149680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7486 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1399 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      995 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7734 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      879 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      968 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4691 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7486 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1387 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      995 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1342 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      968 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7687 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.153680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      947 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7687 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1033 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      918 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7878 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1400 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      990 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4568 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      987 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      996 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6763 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      663 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      963 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      957 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      970 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    14079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.925683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      938 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      961 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.157680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7513 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      971 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      904 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    11484 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1055 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      964 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      957 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      970 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4691 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7298 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1240 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      986 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1087 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      913 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     6608 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      678 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      963 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      970 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.161680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4573 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1003 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      993 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7355 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      877 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      972 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4017 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1067 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4185 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1186 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      917 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7674 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1088 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      906 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8176 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1039 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1176 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      967 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4394 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      991 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      993 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.165680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7878 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1388 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      990 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1075 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      913 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    14135 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      942 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      954 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.929683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1181 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      971 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1169 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      912 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7513 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1058 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      960 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.169680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      915 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7674 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1088 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      906 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7355 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.933683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      881 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      969 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4565 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1021 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      919 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1072 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4185 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1186 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      917 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8592 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.941683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      967 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1001 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7850 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7674 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1076 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      906 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7458 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1084 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      911 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.173680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7516 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      945 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      969 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7878 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1400 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      990 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.945683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7533 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.949683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1262 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      989 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4228 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1192 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      988 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7307 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1339 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      973 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4407 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1192 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      988 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7293 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1237 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      988 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7699 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.957683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1169 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      912 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8172 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      909 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    13973 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      954 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      962 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4017 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1079 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      910 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.961683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.177680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4573 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      999 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      996 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7878 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1390 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      991 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    11538 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1055 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     8176 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1039 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      956 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7689 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      962 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      909 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     4185 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1174 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      917 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.965683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     5438 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      975 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1001 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7486 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1387 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      995 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7717 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1270 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      989 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     7345 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/.get
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      869 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      916 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.mozinfo.json
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-hg/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-hg/mozilla-central/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-hg/mozilla-central/json-rev/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)   138719 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-hg/mozilla-central/json-rev/24938c537a55
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)    36254 2021-06-09 14:19:57.000000 fuzzfetch-2.2.2/tests/mock-hg/mozilla-central/json-rev/32fba417ebd01dfb2c2a392cdb1fad7ef66e96e8
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:47.969683 fuzzfetch-2.2.2/tests/mock-product-details/
-drwxrwxr-x   0 jkratzer  (1000) jkratzer  (1000)        0 2022-12-01 23:32:48.181680 fuzzfetch-2.2.2/tests/mock-product-details/1.0/
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)      702 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/mock-product-details/1.0/firefox_versions.json
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     2266 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/test_extract.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     9085 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tests/test_fetch.py
--rw-rw-r--   0 jkratzer  (1000) jkratzer  (1000)     1290 2022-11-29 14:37:56.000000 fuzzfetch-2.2.2/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)       55 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/.codecov.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      386 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     1783 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     3570 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    15550 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/LICENSE.md
+-rw-r--r--   0 worker    (1000) worker    (1000)     5422 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     4501 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)      891 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1171 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.960429 fuzzfetch-2.3.0/src/fuzzfetch/
+-rw-r--r--   0 worker    (1000) worker    (1000)      586 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      266 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/__main__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9531 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/args.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    31860 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/core.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2886 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/download.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      358 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/errors.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     5634 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/extract.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    13232 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/models.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2685 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/path.py
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/src/fuzzfetch/py.typed
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.960429 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     5422 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)    74557 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       53 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)       82 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)       10 2023-06-08 15:57:43.000000 fuzzfetch-2.3.0/src/fuzzfetch.egg-info/top_level.txt
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.960429 fuzzfetch-2.3.0/tests/
+-rw-r--r--   0 worker    (1000) worker    (1000)     3880 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/conftest.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.968429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/
+-rw-r--r--   0 worker    (1000) worker    (1000)      522 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.06
+-rw-r--r--   0 worker    (1000) worker    (1000)      522 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.09
+-rw-r--r--   0 worker    (1000) worker    (1000)      693 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      693 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.08
+-rw-r--r--   0 worker    (1000) worker    (1000)       23 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.09
+-rw-r--r--   0 worker    (1000) worker    (1000)     1035 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      864 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.10
+-rw-r--r--   0 worker    (1000) worker    (1000)      693 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.18
+-rw-r--r--   0 worker    (1000) worker    (1000)      522 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.21
+-rw-r--r--   0 worker    (1000) worker    (1000)      185 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2020.06.06
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2020.06.09
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2021.06.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2021.06.08
+-rw-r--r--   0 worker    (1000) worker    (1000)       23 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2021.06.09
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.08.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.08.10
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.11.18
+-rw-r--r--   0 worker    (1000) worker    (1000)      341 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.shippable.2022.11.21
+-rw-r--r--   0 worker    (1000) worker    (1000)      349 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr102.pushdate.2022.11.17
+-rw-r--r--   0 worker    (1000) worker    (1000)      339 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-esr102.shippable.2022.11.17
+-rw-r--r--   0 worker    (1000) worker    (1000)    24654 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.04
+-rw-r--r--   0 worker    (1000) worker    (1000)    30219 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.08
+-rw-r--r--   0 worker    (1000) worker    (1000)    26721 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.08.10
+-rw-r--r--   0 worker    (1000) worker    (1000)    22269 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.18
+-rw-r--r--   0 worker    (1000) worker    (1000)    14796 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.21
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2021.06.04
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2021.06.08
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2022.08.10
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2022.11.18
+-rw-r--r--   0 worker    (1000) worker    (1000)      317 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.shippable.2022.11.21
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/
+-rw-r--r--   0 worker    (1000) worker    (1000)      188 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      190 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-nyx-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.linux64-valgrind-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      191 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      202 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      199 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      202 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.sm-linux64-fuzzilli-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      188 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      191 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      199 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      182 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      188 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.mobile.android-api-16-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.latest.mobile.android-x86-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.04.20210604102111.mobile.android-api-16-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.linux64-valgrind-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.win64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608040833.mobile.android-x86-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608091819.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.20210608155750.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      208 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2021.06.08.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.08.04.20220804043413.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.08.10.20220810043040.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.18.20221118041845.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.21.20221121093640.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.pushdate.2022.11.21.20221121093640.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.23d50b5617def9d4152023fd98210c0a9723e3c0.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.24938c537a55f9db3913072d33b178b210e7d6b5.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      242 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      242 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.61484a56d30a2bbc5a3d6903e6258ae3acd714bf.mobile.android-api-16-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      236 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-ccov-fuzzing-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-ccov-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      233 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      236 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      240 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux64-valgrind-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      234 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      245 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      237 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      234 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-x86-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      231 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.c48baf52b5d666a2c67cf9e47ec408cf7e1c3281.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.c48baf52b5d666a2c67cf9e47ec408cf7e1c3281.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      253 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.ec2ad590b1485ab7d895d3d8ba9434739f8dd603.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      250 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.revision.ec2ad590b1485ab7d895d3d8ba9434739f8dd603.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2020.06.09.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.04.latest.mobile.android-api-16-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      210 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      216 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2021.06.08.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2022.08.10.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.2022.11.18.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      199 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      196 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-api-16-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      250 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.3b5a8f67189bd6549f0da19ea5da4a53f7e5c79a.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      247 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.61484a56d30a2bbc5a3d6903e6258ae3acd714bf.mobile.android-api-16-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      242 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      239 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      248 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      247 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-central.shippable.revision.a5021586700fde2e70f3f39ca335557c874832fa.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      200 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      190 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      201 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.latest.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      220 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      228 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.pushdate.2022.11.17.20221117142136.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      243 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      240 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      233 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      228 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      208 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.2022.11.17.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.mozilla-esr102.shippable.revision.83fd4c934380d8c103220d8d6bae8b7714cbe572.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      175 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      181 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      178 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      186 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      181 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      185 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.linux64-valgrind-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      179 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      190 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.mobile.android-api-16-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.latest.mobile.android-x86-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      214 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      209 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      207 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608002426.mobile.android-x86-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608003958.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608075328.mobile.android-api-16-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      213 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2021.06.08.20210608152401.firefox.linux64-valgrind-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.08.10.20220810000056.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118003844.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      215 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118145344.firefox.linux-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      212 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.18.20221118145344.firefox.linux-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.21.20221121064514.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      223 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.pushdate.2022.11.21.20221121064514.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.0547f30d952e6c2114c016931d22e674ddf979b2.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      218 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.06759ac6f0a0520ad12fdb1bd15153d0dad3d4ce.firefox.linux64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.07465e448535839fec01901d138272da43c65419.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      226 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.07465e448535839fec01901d138272da43c65419.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.1ce3156a65999be49e3e7a09063095a33c8419c9.firefox.linux64-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      222 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.1ce3156a65999be49e3e7a09063095a33c8419c9.firefox.macosx64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.1ce3156a65999be49e3e7a09063095a33c8419c9.firefox.win64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      228 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.3de9c0f587a7c4bfd19e837c7b4061397d587788.firefox.linux64-valgrind-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.5aa051db918dab86c02e777058919783d750851d.firefox.linux-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.5aa051db918dab86c02e777058919783d750851d.firefox.linux-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      217 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.703dfca614b098dfe633c167400f87a56d8ab24a.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.linux64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.linux64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.linux64-fuzzing-tsan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      233 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.macosx64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.7424b595506aef9ec1ac98c0c2d31f3c2b03d84e.firefox.win64-aarch64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.8031852ced6910fac9ab16c1f002bdd61ff7a3b2.mobile.android-api-16-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      241 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.9791bdb6208f5f9b69e7bab87c45f358312ed06e.firefox.macosx64-aarch64-fuzzing-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.9791bdb6208f5f9b69e7bab87c45f358312ed06e.firefox.macosx64-aarch64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      224 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.ba61ef86b157c63050d313a12b7bd40d1ed44435.firefox.linux64-asan-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      221 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.d6ee22ff0b33856f73a467af9c60088311b77c0c.firefox.linux64-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e18b328a3bd5837ed932e0934d3976f8131b094f.firefox.linux-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e72dcb1faf05191e689ef94b756ffcda514f2531.firefox.macosx64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e72dcb1faf05191e689ef94b756ffcda514f2531.firefox.win32-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.e72dcb1faf05191e689ef94b756ffcda514f2531.firefox.win64-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      225 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.f33d0ad1e90da6318f81a62d66edc9bc43384699.mobile.android-api-16-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      219 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.f56f27ff9c0fb3c901be7f8661358c4e3ed18cf8.firefox.win32-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.revision.fb147ea9f80500e2191ad6489de2a8f082919bc6.mobile.android-x86-fuzzing-debug
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.04.latest.mobile.android-api-16-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      197 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      198 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      204 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      200 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      203 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2021.06.08.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2022.08.10.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      206 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.2022.11.18.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      186 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.linux64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      195 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      187 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win32-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.firefox.win64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      193 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-api-16-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      189 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      192 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.latest.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      227 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.07465e448535839fec01901d138272da43c65419.firefox.linux-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      232 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.4119fae76a8f8c4d613ce6fd491c514b525b9b05.mobile.android-x86-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      235 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.4119fae76a8f8c4d613ce6fd491c514b525b9b05.mobile.android-x86_64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      230 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.703dfca614b098dfe633c167400f87a56d8ab24a.firefox.macosx64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.7b5b77dd3f3faa76362dd0dea4cf961cd75d374c.firefox.macosx64-aarch64-opt
+-rw-r--r--   0 worker    (1000) worker    (1000)      229 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/task/gecko.v2.try.shippable.revision.fc3b84c96d35d6e0a6a98ffa81e660e88b511e3a.firefox.linux64-opt
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4185 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1174 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      917 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.904429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1067 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    14322 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      930 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      961 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4565 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1033 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      919 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.012430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    11538 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1067 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6248 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1064 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4568 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      991 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7734 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      871 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      968 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6773 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      669 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4565 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1033 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      919 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6608 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      697 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.908429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.016430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7295 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      952 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      923 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4573 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1003 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    13811 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      926 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      955 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1087 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      913 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7689 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.020430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1048 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      965 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    14054 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      955 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1075 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      913 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1181 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      912 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.912429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1388 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      990 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      959 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      974 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4573 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      999 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      996 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.024430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4017 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4552 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1264 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      966 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6248 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1206 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      966 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7687 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1017 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     5438 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      975 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     1001 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1051 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.028430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1184 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      969 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4565 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1021 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      919 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      963 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      971 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    14027 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.916429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      950 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      954 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    11148 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      694 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      952 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7295 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      952 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      923 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.032430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7689 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      954 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      909 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7687 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      935 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1418 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      100 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      912 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7513 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      952 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      904 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8172 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      909 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7687 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      947 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.036430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7674 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1076 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      906 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6934 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      665 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.920429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7307 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      839 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      879 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1181 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      912 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      945 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      970 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6248 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1056 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.040430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7674 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1186 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      962 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4394 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      987 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      996 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    13892 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      935 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      963 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    11538 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1067 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7878 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1390 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      991 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1334 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      968 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      966 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.924429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.044430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      957 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      969 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    11538 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1055 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      955 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7878 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1402 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      991 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1067 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1244 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      970 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.048430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1051 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8592 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     1001 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1181 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      971 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7687 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.928429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      935 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7486 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1399 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      995 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7734 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      879 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      968 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4691 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7486 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1387 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      995 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.052430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1342 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      968 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7687 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      947 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7687 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1033 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      918 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7878 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1400 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      990 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4568 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.932429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      987 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      996 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6763 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      663 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      963 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      957 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      970 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    14079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.056430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      938 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      961 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7513 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      971 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      904 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    11484 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1055 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      964 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      957 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      970 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4691 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7298 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1240 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      986 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1087 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      913 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6608 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      678 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.936429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.060430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      963 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      970 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4573 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1003 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7355 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      877 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      972 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4017 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1067 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4185 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1186 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      917 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7674 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1088 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      906 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1039 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4394 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      991 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      993 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.064430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7878 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1388 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      990 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.940429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1075 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      913 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    14135 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      942 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      954 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1181 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      971 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1169 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      912 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7513 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1058 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      960 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      915 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7674 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1088 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      906 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7355 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.068430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      881 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      969 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4565 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.944429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1021 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      919 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1072 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4185 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1186 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      917 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8592 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      967 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     1001 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7850 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7674 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.072430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1076 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      906 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7458 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1084 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      911 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7516 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      945 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      969 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7878 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1400 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      990 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7533 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1262 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      989 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4228 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.948429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1192 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      988 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7307 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.076430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1339 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      973 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4407 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1192 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      988 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7293 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1237 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      988 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7699 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1169 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      912 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8172 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      909 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    13973 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/
+-rw-r--r--   0 worker    (1000) worker    (1000)      954 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      962 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4017 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1079 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      910 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4573 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      999 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      996 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7878 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1390 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      991 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)    11538 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.080430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1055 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.952429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     8176 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1039 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      956 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7689 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      962 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      909 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     4185 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1174 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      917 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     5438 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      975 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     1001 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7486 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1387 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      995 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7717 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.084430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1270 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      989 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7345 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/.get
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/
+-rw-r--r--   0 worker    (1000) worker    (1000)      869 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.json
+-rw-r--r--   0 worker    (1000) worker    (1000)      916 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.mozinfo.json
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-hg/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-hg/mozilla-central/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/tests/mock-hg/mozilla-central/json-rev/
+-rw-r--r--   0 worker    (1000) worker    (1000)   138719 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-hg/mozilla-central/json-rev/24938c537a55
+-rw-r--r--   0 worker    (1000) worker    (1000)    36254 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-hg/mozilla-central/json-rev/32fba417ebd01dfb2c2a392cdb1fad7ef66e96e8
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:43.956429 fuzzfetch-2.3.0/tests/mock-product-details/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-06-08 15:57:44.088430 fuzzfetch-2.3.0/tests/mock-product-details/1.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)      702 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/mock-product-details/1.0/firefox_versions.json
+-rw-r--r--   0 worker    (1000) worker    (1000)     2266 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/test_extract.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9085 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tests/test_fetch.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1304 2023-06-08 15:57:36.000000 fuzzfetch-2.3.0/tox.ini
```

### Comparing `fuzzfetch-2.2.2/.pre-commit-config.yaml` & `fuzzfetch-2.3.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 repos:
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/yesqa
     rev: v1.4.0
     hooks:
       - id: yesqa
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.2
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: ['--py37-plus']
   - repo: https://github.com/ambv/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/pre-commit-hooks
@@ -33,15 +33,15 @@
       - id: trailing-whitespace
       - id: check-yaml
       - id: mixed-line-ending
       - id: name-tests-test
         args: ['--django']
       - id: check-json
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         exclude_types: [json]
         exclude: ^tests/mock-+
   - repo: https://github.com/marco-c/taskcluster_yml_validator
     rev: v0.0.9
     hooks:
```

### Comparing `fuzzfetch-2.2.2/.taskcluster.yml` & `fuzzfetch-2.3.0/.taskcluster.yml`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,16 @@
             version: "3.11"
             env:
               TOXENV: py311
           - name: lint python 3.11
             version: "3.11"
             env:
               TOXENV: lint
+            script:
+              - tox
           - name: PyPI upload
             version: "3.11"
             env:
               TOXENV: pypi
             script:
               - tox
             when:
```

### Comparing `fuzzfetch-2.2.2/CODE_OF_CONDUCT.md` & `fuzzfetch-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/LICENSE.md` & `fuzzfetch-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/PKG-INFO` & `fuzzfetch-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzfetch
-Version: 2.2.2
+Version: 2.3.0
 Summary: Downloader for firefox/jsshell builds.
 Home-page: https://github.com/MozillaSecurity/fuzzfetch
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz fuzzing security test testing
 Platform: any
```

### Comparing `fuzzfetch-2.2.2/README.md` & `fuzzfetch-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/pyproject.toml` & `fuzzfetch-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/setup.cfg` & `fuzzfetch-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/__init__.py` & `fuzzfetch-2.3.0/src/fuzzfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/args.py` & `fuzzfetch-2.3.0/src/fuzzfetch/args.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/core.py` & `fuzzfetch-2.3.0/src/fuzzfetch/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 if version_info[:2] < (3, 8):
     # pylint: disable=import-error
     from importlib_metadata import PackageNotFoundError, version
 else:
     # pylint: disable=import-error
     from importlib.metadata import PackageNotFoundError, version
 
-
 try:
     __version__ = version("fuzzfetch")
 except PackageNotFoundError:
     # package is not installed
     __version__ = None
 
 LOG = logging.getLogger("fuzzfetch")
@@ -294,23 +293,15 @@
 
             if build == "latest" and (now - self.datetime).total_seconds() > 86400:
                 LOG.warning("Latest available build is older than 1 day: %s", self.id)
 
         else:
             self._task = build
 
-        # build the automatic name
-        if (
-            not isinstance(build, BuildTask)
-            and isinstance(self.moz_info["platform_guess"], str)
-            and self.moz_info["platform_guess"] in build
-        ):
-            options = build.split(self.moz_info["platform_guess"], 1)[1]
-        else:
-            options = self._flags.build_string()
+        options = self._flags.build_string()
         if self._branch in {"autoland", "try"}:
             branch = self._branch
         else:
             branch = f"m-{self._branch[0]}"
         self._auto_name = (
             f"{self._platform.auto_name_prefix()}{branch}-{self.id}{options}"
         )
@@ -385,15 +376,22 @@
         """Return the build's revision"""
         return self.build_info["moz_source_stamp"]
 
     @property
     def moz_info(self) -> Dict[str, Union[str, bool, int]]:
         """Return the build's mozinfo"""
         if "moz_info" not in self._memo:
-            self._memo["moz_info"] = get_url(self.artifact_url("mozinfo.json")).json()
+            try:
+                self._memo["moz_info"] = get_url(
+                    self.artifact_url("mozinfo.json")
+                ).json()
+            except FetcherException:
+                # If mozinfo doesn't exist, set the default topsrcdir
+                self._memo["moz_info"] = {"topsrcdir": "/builds/worker/checkouts/gecko"}
+
         assert isinstance(self._memo["moz_info"], dict)
         return self._memo["moz_info"]
 
     @property
     def rank(self) -> int:
         """Return the build's rank"""
         assert isinstance(self._task, BuildTask)
@@ -592,33 +590,27 @@
 
         Arguments:
             target: firefox/js
             path: fuzzmanager config path
         """
         output = configparser.RawConfigParser()
         output.add_section("Main")
-        processor = self.moz_info["processor"]
+        processor = self._platform.machine
         assert isinstance(processor, str)
         output.set("Main", "platform", processor.replace("_", "-"))
         output.set("Main", "product", f"mozilla-{self._branch}")
         output.set("Main", "product_version", f"{self.id:.8}-{self.changeset:.12}")
-        # make sure 'os' match what FM expects
-        os_cfg = self.moz_info["os"]
-        assert isinstance(os_cfg, str)
-        os_name = os_cfg.lower()
-        if os_name.startswith("android"):
+        if self._platform.system == "Android":
             output.set("Main", "os", "android")
-        elif os_name.startswith("lin"):
+        elif self._platform.system == "Linux":
             output.set("Main", "os", "linux")
-        elif os_name.startswith("mac"):
+        elif self._platform.system == "Darwin":
             output.set("Main", "os", "macosx")
-        elif os_name.startswith("win"):
+        elif self._platform.system == "Windows":
             output.set("Main", "os", "windows")
-        else:
-            output.set("Main", "os", os_cfg)
         output.add_section("Metadata")
         topsrcdir = self.moz_info["topsrcdir"]
         assert isinstance(topsrcdir, str)
         output.set("Metadata", "pathPrefix", topsrcdir)
         output.set("Metadata", "buildType", self._flags.build_string().lstrip("-"))
 
         if self._platform.system == "Windows":
```

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/download.py` & `fuzzfetch-2.3.0/src/fuzzfetch/download.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/extract.py` & `fuzzfetch-2.3.0/src/fuzzfetch/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             cmd.extend(("-xf", str(tar_fn)))
             check_call(cmd)
         else:
             with tarfile.open(tar_fn, mode=f"r:{mode}") as tar:
                 members = []
                 for member in tar.getmembers():
                     if not _is_within_directory(path, Path(path) / member.name):
-                        raise Exception("Attempted Path Traversal in Tar File")
+                        raise RuntimeError("Attempted Path Traversal in Tar File")
                     if member.name.startswith("firefox/"):
                         member.name = member.name[8:]
                         members.append(member)
                     elif member.name != "firefox":
                         # Ignore top-level build directory
                         members.append(member)
                 tar.extractall(members=members, path=path)
```

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/models.py` & `fuzzfetch-2.3.0/src/fuzzfetch/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,18 +173,17 @@
 
         else:
             # try to use build argument directly as a namespace
             task_path = f"/task/{build}"
             is_namespace = True
             task_template_paths = ((cls.TASKCLUSTER_API, task_path),)
 
-        for (template_path, try_wo_opt) in itertools.product(
+        for template_path, try_wo_opt in itertools.product(
             task_template_paths, (False, True)
         ):
-
             template, path = template_path
 
             if try_wo_opt:
                 if "-opt" not in path or is_namespace:
                     continue
                 path = path.replace("-opt", "")
```

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch/path.py` & `fuzzfetch-2.3.0/src/fuzzfetch/path.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch.egg-info/PKG-INFO` & `fuzzfetch-2.3.0/src/fuzzfetch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzfetch
-Version: 2.2.2
+Version: 2.3.0
 Summary: Downloader for firefox/jsshell builds.
 Home-page: https://github.com/MozillaSecurity/fuzzfetch
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz fuzzing security test testing
 Platform: any
```

### Comparing `fuzzfetch-2.2.2/src/fuzzfetch.egg-info/SOURCES.txt` & `fuzzfetch-2.3.0/src/fuzzfetch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/conftest.py` & `fuzzfetch-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.06` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.06`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.09` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2020.06.09`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.04` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.04`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.08` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2021.06.08`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.04` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.04`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.10` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.08.10`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.18` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.18`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.21` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.mozilla-central.pushdate.2022.11.21`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.04` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.04`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.08` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2021.06.08`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.08.10` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.08.10`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.18` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.18`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.21` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/index/v1/namespaces/gecko.v2.try.pushdate.2022.11.21`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AIHXH3fUR3ycXNpr0zZqrg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AM-ziKlUQVmZPbH7EOrDfw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AOE-3z0-SGOh7CWbjijxnA/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/AQp7yuOrSa6As8Fy_sk9Tw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Al9ARG6yTa2ouCDFtvGrRQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Aq0k4cb9TIK7GRlawjJ7jA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BB34i6iBTEK_cMwMtt6aLw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BG3ISZV-Rue7vzLGN2gmAQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BM2I6HQ_QYuCcerJSpMv9w/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BUxkeTC-TSKXVY8PWUTa1g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Bdv6e5gjRKyKHAI85Cuz3g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BoXhgvh7Sk2a7hJ-BeK3VA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/BukaBezMSZS5oaZzm82SSg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CNcbd9tRT4aJ1lZPDjKHbQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CVGYA728Ru6Kyl4NITwFPQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/CppP0yhERdKFQwFqiTb8Kw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Dfxp34t2QJSgzeQeyc4zIw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DhULMxzrSg-ugmG5fapYfQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/DqKoKPCFQDKCNmos7fHwZQ/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/E7NK8SGcT2WEkx_Kz8v9aw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EB4DstCzTZa1t2nXPAlqwA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EM8f7jnZRdmccoN_zuHFWw/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EYxf2JSSStKNxu8US6XA0g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/EpsvnGHSRV2zsUI68iWwgw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ev4u5HK2RP2Jfb34LHjA5w/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FPqvhlhORp2cgXTcss5Puw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ff-UVmrfSD6SW-ktnnkHlg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FjbkbSGSQqG89fTYdw_cbA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FoqOpQbzQKiI3aUrwi2RBw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/FwCLkVFmQN-o498tbCNuLA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/G4NbCMtWTqyz43-EbzohDw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/GQECeleURW68fxTyj_JeiA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/H6ENxWvMRSOV-EoxG15eiA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HCDI380WTCS6zmqj12SoCQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HMvPc8zBSS2QHVNGaoA_XQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HYMyXi7cQJmb56ia7M3meQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HdP1wiL4Q2KCW7ZCVN9vmg/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/HeNOlkEMQz27REJzoCcadw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Io8aoK_PRziSFwpa1QlSlw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/IpfrKzXqRSq3O4K_khde8Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J0mgiFlaSbS4D4PXLzjG-A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JGmoSh_MTK6rN6gEj7f1ag/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JHacuOehQgayBk3QzKI-CQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JKLY5qoAT42kHAcouIeDNg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JVXwuWxlTbGVD-zVvwyuoQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/JXI_ZWVGQXqwo2X2sW4hog/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_1COVWbSEa3qgVDzSu5Cg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/J_DdUB3SSDWs12GWfdSDvg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/K26i8CDQSnaeWkvON-_fig/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KB91lAZkSDapKNsB1w3p8g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KNIrT4NrRLm7vVrBFukuQw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/KUpNi6UARJ-POV9L0z3-gw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Ky4aRwY_R5-MyaAQLKUR2A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L1z_5pvSQQuRwkruyL14QA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LHpEMVuQQAKI0w_c-hE6GA/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LKA8AvfsQLaO3aC42kbrzg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LMVTsy-qRDqVldUcxSFFGg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LQHtVtxAROmbDkdvQrwmaQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LVbos0uSTmCtgOhorg3JbQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/L_osSpWCSWGYm4xaiMd0Xw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LejjzeeCTPCWTgpIRtEiGg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LfwJETqAR46XGInUj1f2hA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LqpQEDMVSsSVc5A7aCBQ9g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Lv0dJkFtQ_yYD68guumkNA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/LzEyQciFSVivC3sf6H5K4Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MTSYnCvLQu22yorwpSj_rg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MV7CdPBBR5OQPVDvlD6JbQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MWS-4QqwRtKmfU6Zn99raA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MatQEB-VREO4oHXDGmZqDA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/MquHnNciRL6OjpOL0cVz_A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ND0BjurQTA-CKrs2PiPIxA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NPD70YgWQ26oTebv7zYwXg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NcoMSqzfSeq4QjHVEnTNjA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NoK2l_oMRye3MYVx5gCEnQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/NvcBVhX1R4a1fPTcIrBAkA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ObwvA77WQK62jQ3r9l7ehw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/P3LhPZoUQfu8wB75oZonlg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PN8h3wtNRkyo273P9BOWNg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PNS3jf-8Sxi6_5hJ36Qw0A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PlHEt6OIQ7KIgQSZeA58cA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/PtsQBQRVRMWxQMZAGOqIOQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Q6DanumkRLGq9wTYt1iakA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QIfIS5t_QZWB_mikzzQdyw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QNGt0k8DRau9ZC4TW40W4g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QOlP-5bPT3SonrcKIGPHbA/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/QfvuqKBURzWSbAzj2nbVKA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R0qGIyR0Q8OGtPSqfcwDvQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/R4zZgQuuSSS6hUR19q7SmA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/RUXb-n8PS4qQszZ2PqQjKQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Rbeiq7YYT1yT9yudYPfucQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/S9plIwQsQ4qpoK1gKlzjrg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SASj9A17Rc63Cfeh43NtbA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SGzSYHoSRBK9d0Ya414bGg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SOvDANfBSfyC6AGlWMgbsA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/SPdMKig3SW-BPGaTBdD75Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T6Za6XNbSoiQfgeJJkvoyA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/T74FA7MkQL6ast37Vjn9Uw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TGbSx7STTYG7vFml4OdKig/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TbeeMmrKR_KRdo1TzPN2tA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/TkFQEj8NSZyYpvFWZPtNZg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UanfilCjRg2KnA-rmcN7-A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/UosWyUNgSnaj-zPkO5WLuA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VKeisaucR7un3NWXITgFfg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Vimrt74VT4aux3nX8cYpsQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/VjCoJHuNRbWEm13q_7Us2Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WXFfnsCoQB67x3ipKEk6Jg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Wi5RlC9NRH-1YnNCWdwfzw/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/WsrSKN0SSBuMYF4eoeYAXA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XaT42pRPSUW8XKxl9do5ow/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/XrOd_IzkTkmesJBz3WK8tQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Y6DYhxk9Q_iZCxolHU-oBQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YHoCYctmTHadKpKt4S1qYg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/YK3-KHSUTfWCzGtwvxAtkA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Z5B9vLTgQQikbJ_V1qIW9g/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZQJWZP7bSgO36k5l6nvONA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/ZWl7Wg3cSXmNHVieK2P03A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/Zpf-3aEaTvGaGPjEPwdr1A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a43kmFM8Rk6WZNoXzVqS4Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a7NIIETiR4yghDuxUQo9Pw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/a8Yg_-85SjOTakYeNZRWEA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/aG_dZ8qSTCy6OOCkWjbsvw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/advbWpxwSAmsfg6QE13lZw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/alOr4fIsTMSSvGwg2c6Ybg/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/b54Ou3C1QHm7o4Oeafa07w/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bKHbmACWQEWpH8j4EeLWnw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bN5bKy9PSGaEz5vr6iS4iQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/bmAA9ErmTPClbfxirOCEMA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/byp1bRw7SVOb3bglsnNbqA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cNnCRR56TueRbbr6aLn0TQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cSzwzvajRra7BIYSnKXKng/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/cx2Fxx3qQPuPGaiF9skNpQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/d--_T-0RSCeZQFXaPdjt4w/artifacts/public/build/en-US/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dBExr9SQQuK4Ig1ETzCb6Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/dCvJLgtUSBaFyvvSeHQ5AQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e-C7OeUUQ5Gx3W77JzRsSQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/e3SFFy8mQJmG8uRYm-JMIw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eKujH_b0RDqbs79AzAOm3Q/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/elGOubw8QFGZsTNACQEV7A/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/enHE0K8PQYGvBb9gBXIovQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/epGnqv1NQluQCKSXKBHquw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/eunDuKWMS4umWG8jKYpCbw/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/f-xR4Q8JSSu0i8uAq9qPJA/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/.get` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/.get`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.mozinfo.json` & `fuzzfetch-2.3.0/tests/mock-firefoxci/api/queue/v1/task/fVCt26jDTTyOc99Vu56miQ/artifacts/public/build/target.mozinfo.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-hg/mozilla-central/json-rev/24938c537a55` & `fuzzfetch-2.3.0/tests/mock-hg/mozilla-central/json-rev/24938c537a55`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-hg/mozilla-central/json-rev/32fba417ebd01dfb2c2a392cdb1fad7ef66e96e8` & `fuzzfetch-2.3.0/tests/mock-hg/mozilla-central/json-rev/32fba417ebd01dfb2c2a392cdb1fad7ef66e96e8`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/mock-product-details/1.0/firefox_versions.json` & `fuzzfetch-2.3.0/tests/mock-product-details/1.0/firefox_versions.json`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/test_extract.py` & `fuzzfetch-2.3.0/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tests/test_fetch.py` & `fuzzfetch-2.3.0/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `fuzzfetch-2.2.2/tox.ini` & `fuzzfetch-2.3.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -21,39 +21,40 @@
     TRAVIS_*
     TWINE_*
     VCS_*
 usedevelop = true
 
 [testenv:codecov]
 commands =
-    codecov -X gcov
-deps =
     codecov
+deps =
     coverage[toml]
 skip_install = true
+allowlist_externals =
+    codecov
 
 [testenv:lint]
 commands =
     pre-commit run -a {posargs}
 deps =
     pre-commit
 skip_install = true
 
 [testenv:mypy]
 commands =
     mypy --install-types --non-interactive {posargs}
 deps =
-    mypy==v0.991
+    mypy==v1.2.0
 usedevelop = true
 
 [testenv:pylint]
 commands =
     pylint {posargs}
 deps =
-    pylint==2.15.6
+    pylint==2.17.2
 usedevelop = true
 
 [testenv:pypi]
 commands =
     python setup.py sdist bdist_wheel
     twine upload --skip-existing dist/*
 deps =
```

