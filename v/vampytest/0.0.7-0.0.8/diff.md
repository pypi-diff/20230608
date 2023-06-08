# Comparing `tmp/vampytest-0.0.7.tar.gz` & `tmp/vampytest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vampytest-0.0.7.tar", last modified: Mon Dec 19 12:40:16 2022, max compression
+gzip compressed data, was "vampytest-0.0.8.tar", last modified: Thu Jun  8 09:05:27 2023, max compression
```

## Comparing `vampytest-0.0.7.tar` & `vampytest-0.0.8.tar`

### file list

```diff
@@ -1,98 +1,121 @@
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.187178 vampytest-0.0.7/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1503 2022-12-19 12:40:16.187178 vampytest-0.0.7/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      323 2022-07-05 13:34:12.000000 vampytest-0.0.7/README.md
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2022-12-19 12:40:16.187178 vampytest-0.0.7/setup.cfg
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2233 2022-07-05 14:00:46.000000 vampytest-0.0.7/setup.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.175178 vampytest-0.0.7/vampytest/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       67 2022-12-19 10:38:18.000000 vampytest-0.0.7/vampytest/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      311 2022-12-19 10:57:15.000000 vampytest-0.0.7/vampytest/__main__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.179178 vampytest-0.0.7/vampytest/core/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      578 2022-07-04 12:54:11.000000 vampytest-0.0.7/vampytest/core/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.179178 vampytest-0.0.7/vampytest/core/assertions/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1368 2022-07-05 18:45:57.000000 vampytest-0.0.7/vampytest/core/assertions/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1812 2022-12-19 10:51:19.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9014 2022-12-16 09:04:53.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_conditional_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1066 2022-12-19 10:51:36.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_contains.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1018 2022-12-19 10:51:36.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_equals.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1331 2022-12-19 10:51:36.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_false.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1126 2022-12-19 10:51:36.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_identical.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4127 2022-12-19 10:51:42.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_instance.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1109 2022-12-19 10:51:47.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_not_contains.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1094 2022-12-19 10:51:52.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_not_equals.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1232 2022-12-19 10:51:57.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_not_identical.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2768 2022-11-13 10:57:23.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_raising.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      587 2022-02-24 15:16:15.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_states.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2922 2022-12-19 10:52:38.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_subtype.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1307 2022-12-19 10:52:38.000000 vampytest-0.0.7/vampytest/core/assertions/assertion_true.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3910 2022-07-09 14:21:39.000000 vampytest-0.0.7/vampytest/core/assertions/exceptions.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.179178 vampytest-0.0.7/vampytest/core/environment/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      326 2022-12-19 11:05:35.000000 vampytest-0.0.7/vampytest/core/environment/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6417 2022-12-19 10:51:03.000000 vampytest-0.0.7/vampytest/core/environment/configuration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      172 2022-07-04 12:58:23.000000 vampytest-0.0.7/vampytest/core/environment/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1893 2022-12-19 10:59:29.000000 vampytest-0.0.7/vampytest/core/environment/default.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2022-12-19 11:04:50.000000 vampytest-0.0.7/vampytest/core/environment/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3365 2022-12-19 10:51:03.000000 vampytest-0.0.7/vampytest/core/environment/manager.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4297 2022-12-19 10:53:55.000000 vampytest-0.0.7/vampytest/core/environment/scarletio_coroutine.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.179178 vampytest-0.0.7/vampytest/core/event_handling/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      228 2022-12-19 10:54:12.000000 vampytest-0.0.7/vampytest/core/event_handling/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4916 2022-12-19 10:54:12.000000 vampytest-0.0.7/vampytest/core/event_handling/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8325 2022-12-19 10:54:12.000000 vampytest-0.0.7/vampytest/core/event_handling/default.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4066 2022-12-19 10:54:46.000000 vampytest-0.0.7/vampytest/core/event_handling/default_output_writer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1196 2022-12-19 10:54:46.000000 vampytest-0.0.7/vampytest/core/event_handling/text_styling.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.183178 vampytest-0.0.7/vampytest/core/events/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      526 2022-07-01 16:44:50.000000 vampytest-0.0.7/vampytest/core/events/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2616 2022-12-19 10:54:46.000000 vampytest-0.0.7/vampytest/core/events/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2022-07-01 16:40:47.000000 vampytest-0.0.7/vampytest/core/events/constants.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      751 2022-07-01 19:12:39.000000 vampytest-0.0.7/vampytest/core/events/file_load_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:39.000000 vampytest-0.0.7/vampytest/core/events/file_registration.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      427 2022-07-01 19:12:39.000000 vampytest-0.0.7/vampytest/core/events/file_registration_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:42.000000 vampytest-0.0.7/vampytest/core/events/file_testing_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      465 2022-07-01 19:15:34.000000 vampytest-0.0.7/vampytest/core/events/test_done.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      371 2022-07-01 19:12:49.000000 vampytest-0.0.7/vampytest/core/events/testing_end.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      381 2022-07-01 19:12:52.000000 vampytest-0.0.7/vampytest/core/events/testing_start.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.183178 vampytest-0.0.7/vampytest/core/file/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      235 2022-07-24 17:11:51.000000 vampytest-0.0.7/vampytest/core/file/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3234 2022-07-24 20:51:54.000000 vampytest-0.0.7/vampytest/core/file/collection.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9472 2022-07-25 09:06:17.000000 vampytest-0.0.7/vampytest/core/file/file_system_entry.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2106 2022-12-19 10:54:46.000000 vampytest-0.0.7/vampytest/core/file/load_failure.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15845 2022-12-19 10:54:52.000000 vampytest-0.0.7/vampytest/core/file/test_file.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    22376 2022-12-19 10:56:39.000000 vampytest-0.0.7/vampytest/core/handle.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6920 2022-06-28 18:27:07.000000 vampytest-0.0.7/vampytest/core/helpers.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.183178 vampytest-0.0.7/vampytest/core/result/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      166 2022-03-20 09:32:25.000000 vampytest-0.0.7/vampytest/core/result/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.183178 vampytest-0.0.7/vampytest/core/result/failures/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      289 2022-06-28 17:55:25.000000 vampytest-0.0.7/vampytest/core/result/failures/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1791 2022-12-19 10:54:59.000000 vampytest-0.0.7/vampytest/core/result/failures/asserting.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      958 2022-03-20 09:38:55.000000 vampytest-0.0.7/vampytest/core/result/failures/base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2237 2022-06-28 18:45:49.000000 vampytest-0.0.7/vampytest/core/result/failures/helpers.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5635 2022-12-19 10:55:05.000000 vampytest-0.0.7/vampytest/core/result/failures/raising.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2437 2022-12-19 10:55:10.000000 vampytest-0.0.7/vampytest/core/result/failures/returning.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      818 2022-06-28 18:45:49.000000 vampytest-0.0.7/vampytest/core/result/failures/reverted.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4705 2022-12-19 10:55:28.000000 vampytest-0.0.7/vampytest/core/result/result.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5253 2022-07-01 16:14:06.000000 vampytest-0.0.7/vampytest/core/result/result_group.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8497 2022-06-30 09:50:37.000000 vampytest-0.0.7/vampytest/core/run_state.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.187178 vampytest-0.0.7/vampytest/core/runner/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      104 2022-12-19 10:55:58.000000 vampytest-0.0.7/vampytest/core/runner/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10582 2022-07-25 09:30:54.000000 vampytest-0.0.7/vampytest/core/runner/context.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10441 2022-12-19 10:55:28.000000 vampytest-0.0.7/vampytest/core/runner/runner.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7720 2022-12-19 10:56:47.000000 vampytest-0.0.7/vampytest/core/test_case.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2388 2022-07-01 15:49:35.000000 vampytest-0.0.7/vampytest/core/utils.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.187178 vampytest-0.0.7/vampytest/core/wrappers/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1415 2022-12-19 10:31:36.000000 vampytest-0.0.7/vampytest/core/wrappers/__init__.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8949 2022-12-19 10:26:18.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_base.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21179 2022-12-19 10:55:58.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_call.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3841 2022-12-19 10:56:02.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_chainer.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3858 2022-12-19 10:32:03.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_conflict.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1768 2022-12-19 10:56:17.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_environment.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2821 2022-12-19 12:32:20.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_garbage_collect.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      913 2022-12-19 10:56:21.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_revert.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      740 2022-12-19 10:56:24.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_skip.py
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1609 2022-12-19 10:56:28.000000 vampytest-0.0.7/vampytest/core/wrappers/wrapper_skip_conditional.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.187178 vampytest-0.0.7/vampytest/main/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5617 2022-12-19 11:06:38.000000 vampytest-0.0.7/vampytest/main/__init__.py
-drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2022-12-19 12:40:16.179178 vampytest-0.0.7/vampytest.egg-info/
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1503 2022-12-19 12:40:16.000000 vampytest-0.0.7/vampytest.egg-info/PKG-INFO
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3168 2022-12-19 12:40:16.000000 vampytest-0.0.7/vampytest.egg-info/SOURCES.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2022-12-19 12:40:16.000000 vampytest-0.0.7/vampytest.egg-info/dependency_links.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2022-12-19 12:40:16.000000 vampytest-0.0.7/vampytest.egg-info/requires.txt
--rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2022-12-19 12:40:16.000000 vampytest-0.0.7/vampytest.egg-info/top_level.txt
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.937160 vampytest-0.0.8/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1506 2023-06-08 09:05:27.937160 vampytest-0.0.8/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      323 2022-07-05 13:34:12.000000 vampytest-0.0.8/README.md
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       38 2023-06-08 09:05:27.937160 vampytest-0.0.8/setup.cfg
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2360 2023-06-04 20:39:03.000000 vampytest-0.0.8/setup.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.917160 vampytest-0.0.8/vampytest/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       67 2023-06-08 09:02:15.000000 vampytest-0.0.8/vampytest/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      311 2022-12-19 10:57:15.000000 vampytest-0.0.8/vampytest/__main__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.917160 vampytest-0.0.8/vampytest/core/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      674 2023-06-04 13:10:23.000000 vampytest-0.0.8/vampytest/core/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.921160 vampytest-0.0.8/vampytest/core/assertions/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1347 2023-06-03 10:56:18.000000 vampytest-0.0.8/vampytest/core/assertions/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1839 2023-06-03 11:01:35.000000 vampytest-0.0.8/vampytest/core/assertions/aliases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1705 2023-06-03 08:34:35.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10829 2023-06-03 16:26:49.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_conditional_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      972 2023-06-03 10:54:02.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_contains.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      933 2023-06-03 11:32:10.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_equals.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1215 2023-06-03 10:54:53.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_false.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      964 2023-06-03 12:54:40.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_identical.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4849 2023-06-03 18:52:54.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_instance.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      994 2023-06-03 10:56:54.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_not_contains.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      943 2023-06-03 10:57:21.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_not_equals.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      982 2023-06-03 12:54:58.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_not_identical.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3467 2023-06-03 19:04:59.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_raising.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      717 2023-06-03 08:30:46.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_states.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3960 2023-06-03 16:28:00.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_subtype.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1200 2023-06-03 10:59:18.000000 vampytest-0.0.8/vampytest/core/assertions/assertion_true.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3973 2023-06-03 08:32:34.000000 vampytest-0.0.8/vampytest/core/assertions/exceptions.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.921160 vampytest-0.0.8/vampytest/core/contexts/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      224 2023-06-04 15:53:08.000000 vampytest-0.0.8/vampytest/core/contexts/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1880 2023-06-04 15:35:26.000000 vampytest-0.0.8/vampytest/core/contexts/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3965 2023-06-04 17:02:08.000000 vampytest-0.0.8/vampytest/core/contexts/calling.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2023-06-04 15:38:42.000000 vampytest-0.0.8/vampytest/core/contexts/garbage_collect.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1614 2023-06-05 07:44:04.000000 vampytest-0.0.8/vampytest/core/contexts/output_capturing.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.925160 vampytest-0.0.8/vampytest/core/environment/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      326 2022-12-19 11:05:35.000000 vampytest-0.0.8/vampytest/core/environment/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     6417 2022-12-19 10:51:03.000000 vampytest-0.0.8/vampytest/core/environment/configuration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      172 2022-07-04 12:58:23.000000 vampytest-0.0.8/vampytest/core/environment/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1899 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/environment/default.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1336 2023-06-03 19:11:36.000000 vampytest-0.0.8/vampytest/core/environment/helpers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3368 2023-06-04 14:14:50.000000 vampytest-0.0.8/vampytest/core/environment/manager.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4303 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/environment/scarletio_coroutine.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.925160 vampytest-0.0.8/vampytest/core/event_handling/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      342 2023-06-04 18:26:40.000000 vampytest-0.0.8/vampytest/core/event_handling/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4916 2022-12-19 10:54:12.000000 vampytest-0.0.8/vampytest/core/event_handling/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      459 2023-06-04 18:26:24.000000 vampytest-0.0.8/vampytest/core/event_handling/colors.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8165 2023-06-04 20:14:28.000000 vampytest-0.0.8/vampytest/core/event_handling/default.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4079 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/event_handling/default_output_writer.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.925160 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      207 2023-06-04 18:27:13.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1964 2023-06-05 06:48:49.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/result_modifier_parameters.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    11879 2023-06-04 20:37:50.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/result_rendering.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2957 2023-06-04 20:17:32.000000 vampytest-0.0.8/vampytest/core/event_handling/rendering_helpers/writers.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1855 2023-06-04 18:36:03.000000 vampytest-0.0.8/vampytest/core/event_handling/text_styling.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.929160 vampytest-0.0.8/vampytest/core/events/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      526 2022-07-01 16:44:50.000000 vampytest-0.0.8/vampytest/core/events/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2545 2023-06-04 07:01:57.000000 vampytest-0.0.8/vampytest/core/events/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      249 2022-07-01 16:40:47.000000 vampytest-0.0.8/vampytest/core/events/constants.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      751 2022-07-01 19:12:39.000000 vampytest-0.0.8/vampytest/core/events/file_load_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:39.000000 vampytest-0.0.8/vampytest/core/events/file_registration.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      427 2022-07-01 19:12:39.000000 vampytest-0.0.8/vampytest/core/events/file_registration_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      470 2022-07-01 19:12:42.000000 vampytest-0.0.8/vampytest/core/events/file_testing_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      438 2023-06-04 07:01:41.000000 vampytest-0.0.8/vampytest/core/events/test_done.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      371 2022-07-01 19:12:49.000000 vampytest-0.0.8/vampytest/core/events/testing_end.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      381 2022-07-01 19:12:52.000000 vampytest-0.0.8/vampytest/core/events/testing_start.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.929160 vampytest-0.0.8/vampytest/core/file/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      235 2022-07-24 17:11:51.000000 vampytest-0.0.8/vampytest/core/file/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3234 2022-07-24 20:51:54.000000 vampytest-0.0.8/vampytest/core/file/collection.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     9474 2023-02-15 17:01:20.000000 vampytest-0.0.8/vampytest/core/file/file_system_entry.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2106 2022-12-19 10:54:46.000000 vampytest-0.0.8/vampytest/core/file/load_failure.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    15847 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/file/test_file.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    21860 2023-06-04 15:55:12.000000 vampytest-0.0.8/vampytest/core/handle.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/helpers/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      273 2023-06-03 15:00:30.000000 vampytest-0.0.8/vampytest/core/helpers/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1518 2023-06-03 18:40:58.000000 vampytest-0.0.8/vampytest/core/helpers/exception_matching.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2549 2023-06-03 14:53:17.000000 vampytest-0.0.8/vampytest/core/helpers/hashing.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1633 2023-06-03 14:55:07.000000 vampytest-0.0.8/vampytest/core/helpers/merging.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2366 2023-06-03 14:57:31.000000 vampytest-0.0.8/vampytest/core/helpers/path_repr.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2354 2023-06-03 14:52:20.000000 vampytest-0.0.8/vampytest/core/helpers/un_nesting.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/result/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      110 2023-06-04 12:40:46.000000 vampytest-0.0.8/vampytest/core/result/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/result/reports/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      241 2023-06-04 19:01:59.000000 vampytest-0.0.8/vampytest/core/result/reports/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1115 2023-06-04 18:41:12.000000 vampytest-0.0.8/vampytest/core/result/reports/asserting.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      869 2023-06-04 16:49:37.000000 vampytest-0.0.8/vampytest/core/result/reports/base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      698 2023-06-04 16:52:34.000000 vampytest-0.0.8/vampytest/core/result/reports/output.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2006 2023-06-04 19:05:23.000000 vampytest-0.0.8/vampytest/core/result/reports/raising.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1472 2023-06-04 19:12:11.000000 vampytest-0.0.8/vampytest/core/result/reports/returning.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10268 2023-06-04 20:37:00.000000 vampytest-0.0.8/vampytest/core/result/result.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     8411 2023-06-04 07:01:08.000000 vampytest-0.0.8/vampytest/core/run_state.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/runner/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      104 2022-12-19 10:55:58.000000 vampytest-0.0.8/vampytest/core/runner/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10798 2023-06-04 20:30:43.000000 vampytest-0.0.8/vampytest/core/runner/context.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    10435 2023-06-04 07:02:40.000000 vampytest-0.0.8/vampytest/core/runner/runner.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7836 2023-06-04 08:01:22.000000 vampytest-0.0.8/vampytest/core/test_case.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.933160 vampytest-0.0.8/vampytest/core/utils/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      207 2023-06-05 06:55:53.000000 vampytest-0.0.8/vampytest/core/utils/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      150 2023-06-05 07:43:47.000000 vampytest-0.0.8/vampytest/core/utils/aliases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2189 2023-06-05 08:05:15.000000 vampytest-0.0.8/vampytest/core/utils/capture_output_context_manager.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      360 2023-06-03 15:06:42.000000 vampytest-0.0.8/vampytest/core/utils/wrap_nothing.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.937160 vampytest-0.0.8/vampytest/core/wrappers/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      883 2023-06-03 19:28:37.000000 vampytest-0.0.8/vampytest/core/wrappers/__init__.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1221 2023-06-05 09:29:38.000000 vampytest-0.0.8/vampytest/core/wrappers/aliases.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     7302 2023-06-05 09:14:21.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_base.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    20677 2023-06-05 09:06:02.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_call.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)    17716 2023-06-05 09:54:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_call_from.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3866 2023-06-03 19:12:42.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_chainer.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     3067 2023-06-04 17:39:27.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_conflict.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1771 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_environment.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     2572 2023-06-04 14:02:29.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_garbage_collect.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      921 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_reverse.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)      743 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip.py
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1612 2023-06-05 09:55:49.000000 vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip_conditional.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.937160 vampytest-0.0.8/vampytest/main/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     5617 2022-12-19 11:06:38.000000 vampytest-0.0.8/vampytest/main/__init__.py
+drwxrwxr-x   0 huyanematsu  (1000) huyanematsu  (1000)        0 2023-06-08 09:05:27.917160 vampytest-0.0.8/vampytest.egg-info/
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     1506 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/PKG-INFO
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)     4021 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/SOURCES.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)        1 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/dependency_links.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/requires.txt
+-rw-rw-r--   0 huyanematsu  (1000) huyanematsu  (1000)       10 2023-06-08 09:05:27.000000 vampytest-0.0.8/vampytest.egg-info/top_level.txt
```

### Comparing `vampytest-0.0.7/PKG-INFO` & `vampytest-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vampytest
-Version: 0.0.7
+Version: 0.0.8
 Summary: A vampy test framework
 Home-page: https://github.com/HuyaneMatsu/vampytest
 Author: HuyaneMatsu
 Author-email: re.ism.tm@gmail.com
 License: DBAD
 Description: <h1 align="center">
             Vampytest
@@ -22,20 +22,20 @@
         
         *The library currently is in alpha stage. It can run tests but many features might be missing.*
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `vampytest-0.0.7/setup.py` & `vampytest-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,24 +18,23 @@
 setup(
     author = 'HuyaneMatsu',
     author_email = 're.ism.tm@gmail.com',
     classifiers = [
         'Development Status :: 2 - Pre-Alpha',
         
         'Intended Audience :: Developers',
-
+        
         'Operating System :: OS Independent',
-
-        'Programming Language :: Python :: 3',
+        
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        #'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.11',
         
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         
         'Topic :: Software Development :: Testing',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
@@ -49,21 +48,25 @@
     long_description = README,
     long_description_content_type = 'text/markdown',
     name = 'vampytest',
     packages = [
         'vampytest',
         'vampytest.core',
         'vampytest.core.assertions',
+        'vampytest.core.contexts',
         'vampytest.core.environment',
         'vampytest.core.event_handling',
+        'vampytest.core.event_handling.rendering_helpers',
         'vampytest.core.events',
         'vampytest.core.file',
+        'vampytest.core.helpers',
         'vampytest.core.result',
-        'vampytest.core.result.failures',
+        'vampytest.core.result.reports',
         'vampytest.core.runner',
+        'vampytest.core.utils',
         'vampytest.core.wrappers',
         'vampytest.main',
     ],
     python_requires = '>=3.6',
     url = 'https://github.com/HuyaneMatsu/vampytest',
     version = version,
 )
```

### Comparing `vampytest-0.0.7/vampytest/core/__init__.py` & `vampytest-0.0.8/vampytest/core/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from .assertions import *
+from .contexts import *
 from .environment import *
 from .event_handling import *
 from .events import *
 from .file import *
+from .helpers import *
 from .result import *
 from .runner import *
+from .utils import *
 from .wrappers import *
 
 from .handle import *
-from .helpers import *
+from .run_state import *
 from .test_case import *
-from .utils import *
 
 
 __all__ = (
     *assertions.__all__,
+    *contexts.__all__,
     *environment.__all__,
     *event_handling.__all__,
     *events.__all__,
     *file.__all__,
+    *helpers.__all__,
     *result.__all__,
     *runner.__all__,
+    *utils.__all__,
     *wrappers.__all__,
     
     *handle.__all__,
-    *helpers.__all__,
+    *run_state.__all__,
     *test_case.__all__,
-    *utils.__all__,
 )
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/__init__.py` & `vampytest-0.0.8/vampytest/core/assertions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     with vampytest.raises(TypeError):
         'nice' + 69
 
 def test_contains():
     vampytest.assert_in(range(7), 5)
 ```
 """
+from .aliases import *
 from .assertion_base import *
 from .assertion_conditional_base import *
 from .assertion_contains import *
 from .assertion_equals import *
 from .assertion_false import *
 from .assertion_identical import *
 from .assertion_instance import *
@@ -30,20 +31,17 @@
 from .assertion_not_identical import *
 from .assertion_raising import *
 from .assertion_states import *
 from .assertion_subtype import *
 from .assertion_true import *
 from .exceptions import *
 
-CONDITION_STATES = assertion_states
-
 
 __all__ = (
-    'CONDITION_STATES',
-    
+    *aliases.__all__,
     *assertion_raising.__all__,
     *assertion_base.__all__,
     *assertion_conditional_base.__all__,
     *assertion_contains.__all__,
     *assertion_equals.__all__,
     *assertion_false.__all__,
     *assertion_identical.__all__,
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_base.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,58 @@
 __all__ = ('AssertionBase',)
 
 from scarletio import RichAttributeErrorBaseType
 
-from . import assertion_states as CONDITION_STATES
-from .assertion_states import get_assertion_state_name
+from .assertion_states import ASSERTION_STATE_NONE, get_assertion_state_name
 
 
 class AssertionBase(RichAttributeErrorBaseType):
     """
     Base class for conditions.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     """
     __slots__ = ('state',)
     
+    
     def __new__(cls):
         """
         Creates a new condition.
         """
         self = object.__new__(cls)
-        self.state = CONDITION_STATES.NONE
+        self.state = ASSERTION_STATE_NONE
         return self
     
     
-    def _cursed_repr_builder(self):
+    def _build_repr_parts_into(self, into):
         """
         Representation builder helper.
         
-        This method is a generator.
-        
-        Examples
-        --------
-        ```
-        for repr_parts in self._cursed_repr_builder():
-            repr_parts.append(', oh no')
-        
-        return ''.join(repr_parts)
-        ```
+        Parameters
+        ----------
+        into : `list` of `str`
+            List of strings to build the representation into.
+        
+        Returns
+        -------
+        into : `list` of `str`
         """
-        repr_parts = ['<', self.__class__.__name__]
-        
-        repr_parts.append(' state=')
-        repr_parts.append(get_assertion_state_name(self.state))
-        
-        yield repr_parts
-        
-        repr_parts.append('>')
+        return into
     
     
     def __repr__(self):
         """Returns the condition's representation."""
-        for repr_parts in self._cursed_repr_builder():
-            pass
-        
+        repr_parts = ['<', self.__class__.__name__]
+        repr_parts.append(' state = ')
+        repr_parts.append(get_assertion_state_name(self.state))
+        repr_parts = self._build_repr_parts_into(repr_parts)
+        repr_parts.append('>')
         return ''.join(repr_parts)
     
     
     def render_failure_message_parts_into(self, failure_message_parts):
         """
         Renders the assertion into the given list.
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_conditional_base.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_conditional_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,106 @@
 __all__ = ('AssertionConditionalBase', 'AssertionConditionalBase1Value', 'AssertionConditionalBase2Value')
 
 from scarletio import copy_docs, include
 
-from . import assertion_states as CONDITION_STATES
 from .assertion_base import AssertionBase
+from .assertion_states import ASSERTION_STATE_CREATED, ASSERTION_STATE_PASSED, ASSERTION_STATE_FAILED
 
 
 AssertionException = include('AssertionException')
 
 
-class AssertionConditionalBase(AssertionBase):
+class InvokeAfterConstructor(type):
+    """
+    Metatype for invoking a test after calling its `__new__`.
+    """
+    def __call__(type_, *positional_parameters, **keyword_parameter):
+        """
+        Instantiates the type and invokes it.
+        
+        Parameters
+        ----------
+        type_ : `type`
+            The type to Instantiate and invoke.
+        *positional_parameters : `tuple<object>`
+            Positional parameters to pass to the type's constructor.
+        keyword_parameter : `dict<str, object>`
+            Keyword parameters to pass to the type's constructor.
+        
+        Returns
+        -------
+        condition_return : `object`
+            The returned value by the condition. Usually a boolean.
+        
+        Raises
+        ------
+        AssertionException
+            The condition failed.
+        BaseException
+            An other occurred exceptions.
+        """
+        return type_.__new__(type_, *positional_parameters, **keyword_parameter).invoke()
+
+
+class AssertionConditionalBase(AssertionBase, metaclass = InvokeAfterConstructor):
     """
     Base class for conditional assertions.
     
     Attributes
     ----------
-    state : `str`
-        The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
+    state : `str`
+        The condition's state.
     """
     __slots__ = ('exception', 'reverse')
     
-    def __new__(cls, *, reverse=False):
+    def __new__(cls, *, reverse = False):
         """
         Creates an new conditional assertion instance.
         
         Parameters
         ----------
         reverse : `bool` = `False`, Optional (Keyword only)
             Whether the condition should be reversed.
         """
         self = AssertionBase.__new__(cls)
         self.exception = None
         self.reverse = reverse
+        self.state = ASSERTION_STATE_CREATED
         return self
     
     
-    @copy_docs(AssertionBase._cursed_repr_builder)
-    def _cursed_repr_builder(self):
-        for repr_parts in AssertionBase._cursed_repr_builder(self):
-            yield repr_parts
-            
-            reverse = self.reverse
-            if reverse:
-                repr_parts.append(', reverse=')
-                repr_parts.append(repr(reverse))
-                
+    @copy_docs(AssertionBase._build_repr_parts_into)
+    def _build_repr_parts_into(self, into):
+        into = AssertionBase._build_repr_parts_into(self, into)
+        
+        reverse = self.reverse
+        if reverse:
+            into.append(', reverse = ')
+            into.append(repr(reverse))
             
-            exception = self.exception
-            if (exception is not None):
-                repr_parts.append(', exception=')
-                repr_parts.append(repr(exception))
+        
+        exception = self.exception
+        if (exception is not None):
+            into.append(', exception = ')
+            into.append(repr(exception))
+        
+        return into
     
     
     def invoke(self):
         """
         Invokes the assertion.
         
         Returns
         -------
-        condition_return : `Any`
+        condition_return : `object`
             The value returned by the condition.
         
         Raises
         ------
         AssertionException
             The condition failed.
         """
@@ -75,41 +109,41 @@
             
             if condition_return:
                 passed = True
             else:
                 passed = False
         
         except BaseException as err:
-            self.state = CONDITION_STATES.FAILED
+            self.state = ASSERTION_STATE_FAILED
             self.exception = err
             
         else:
             if self.reverse:
                 passed = not passed
             
             if passed:
-                self.state = CONDITION_STATES.PASSED
+                self.state = ASSERTION_STATE_PASSED
                 return condition_return
             
-            self.state = CONDITION_STATES.FAILED
+            self.state = ASSERTION_STATE_FAILED
         
         try:
             raise AssertionException(self)
         finally:
             # Remove self reference, so garbage collection wont fail
             self = None
     
     
     def invoke_condition(self):
         """
         Invokes the condition.
         
         Returns
         -------
-        result : `Any`
+        result : `object`
             The condition's result.
         """
         raise NotImplementedError
     
     
     def _get_operation_representation(self):
         """
@@ -148,23 +182,23 @@
     @copy_docs(AssertionBase.render_failure_message_parts_into)
     def render_failure_message_parts_into(self, failure_message_parts):
         self._render_operation_representation_into(failure_message_parts)
         failure_message_parts.append('\n')
         return failure_message_parts
 
 
-def _add_parameters_representation_into(parameter_name, parameter_value, into):
+def _render_parameters_representation_into(parameter_name, parameter_value, into):
     """
     Renders the given parameter into the given list of strings.
     
     Parameters
     ----------
     parameter_name : `str`
         The parameter's name.
-    parameter_value : `Any`
+    parameter_value : `object`
         The parameter's value.
     into : `list` of `str`
         A list to extend with the rendered strings.
     
     Returns
     -------
     into : `list` of `str`
@@ -173,67 +207,102 @@
     into.append(' = ')
     into.append(repr(parameter_value))
     into.append('\n')
     
     return into
 
 
+def _render_types_parameter_representation_into(parameter_name, types, into):
+    """
+    Renders the given types parameter into the given list of strings.
+    
+    Parameters
+    ----------
+    parameter_name : `str`
+        The parameter's name.
+    types : `set` of `type`
+        The parameter's value.
+    into : `list` of `str`
+        A list to extend with the rendered strings.
+    
+    Returns
+    -------
+    into : `list` of `str`
+    """
+    into.append(parameter_name)
+    into.append(' = ')
+    
+    type_representations = sorted(str(type.__name__) for type in types)
+    length = len(type_representations)
+    if length:
+        index = 0
+        
+        while True:
+            type_representation = type_representations[index]
+            into.append(type_representation)
+            
+            index += 1
+            if index == length:
+                break
+            
+            into.append(', ')
+            continue
+    
+    into.append('\n')
+    
+    return into
+
+
 class AssertionConditionalBase1Value(AssertionConditionalBase):
     """
     Base class for executing a one value assertion.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
+    value_0 : `object`
         The value to call the condition on.
     """
-    __slots__ = ('value_1',)
+    __slots__ = ('value_0',)
 
-    def __new__(cls, value_1, *, reverse=False):
+    def __new__(cls, value_0, *, reverse = False):
         """
         Asserts whether the two values are equal. Fails the test if not.
         
         Parameters
         ----------
-        value_1 : `Any`
+        value_0 : `object`
             First value to assert equality with.
-        value_2 : `Any`
-            The second value to assert equality with.
         reverse : `bool` = `False`, Optional (Keyword only)
             Whether the condition should be reversed.
         """
-        self = AssertionConditionalBase.__new__(cls, reverse=reverse)
-        
-        self.value_1 = value_1
-        
-        self.state = CONDITION_STATES.CREATED
-        
-        return self.invoke()
+        self = AssertionConditionalBase.__new__(cls, reverse = reverse)
+        self.value_0 = value_0
+        return self
     
     
-    @copy_docs(AssertionConditionalBase._cursed_repr_builder)
-    def _cursed_repr_builder(self):
-        for repr_parts in AssertionConditionalBase._cursed_repr_builder(self):
-            
-            repr_parts.append(', value_1=')
-            repr_parts.append(repr(self.value_1))
-            
-            yield repr_parts
+    @copy_docs(AssertionConditionalBase._build_repr_parts_into)
+    def _build_repr_parts_into(self, into):
+        into = AssertionConditionalBase._build_repr_parts_into(self, into)
+        
+        into.append(', value_0 = ')
+        into.append(repr(self.value_0))
+        
+        return into
     
     
     @copy_docs(AssertionConditionalBase.render_failure_message_parts_into)
     def render_failure_message_parts_into(self, failure_message_parts):
         AssertionConditionalBase.render_failure_message_parts_into(self, failure_message_parts)
-        _add_parameters_representation_into('parameter', self.value_1, failure_message_parts)
+        _render_parameters_representation_into('parameter', self.value_0, failure_message_parts)
         return failure_message_parts
 
 
 class AssertionConditionalBase2Value(AssertionConditionalBase1Value):
     """
     Base class for executing a two value assertion.
     
@@ -241,62 +310,57 @@
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
+    value_0 : `object`
         The value to call the condition on.
-    value_2 : `Any`
+    value_1 : `object`
         The value to call the condition with.
     """
-    __slots__ = ('value_2',)
+    __slots__ = ('value_1',)
     
-    def __new__(cls, value_1, value_2, *, reverse=False):
+    def __new__(cls, value_0, value_1, *, reverse = False):
         """
         Asserts whether the two values are equal. Fails the test if not.
         
         Parameters
         ----------
-        value_1 : `Any`
+        value_0 : `object`
             First value to assert equality with.
-        value_2 : `Any`
+        value_1 : `object`
             The second value to assert equality with.
         reverse : `bool` = `False`, Optional (Keyword only)
             Whether the condition should be reversed.
         """
-        self = AssertionConditionalBase.__new__(cls, reverse=reverse)
-        
+        self = AssertionConditionalBase1Value.__new__(cls, value_0, reverse = reverse)
         self.value_1 = value_1
-        self.value_2 = value_2
-        
-        self.state = CONDITION_STATES.CREATED
-        
-        return self.invoke()
+        return self
     
     
-    @copy_docs(AssertionConditionalBase1Value._cursed_repr_builder)
-    def _cursed_repr_builder(self):
-        for repr_parts in AssertionConditionalBase1Value._cursed_repr_builder(self):
-            
-            repr_parts.append(', value_2=')
-            repr_parts.append(repr(self.value_2))
-            
-            yield repr_parts
+    @copy_docs(AssertionConditionalBase1Value._build_repr_parts_into)
+    def _build_repr_parts_into(self, into):
+        into = AssertionConditionalBase1Value._build_repr_parts_into(self, into)
+        
+        into.append(', value_1 = ')
+        into.append(repr(self.value_1))
+        
+        return into
     
     
-    @copy_docs(AssertionConditionalBase._render_operation_representation_into)
+    @copy_docs(AssertionConditionalBase1Value._render_operation_representation_into)
     def _render_operation_representation_into(self, into):
         AssertionConditionalBase._render_operation_representation_into(self, into)
-        into.append(' as "parameter_1 ')
+        into.append(' as "parameter_0 ')
         into.append(self._get_operation_representation())
-        into.append(' parameter_2"')
+        into.append(' parameter_1"')
         return into
     
     
-    @copy_docs(AssertionConditionalBase.render_failure_message_parts_into)
+    @copy_docs(AssertionConditionalBase1Value.render_failure_message_parts_into)
     def render_failure_message_parts_into(self, failure_message_parts):
         AssertionConditionalBase.render_failure_message_parts_into(self, failure_message_parts)
-        _add_parameters_representation_into('parameter_1', self.value_1, failure_message_parts)
-        _add_parameters_representation_into('parameter_2', self.value_2, failure_message_parts)
+        _render_parameters_representation_into('parameter_0', self.value_0, failure_message_parts)
+        _render_parameters_representation_into('parameter_1', self.value_1, failure_message_parts)
         return failure_message_parts
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_contains.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_identical.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-__all__ = ('AssertionContains', 'assert_contains', 'assert_in',)
+__all__ = ('AssertionIdentical',)
 
 from scarletio import copy_docs
 
 from .assertion_conditional_base import AssertionConditionalBase2Value
 
 
-class AssertionContains(AssertionConditionalBase2Value):
+class AssertionIdentical(AssertionConditionalBase2Value):
     """
-    Asserts whether the second value contains the first.
+    Asserts whether two objects are identical.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
-        First value to assert contains with.
-    value_2 : `Any`
-        The second value to assert contains with.
+    value_0 : `object`
+        First value to assert identity with.
+    value_1 : `object`
+        The second value to assert identity with.
     """
     __slots__ = ()
     
     @copy_docs(AssertionConditionalBase2Value.invoke_condition)
     def invoke_condition(self):
-        return self.value_1 in self.value_2
+        return self.value_0 is self.value_1
     
     
     @copy_docs(AssertionConditionalBase2Value._get_operation_representation)
     def _get_operation_representation(self):
-        return 'in'
-
-
-assert_contains = AssertionContains
-assert_in = AssertionContains
+        return 'is'
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_equals.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_not_equals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-__all__ = ('AssertionEquals', 'assert_eq', 'assert_equals')
+__all__ = ('AssertionNotEquals',)
 
 from scarletio import copy_docs
 
 from .assertion_conditional_base import AssertionConditionalBase2Value
 
 
-class AssertionEquals(AssertionConditionalBase2Value):
+class AssertionNotEquals(AssertionConditionalBase2Value):
     """
-    Asserts equality.
+    Asserts not equality.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
+    value_0 : `object`
         First value to assert equality with.
-    value_2 : `Any`
+    value_1 : `object`
         The second value to assert equality with.
     """
     __slots__ = ()
     
     @copy_docs(AssertionConditionalBase2Value.invoke_condition)
     def invoke_condition(self):
-        return self.value_1 == self.value_2
+        return self.value_0 != self.value_1
     
     
     @copy_docs(AssertionConditionalBase2Value._get_operation_representation)
     def _get_operation_representation(self):
-        return '=='
-
-
-assert_eq = AssertionEquals
-assert_equals = AssertionEquals
+        return '!='
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_false.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_false.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ('AssertionValueEvaluationFalse', 'assert_false', 'assert_not')
+__all__ = ('AssertionValueEvaluationFalse',)
 
 from scarletio import copy_docs
 
 from .assertion_conditional_base import AssertionConditionalBase1Value
 
 
 class AssertionValueEvaluationFalse(AssertionConditionalBase1Value):
@@ -13,31 +13,27 @@
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
+    value_0 : `object`
         First value to assert.
     """
     __slots__ = ()
     
     @copy_docs(AssertionConditionalBase1Value.invoke_condition)
     def invoke_condition(self):
-        return not self.value_1
+        return not self.value_0
     
     
     @copy_docs(AssertionConditionalBase1Value._get_operation_representation)
     def _get_operation_representation(self):
         return 'not bool(...)'
     
     
     @copy_docs(AssertionConditionalBase1Value._render_operation_representation_into)
     def _render_operation_representation_into(self, into):
         AssertionConditionalBase1Value._render_operation_representation_into(self, into)
         into.append(' as "not bool(parameter)"')
         return into
-
-
-assert_false = AssertionValueEvaluationFalse
-assert_not = AssertionValueEvaluationFalse
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_identical.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_contains.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-__all__ = ('AssertionIdentical', 'assert_id', 'assert_is', 'assert_identical')
+__all__ = ('AssertionContains',)
 
 from scarletio import copy_docs
 
 from .assertion_conditional_base import AssertionConditionalBase2Value
 
 
-class AssertionIdentical(AssertionConditionalBase2Value):
+class AssertionContains(AssertionConditionalBase2Value):
     """
-    Asserts whether two objects are identical.
+    Asserts whether the second value contains the first.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
-        First value to assert identity with.
-    value_2 : `Any`
-        The second value to assert identity with.
+    value_0 : `object`
+        First value to assert contains with.
+    value_1 : `object`
+        The second value to assert contains with.
     """
-    __slots__ = ('value_1', 'value_2',)
+    __slots__ = ()
     
     @copy_docs(AssertionConditionalBase2Value.invoke_condition)
     def invoke_condition(self):
-        return self.value_1 is self.value_2
+        return self.value_0 in self.value_1
     
     
     @copy_docs(AssertionConditionalBase2Value._get_operation_representation)
     def _get_operation_representation(self):
-        return 'is'
-
-
-assert_id = AssertionIdentical
-assert_is = AssertionIdentical
-assert_identical = AssertionIdentical
+        return 'in'
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_not_contains.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_not_contains.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ('AssertionNotContains', 'assert_not_contains', 'assert_not_in')
+__all__ = ('AssertionNotContains',)
 
 from scarletio import copy_docs
 
 from .assertion_conditional_base import AssertionConditionalBase2Value
 
 
 class AssertionNotContains(AssertionConditionalBase2Value):
@@ -13,26 +13,22 @@
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
+    value_0 : `object`
         First value to assert contains with.
-    value_2 : `Any`
+    value_1 : `object`
         The second value to assert contains with.
     """
     __slots__ = ()
     
     @copy_docs(AssertionConditionalBase2Value.invoke_condition)
     def invoke_condition(self):
-        return self.value_1 not in self.value_2
+        return self.value_0 not in self.value_1
     
     
     @copy_docs(AssertionConditionalBase2Value._get_operation_representation)
     def _get_operation_representation(self):
         return 'not in'
-
-
-assert_not_contains = AssertionNotContains
-assert_not_in = AssertionNotContains
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_not_equals.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_not_identical.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-__all__ = ('AssertionNotEquals', 'assert_ne', 'assert_not_eq', 'assert_not_equals')
+__all__ = ('AssertionNotIdentical',)
 
 from scarletio import copy_docs
 
 from .assertion_conditional_base import AssertionConditionalBase2Value
 
 
-class AssertionNotEquals(AssertionConditionalBase2Value):
+class AssertionNotIdentical(AssertionConditionalBase2Value):
     """
-    Asserts not equality.
+    Asserts whether two objects are not identical.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
-        First value to assert equality with.
-    value_2 : `Any`
-        The second value to assert equality with.
+    value_0 : `object`
+        First value to assert identity with.
+    value_1 : `object`
+        The second value to assert identity with.
     """
     __slots__ = ()
     
     @copy_docs(AssertionConditionalBase2Value.invoke_condition)
     def invoke_condition(self):
-        return self.value_1 != self.value_2
+        return self.value_0 is not self.value_1
     
     
     @copy_docs(AssertionConditionalBase2Value._get_operation_representation)
     def _get_operation_representation(self):
-        return '!='
-
-
-assert_ne = AssertionNotEquals
-assert_not_eq = AssertionNotEquals
-assert_not_equals = AssertionNotEquals
+        return 'is not'
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_raising.py` & `vampytest-0.0.8/vampytest/core/helpers/un_nesting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,109 @@
-__all__ = ('AssertionRaising', 'assert_raises')
+__all__ = ()
 
-from ..helpers import try_match_exception, un_nest_expected_exceptions
 
-from . import assertion_states as CONDITION_STATES
-from .assertion_base import AssertionBase
-from .exceptions import AssertionException
+def un_nest(value):
+    """
+    Un-nests the given value into a tuple.
+    
+    Parameters
+    ----------
+    value : `tuple<object>`, `object`
+        The value to un-nest.
+    
+    Returns
+    -------
+    value : `tuple<object>`
+    """
+    return {*iter_un_nest(value)}
 
 
-class AssertionRaising(AssertionBase):
+def iter_un_nest(value):
     """
-    Context manager, which checks for exception raise.
+    Un-nests the given tuple.
+    
+    This function is an iterable generator.
     
-    Attributes
+    Parameters
     ----------
-    state : `str`
-        The condition's state.
-    exception : `None`, `BaseException`
-        Exception raised within the context block if any.
-    accept_subtypes : `bool`
-        Whether subclasses are accepted as well.
-    expected_exceptions : `set` of ``BaseException``
-        The expected exception types.
-    
-    Examples
-    --------
-    ```py
-    with AssertionRaising(TypeError):
-        'nice' + 69
-    ```
-    """
-    __slots__ = ('accept_subtypes', 'exception', 'expected_exceptions')
-    
-    def __new__(cls, *expected_exceptions, accept_subtypes = True):
-        """
-        Creates a new raise asserting context manager.
-        
-        Parameters
-        ----------
-        *expected_exceptions : tuple` of (`BaseException`, ...)
-            Exception types to expect.
-        accept_subtypes : `bool` = `True`, optional (Keyword only)
-            Whether subclasses are accepted as well.
-        
-        Raises
-        ------
-        TypeError
-            If an `expected_exceptions`'s type is incorrect.
-        ValueError
-            If no exception was passed.
-        """
-        expected_exceptions = un_nest_expected_exceptions(expected_exceptions)
-        if not expected_exceptions:
-            raise ValueError(
-                'At least 1 exception is required.'
-            )
-        
-        self = AssertionBase.__new__(cls)
-        self.expected_exceptions = expected_exceptions
-        self.accept_subtypes = accept_subtypes
-        
-        return self
+    value : `tuple<object>`, `object`
+        The value to un-nest.
     
+    Yields
+    ------
+    value : `object`
+    """
+    to_do = [value]
     
-    def __enter__(self):
-        """Enters as context manager."""
-        self.state = CONDITION_STATES.CREATED
-        return None
-    
-    
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        """Exits the context manager."""
-        if exc_type is None:
-            self.state = CONDITION_STATES.FAILED
-            try:
-                raise AssertionException(self)
-            finally:
-                # Clear reference to self
-                self = None
+    while to_do:
+        value = to_do.pop()
+        if isinstance(value, tuple):
+            to_do.extend(value)
+            continue
         
-        self.exception = exc_val
-        
-        if try_match_exception(self.expected_exceptions, exc_val, self.accept_subtypes):
-            state = CONDITION_STATES.PASSED
-            silence = True
+        yield value
+        continue
+
+
+def un_nest_exceptions(exceptions):
+    """
+    Un-nests the given `exceptions`.
+    
+    Parameters
+    ----------
+    exceptions : `BaseException | type<BaseException> | tuple<BaseException, <type<BaseException>, ...>`
+        The exceptions to un-nest.
+    
+    Returns
+    -------
+    exceptions : `set` of (`BaseException`, `type<BaseException>`)
+    
+    Raises
+    ------
+    TypeError
+        If an element's type is incorrect.
+    """
+    exceptions = un_nest(exceptions)
+    
+    for exception in exceptions:
+        if isinstance(exception, BaseException):
+            continue
         
-        else:
-            state = CONDITION_STATES.FAILED
-            silence = False
+        if isinstance(exception, type) and issubclass(exception, BaseException):
+            continue
         
-        self.state = state
-        return silence
+        raise TypeError(
+            f'`exception` can be `BaseException` or its instance, `tuple` of (`BaseException`, ...)`, '
+            f'got {exception.__class__.__name__}; {exception!r}.'
+        )
+    
+    return exceptions
 
 
-assert_raises = AssertionRaising
+def un_nest_types(types):
+    """
+    Un-nests the given `types`.
+    
+    Parameters
+    ----------
+    types : `type<type> | tuple<type<type>, ...>`
+        The types to un-nest.
+    
+    Returns
+    -------
+    types : `set` of `type`
+    
+    Raises
+    ------
+    TypeError
+        If an element's type is incorrect.
+    """
+    types = un_nest(types)
+    
+    for type_value in types:
+        if not isinstance(type_value, type):
+            raise TypeError(
+                f'`type` can be `type`, `tuple` of (`type`, ...)`, '
+                f'got {type_value.__class__.__name__}; {type_value!r}.'
+            )
+    
+    return types
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_states.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_states.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 __all__ = ('get_assertion_state_name', )
 
-NONE = 0
-CREATED = 1
-FAILED = 2
-PASSED = 3
+
+ASSERTION_STATE_NONE = 0
+ASSERTION_STATE_CREATED = 1
+ASSERTION_STATE_FAILED = 2
+ASSERTION_STATE_PASSED = 3
 
 DEFAULT_ASSERTION_STATE_NAME = 'unknown'
 
 ASSERTION_STATE_TO_NAME = {
-    NONE: 'none',
-    CREATED: 'created',
-    FAILED: 'failed',
-    PASSED: 'passed',
+    ASSERTION_STATE_NONE: 'none',
+    ASSERTION_STATE_CREATED: 'created',
+    ASSERTION_STATE_FAILED: 'failed',
+    ASSERTION_STATE_PASSED: 'passed',
 }
 
+
 def get_assertion_state_name(state):
     """
     Returns the condition state's name.
     
     Parameters
     ----------
     state : `int`
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/assertion_true.py` & `vampytest-0.0.8/vampytest/core/assertions/assertion_equals.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-__all__ = ('AssertionValueEvaluationTrue', 'assert_', 'assert_true',)
+__all__ = ('AssertionEquals',)
 
 from scarletio import copy_docs
 
-from .assertion_conditional_base import AssertionConditionalBase1Value
+from .assertion_conditional_base import AssertionConditionalBase2Value
 
 
-class AssertionValueEvaluationTrue(AssertionConditionalBase1Value):
+class AssertionEquals(AssertionConditionalBase2Value):
     """
-    Asserts whether the value evaluates to `True`.
+    Asserts equality.
     
     Attributes
     ----------
     state : `str`
         The condition's state.
     exception : `None`, `BaseException`
         Exception raised by the condition if any.
     reverse : `bool`
         Whether the condition should be reversed.
-    value_1 : `Any`
-        First value to assert.
+    value_0 : `object`
+        First value to assert equality with.
+    value_1 : `object`
+        The second value to assert equality with.
     """
     __slots__ = ()
     
-    @copy_docs(AssertionConditionalBase1Value.invoke_condition)
+    @copy_docs(AssertionConditionalBase2Value.invoke_condition)
     def invoke_condition(self):
-        return self.value_1
+        return self.value_0 == self.value_1
     
     
-    @copy_docs(AssertionConditionalBase1Value._get_operation_representation)
+    @copy_docs(AssertionConditionalBase2Value._get_operation_representation)
     def _get_operation_representation(self):
-        return 'bool(...)'
-    
-    
-    @copy_docs(AssertionConditionalBase1Value._render_operation_representation_into)
-    def _render_operation_representation_into(self, into):
-        AssertionConditionalBase1Value._render_operation_representation_into(self, into)
-        into.append(' as "bool(parameter)"')
-        return into
-
-
-assert_ = AssertionValueEvaluationTrue
-assert_true = AssertionValueEvaluationTrue
+        return '=='
```

### Comparing `vampytest-0.0.7/vampytest/core/assertions/exceptions.py` & `vampytest-0.0.8/vampytest/core/assertions/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     -------
     should_show_frame : `bool`
         Whether the frame should be shown.
     """
     should_show_frame = True
     
     if file_name == VAMPYTEST_ASSERTION_CONDITION_BASE_FILE_PATH:
-        if name == '__new__':
-            if line == 'return self.invoke()':
+        if name == '__call__':
+            if line == 'return type_.__new__(type_, *positional_parameters, **keyword_parameter).invoke()':
                 should_show_frame = False
         
         elif name == 'invoke':
             if line == 'raise AssertionException(self)':
                 should_show_frame = False
     
     elif file_name == VAMPYTEST_ASSERTION_INSTANCE_FILE_PATH:
@@ -68,15 +68,14 @@
             if line == 'returned_value = await test(*positional_parameters, **keyword_parameters)':
                 should_show_frame = False
     
     
     return should_show_frame
 
 
-
 @export
 class AssertionException(BaseException):
     """
     Raised when an exception fails.
     
     Attributes
     ----------
@@ -107,11 +106,11 @@
         
         Returns
         -------
         failure_message_parts : `list` of `str`
         """
         frames = _get_exception_frames(self)
         failure_message_parts.append('\n')
-        render_frames_into(frames, failure_message_parts, filter=_ignore_assertion_frames)
+        render_frames_into(frames, failure_message_parts, filter = _ignore_assertion_frames)
         failure_message_parts.append('\n')
         self.assertion.render_failure_message_parts_into(failure_message_parts)
         return failure_message_parts
```

### Comparing `vampytest-0.0.7/vampytest/core/environment/configuration.py` & `vampytest-0.0.8/vampytest/core/environment/configuration.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest/core/environment/default.py` & `vampytest-0.0.8/vampytest/core/environment/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         """
         Runs the defined test with the given parameters.
         
         Parameters
         ----------
         test : `callable`
             The test to call
-        positional_parameters : `list` of `Any`
+        positional_parameters : `list` of `object`
             Positional parameters to call the test with.
-        keyword_parameters : `dict` of (`str`, `Any`) items
+        keyword_parameters : `dict` of (`str`, `object`) items
             Keyword parameters to call the test with.
         
         Returns
         -------
         result_state : ``ResultState``
             The result's product.
         """
```

### Comparing `vampytest-0.0.7/vampytest/core/environment/helpers.py` & `vampytest-0.0.8/vampytest/core/environment/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,13 +32,13 @@
         return ENVIRONMENT_TYPE_GENERATOR
     
     return ENVIRONMENT_TYPE_DEFAULT
 
 
 def shutdown_environments():
     """
-    Shuts down all the registered environments. This operation cannot be reverted.
+    Shuts down all the registered environments. This operation cannot be reversed.
     """
     for environment_by_detail in ENVIRONMENTS_BY_SCOPE.values():
         for environments_by_identifier in environment_by_detail.values():
             for environment in environments_by_identifier.values():
                 environment.shutdown()
```

### Comparing `vampytest-0.0.7/vampytest/core/environment/manager.py` & `vampytest-0.0.8/vampytest/core/environment/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,27 @@
     """
     Represents an environment manager managing testing environments.
     
     Attributes
     ----------
     _environments_by_identifier : `dict` of (`int`, ``DefaultEnvironment``) items
     """
-    __slots__ = ('_environments_by_identifier')
+    __slots__ = ('_environments_by_identifier',)
     
     def __new__(cls):
         """
         Creates a new environment manager.
         """
         self = object.__new__(cls)
         self._environments_by_identifier = {}
         return self
     
     def __repr__(self):
         """Returns the testing environment's representation."""
-        return f'<{self.__class__.__name__} environments_by_identifier={self._environments_by_identifier!r}>'
+        return f'<{self.__class__.__name__} environments_by_identifier = {self._environments_by_identifier!r}>'
     
     
     def get_environment_for_test(self, test):
         """
         Gets environment for the given test.
         
         Parameters
```

### Comparing `vampytest-0.0.7/vampytest/core/environment/scarletio_coroutine.py` & `vampytest-0.0.8/vampytest/core/environment/scarletio_coroutine.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
         
         This method is a coroutine.
         
         Parameters
         ----------
         test : `callable`
             The test to call
-        positional_parameters : `list` of `Any`
+        positional_parameters : `list` of `object`
             Positional parameters to call the test with.
-        keyword_parameters : `dict` of (`str`, `Any`) items
+        keyword_parameters : `dict` of (`str`, `object`) items
             Keyword parameters to call the test with.
         
         Returns
         -------
         result_state : ``ResultState``
             The result's product.
         """
```

### Comparing `vampytest-0.0.7/vampytest/core/event_handling/base.py` & `vampytest-0.0.8/vampytest/core/event_handling/base.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest/core/event_handling/default.py` & `vampytest-0.0.8/vampytest/core/event_handling/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 __all__ = ('create_default_event_handler_manager',)
 
-from scarletio import RichAttributeErrorBaseType, create_ansi_format_code
+from scarletio import RichAttributeErrorBaseType
 
 from ..events import FileLoadDoneEvent, FileRegistrationDoneEvent, FileTestingDoneEvent, TestDoneEvent, TestingEndEvent
 
 from .base import EventHandlerManager
+from .colors import COLOR_FAIL, COLOR_PASS, COLOR_SKIP, COLOR_UNKNOWN
 from .default_output_writer import OutputWriter
+from .rendering_helpers.result_modifier_parameters import build_result_modifier_parameters
+from .rendering_helpers.writers import write_load_failure, write_result_failing, write_result_informal
 from .text_styling import style_text
 
 
-COLOR_FAIL = create_ansi_format_code(foreground_color = (255, 0, 0))
-COLOR_PASS = create_ansi_format_code(foreground_color = (0, 255, 0))
-COLOR_SKIP = create_ansi_format_code(foreground_color = (0, 255, 255))
-COLOR_UNKNOWN = create_ansi_format_code(foreground_color = (255, 0, 255))
-COLOR_RESET = create_ansi_format_code()
-
-
 def create_default_event_handler_manager():
     """
     Creates a default event handler manager if non is given.
     
     Returns
     ----------
     event_handler_manager : ``EventHandlerManager``
@@ -45,15 +41,15 @@
     rendered_entries : `set` of ``FileSystemEntry``
         The rendered entries by the
     output_writer : ``OutputWriter``
         The output writer to write the output with.
     """
     __slots__ = ('rendered_entries', 'output_writer',)
     
-    def __new__(cls, output_writer=None):
+    def __new__(cls, output_writer = None):
         """
         Creates a new default event formatter.
         
         Parameters
         ----------
         output_writer : `None`, ``OutputWriter` = `None`, Optional
             The output writer to write the output with.
@@ -65,15 +61,15 @@
         self.rendered_entries = set()
         self.output_writer = output_writer
         return self
     
     
     def __repr__(self):
         """Returns the output formatter representation."""
-        return f'<{self.__class__.__name__} output_writer={self.output_writer!r}>'
+        return f'<{self.__class__.__name__} output_writer = {self.output_writer!r}>'
     
     
     def file_registration_done(self, event: FileRegistrationDoneEvent):
         """
         Called when all files are registered.
         
         Parameters
@@ -105,15 +101,15 @@
                     COLOR_FAIL,
                 ),
             )
             
             self.output_writer.write_line(''.join(message_parts))
     
     
-    def _maybe_render_test_file_into(self, into, entry, *, name=None):
+    def _maybe_render_test_file_into(self, into, entry, *, name = None):
         """
         Helpers method for rendering file structure tree.
         
         Parameters
         ----------
         into : `list` of `str`
             List to render the structure parts into.
@@ -132,63 +128,67 @@
             for sub_entry in entry.iter_parents():
                 if sub_entry in rendered_entries:
                     continue
                     
                 into = sub_entry.render_into(into)
                 rendered_entries.add(sub_entry)
             
-            into = entry.render_into(into, name=name)
+            into = entry.render_into(into, name = name)
             rendered_entries.add(entry)
         
         return into
     
     
     def test_done(self, event: TestDoneEvent):
         """
         Called when a test is done.
         
         Parameters
         ----------
         event : ``TestDoneEvent``
             The dispatched event.
         """
-        test_file = event.result_group.case.get_test_file()
+        test_file = event.result.case.get_test_file()
         if (test_file is None):
             # Should not happen
             return
         
         message_parts = self._maybe_render_test_file_into([], test_file.entry)
         
-        result_group = event.result_group
-        if result_group.is_skipped():
+        result = event.result
+        if result.is_skipped():
             keyword = 'S'
             foreground = COLOR_SKIP
         
-        elif result_group.is_passed():
+        elif result.is_conflicted():
+            keyword = 'C'
+            foreground = COLOR_FAIL
+            
+        elif result.is_passed():
             keyword = 'P'
             foreground = COLOR_PASS
         
-        elif result_group.is_failed():
+        elif result.is_failed():
             keyword = 'F'
             foreground = COLOR_FAIL
         
         else:
             keyword = '?'
             foreground = COLOR_UNKNOWN
         
+        result_modifiers = build_result_modifier_parameters(result.get_modifier_parameters())
         message_parts = test_file.entry.render_custom_sub_directory_into(
             message_parts,
-            style_text(f'{keyword} {result_group.case.name}', foreground),
-            result_group.case.is_last(),
+            style_text(f'{keyword} {result.case.name}{result_modifiers}', foreground),
+            result.is_last() and result.case.is_last(),
         )
         
         self.output_writer.write_line(''.join(message_parts))
     
-
-
+    
     def file_testing_done(self, event: FileTestingDoneEvent):
         """
         Called when all tests of a file is done
         
         Parameters
         ----------
         event : ``FileTestingDoneEvent``
@@ -210,37 +210,27 @@
         """
         output_writer = self.output_writer
         output_writer.write_break_line()
         
         context = event.context
         
         load_failures = context.get_file_load_failures()
-        
         for load_failure in load_failures:
-            message = ''.join([
-                'Exception occurred while loading:\n',
-                load_failure.path,
-                '\n\n',
-                load_failure.exception_message,
-            ])
-            
-            output_writer.write_line(message)
-            output_writer.write_break_line()
+            write_load_failure(output_writer, load_failure)
         
-        
-        for result_group in context.iter_failed_result_groups():
-            for failure_message in result_group.iter_failure_messages():
-                output_writer.write_line(failure_message)
-                output_writer.write_break_line()
+        for result in context.iter_failed_results():
+            write_result_failing(output_writer, result)
         
         failed_count = context.get_failed_test_count()
         failed_message_part = f'{failed_count} failed'
         if failed_count:
             failed_message_part = style_text(failed_message_part, COLOR_FAIL)
-        
+        else:
+            for result in context.iter_informal_results():
+                write_result_informal(output_writer, result)
         
         skipped_count = context.get_skipped_test_count()
         skipped_message_part = f'{skipped_count} skipped'
         if skipped_count:
             skipped_message_part = style_text(skipped_message_part, COLOR_SKIP)
```

### Comparing `vampytest-0.0.7/vampytest/core/event_handling/default_output_writer.py` & `vampytest-0.0.8/vampytest/core/event_handling/default_output_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,37 +15,37 @@
     
     Attributes
     ----------
     _last_chunk_break_line : `bool`
         Whether the last written line was a break line.
     _last_write_ended_with_linebreak : `bool`
         Whether the last write ended with a linebreak.
-    file : `Any`
-        Any writable object.
+    file : `io-like`
+        object writable object.
     """
     def __new__(cls, file = None):
         """
         Creates a new test output writer.
         
         Parameters
         ----------
-        file : `None`, `Any` = `None`, Optional
+        file : `None`, `io-like` = `None`, Optional
             Writable object. If not given defaults to `sys.stdout`.
         """
         if file is None:
             file = sys.stdout
         
         self = object.__new__(cls)
         self._last_chunk_break_line = False
         self._last_write_ended_with_linebreak = False
         self.file = file
         return self
     
     
-    def write_break_line(self, character="="):
+    def write_break_line(self, character = '='):
         """
         Writes a break line.
         
         Parameters
         ----------
         character : `str` = `'='`, Optional
             The character to use.
```

### Comparing `vampytest-0.0.7/vampytest/core/event_handling/text_styling.py` & `vampytest-0.0.8/vampytest/core/event_handling/text_styling.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,42 +19,73 @@
     format_code : `str`
         Format code to style the text with.
     
     Returns
     -------
     text : `str`
     """
-    return ''.join(style_text_into(text, [], format_code))
+    return ''.join(style_text_into([], text, format_code))
 
 
 if sys.platform == 'win32':
-    def style_text_into(text, into, format_code):
+    def style_text_into(into, text, format_code):
         into.append(text)
         return into
     
+    def style_text_block(into, format_code):
+        yield
+
 else:
-    def style_text_into(text, into, format_code):
+    def style_text_into(into, text, format_code):
         into.append(format_code)
         into.append(text)
         into.append(STYLE_RESET)
         return into
+    
+    def style_text_block(into, format_code):
+        into.append(format_code)
+        yield
+        into.append(STYLE_RESET)
 
 
 set_docs(
     style_text_into,
     """
     Renders the given text with the style parts into the given list.
     
     Parameters
     ----------
-    text : `str`
-        Text to render with the given style.
     into : `list` of `str`
         The list of strings to add the new parts into.
+    text : `str`
+        Text to render with the given style.
     format_code : `str`
         Format code to style the text with.
     
     Returns
     -------
     into : `list` of `str`
     """
 )
+
+
+set_docs(
+    style_text_block,
+    """
+    Renders the style into the given parts. Can be used as a block.
+    
+    ```py
+    for _ in style_text_into(into, format_code):
+        into.append(text_part)
+        ...
+    ```
+    
+    This function is an iterable generator.
+    
+    Parameters
+    ----------
+    into : `list` of `str`
+        The list of strings to add the new parts into.
+    format_code : `str`
+        Format code to style the text with.
+    """
+)
```

### Comparing `vampytest-0.0.7/vampytest/core/events/__init__.py` & `vampytest-0.0.8/vampytest/core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest/core/events/base.py` & `vampytest-0.0.8/vampytest/core/events/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,42 +64,42 @@
         self = EventBase.__new__(cls, context)
         self.file = file
         return self
     
     
     @copy_docs(EventBase.__repr__)
     def __repr__(self):
-        return f'<{self.__class__.__name__} file={self.file!r}>'
+        return f'<{self.__class__.__name__} file = {self.file!r}>'
 
 
-class ResultGroupEventBase(EventBase):
+class ResultEventBase(EventBase):
     """
     Represents a dispatched event by a test runner.
     
     Attributes
     ----------
     context : ``RunnerContext``
         The respective test running context.
-    result_group : ``ResultGroup``
-        The respective result group.
+    result : ``Result``
+        The respective result.
     """
-    __slots__ = ('result_group',)
+    __slots__ = ('result',)
     
-    def __new__(cls, context, result_group):
+    def __new__(cls, context, result):
         """
         Creates a new file event instance.
         
         Parameters
         ----------
         context : ``RunnerContext``
             The respective test running context.
-        result_group : ``ResultGroup``
-            The respective result group.
+        result : ``Result``
+            The respective result.
         """
         self = EventBase.__new__(cls, context)
-        self.result_group = result_group
+        self.result = result
         return self
     
     
     @copy_docs(EventBase.__repr__)
     def __repr__(self):
-        return f'<{self.__class__.__name__} result_group={self.result_group!r}>'
+        return f'<{self.__class__.__name__} result = {self.result!r}>'
```

### Comparing `vampytest-0.0.7/vampytest/core/events/file_load_done.py` & `vampytest-0.0.8/vampytest/core/events/file_load_done.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest/core/file/collection.py` & `vampytest-0.0.8/vampytest/core/file/collection.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest/core/file/file_system_entry.py` & `vampytest-0.0.8/vampytest/core/file/file_system_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                 entries.append(entry)
         
         self._entries = entries
         
         return True
     
     
-    def render_into(self, into, *, name=None):
+    def render_into(self, into, *, name = None):
         """
         Renders the path access into the given list of strings.
         
         Parameters
         ----------
         into : `list` of `str`
             List to render self into.
```

### Comparing `vampytest-0.0.7/vampytest/core/file/load_failure.py` & `vampytest-0.0.8/vampytest/core/file/load_failure.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest/core/file/test_file.py` & `vampytest-0.0.8/vampytest/core/file/test_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ('TestFile', )
 
 import sys
 
 from scarletio import RichAttributeErrorBaseType
 
 from ..environment import apply_environments_for_file_at
-from ..utils import get_short_path_repr
+from ..helpers.path_repr import get_short_path_repr
 from ..test_case import TestCase
 from ..wrappers import WrapperBase
 
 from .load_failure import TestFileLoadFailure
 
 
 def is_test_name(name):
@@ -38,15 +38,15 @@
     """
     Returns whether the given name - value pair refers to a test.
     
     Parameters
     ----------
     name : `str`
         The name of a a variable.
-    value : `Any`
+    value : `object`
         The variable's value.
     
     Returns
     -------
     is_test : `bool`
     """
     if not is_test_name(name):
@@ -80,15 +80,15 @@
     
     Attributes
     ----------
     _load_failure : `None`, ``TestFileLoadFailure``
         If loading the test file fails, this attribute is set to details about the occurred exception.
     _module : `None`, `ModuleType`
         The module of the test file. Only set when the first call is made to it.
-    _result_groups : `None`, `list` of ``ResultGroup``
+    _results : `None`, `list` of ``Result``
         Results of already ran tests.
     _sub_files : `None`, `list` of ``TestFile``
         Sub files if we are a directory.
     _test_cases : `None`, `list` of ``TestCase``
         The collected test_cases from the file if any. These test_cases are on collected after calling ``.get_test_cases`` for
         the first time.
     entry : ``FileSystemEntry``
@@ -104,18 +104,18 @@
         - ``.is_loaded_with_failure``
         - ``.get_load_failure``
         - ``.is_directory``
         - ``.is_loaded``
     
     - Iterators
     
-        - ``.iter_result_groups``
-        - ``.iter_passed_result_groups``
-        - ``.iter_skipped_result_groups``
-        - ``.iter_failed_result_groups``
+        - ``.iter_results``
+        - ``.iter_passed_results``
+        - ``.iter_skipped_results``
+        - ``.iter_failed_results``
         - ``.iter_sub_files``
     
     - Counters
     
         - ``.get_test_case_count``
         - ``.get_ran_test_count``
         - ``.get_passed_test_count``
@@ -130,15 +130,15 @@
         - ``.get_test_cases``
         - ``.iter_test_cases``
         - ``.iter_invoke_test_cases``
         - ``.feed_sub_file``
         - ``.iter_test_files``
     """
     __slots__ = (
-        '__weakref__', '_load_failure', '_module', '_result_groups', '_sub_files', '_test_cases', 'entry', 'import_route'
+        '__weakref__', '_load_failure', '_module', '_results', '_sub_files', '_test_cases', 'entry', 'import_route'
     )
     
     def __new__(cls, entry):
         """
         Creates an new test file.
         
         Parameters
@@ -160,15 +160,15 @@
         
         
         import_route = '.'.join(path_parts)
         
         self = object.__new__(cls)
         self._load_failure = None
         self._module = None
-        self._result_groups = None
+        self._results = None
         self._sub_files = None
         self._test_cases = None
         self.entry = entry
         self.import_route = import_route
         return self
     
     
@@ -372,52 +372,51 @@
         Parameters
         ----------
         environment_manager : ``EnvironmentManager``
             Testing environment manager.
         
         Yields
         ------
-        result_group : ``ResultGroup``
+        result : ``Result``
         """
         if self.is_directory():
             return
         
-        result_groups = self._result_groups
-        if (result_groups is not None):
-            return (yield from result_groups)
+        results = self._results
+        if (results is not None):
+            return (yield from results)
         
         environment_manager = apply_environments_for_file_at(environment_manager, self.path)
         for test_case in self.iter_test_cases():
-            result_group = test_case.invoke(environment_manager)
-            
-            if (result_groups is None):
-                result_groups = []
-                self._result_groups = result_groups
-            
-            result_groups.append(result_group)
-            
-            yield result_group
+            for result in test_case.iter_invoke(environment_manager):
+                if (results is None):
+                    results = []
+                    self._results = results
+                
+                results.append(result)
+                
+                yield result
     
     
-    def iter_result_groups(self):
+    def iter_results(self):
         """
-        Iterates over the result groups of the test file.
+        Iterates over the results of the test file.
         
         This method is an iterable generator.
         
         Yields
         ------
-        result_group : ``ResultGroup``
+        result : ``Result``
         """
-        result_groups = self._result_groups
-        if (result_groups is not None):
-            yield from result_groups
+        results = self._results
+        if (results is not None):
+            yield from results
         
         for sub_file in self.iter_sub_files():
-            yield from sub_file.iter_result_groups()
+            yield from sub_file.iter_results()
     
     
     def get_test_case_count(self):
         """
         Returns how much test cases are in the test file collected.
         
         Returns
@@ -440,102 +439,117 @@
         """
         Returns how much tests already ran of the file.
         
         Returns
         -------
         ran_test_count : `int`
         """
-        result_groups = self._result_groups
-        if (result_groups is None):
+        results = self._results
+        if (results is None):
             ran_test_count = 0
         else:
-            ran_test_count = len(result_groups)
+            ran_test_count = len(results)
         
         for sub_file in self.iter_sub_files():
             ran_test_count += sub_file.get_ran_test_count()
         
         return ran_test_count
     
     
-    def iter_passed_result_groups(self):
+    def iter_passed_results(self):
+        """
+        Iterates over the passed results of the test file.
+        
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        result : ``Result``
+        """
+        for result in self.iter_results():
+            if result.is_passed():
+                yield result
+    
+    
+    def iter_skipped_results(self):
         """
-        Iterates over the passed result groups of the test file.
+        Iterates over the skipped results of the test file.
         
         This method is an iterable generator.
         
         Yields
         ------
-        result_group : ``ResultGroup``
+        result : ``Result``
         """
-        for result_group in self.iter_result_groups():
-            if result_group.is_passed():
-                yield result_group
+        for result in self.iter_results():
+            if result.is_skipped():
+                yield result
     
     
-    def iter_skipped_result_groups(self):
+    def iter_failed_results(self):
         """
-        Iterates over the skipped result groups of the test file.
+        Iterates over the failed results of the test file.
         
         This method is an iterable generator.
         
         Yields
         ------
-        result_group : ``ResultGroup``
+        result : ``Result``
         """
-        for result_group in self.iter_result_groups():
-            if result_group.is_skipped():
-                yield result_group
+        for result in self.iter_results():
+            if result.is_failed():
+                yield result
     
     
-    def iter_failed_result_groups(self):
+    def iter_informal_results(self):
         """
-        Iterates over the failed result groups of the test file.
+        Iterates over the informal results of the test file.
         
         This method is an iterable generator.
         
         Yields
         ------
-        result_group : ``ResultGroup``
+        result : ``Result``
         """
-        for result_group in self.iter_result_groups():
-            if result_group.is_failed():
-                yield result_group
+        for result in self.iter_results():
+            if result.is_informal():
+                yield result
     
     
     def get_passed_test_count(self):
         """
         Returns how much test passed.
         
         Returns
         -------
         passed_test_count : `int`
         """
-        return sum(result_group.is_passed() for result_group in self.iter_result_groups())
+        return sum(result.is_passed() for result in self.iter_results())
     
     
     def get_skipped_test_count(self):
         """
         Returns how much test was skipped.
         
         Returns
         -------
         passed_test_count : `int`
         """
-        return sum(result_group.is_skipped() for result_group in self.iter_result_groups())
+        return sum(result.is_skipped() for result in self.iter_results())
     
     
     def get_failed_test_count(self):
         """
         Returns how much test failed.
         
         Returns
         -------
         passed_test_count : `int`
         """
-        return sum(result_group.is_failed() for result_group in self.iter_result_groups())
+        return sum(result.is_failed() for result in self.iter_results())
     
     
     def feed_sub_file(self, sub_file):
         """
         Adds a sub-file if the file is a directory.
         
         Parameters
```

### Comparing `vampytest-0.0.7/vampytest/core/handle.py` & `vampytest-0.0.8/vampytest/core/handle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 __all__ = ('CallState', 'ResultState', 'Handle',)
 
 import reprlib
 
 from scarletio import RichAttributeErrorBaseType, include
 
-from .helpers import hash_dict, hash_list, hash_object, maybe_merge_iterables, maybe_merge_mappings
+from .contexts import ContextOutputCapturing
+from .helpers.hashing import hash_dict, hash_list, hash_object
+from .helpers.merging import maybe_merge_iterables, maybe_merge_mappings
 
 
 Result = include('Result')
 AssertionException = include('AssertionException')
 
 
 class CallState(RichAttributeErrorBaseType):
     """
     Defines how the function should be called.
     
     Attributes
     ----------
-    keyword_parameters : `None`, `dict` of (`str`, `Any`) items
+    keyword_parameters : `None`, `dict` of (`str`, `object`) items
         Keyword parameters to the call the test function with.
-    positional_parameters : `None`, `list` of `Any`
+    positional_parameters : `None`, `list` of `object`
         Positional parameters to the the test function with.
     """
     __slots__ = ('keyword_parameters', 'positional_parameters')
     
     def __new__(cls):
         """
         Creates a new calls state.
@@ -98,15 +100,15 @@
     
     def copy(self):
         """
         Copies the call state.
         
         Returns
         -------
-        new : ``CallState``
+        new : `instance<type<self>`
         """
         keyword_parameters = self.keyword_parameters
         if (keyword_parameters is not None):
             keyword_parameters = keyword_parameters.copy()
         
         positional_parameters = self.positional_parameters
         if (positional_parameters is not None):
@@ -120,22 +122,22 @@
     
     def with_parameters(self, positional_parameters, keyword_parameters):
         """
         Creates a new call state with merged parameters.
         
         Parameters
         ----------
-        positional_parameters : `None`, `list` of `Any`
+        positional_parameters : `None`, `list` of `object`
             Positional parameters to the the test function with.
-        keyword_parameters : `None`, `dict` of (`str`, `Any`) items
+        keyword_parameters : `None`, `dict` of (`str`, `object`) items
             Keyword parameters to the call the test function with.
         
         Returns
         -------
-        new : ``CallState``
+        new : `instance<type<self>>`
         """
         positional_parameters = maybe_merge_iterables(self.positional_parameters, positional_parameters)
         keyword_parameters = maybe_merge_mappings(self.keyword_parameters, keyword_parameters)
         
         new = object.__new__(type(self))
         new.keyword_parameters = keyword_parameters
         new.positional_parameters = positional_parameters
@@ -157,26 +159,26 @@
     """
     Represents a test's output.
     
     Attributes
     ----------
     raised_exception : `None`, `BaseException`
         The raised exception by the test.
-    returned_value : `None`, `Any`
+    returned_value : `None`, `object`
         The returned value by the test.
     """
-    __slots__ = ('raised_exception', 'returned_value')
+    __slots__ = ('raised_exception', 'returned_value',)
     
     def __new__(cls, returned_value, raised_exception):
         """
         Creates a new result state.
         
         Parameters
         ----------
-        returned_value : `None`, `Any`
+        returned_value : `None`, `object`
             The returned value by the test.
         raised_exception : `None`, `BaseException`
             The raised exception by the test.
         """
         self = object.__new__(cls)
         self.raised_exception = raised_exception
         self.returned_value = returned_value
@@ -192,28 +194,27 @@
         returned_value = self.returned_value
         if (returned_value is not None):
             if field_added:
                 repr_parts.append(',')
             else:
                 field_added = True
             
-            repr_parts.append(' returned_value')
+            repr_parts.append(' returned_value = ')
             repr_parts.append(repr(returned_value))
         
         raised_exception = self.raised_exception
         if (raised_exception is not None):
             if field_added:
                 repr_parts.append(',')
             else:
                 field_added = True
             
-            repr_parts.append(' raised_exception')
+            repr_parts.append(' raised_exception = ')
             repr_parts.append(repr(raised_exception))
         
-        
         repr_parts.append('>')
         return ''.join(repr_parts)
     
     
     def __eq__(self, other):
         """Returns whether the two result states are equal."""
         if type(self) is not type(other):
@@ -247,15 +248,15 @@
     
     def copy(self):
         """
         Copies the result state.
         
         Returns
         -------
-        new : ``ResultState``
+        new : `instance<type<self>>`
         """
         new = object.__new__(type(self))
         new.raised_exception = self.raised_exception
         new.returned_value = self.returned_value
         return new
     
     
@@ -272,20 +273,20 @@
     
     def with_return(self, returned_value):
         """
         Creates a new call state overwriting the old one.
         
         Parameters
         ----------
-        returned_value : `None`, `Any`
+        returned_value : `None`, `object`
             The returned value by the test.
         
         Returns
         -------
-        new : ``ResultState``
+        new : `instance<type<self>>`
         """
         new = object.__new__(type(self))
         new.raised_exception = None
         new.returned_value = returned_value
         return new
     
     
@@ -296,15 +297,15 @@
         Parameters
         ----------
         raised_exception : `None`, `BaseException`
             The raised exception by the test.
         
         Returns
         -------
-        new : ``ResultState``
+        new : `instance<type<self>>`
         """
         new = object.__new__(type(self))
         new.raised_exception = raised_exception
         new.returned_value = None
         return new
 
 
@@ -367,133 +368,169 @@
         return self
     
     
     def __repr__(self):
         """Returns the test handle's representation."""
         repr_parts = ['<', self.__class__.__name__]
         
-        repr_parts.append(' test=')
+        repr_parts.append(' test = ')
         repr_parts.append(reprlib.repr(self.test))
         
         wrappers = self.wrappers
         if (wrappers is not None):
-            repr_parts.append(', wrappers=')
+            repr_parts.append(', wrappers = ')
             repr_parts.append(repr(wrappers))
         
         original_call_state = self.original_call_state
         if (original_call_state is not None) and original_call_state:
-            repr_parts.append(', original_call_state=')
+            repr_parts.append(', original_call_state = ')
             repr_parts.append(repr(original_call_state))
         
         final_call_state = self.final_call_state
         if (final_call_state is not None) and final_call_state:
-            repr_parts.append(', final_call_state=')
+            repr_parts.append(', final_call_state = ')
             repr_parts.append(repr(final_call_state))
             
         original_result_state = self.original_result_state
         if (original_result_state is not None) and original_result_state:
-            repr_parts.append(', original_result_state=')
+            repr_parts.append(', original_result_state = ')
             repr_parts.append(repr(original_result_state))
         
         final_result_state = self.final_result_state
         if (final_result_state is not None) and final_result_state:
-            repr_parts.append(', final_result_state=')
+            repr_parts.append(', final_result_state = ')
             repr_parts.append(repr(final_result_state))
         
         repr_parts.append('>')
         return ''.join(repr_parts)
     
     
-    def _initialise_test_wrapper_contexts(self, test_wrapper_contexts):
+    def _collect_contexts_into(self, contexts):
         """
         Initialises the wrappers of the test handle.
         
         Parameters
         ----------
-        test_wrapper_contexts : `list` of `GeneratorType`
-            Test wrappers to initialize into
+        contexts : `list` of ``ContextBase```
+            Test contexts to put the new ones into.
         """
         wrappers = self.wrappers
         if wrappers is not None:
             for wrapper in wrappers:
-                context = wrapper.context(self)
-                test_wrapper_contexts.append(context)
+                context = wrapper.get_context(self)
+                if (context is not None):
+                    contexts.append(context)
     
     
-    def _start_test_wrapper_contexts(self, test_wrapper_contexts):
+    def _start_contexts(self, contexts):
         """
         Starts the text wrapper contexts.
         
         Parameters
         ----------
-        test_wrapper_contexts : `list` of `GeneratorType`
-            Test wrappers to initialize into
+        contexts : `list` of ``ContextBase``
+            Contexts to start.
         
         Returns
         -------
         test_result : `None`, ``Result``
             Result of the test.
         """
-        for test_wrapper_context in test_wrapper_contexts:
-            try:
-                test_result = test_wrapper_context.send(None)
-            except StopIteration as err:
-                test_result = err.value
-            
+        for context in contexts:
+            test_result = context.start()
             if (test_result is not None):
                 return test_result
     
     
-    def _enter_test_wrapper_contexts(self, test_wrapper_contexts):
+    def _enter_contexts(self, contexts):
         """
         Enters the text wrapper contexts passing them a ``CallState``, expecting them to return a new call state, or
         a test result.
         
         Parameters
         ----------
-        test_wrapper_contexts : `list` of `GeneratorType`
-            Test wrappers to start.
+        contexts : `list` of ``ContextBase``
+            Contexts to enter.
         
         Returns
         -------
         test_result : `None`, ``Result``
             Result of the test.
         """
         call_state = CallState()
         self.original_call_state = call_state
         
         try:
-            for test_wrapper_context in test_wrapper_contexts:
-                try:
-                    enter_result = test_wrapper_context.send(call_state)
-                except StopIteration as err:
-                    enter_result = err.value
+            for context in contexts:
+                test_result, new_call_state = context.enter(call_state)
+                
+                if (new_call_state is not None):
+                    call_state = new_call_state
                 
-                if enter_result is None:
-                    continue
+                if (test_result is not None):
+                    return test_result
+        
+        finally:
+            self.final_call_state = call_state
+    
+    
+    def _exit_contexts(self, contexts):
+        """
+        Exits the contexts passing them a ``ResultState``, expecting them to return a result state, or a result.
+        
+        Parameters
+        ----------
+        contexts : `list` of ``ContextBase``
+            Contexts to exit.
+        
+        Returns
+        -------
+        test_result : `None`, ``Result``
+            Result of the test.
+        """
+        result_state = self.original_result_state
+        
+        try:
+            for context in reversed(contexts):
+                test_result, new_result_state = context.exit(result_state)
                 
-                if isinstance(enter_result, CallState):
-                    call_state = enter_result
+                if (new_result_state is not None):
+                    result_state = new_result_state
                 
-                if isinstance(enter_result, Result):
-                    return enter_result
+                if (test_result is not None):
+                    return test_result
             
         finally:
-            self.final_call_state = call_state
+            self.final_result_state = result_state
+    
+    
+    def _close_contexts(self, contexts, result):
+        """
+        Exits the contexts.
+        
+        Parameters
+        ----------
+        contexts : `list` of ``ContextBase``
+            Contexts to exit.
+        result : `None`, ``Result˙`
+            Result of the test.
+        """
+        for context in reversed(contexts):
+            context.close(result)
     
     
     def _get_call_parameters(self):
         """
         Gets call parameters to invoke the test with.
         
         Returns
         -------
-        positional_parameters : `list` of `Any`
+        positional_parameters : `list` of `object`
             Positional parameters to call the test with.
-        keyword_parameters : `dict` of (`str`, `Any`) items
+        keyword_parameters : `dict` of (`str`, `object`) items
             Keyword parameters to call the test with.
         """
         call_state = self.final_call_state
         
         if call_state is None:
             positional_parameters = None
             keyword_parameters = None
@@ -517,77 +554,35 @@
         
         Parameters
         ----------
         environment_manager : ``EnvironmentManager``
             Testing environment manager.
         """
         positional_parameters, keyword_parameters = self._get_call_parameters()
-        
         test = self.test
-        
         environment = environment_manager.get_environment_for_test(test)
-        
         result_state = environment.run(test, positional_parameters, keyword_parameters)
-        
         self.original_result_state = result_state
     
     
-    def _exit_test_wrapper_contexts(self, test_wrapper_contexts):
-        """
-        Exits the text wrapper contexts passing them a ``ResultState``, expecting them to return a new call state, or
-        a test result.
-        
-        Parameters
-        ----------
-        test_wrapper_contexts : `list` of `GeneratorType`
-            Test wrappers to start.
-        
-        Returns
-        -------
-        test_result : `None`, ``Result``
-            Result of the test.
-        """
-        result_state = self.original_result_state
-        
-        try:
-            for test_wrapper_context in test_wrapper_contexts:
-                try:
-                    exit_result = test_wrapper_context.send(result_state)
-                except StopIteration as err:
-                    exit_result = err.value
-                
-                if exit_result is None:
-                    continue
-                
-                if isinstance(exit_result, ResultState):
-                    result_state = exit_result
-                
-                if isinstance(exit_result, Result):
-                    return exit_result
-            
-        finally:
-            self.final_result_state = result_state
-    
-    
     def _build_default_test_result(self):
         """
         Builds test result if non of the wrappers did before.
         
         Returns
         -------
         test_result : ``Result``
             Result of the test.
         """
-        test_result = Result(self)
+        test_result = Result(self.case).with_handle(self)
         
         raised_exception = self.final_result_state.raised_exception
         if (raised_exception is not None):
             if isinstance(raised_exception, AssertionException):
                 test_result = test_result.with_assertion(raised_exception)
-            
             else:
                 test_result = test_result.with_exception(None, raised_exception, False)
         
         return test_result
     
     
     def _iter_applied_environments(self):
@@ -600,14 +595,15 @@
         ------
         environment : ``Environment``
         """
         environments = self.environments
         if (environments is not None):
             yield from environments
     
+    
     def invoke(self, environment_manager):
         """
         Invokes the test.
         
         Parameters
         ----------
         environment_manager : ``EnvironmentManager``
@@ -616,43 +612,39 @@
         Returns
         -------
         test_result : ``Result``
             Result of the test.
         """
         environment_manager = environment_manager.with_environment(*self._iter_applied_environments())
         
-        test_wrapper_contexts = []
+        contexts = [ContextOutputCapturing()]
+        test_result = None
+        
         try:
-            self._initialise_test_wrapper_contexts(test_wrapper_contexts)
+            self._collect_contexts_into(contexts)
             
-            test_result = self._start_test_wrapper_contexts(test_wrapper_contexts)
+            test_result = self._start_contexts(contexts)
             if (test_result is not None):
                 return test_result
             
-            
-            test_result = self._enter_test_wrapper_contexts(test_wrapper_contexts)
+            test_result = self._enter_contexts(contexts)
             if (test_result is not None):
                 return test_result
             
-            try:
-                self._invoke_test(environment_manager)
-            except:
-                self._exit_test_wrapper_contexts(test_wrapper_contexts)
-                raise
+            self._invoke_test(environment_manager)
             
-            else:
-                test_result = self._exit_test_wrapper_contexts(test_wrapper_contexts)
-                if (test_result is not None):
-                    return test_result
-            
-            return self._build_default_test_result()
+            test_result = self._exit_contexts(contexts)
+            if (test_result is not None):
+                return test_result
             
+            test_result = self._build_default_test_result()
+            return test_result
+        
         finally:
-            for test_wrapper_context in test_wrapper_contexts:
-                test_wrapper_context.close()
+            self._close_contexts(contexts, test_result)
     
     
     def get_test_documentation(self):
         """
         Returns the test's documentation.
         
         Returns
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vampytest-0.0.7/vampytest/core/helpers.py` & `vampytest-0.0.8/vampytest/core/test_case.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,309 +1,289 @@
-__all__ = ()
+__all__ = ('TestCase', )
 
-def un_nest_expected_exceptions(exceptions):
-    """
-    Un-wraps the given `exceptions` recursively.
-    
-    Parameters
-    ----------
-    exceptions : `tuple` of (`BaseException`, ...)
-        The exceptions to unwrap.
-    
-    Returns
-    -------
-    exceptions : `set` of ``BaseException``
-    
-    Raises
-    ------
-    TypeError
-        If an element's type is incorrect.
-    """
-    return set(iter_un_nest_expected_exceptions(exceptions))
+import reprlib
 
+from scarletio import RichAttributeErrorBaseType, WeakReferer
 
-def iter_un_nest_expected_exceptions(exceptions):
-    """
-    Called by ``un_nest_expected_exceptions`` or by itself to unwrap the exceptions.
-    
-    This method is an iterable generator.
-    
-    Parameters
-    ----------
-    exceptions : `tuple` of (`BaseException`, ...)
-        The exceptions to unwrap.
-    
-    Yields
-    ------
-    exception : `BaseException`
-    
-    Raises
-    ------
-    TypeError
-        If an element's type is incorrect.
-    """
-    if isinstance(exceptions, tuple):
-        for exception in exceptions:
-            yield from iter_un_nest_expected_exceptions(exception)
-        
-        return
-    
-    if (
-        (
-            isinstance(exceptions, type) and
-            issubclass(exceptions, BaseException)
-        ) or
-        isinstance(exceptions, BaseException)
-    ):
-        yield exceptions
-        return
-    
-    raise TypeError(
-        f'`exceptions` can be `tuple` of (`BaseException`, ...)`, got {exceptions.__class__.__name__}; {exceptions!r}.'
-    )
+from .handle import Handle
+from .helpers.hashing import hash_object
+from .result import Result
+from .wrappers import WrapperBase
 
 
-def hash_object(object_):
+class TestCase(RichAttributeErrorBaseType):
     """
-    Returns the hash value of the given object even if it not defines `__hash__`.
+    Represents a test.
     
-    Parameters
+    Attributes
     ----------
-    object_ : `Any`
-        The object to get it's hash value of.
-    
-    Returns
-    -------
-    hash_value : `int`
+    _test_file_reference : `None`, ``WeakReferer`` to ``TestFile``
+        The parent test file of the case.
+    name : `str`
+        The test's name.
+    test : `callable`, ``WrapperBase``
+        The test itself, or the wrapped test.
+    wrapper : `None`, ``WrapperBase``
+        Wrappers containing the test if any.    
     """
-    try:
-        hash_value = hash(object_)
-    except (TypeError, NotImplementedError):
-        hash_value = object.__hash__(object_)
+    __slots__ = ('_test_file_reference', 'name', 'test', 'wrapper')
     
-    return hash_value
-
-
-def try_hash_method(object_):
-    """
-    Tries different hash methods on the given object based on it's type.
-    
-    Parameters
-    ----------
-    object_ : `Any`
-        The object to get it's hash value of.
-    
-    Returns
-    -------
-    hash_value : `int`
-    """
-    if isinstance(object_, tuple):
-        return hash_tuple(object_)
-    
-    if isinstance(object_, list):
-        return hash_list(object_)
-    
-    if isinstance(object_, dict):
-        return hash_dict(object_)
+    def __new__(cls, test_file, name, test):
+        """
+        Creates a new test case.
+        
+        Parameters
+        ----------
+        test_file : ``TestFile``
+            The parent test file.
+        name : `str`
+            The test's name.
+        test : `callable`, ``WrapperBase``
+            The test itself, or the wrapped test.
+        """
+        if isinstance(test, WrapperBase):
+            wrapper = test
+            test = test.unbind_test()
+        else:
+            wrapper = None
+            test = test
+        
+        self = object.__new__(cls)
+        self._test_file_reference = WeakReferer(test_file)
+        self.name = name
+        self.test = test
+        self.wrapper = wrapper
+        return self
     
-    if isinstance(object_, set):
-        return hash_set(object_)
     
-    return hash_object(object_)
-
-
-def hash_tuple(tuple_):
-    """
-    Returns the hash value of the given tuple.
-    
-    Parameters
-    ----------
-    tuple_ : `tuple` of `Any`
-        The tuple to hash.
+    def __eq__(self, other):
+        """Returns whether the two test cases are equal."""
+        if type(self) is not type(other):
+            return NotImplemented
+        
+        return False
     
-    Returns
-    -------
-    hash_value : `int`
-    """
-    hash_value = len(tuple_) << 4
-    for element in tuple_:
-        hash_value ^= try_hash_method(element)
     
-    return hash_value
-
-
-def hash_list(list_):
-    """
-    Returns the hash value of the given list.
+    def __hash__(self):
+        """Returns the test case's hash value."""
+        hash_value = 0
+        
+        hash_value ^= hash(self.name)
+        hash_value ^= hash_object(self.test)
+        
+        wrapper = self.wrapper
+        if (wrapper is not None):
+            hash_value ^= hash(wrapper)
+        
+        return hash_value
     
-    Parameters
-    ----------
-    list_ : `list` of `Any`
-        The list to hash.
     
-    Returns
-    -------
-    hash_value : `int`
-    """
-    hash_value = len(list_) << 8
-    for element in list_:
-        hash_value ^= try_hash_method(element)
+    def __repr__(self):
+        """Returns the test case's representation."""
+        repr_parts = ['<', self.__class__.__name__]
+        
+        repr_parts.append(' name = ')
+        repr_parts.append(repr(self.name))
+        
+        repr_parts.append(', test = ')
+        repr_parts.append(reprlib.repr(self.test))
+        
+        wrapper = self.wrapper
+        if (wrapper is not None):
+            repr_parts.append(', wrapper = ')
+            repr_parts.append(repr(self.wrapper))
+        
+        if self.do_skip():
+            repr_parts.append(', skipped')
+        
+        if self.do_reverse():
+            repr_parts.append(', reversed')
+        
+        repr_parts.append('>')
+        return ''.join(repr_parts)
     
-    return hash_value
-
-
-def hash_dict(dict_):
-    """
-    Returns the hash value of the given dict.
     
-    Parameters
-    ----------
-    dict_ : `dict` of `Any`
-        The dict to hash.
-    
-    Returns
-    -------
-    hash_value : `int`
-    """
-    hash_value = len(dict_) << 12
+    def do_skip(self):
+        """
+        Returns whether the test should be skipped.
+        
+        Returns
+        -------
+        do_skip : `bool`
+        """
+        wrapper = self.wrapper
+        if wrapper is None:
+            return False
+        
+        return wrapper.do_skip()
     
-    for key, value in dict_.items():
-        hash_value ^= try_hash_method(key) & try_hash_method(value)
     
-    return hash_value
-
-
-def hash_set(set_):
-    """
-    Returns the hash value of the given set.
+    def do_reverse(self):
+        """
+        Returns whether the test's result should be reversed.
+        
+        Returns
+        -------
+        do_reverse : `bool`
+        """
+        wrapper = self.wrapper
+        if wrapper is None:
+            return False
+        
+        return wrapper.do_reverse()
     
-    Parameters
-    ----------
-    set_ : `set` of `Any`
-        The set to hash.
     
-    Returns
-    -------
-    hash_value : `int`
-    """
-    hash_value = len(set_) << 16
-    for element in set_:
-        hash_value ^= try_hash_method(element)
+    def check_conflicts(self):
+        """
+        Checks the test case's wrappers' conflicts.
+        
+        Returns
+        ------
+        wrapper_conflict: `None`, ``WrapperConflict``
+        """
+        wrapper = self.wrapper
+        if (wrapper is not None):
+            return wrapper.check_conflicts()
     
-    return hash_value
-
-
-def maybe_merge_iterables(iterable_1, iterable_2):
-    """
-    Merges the two maybe iterable if applicable returning a new one.
     
-    Parameters
-    ----------
-    iterable_1 : `None`, `iterable`
-        Iterable to merge.
-    iterable_2 : `None`, `iterable`
-        Iterable to merge.
-    
-    Returns
-    -------
-    merged : `None`, `list`
-    """
-    if (iterable_1 is not None) and (not iterable_1):
-        iterable_1 = None
+    def iter_invoke(self, environment_manager):
+        """
+        Invokes the test case yielding the results of it.
+        
+        This method is an iterable generator.
+        
+        Parameters
+        ----------
+        environment_manager : ``EnvironmentManager``
+            Testing environment manager.
+        
+        Yields
+        -------
+        result : ``Result``
+        """
+        conflict = self.check_conflicts()
+        if (conflict is not None):
+            yield Result(self).with_conflict(conflict)
+            return
+        
+        if self.do_skip():
+            yield Result(self).as_skipped()
+            return
+        
+        handles = [*self._iter_handles()]
+        for handle, index in zip(handles, reversed(range(len(handles)))):
+            result = handle.invoke(environment_manager)
+            if index:
+                result = result.as_continuous()
+            yield result
     
-    if (iterable_2 is not None) and (not iterable_2):
-        iterable_2 = None
     
-    if iterable_1 is None:
-        if iterable_2 is None:
-            merged = None
+    def _iter_handles(self):
+        """
+        Iterates over the test handles of the test case.
+        
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        handle : ``Handle``
+        """
+        wrapper = self.wrapper
+        if (wrapper is None):
+            wrapper_groups = None
+            environments = None
+        
         else:
-            merged = [*iterable_2]
-    else:
-        if iterable_2 is None:
-            merged = [*iterable_1]
+            wrapper_groups = set()
+            
+            environment_wrappers = [*wrapper.iter_environments()]
+            if environment_wrappers:
+                environments = tuple(environment_wrappers)
+            else:
+                environments = None
+            
+            wrappers = [wrapper for wrapper in wrapper.iter_wrappers() if not wrapper.is_ignored_when_testing()]
+            
+            while wrappers:
+                wrapper_to_check = wrappers.pop()
+                wrapper_group = [wrapper_to_check]
+                
+                for wrapper in wrappers:
+                    if wrapper.is_mutually_exclusive_with(wrapper_to_check):
+                        continue
+                    
+                    if wrapper_to_check.is_mutually_exclusive_with(wrapper):
+                        continue
+                    
+                    wrapper_group.append(wrapper_to_check)
+                    continue
+                
+                wrapper_group = frozenset(wrapper_group)
+                wrapper_groups.add(wrapper_group)
+            
+            if not wrapper_groups:
+                wrapper_groups = None
+        
+        test = self.test
+        
+        if (wrapper_groups is None):
+            yield Handle(self, test, None, environments)
+        
         else:
-            merged = [*iterable_1, *iterable_2]
-    
-    return merged
-
-
-def maybe_merge_mappings(mapping_1, mapping_2):
-    """
-    Merges the two maybe mapping if applicable returning a new one.
-    
-    Parameters
-    ----------
-    mapping_1 : `None`, `mapping`
-        Mapping to merge.
-    mapping_2 : `None`, `mapping`
-        Mapping to merge.
-    
-    Returns
-    -------
-    merged : `None`, `dict`
-    """
-    if (mapping_1 is not None) and (not mapping_1):
-        mapping_1 = None
+            for wrapper_group in wrapper_groups:
+                if (wrapper_group is not None):
+                    wrapper_group = tuple(wrapper_group)
+                
+                yield Handle(self, test, wrapper_group, environments)
     
-    if (mapping_2 is not None) and (not mapping_2):
-        mapping_2 = None
     
-    if mapping_1 is None:
-        if mapping_2 is None:
-            merged = None
-        else:
-            merged = {**mapping_2}
-    else:
-        if mapping_2 is None:
-            merged = {**mapping_1}
-        else:
-            merged = {**mapping_1, **mapping_2}
+    def get_test_file(self):
+        """
+        Returns the test file of the case.
+        
+        Returns
+        -------
+        test_file : `None`, ``TestFile``
+        """
+        test_file_reference = self._test_file_reference
+        if (test_file_reference is not None):
+            return test_file_reference()
     
-    return merged
-
-
-def try_match_exception(expected_exceptions, received_exception, accept_subtypes):
-    """
-    Checks whether the received exception matches the preset ones.
     
-    Parameters
-    ----------
-    expected_exceptions : `set` of `BaseException`
-        The expected exceptions.
-    received_exception : `BaseException`
-        The received exception.
-    accept_subtypes : `bool`
-        Whether sub classes are allowed.
-    
-    Returns
-    -------
-    exception_matched : `bool`
-    """
-    for expected_exception in expected_exceptions:
-        if isinstance(expected_exception, type):
-            exception_type = expected_exception
-            exception_value = None
+    @property
+    def import_route(self):
+        """
+        Returns the import route from the base path to import the file from.
         
+        Returns
+        -------
+        import_route : `str`
+        """
+        test_file = self.get_test_file()
+        if (test_file is None):
+            import_route = ''
         else:
-            exception_type = type(expected_exception)
-            exception_value = expected_exception
+            import_route = test_file.import_route
         
+        return import_route
+    
+    
+    def is_last(self):
+        """
+        Returns whether self is the last test case of the file.
         
-        if accept_subtypes:
-            if not isinstance(received_exception, exception_type):
-                continue
+        Returns
+        -------
+        is_last : `bool`
+        """
+        test_file = self.get_test_file()
+        if (test_file is None):
+            return True
         
-        else:
-            if type(received_exception) is not exception_type:
-                continue
+        test_cases = test_file._test_cases
+        if test_cases is None:
+            return True
         
-        if (exception_value is not None) and (exception_value.args != received_exception.args):
-            continue
+        if self is test_cases[-1]:
+            return True
         
-        exception_matched = True
-        break
-    
-    else:
-        exception_matched = False
-    
-    return exception_matched
+        return False
```

### Comparing `vampytest-0.0.7/vampytest/core/run_state.py` & `vampytest-0.0.8/vampytest/core/runner/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,323 +1,405 @@
-__all__ = ('RunState',)
+__all__ = ('RunnerContext',)
 
 from scarletio import RichAttributeErrorBaseType
 
 
-class RunState(RichAttributeErrorBaseType):
+class RunnerContext(RichAttributeErrorBaseType):
     """
-    Represents a test runner's run state.
+    Represents a test's context. Test contexts are present while running a test.
     
     Attributes
     ----------
-    _load_failures : `None`, `list` of ``TestFileLoadFailure``
-        Load failures.
-    _loaded_test_files : `None`, `list` of ``TestFile``
-        The test files which have been successfully loaded.
-    _result_groups : `None`, `list` of ``ResultGroup``
-        The ran tests' results.
-    _test_files : `None`, `list` of ``TestFile``
+    _registered_files : `None`, `list` of ``TestFile``
         The collected test files.
+    runner : ``TestRunner``
+        The respective test runner running tests.
+    
+    Utility Methods
+    ---------------
+    - Count getters
+    
+        - ``.get_registered_file_count``
+        - ``.get_test_case_count``
+        - ``.get_ran_test_count``
+        - ``.get_passed_test_count``
+        - ``.get_skipped_test_count``
+        - ``.get_failed_test_count``
+        - ``.get_load_failed_file_count``
+        - ``.get_load_succeeded_file_count``
+    
+    - Iterators
+    
+        - ``.iter_registered_files``
+        - ``.iter_results``
+        - ``.iter_passed_results``
+        - ``.iter_skipped_results``
+        - ``.iter_failed_results``
+        - ``.iter_load_failed_files``
+        - ``.iter_load_succeeded_files``
+        - ``.iter_file_load_failures``
+    
+    - Getters
+    
+        - ``.get_registered_files``
+        - ``.get_failed_to_load``
+        - ``.get_file_load_failures``
+        - ``.get_skipped_results``
+        - ``.get_failed_results``
+        - ``.get_load_failed_file_count``
+    
+    - Internal
+    
+        - ``.register_file``
     """
-    __slots__ = ('_load_failures', '_loaded_test_files', '_result_groups', '_test_files',)
+    __slots__ = ('_registered_files', 'file_system_entry', 'runner',)
     
-    def __new__(cls):
+    def __new__(cls, runner, file_system_entry):
         """
-        Creates a new run state.
+        Creates a new runner context.
+        
+        Parameters
+        ----------
+        file_system_entry : ``FileSystemEntry`
+            The file system entry built with the test runner's settings.
+        runner : ``TestRunner``
+            The respective test runner running tests.
         """
         self = object.__new__(cls)
-        self._load_failures = None
-        self._loaded_test_files = None
-        self._result_groups = None
-        self._test_files = None
+        self._registered_files = None
+        self.file_system_entry = file_system_entry
+        self.runner = runner
         return self
     
-    # generic interaction methods
     
-    def get_load_failure_count(self):
+    def get_registered_file_count(self):
         """
-        Returns how much much tests files were collected.
+        Returns how much much registered files were collected.
         """
-        load_failures = self._load_failures
-        if (load_failures is None):
-            load_failure_count = 0
-        else:
-            load_failure_count = len(load_failures)
+        registered_file_count = 0
         
-        return load_failure_count
+        for registered_file in self.iter_registered_files():
+            registered_file_count += registered_file.get_test_file_count()
+        
+        return registered_file_count
     
     
-    def iter_load_failures(self):
+    def iter_registered_files_shallow(self):
         """
-        Iterates over the load failures.
+        Shallow iterates over the registered files.
         
         This method is an iterable generator.
         
         Yields
         ------
-        load_failure : ``TestFileLoadFailure``
+        registered_file : ``TestFile``
         """
-        load_failures = self._load_failures
-        if (load_failures is not None):
-            yield from load_failures
+        registered_files = self._registered_files
+        if (registered_files is not None):
+            yield from registered_files
     
     
-    def get_load_failures(self):
+    def iter_registered_files(self):
         """
-        Returns a copy of the load failures.
+        Iterates over the registered files.
+        
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        registered_file : ``TestFile``
+        """
+        registered_files = self._registered_files
+        if (registered_files is not None):
+            for registered_file in registered_files:
+                yield from registered_file.iter_test_files()
+    
+    
+    def get_registered_files(self):
+        """
+        Returns a copy of the registered files.
         
         Returns
         -------
-        load_failures : `list` of ``TestFileLoadFailure``
+        registered_files : `list` of ``TestFile``
         """
-        load_failures = self._load_failures
-        if load_failures is None:
-            load_failures = []
-        else:
-            load_failures = load_failures.copy()
-        
-        return load_failures
+        return [*self.iter_registered_files()]
     
     
-    def add_load_failure(self, load_failure):
+    def register_file(self, registered_file):
         """
-        Adds a new load failure.
+        Adds a new registered file.
         
         Parameters
         ----------
-        load_failure : ``TestFileLoadFailure``
+        registered_file : ``TestFile``
         """
-        load_failures = self._load_failures
-        if load_failures is None:
-            load_failures = []
-            self._load_failures = load_failures
+        registered_files = self._registered_files
+        if registered_files is None:
+            registered_files = []
+            self._registered_files = registered_files
         
-        load_failures.append(load_failure)
+        registered_files.append(registered_file)
     
     
-
-    def get_loaded_test_file_count(self):
+    def get_test_case_count(self):
+        """
+        Returns how much test cases are in the test files collected.
+        
+        Returns
+        -------
+        test_case_count : `int`
         """
-        Returns how much much loaded tests files were collected.
+        return sum(test_file.get_test_case_count() for test_file in self.iter_registered_files())
+    
+    
+    def get_ran_test_count(self):
         """
-        loaded_test_files = self._loaded_test_files
-        if (loaded_test_files is None):
-            loaded_test_file_count = 0
-        else:
-            loaded_test_file_count = len(loaded_test_files)
+        Returns how much tests already ran.
         
-        return loaded_test_file_count
+        Returns
+        -------
+        ran_test_count : `int`
+        """
+        return sum(test_file.get_ran_test_count() for test_file in self.iter_registered_files())
     
     
-    def iter_loaded_test_files(self):
+    def iter_results(self):
         """
-        Iterates over the loaded  test files.
+        Iterates over the results.
         
         This method is an iterable generator.
         
         Yields
         ------
-        loaded_test_files : ``TestFile``
+        result : ``Result``
         """
-        loaded_test_files = self._loaded_test_files
-        if (loaded_test_files is not None):
-            yield from loaded_test_files
+        for test_file in self.iter_registered_files():
+            yield from test_file.iter_results()
     
     
-    def get_loaded_test_files(self):
+    def iter_passed_results(self):
         """
-        Returns a copy of the loaded test files.
+        Iterates over the passed results of the runner context.
         
-        Returns
-        -------
-        loaded_test_files : `list` of ``TestFile``
-        """
-        loaded_test_files = self._loaded_test_files
-        if loaded_test_files is None:
-            loaded_test_files = []
-        else:
-            loaded_test_files = loaded_test_files.copy()
+        This method is an iterable generator.
         
-        return loaded_test_files
+        Yields
+        ------
+        result : ``Result``
+        """
+        for test_file in self.iter_registered_files():
+            if not test_file.is_directory():
+                yield from test_file.iter_passed_results()
     
     
-    def add_loaded_test_files(self, loaded_test_file):
+    def iter_skipped_results(self):
         """
-        Adds a new loaded test file.
+        Iterates over the skipped results of the runner context.
         
-        Parameters
-        ----------
-        loaded_test_file : ``TestFile``
-        """
-        loaded_test_files = self._loaded_test_files
-        if loaded_test_files is None:
-            loaded_test_files = []
-            self._loaded_test_files = loaded_test_files
+        This method is an iterable generator.
         
-        loaded_test_files.append(loaded_test_file)
-    
-
-    def get_result_group_count(self):
+        Yields
+        ------
+        result : ``Result``
         """
-        Returns how much much tests files were collected.
+        for test_file in self.iter_registered_files():
+            if not test_file.is_directory():
+                yield from test_file.iter_skipped_results()
+    
+    
+    def iter_failed_results(self):
         """
-        result_groups = self._result_groups
-        if (result_groups is None):
-            result_group_count = 0
-        else:
-            result_group_count = len(result_groups)
+        Iterates over the failed results of the runner context.
         
-        return result_group_count
+        This method is an iterable generator.
+        
+        Yields
+        ------
+        result : ``Result``
+        """
+        for test_file in self.iter_registered_files():
+            if not test_file.is_directory():
+                yield from test_file.iter_failed_results()
     
     
-    def iter_result_groups(self):
+    def iter_informal_results(self):
         """
-        Iterates over the result groups.
+        Iterates over the informal only results of the runner context.
         
         This method is an iterable generator.
         
         Yields
         ------
-        result_group : ``ResultGroup``
+        result : ``Result``
         """
-        result_groups = self._result_groups
-        if (result_groups is not None):
-            yield from result_groups
+        for test_file in self.iter_registered_files():
+            if not test_file.is_directory():
+                yield from test_file.iter_informal_results()
     
     
-    def get_result_groups(self):
+    def get_passed_test_count(self):
         """
-        Returns a copy of the result groups.
+        Returns how much test passed.
         
         Returns
         -------
-        result_groups : `list` of ``ResultGroup``
+        passed_test_count : `int`
         """
-        result_groups = self._result_groups
-        if result_groups is None:
-            result_groups = []
-        else:
-            result_groups = result_groups.copy()
-        
-        return result_groups
+        return sum(
+            test_file.get_passed_test_count()
+            for test_file in self.iter_registered_files()
+            if not test_file.is_directory()
+        )
     
     
-    def add_result_group(self, result_group):
+    def get_skipped_test_count(self):
         """
-        Adds a new result group.
+        Returns how much test was skipped.
         
-        Parameters
-        ----------
-        result_group : ``ResultGroup``
+        Returns
+        -------
+        passed_test_count : `int`
         """
-        result_groups = self._result_groups
-        if result_groups is None:
-            result_groups = []
-            self._result_groups = result_groups
-        
-        result_groups.append(result_group)
+        return sum(
+            test_file.get_skipped_test_count()
+            for test_file in self.iter_registered_files()
+            if not test_file.is_directory()
+        )
     
     
-    def get_test_file_count(self):
+    def get_failed_test_count(self):
         """
-        Returns how much much tests files were collected.
-        """
-        test_files = self._test_files
-        if (test_files is None):
-            test_file_count = 0
-        else:
-            test_file_count = len(test_files)
+        Returns how much test failed.
         
-        return test_file_count
+        Returns
+        -------
+        passed_test_count : `int`
+        """
+        return sum(
+            test_file.get_failed_test_count()
+            for test_file in self.iter_registered_files()
+            if not test_file.is_directory()
+        )
     
     
-    def iter_test_files(self):
+    def get_passed_results(self):
         """
-        Iterates over the test files.
+        Iterates over the passed results of the runner context.
         
-        This method is an iterable generator.
-        
-        Yields
-        ------
-        test_file : ``TestFile``
+        Returns
+        -------
+        results : `list` of ``Result``
         """
-        test_files = self._test_files
-        if (test_files is not None):
-            yield from test_files
+        return [*self.iter_passed_results()]
     
     
-    def get_test_files(self):
+    def get_skipped_results(self):
         """
-        Returns a copy of the test files.
+        Iterates over the skipped results of the runner context.
         
         Returns
         -------
-        test_files : `list` of ``TestFile``
+        results : `list` of ``Result``
         """
-        test_files = self._test_files
-        if test_files is None:
-            test_files = []
-        else:
-            test_files = test_files.copy()
+        return [*self.iter_skipped_results()]
+    
+    
+    def get_failed_results(self):
+        """
+        Iterates over the failed results of the runner context.
         
-        return test_files
+        Returns
+        -------
+        results : `list` of ``Result``
+        """
+        return [*self.iter_failed_results()]
     
     
-    def add_test_file(self, test_file):
+    def get_load_failed_file_count(self):
         """
-        Adds a new test file.
+        Returns how much files failed to load.
         
-        Parameters
-        ----------
-        test_file : ``TestFile``
+        Returns
+        -------
+        load_failed_file_count : `bool`
         """
-        test_files = self._test_files
-        if test_files is None:
-            test_files = []
-            self._test_files = test_files
+        return sum(test_file.is_loaded_with_failure() for test_file in self.iter_registered_files())
+    
+    
+    def get_load_succeeded_file_count(self):
+        """
+        Returns how much files failed to load.
         
-        test_files.append(test_file)
+        Returns
+        -------
+        load_succeeded_file_count : `bool`
+        """
+        return sum(test_file.is_loaded_with_success() for test_file in self.iter_registered_files())
     
-    # Added features
     
-    def __repr__(self):
-        """Returns the run state's representation."""
-        repr_parts = ['<', self.__class__.__name__]
+    def get_not_loaded_file_count(self):
+        """
+        Returns how much file was not loaded.
         
-        repr_parts.append(' loaded_test_files: ')
-        repr_parts.append(repr(self.get_loaded_test_file_count()))
-        repr_parts.append(' / ')
-        repr_parts.append(repr(self.get_test_file_count()))
+        Returns
+        -------
+        not_loaded_file_count : `bool`
+        """
+        return sum((not test_file.is_loaded()) for test_file in self.iter_registered_files())
+    
+    
+    def iter_load_failed_files(self):
+        """
+        Iterates over the files which failed to load.
         
-        repr_parts.append(' tests_ran: ')
-        repr_parts.append(repr(self.get_result_group_count()))
+        This method is an iterable generator.
         
-        repr_parts.append('>')
-        return ''.join(repr_parts)
+        Yields
+        -------
+        test_file : ``TestFile``
+        """
+        for test_file in self.iter_registered_files():
+            if test_file.is_loaded_with_failure():
+                yield test_file
     
     
-    def get_total_registered_test_count(self):
+    def iter_load_succeeded_files(self):
         """
-        Returns how much tests were registered by the loaded test files.
+        Iterates over the files which succeeded to load.
         
-        Returns
+        This method is an iterable generator.
+        
+        Yields
         -------
-        total_registered_test_count : `int`
+        test_file : ``TestFile``
+        """
+        for test_file in self.iter_registered_files():
+            if test_file.is_loaded_with_success():
+                yield test_file
+    
+    
+    def iter_file_load_failures(self):
         """
-        total_registered_test_count = 0
+        Iterates over the file load failures.
         
-        for test_file in self.iter_loaded_test_files():
-            total_registered_test_count += test_file.get_test_count()
+        This method is an iterable generator.
         
-        return total_registered_test_count
+        Yields
+        -------
+        load_failure : ``TestFileLoadFailure``
+        """
+        for test_file in self.iter_registered_files():
+            load_failure = test_file.get_load_failure()
+            if (load_failure is not None):
+                yield load_failure
     
     
-    def iter_test_cases(self):
+    def get_file_load_failures(self):
         """
-        Iterates over the test cases.
+        Returns the file load failures.
         
-        Yields
-        ------
-        test_case : ``TestCase``
+        Returns
+        -------
+        load_failures : `list` of ``TestFileLoadFailure``
         """
-        for test_file in self.iter_test_files():
-            yield from test_file.iter_tests()
+        return [*self.iter_file_load_failures()]
```

### Comparing `vampytest-0.0.7/vampytest/core/runner/runner.py` & `vampytest-0.0.8/vampytest/core/runner/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     - ``.stop``
     - ``.add_teardown_callback``
     """
     __slots__ = (
         '_base_path', '_path_parts', '_stopped', '_teardown_callbacks', 'environment_manager', 'event_handler_manager'
     )
     
-    def __new__(cls, base_path, path_parts=None, *, environment_manager=None, event_handler_manager=None):
+    def __new__(cls, base_path, path_parts = None, *, environment_manager = None, event_handler_manager = None):
         """
         Parameters
         ----------
         base_path : `str`
             The path to run tests from.
         path_parts : `None`, `list` of `str` = `None`, Optional
             Added path parts to specify from which which directory we want to collect the tests from.
@@ -284,16 +284,16 @@
                         test_file.try_load_test_cases()
                         
                         yield FileLoadDoneEvent(context, test_file)
                         
                         # Run test file if loaded successfully
                         if test_file.is_loaded_with_success():
                             
-                            for result_group in test_file.iter_invoke_test_cases(self.environment_manager):
-                                yield TestDoneEvent(context, result_group)
+                            for result in test_file.iter_invoke_test_cases(self.environment_manager):
+                                yield TestDoneEvent(context, result)
                             
                             yield FileTestingDoneEvent(context, test_file)
             
             yield TestingEndEvent(context)
         
         finally:
             self._teardown()
```

### Comparing `vampytest-0.0.7/vampytest/core/test_case.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,286 +1,305 @@
-__all__ = ('TestCase', )
+__all__ = ('WrapperBase', )
 
-import reprlib
+from scarletio import RichAttributeErrorBaseType, include
 
-from scarletio import RichAttributeErrorBaseType, WeakReferer
+from ..helpers.hashing import hash_object
 
-from .handle import Handle
-from .helpers import hash_object
-from .result import ResultGroup
-from .wrappers import WrapperBase
 
+WrapperChainer = include('WrapperChainer')
 
-class TestCase(RichAttributeErrorBaseType):
+
+class WrapperBase(RichAttributeErrorBaseType):
     """
-    Represents a test.
+    Base class for test wrappers defining shared functionality.
     
     Attributes
     ----------
-    _test_file_reference : `None`, ``WeakReferer`` to ``TestFile``
-        The parent test file of the case.
-    name : `str`
-        The test's name.
-    test : `callable`, ``WrapperBase``
-        The test itself, or the wrapped test.
-    wrapper : `None`, ``WrapperBase``
-        Wrappers containing the test if any.    
+    wrapped : `None`, `object`
+        The wrapped test.
     """
-    __slots__ = ('_test_file_reference', 'name', 'test', 'wrapper')
+    __slots__ = ('wrapped', )
+    
+    def __new__(cls):
+        """
+        Creates a new test wrapper.
+        """
+        self = object.__new__(cls)
+        self.wrapped = None
+        return self
     
-    def __new__(cls, test_file, name, test):
+    
+    def __call__(self, to_wrap):
         """
-        Creates a new test case.
+        Calls the wrapper.
         
         Parameters
         ----------
-        test_file : ``TestFile``
-            The parent test file.
-        name : `str`
-            The test's name.
-        test : `callable`, ``WrapperBase``
-            The test itself, or the wrapped test.
-        """
-        if isinstance(test, WrapperBase):
-            wrapper = test
-            test = test.unbind_test()
-        else:
-            wrapper = None
-            test = test
+        to_wrap : `object`
+            The object to wrap. It can be either a function or an another wrapper.
         
-        self = object.__new__(cls)
-        self._test_file_reference = WeakReferer(test_file)
-        self.name = name
-        self.test = test
-        self.wrapper = wrapper
+        Returns
+        -------
+        to_wrap : ``WrapperBase``
+            The same or a newly created wrapper.
+        
+        Raises
+        ------
+        RuntimeError
+            Wrapper already called.
+        """
+        if to_wrap is None:
+            raise RuntimeError(f'Cannot wrap `None`; self={self!r}.')
+        
+        
+        wrapped = self.wrapped
+        
+        if isinstance(to_wrap, WrapperBase):
+            
+            if (wrapped is not None) and (to_wrap.wrapped is not None):
+                raise RuntimeError(
+                    f'Both self and other wrappers are already wrapped; self = {self!r}; other = {to_wrap!r}.'
+                )
+            
+            if isinstance(to_wrap, WrapperChainer):
+                to_wrap.append(self)
+                
+                if (wrapped is not None):
+                    to_wrap(wrapped)
+                
+                return to_wrap
+            
+            if wrapped is None:
+                wrapped = to_wrap.wrapped
+            
+            wrapper_chainer = WrapperChainer(wrapped)
+            wrapper_chainer.append(self)
+            wrapper_chainer.append(to_wrap)
+            return wrapper_chainer
+        
+        
+        if (wrapped is not None):
+            raise RuntimeError(f'Wrapped already wrapped; self = {self!r}, to_wrap = {to_wrap!r}.')
+        
+        self.wrapped = to_wrap
         return self
     
     
-    def __eq__(self, other):
-        """Returns whether the two test cases are equal."""
-        if type(self) is not type(other):
-            return NotImplemented
-        
-        return False
+    def __matmul__(self, other):
+        """Returns `self(other)`"""
+        return self.__call__(other)
     
     
-    def __hash__(self):
-        """Returns the test case's hash value."""
-        hash_value = 0
-        
-        hash_value ^= hash(self.name)
-        hash_value ^= hash_object(self.test)
-        
-        wrapper = self.wrapper
-        if (wrapper is not None):
-            hash_value ^= hash(wrapper)
+    def __rmatmul__(self, other):
+        """Returns `self(other)`"""
+        return self.__call__(other)
         
-        return hash_value
-    
     
-    def __repr__(self):
-        """Returns the test case's representation."""
-        repr_parts = ['<', self.__class__.__name__]
+    def _cursed_repr_builder(self):
+        """
+        Representation builder helper.
         
-        repr_parts.append(' name=')
-        repr_parts.append(repr(self.name))
+        This method is a generator.
         
-        repr_parts.append(', test=')
-        repr_parts.append(reprlib.repr(self.test))
+        Examples
+        --------
+        ```
+        for field_added, repr_parts in self._cursed_repr_builder():
+            if not field_added:
+                repr_parts.append(',')
+            
+            repr_parts.append(' oh no')
         
-        wrapper = self.wrapper
-        if (wrapper is not None):
-            repr_parts.append(', wrapper=')
-            repr_parts.append(repr(self.wrapper))
+        return ''.join(repr_parts)
+        ```
+        """
+        repr_parts = ['<', self.__class__.__name__]
         
-        if self.do_skip():
-            repr_parts.append(', skipped')
+        wrapped = self.wrapped
+        if (wrapped is None):
+            repr_parts.append(' wrapped = ')
+            repr_parts.append(repr(wrapped))
+            
+            field_added = True
+        else:
+            field_added = False
         
-        if self.do_revert():
-            repr_parts.append(', reverted')
+        yield field_added, repr_parts
         
         repr_parts.append('>')
         return ''.join(repr_parts)
     
     
+    def __repr__(self):
+        """Returns the wrapper's representation."""
+        for field_added, repr_parts in self._cursed_repr_builder():
+            pass
+        
+        return ''.join(repr_parts)
+    
+    
+    def __hash__(self):
+        """Returns the wrapper's representation."""
+        wrapped = self.wrapped
+        if wrapped is None:
+            hash_value = 0
+        else:
+            hash_value = hash_object(wrapped)
+        
+        return hash_value
+    
+    
+    def __eq__(self, other):
+        """return whether the two wrappers are equal."""
+        if type(self) is not type(other):
+            return NotImplemented
+        
+        if self.wrapped != other.wrapped:
+            return False
+        
+        return True
+    
+    
     def do_skip(self):
         """
-        Returns whether the test should be skipped.
+        Whether the test should be skipped.
         
         Returns
         -------
         do_skip : `bool`
         """
-        wrapper = self.wrapper
-        if wrapper is None:
-            return False
-        
-        return wrapper.do_skip()
+        return False
     
     
-    def do_revert(self):
+    def do_reverse(self):
         """
-        Returns whether the test's result should be reverted.
+        Tests whether the test's result should be reversed.
         
         Returns
         -------
-        do_revert : `bool`
+        do_reverse : `bool`
         """
-        wrapper = self.wrapper
-        if wrapper is None:
-            return False
-        
-        return wrapper.do_revert()
+        return False
     
     
     def check_conflicts(self):
         """
-        Checks the test case's wrappers' conflicts.
+        Checks whether the wrapper has internal conflict.
         
         Returns
         ------
         wrapper_conflict: `None`, ``WrapperConflict``
         """
-        wrapper = self.wrapper
-        if (wrapper is not None):
-            return wrapper.check_conflicts()
+        pass
     
     
-    def invoke(self, environment_manager):
+    def check_conflict_with(self, other):
         """
-        Invokes the test case.
+        Checks whether the wrapper has conflict with the other one.
         
-        Parameters
-        ----------
-        environment_manager : ``EnvironmentManager``
-            Testing environment manager.
+        Returns
+        ------
+        wrapper_conflict: `None`, ``WrapperConflict``
+        """
+        pass
+    
+    
+    def has_bound_test(self):
+        """
+        Returns whether the wrapper wraps a test.
         
         Returns
         -------
-        test_result : ``Result``
+        has_bound_test : `bool`
         """
-        test_result_group = ResultGroup(self)
-        conflict = self.check_conflicts()
-        if (conflict is not None):
-            return test_result_group.with_conflict(conflict)
+        return (self.wrapped is not None)
+    
+    
+    def unbind_test(self):
+        """
+        Unbinds the wrappers test.
         
-        if self.do_skip():
-            return test_result_group.as_skipped()
+        Returns
+        -------
+        test : `object`
         
-        for handler in self._iter_handles():
-            test_result = handler.invoke(environment_manager)
-            test_result_group = test_result_group.with_result(test_result)
+        Raises
+        ------
+        RuntimeError
+            The wrapper had no test or already unbind.
+        """
+        wrapped = self.wrapped
+        if wrapped is None:
+            raise RuntimeError(f'The wrapper had no test or already unbind; self = {self!r}.')
         
-        return test_result_group
+        self.wrapped = None
+        return wrapped
     
     
-    def _iter_handles(self):
+    def iter_wrappers(self):
         """
-        Iterates over the test handles of the test case.
+        Iterates over the wrappers encapsulated by this wrapper. This method is used to un-nest wrapper groups if
+        required.
         
         This method is an iterable generator.
         
         Yields
         ------
-        handle : ``Handle``
+        wrapper : ``WrapperBase``
         """
-        wrapper = self.wrapper
-        if (wrapper is None):
-            wrapper_groups = None
-            environments = None
-        
-        else:
-            wrapper_groups = set()
-            
-            environment_wrappers = [*wrapper.iter_environments()]
-            if environment_wrappers:
-                environments = tuple(environment_wrappers)
-            else:
-                environments = None
-            
-            wrappers = [wrapper for wrapper in wrapper.iter_wrappers() if not wrapper.is_ignored_when_testing()]
-            
-            while wrappers:
-                wrapper_to_check = wrappers.pop()
-                wrapper_group = [wrapper_to_check]
-                
-                for wrapper in wrappers:
-                    if wrapper.is_mutually_exclusive_with(wrapper_to_check):
-                        continue
-                    
-                    if wrapper_to_check.is_mutually_exclusive_with(wrapper):
-                        continue
-                    
-                    wrapper_group.append(wrapper_to_check)
-                    continue
-                
-                wrapper_group = frozenset(wrapper_group)
-                wrapper_groups.add(wrapper_group)
-            
-            if not wrapper_groups:
-                wrapper_groups = None
-        
-        test = self.test
-        
-        if (wrapper_groups is None):
-            yield Handle(self, test, None, environments)
-        
-        else:
-            for wrapper_group in wrapper_groups:
-                if (wrapper_group is not None):
-                    wrapper_group = tuple(wrapper_group)
-                
-                yield Handle(self, test, wrapper_group, environments)
+        yield self
     
     
-    def get_test_file(self):
+    def is_ignored_when_testing(self):
         """
-        Returns the test file of the case.
+        Returns whether the wrapper can be ignore when testing, but is used instead for just pre-checks.
         
         Returns
         -------
-        test_file : `None`, ``TestFile``
+        is_ignored_when_testing : `bool`
         """
-        test_file_reference = self._test_file_reference
-        if (test_file_reference is not None):
-            return test_file_reference()
+        return True
     
     
-    @property
-    def import_route(self):
+    def is_mutually_exclusive_with(self, other):
         """
-        Returns the import route from the base path to import the file from.
+        Returns whether the wrapper is mutually exclusive with the other one.
+        
+        Parameters
+        ----------
+        other : ``WrapperBase``
         
         Returns
         -------
-        import_route : `str`
+        is_mutually_exclusive_with : `bool`
         """
-        test_file = self.get_test_file()
-        if (test_file is None):
-            import_route = ''
-        else:
-            import_route = test_file.import_route
-        
-        return import_route
+        return False
     
     
-    def is_last(self):
+    def get_context(self, handle):
         """
-        Returns whether self is the last test case of the file.
+        Returns a context over a test handle.
+        
+        Parameters
+        ----------
+        handle : ``Handle``
+            Test handle.
         
         Returns
         -------
-        is_last : `bool`
+        context : ``ContextBase``
+        """
+        return None
+    
+    
+    def iter_environments(self):
         """
-        test_file = self.get_test_file()
-        if (test_file is None):
-            return True
-        
-        test_cases = test_file._test_cases
-        if test_cases is None:
-            return True
+        Iterates over the environments registered to the wrapper.
         
-        if self is test_cases[-1]:
-            return True
+        This method is an iterable generator.
         
-        return False
-
+        Yields
+        ------
+        environment : ``DefaultEnvironment``
+        """
+        return
+        yield
```

### Comparing `vampytest-0.0.7/vampytest/core/utils.py` & `vampytest-0.0.8/vampytest/core/helpers/path_repr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ('get_short_path_repr',)
+__all__ = ()
 
 from os.path import sep as PATH_SEPARATOR
 
 
 PATH_REPR_MAX_PARTS = 4
 PATH_REPR_PART_PLACEHOLDER = '.'
 PATH_REPR_MAX_LENGTH = 80
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/__init__.py` & `vampytest-0.0.8/vampytest/core/wrappers/aliases.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,39 @@
-"""
-Test assertions
-
-Examples
---------
-```
-import vampytest
-
-
-@vampytest.call_with('cake', 'cake')
-def test_is_equal(p1, p2):
-    vampytest.assert_equals(p1, p2)
-
-
-@vampytest.returning('cake')
-def test_returning_cake():
-    return 'cake'
-```
-"""
-
-from .wrapper_base import *
-from .wrapper_call import *
-from .wrapper_chainer import *
-from .wrapper_conflict import *
-from .wrapper_environment import *
-from .wrapper_garbage_collect import *
-from .wrapper_revert import *
-from .wrapper_skip import *
-from .wrapper_skip_conditional import *
-
-
-returning = WrapperCall.returning_constructor
-raising = WrapperCall.raising_constructor
-call_with = WrapperCall.call_with_constructor
-
-from .wrapper_environment import WrapperEnvironment as in_environment
-from .wrapper_garbage_collect import WrapperGarbageCollect as with_gc
-from .wrapper_revert import WrapperRevert as revert
-from .wrapper_skip import WrapperSkip as skip
-from .wrapper_skip_conditional import WrapperSkipConditional as skip_if
-
-
 __all__ = (
-    'call_with',
-    'in_environment',
-    'raising',
-    'returning',
-    'revert',
-    'skip',
-    'skip_if',
+    'call_from', 'call_with', 'in_environment', 'raising', 'returning', 'reverse', 'revert', 'skip', 'skip_if',
     'with_gc',
-    
-    *wrapper_base.__all__,
-    *wrapper_call.__all__,
-    *wrapper_chainer.__all__,
-    *wrapper_conflict.__all__,
-    *wrapper_environment.__all__,
-    *wrapper_garbage_collect.__all__,
-    *wrapper_revert.__all__,
-    *wrapper_skip.__all__,
-    *wrapper_skip_conditional.__all__,
 )
+
+import warnings
+
+from .wrapper_call import WrapperCalling
+from .wrapper_call_from import WrapperCallingFrom
+from .wrapper_environment import WrapperEnvironment
+from .wrapper_garbage_collect import WrapperGarbageCollect
+from .wrapper_reverse import WrapperReverse
+from .wrapper_skip import WrapperSkip
+from .wrapper_skip_conditional import WrapperSkipConditional
+
+call_from = WrapperCallingFrom.calling_from_constructor
+call_with = WrapperCalling.call_with_constructor
+in_environment = WrapperEnvironment
+raising = WrapperCalling.raising_constructor
+returning = WrapperCalling.returning_constructor
+reverse = WrapperReverse
+skip = WrapperSkip
+skip_if = WrapperSkipConditional
+with_gc = WrapperGarbageCollect
+
+
+def revert(*pp, **kp):
+    """
+    Deprecated and will be removed in 2024 February. Please use ``reverse`` instead.
+    """
+    warnings.warn(
+        (
+            f'`revert` is deprecated and will be removed in 2024 February. '
+            f'Please use `.reverse` instead.'
+        ),
+        FutureWarning,
+        stacklevel = 2,
+    )
+    return reverse(*pp, **kp)
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_call.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,174 +1,176 @@
-__all__ = ('WrapperCall',)
+__all__ = ('WrapperCalling',)
 
 import reprlib
 
 from scarletio import copy_docs
 
+from ..contexts import ContextCalling
+from ..helpers.hashing import hash_dict, hash_set, hash_tuple, try_hash_method
+from ..helpers.un_nesting import un_nest_exceptions
 
-from ..assertions import AssertionException
-from ..helpers import hash_dict, hash_set, hash_tuple, try_hash_method, try_match_exception, un_nest_expected_exceptions
-from ..result import Result
-
-from .wrapper_conflict import WrapperConflict
 from .wrapper_base import WrapperBase
+from .wrapper_conflict import WrapperConflict
+
+
+MODE_RAISING = 1 << 0
+MODE_RETURNING = 1 << 2
+MODE_CALL_WITH = 1 << 3
 
 
-class WrapperCall(WrapperBase):
+class WrapperCalling(WrapperBase):
     """
     Combined wrapper supporting `call_with`, `returning` and `raising`.
     
     Attributes
     ----------
-    wrapped : `Any`
+    wrapped : `object`
         The wrapped test.
-    calling_keyword_parameters : `None`, `dict` of (`str`, `Any`) items
+    calling_keyword_parameters : `None`, `dict` of (`str`, `object`) items
         Keyword parameters to call the test with if ``.is_call_with``.
-    calling_positional_parameters : `None`, `tuple` of `Any`
+    calling_positional_parameters : `None`, `tuple` of `object`
         Positional parameter to call the test with if ``.is_call_with``.
-    is_raising : `bool`
-        Whether raised exceptions of the test should be checked.
-    is_returning : `bool`
-        Whether returned value of the test should be checked.
-    is_call_with : `bool`
-        Whether the test should be called with specific parameters.
+    mode : `int`
+        Bitwise flag containing the mode of calling and handling returns.
     raising_accept_subtypes : `bool`
         Whether exception subclasses are accepted as well if ``.is_raising``.
     raising_exceptions : `None`, `set` of ``BaseException``
-        The raising_exceptions expected to be raised if ``.is_raising``.
-    returning_value : `None`, `Any`
+        The raised exceptions to be expected to be raised if ``.is_raising``.
+    raising_where : `None`, `callable`
+        Additional check to check the raised exception if ``.is_raising`.
+    returning_value : `None`, `object`
         The expected returned value of the test if ``.is_returning``.
     """
     __slots__ = (
-        'calling_keyword_parameters', 'calling_positional_parameters', 'is_call_with', 'is_raising', 'is_returning',
-        'raising_exceptions', 'raising_accept_subtypes', 'returning_value'
+        'calling_keyword_parameters', 'calling_positional_parameters', 'mode', 'raising_exceptions',
+        'raising_accept_subtypes', 'raising_where', 'returning_value'
     )
     
-    def __new__(cls, wrapped=None, *, raising=None, returning=None, call_with=None):
+    def __new__(cls, wrapped = None, *, call_with = None, raising = None, returning = None):
         """
         Creates a new combined test wrapper.
         
         Parameters
         ----------
-        wrapped : `None`, `Any` = `None`, Optional
+        wrapped : `None`, `object` = `None`, Optional
             The wrapped test if any.
-        raising : `None`, `tuple` (`set` of ``BaseException``, `bool`) = `None`, Optional (Keyword only)
-            Whether the test is raising.
-        returning : `None`, `tuple` (`Any`) = `None`, Optional (Keyword only)
-            Whether the test is returning.
-        call_with : `None`, `tuple` (`tuple` of `Any`, `dict` of (`str`, `Any`) items) = `None`
+        call_with : `None`, `tuple` (`tuple` of `object`, `dict` of (`str`, `object`) items) = `None`
                 , Optional (Keyword only)
             Whether the test should be called with parameters.
+        raising : `None`, `tuple` (`set` of ``BaseException``, `bool`, (`None`, `callable`)) = `None` \
+                , Optional (Keyword only)
+            Whether the test is raising.
+        returning : `None`, `tuple` (`object`) = `None`, Optional (Keyword only)
+            Whether the test is returning.
         """
+        mode = 0
+        
         if raising is None:
-            is_raising = False
             raising_exceptions = None
             raising_accept_subtypes = None
+            raising_where = None
         
         else:
-            is_raising = True
-            raising_exceptions, raising_accept_subtypes = raising
+            mode |= MODE_RAISING
+            raising_exceptions, raising_accept_subtypes, raising_where = raising
         
         
         if returning is None:
-            is_returning = False
             returning_value = None
         
         else:
-            is_returning = True
-            returning_value = returning[0]
+            mode |= MODE_RETURNING
+            returning_value, = returning
         
         
         if call_with is None:
-            is_call_with = False
             calling_keyword_parameters = None
             calling_positional_parameters = None
         
         else:
-            is_call_with = True
+            mode |= MODE_CALL_WITH
             calling_positional_parameters, calling_keyword_parameters = call_with
         
         
         self = object.__new__(cls)
         self.wrapped = wrapped
         
-        self.raising_accept_subtypes = raising_accept_subtypes
-        self.raising_exceptions = raising_exceptions
-        self.is_raising = is_raising
-        self.is_returning = is_returning
-        self.is_call_with = is_call_with
         self.calling_keyword_parameters = calling_keyword_parameters
         self.calling_positional_parameters = calling_positional_parameters
+        self.mode = mode
+        self.raising_accept_subtypes = raising_accept_subtypes
+        self.raising_exceptions = raising_exceptions
+        self.raising_where = raising_where
         self.returning_value = returning_value
         
         return self
     
     
     @copy_docs(WrapperBase.__repr__)
     def __repr__(self):
         for field_added, repr_parts in self._cursed_repr_builder():
             
+            mode = self.mode
             repr_parts.append(' (')
             type_field_added = False
             
-            is_raising = self.is_raising
-            if is_raising:
+            if mode & MODE_RAISING:
                 if type_field_added:
                     repr_parts.append(', ')
                 else:
                     type_field_added = True
                 
                 repr_parts.append('raising')
             
-            
-            is_returning = self.is_returning
-            if is_returning:
+            if mode & MODE_RETURNING:
                 if type_field_added:
                     repr_parts.append(', ')
                 else:
                     type_field_added = True
             
                 repr_parts.append('returning')
             
-            is_call_with = self.is_call_with
-            
-            if is_call_with:
+            if mode & MODE_CALL_WITH:
                 if type_field_added:
                     repr_parts.append(', ')
                 else:
                     type_field_added = True
             
                 repr_parts.append('call_with')
             
             repr_parts.append(')')
             
             
-            if is_raising:
+            if mode & MODE_RAISING:
                 if field_added:
                     repr_parts.append(',')
                 else:
                     field_added = True
                 
                 repr_parts.append(' raising_exceptions = ')
                 repr_parts.append(repr(self.raising_exceptions))
                 
                 repr_parts.append(', raising_accept_subtypes = ')
                 repr_parts.append(repr(self.raising_accept_subtypes))
+                
+                raising_where = self.raising_where
+                if (raising_where is not None):
+                    repr_parts.append(', raising_where = ')
+                    repr_parts.append(repr(raising_where))
             
-            if is_returning:
+            if mode & MODE_RETURNING:
                 if field_added:
                     repr_parts.append(',')
                 else:
                     field_added = True
                 
-                repr_parts.append(' self.returning_value = ')
+                repr_parts.append(', returning_value = ')
                 repr_parts.append(reprlib.repr(self.returning_value))
             
-            
-            if is_call_with:
+            if mode & MODE_CALL_WITH:
                 calling_positional_parameters = self.calling_positional_parameters
                 if calling_positional_parameters:
                     if field_added:
                         repr_parts.append(',')
                     else:
                         field_added = True
                     
@@ -188,88 +190,84 @@
         return ''.join(repr_parts)
     
     
     @copy_docs(WrapperBase.__hash__)
     def __hash__(self):
         hash_value = WrapperBase.__hash__(self)
         
-        if self.is_raising:
+        if self.is_raising():
             hash_value ^= hash_set(self.raising_exceptions)
             hash_value ^= self.raising_accept_subtypes
-        
-        if self.is_returning:
+            raising_where = self.raising_where
+            if (raising_where is not None):
+                hash_value ^= try_hash_method(raising_where)
+                
+        if self.is_returning():
             hash_value ^= try_hash_method(self.returning_value)
         
-        
-        if self.is_call_with:
+        if self.is_call_with():
             hash_value ^= hash_tuple(self.calling_positional_parameters)
             hash_value ^= hash_dict(self.calling_keyword_parameters)
         
-        
         return hash_value
     
     
     @copy_docs(WrapperBase.__eq__)
     def __eq__(self, other):
         if type(self) is not type(other):
             return NotImplemented
         
-        is_raising = self.is_raising
-        if is_raising != other.is_raising:
+        self_mode = self.mode
+        if self_mode != other.mode:
             return False
         
-        if is_raising:
+        if self_mode & MODE_RAISING:
             if self.raising_exceptions != other.raising_exceptions:
                 return False
             
             if self.raising_accept_subtypes != other.raising_accept_subtypes:
                 return False
+            
+            if self.raising_where != other.raising_where:
+                return False
         
-        is_returning = self.is_returning
-        if is_returning != other.is_returning:
-            return False
-        
-        if is_returning:
+        if self_mode & MODE_RETURNING:
             if self.returning_value != other.returning_value:
                 return False
         
-        is_call_with = self.is_call_with
-        if is_call_with != other.is_call_with:
-            return False
-        
-        if is_call_with:
+        if self_mode & MODE_CALL_WITH:
             if self.calling_positional_parameters != other.calling_positional_parameters:
                 return False
             
             if self.calling_keyword_parameters != other.calling_keyword_parameters:
                 return False
         
         return True
     
     
     @copy_docs(WrapperBase.check_conflicts)
     def check_conflicts(self):
-        if self.is_raising and self.is_returning:
+        if self.is_raising() and self.is_returning():
             return WrapperConflict(
                 self,
                 reason = 'A call wrapper cannot be returning & raising at the same time.',
             )
     
     
     @copy_docs(WrapperBase.check_conflict_with)
     def check_conflict_with(self, other):
         if not isinstance(other, type(self)):
             return
         
         
-        self_input_field_count = self.is_call_with
-        self_output_field_count = self.is_raising + self.is_returning
+        self_input_field_count = self.is_call_with()
+        self_output_field_count = self.is_raising() + self.is_returning()
         
-        other_input_count = other.is_call_with
-        other_output_field_count = other.is_raising + other.is_returning
+        other_input_count = other.is_call_with()
+        other_output_field_count = other.is_raising() + other.is_returning()
         
         if (self_input_field_count + self_output_field_count) == (other_input_count + other_output_field_count):
             # Both defined input and output, so we accept both.
             return
         
         
         if (self_input_field_count + self_output_field_count) != (other_input_count + other_output_field_count):
@@ -298,218 +296,173 @@
     
     
     @copy_docs(WrapperBase.is_mutually_exclusive_with)
     def is_mutually_exclusive_with(self, other):
         if type(self) is not type(other):
             return False
         
-        if self.is_call_with and other.is_call_with:
+        if self.is_call_with() and other.is_call_with():
             return True
         
         return False
     
     
-    @copy_docs(WrapperBase.context)
-    def context(self, handle):
-        call_state = yield None
-        
-        if self.is_call_with:
-            call_state = call_state.with_parameters(
-                self.calling_positional_parameters,
-                self.calling_keyword_parameters,
-            )
-        
-        result_state = yield call_state
-        
-        # Ignore `AssertionException`-s.
-        if result_state is None:
-            raised_exception = None
-        else:
-            raised_exception = result_state.raised_exception
-        
-        if (raised_exception is None) or (not isinstance(raised_exception, AssertionException)):
-            
-            if self.is_raising:
-                raising_exceptions = self.raising_exceptions
-                raising_accept_subtypes = self.raising_accept_subtypes
-                if raised_exception is None:
-                    return Result(handle).with_exception(
-                        raising_exceptions,
-                        None,
-                        raising_accept_subtypes,
-                    )
-                
-                if try_match_exception(raising_exceptions, raised_exception, raising_accept_subtypes):
-                    if (result_state is not None):
-                        result_state = result_state.with_exception(None)
-                
-                else:
-                    return Result(handle).with_exception(
-                        raising_exceptions,
-                        raised_exception,
-                        raising_accept_subtypes,
-                    )
-            
-            elif self.is_returning:
-                if (raised_exception is not None):
-                    return Result(handle).with_exception(None, raised_exception, False)
-                
-                if (result_state is None):
-                    returned_value = None
-                else:
-                    returned_value = result_state.returned_value
-                
-                returning_value = self.returning_value
-                
-                if returned_value != returning_value:
-                    return Result(handle).with_return(returning_value, returned_value)
-        
-        yield result_state
+    @copy_docs(WrapperBase.get_context)
+    def get_context(self, handle):
+        return ContextCalling(handle, self)
     
     
     @property
     def raising_key(self):
         """
         Returns the wrapper's raising key.
         
         Returns
         -------
-        raising_key : `None`, `tuple` (`set` of ``BaseException``, `bool`)
+        raising_key : `None`, `tuple` (`set` of ``BaseException``, `bool`, (`None`, `callable`))
         """
-        if self.is_raising:
-            return (self.raising_exceptions, self.raising_accept_subtypes)
+        if self.is_raising():
+            return (self.raising_exceptions, self.raising_accept_subtypes, self.raising_where)
     
     
     @property
     def returning_key(self):
         """
         Returns the wrapper's raising key.
         
         Returns
         -------
-        raising_key : `None`, `tuple` (`set` of ``BaseException``, `bool`)
+        returning_key : `None`, `tuple` (`object`)
         """
-        if self.is_raising:
+        if self.is_returning():
             return (self.returning_value, )
     
     
     @property
     def call_with_key(self):
         """
         Returns the wrapper's raising key.
         
         Returns
         -------
-        call_with_key : `None`, `tuple` (`tuple` of `Any`, `dict` of (`str`, `Any`) items)
+        call_with_key : `None`, `tuple` (`tuple` of `object`, `dict` of (`str`, `object`) items)
         """
-        if self.is_call_with:
+        if self.is_call_with():
             return (self.calling_positional_parameters, self.calling_keyword_parameters)
     
     
     @classmethod
-    def raising_constructor(cls,  *exception_types, raising_accept_subtypes = True):
+    def raising_constructor(cls, exception_type, *exception_types, accept_subtypes = True, where = None):
         """
         Creates a new raising wrapper.
         
         Parameters
         ----------
-        *exception_types : tuple` of (`BaseException`, ...)
-            Exception types to expect.
-        raising_accept_subtypes : `bool` = `True`
+        exception_type : `type<BaseException> | BaseException>
+            Exception type to expect.
+        *exception_types : `tuple<type<BaseException>, BaseException, ...>`
+            Additional exception types.
+        accept_subtypes : `bool` = `True`
             Whether subclasses are accepted as well.
+        where : `None`, `callable` = `None`, Optional (Keyword only)
+            Additional check to check the raised exception.
         
         Raises
         ------
         TypeError
             If an `exception_types`'s type is incorrect.
         ValueError
             If no exception was passed.
         
         Returns
         -------
-        new : ``WrapperCall``
+        self : `instance<self>`
         """
-        exception_types = un_nest_expected_exceptions(exception_types)
+        exception_types = un_nest_exceptions((exception_type, *exception_types))
         if not exception_types:
             raise ValueError(
                 'At least 1 exception is required.'
             )
         
         return cls(
-            raising = (exception_types, raising_accept_subtypes),
+            raising = (exception_types, accept_subtypes, where),
         )
     
     
-    def raising(self,  *exception_types, raising_accept_subtypes = True):
+    def raising(self, exception_type, *exception_types, accept_subtypes = True, where = None):
         """
         Creates a new raising wrapper extending self.
         
         Parameters
         ----------
-        *exception_types : tuple` of (`BaseException`, ...)
-            Exception types to expect.
-        raising_accept_subtypes : `bool` = `True`
+        exception_type : `type<BaseException> | BaseException>
+            Exception type to expect.
+        *exception_types : `tuple<type<BaseException>, BaseException, ...>`
+            Additional exception types.
+        accept_subtypes : `bool` = `True`
             Whether subclasses are accepted as well.
+        where : `None`, `callable` = `None`, Optional (Keyword only)
+            Additional check to check the raised exception.
+        
+        Returns
+        -------
+        new : `instance<type<self>>`
         
         Raises
         ------
         TypeError
             If an `exception_types`'s type is incorrect.
         ValueError
             If no exception was passed.
-        
-        Returns
-        -------
-        new : ``WrapperCall``
         """
-        exception_types = un_nest_expected_exceptions(exception_types)
+        exception_types = un_nest_exceptions((exception_type, *exception_types))
         if not exception_types:
             raise ValueError(
                 'At least 1 exception is required.'
             )
         
         return type(self)(
             self.wrapped,
-            raising = (exception_types, raising_accept_subtypes),
+            raising = (exception_types, accept_subtypes, where),
             returning = self.returning_key,
             call_with = self.call_with_key,
         )
     
     
     @classmethod
     def returning_constructor(cls, returning):
         """
         Creates a new returning wrapper.
         
         Parameters
         ----------
-        returning : `Any`
+        returning : `object`
             The expected value to be returned.
         
         Returns
         -------
-        self : ``WrapperCall``
+        self : `instance<self>`
         """
         return cls(
             returning = (returning, ),
         )
     
     
     def returning(self, returning_value):
         """
         Creates a new returning wrapper extending self.
         
         Parameters
         ----------
-        returning_value : `Any`
+        returning_value : `object`
             The expected value to be returned.
         
         Returns
         -------
-        new : ``WrapperCall``
+        new : `instance<type<self>>`
         """
         return type(self)(
             self.wrapped,
             raising = self.raising_key,
             returning = (returning_value, ),
             call_with = self.call_with_key,
         )
@@ -521,24 +474,24 @@
         
         Parameters
         ----------
         transformer : `callable`
         
         Returns
         -------
-        new : ``WrapperCall``
+        new : `instance<type<self>>`
         
         Raises
         ------
         ValueError
             The wrapper is not parameterised, or incorrect amount parameters registered.
         """
-        if not self.is_call_with:
+        if not self.is_call_with():
             raise ValueError(
-                f'Call wrapper cannot check for return value if it has no parameters added; self={self!r}.'
+                f'Call wrapper cannot check for return value if it has no parameters added; self = {self!r}.'
             )
         
         calling_positional_parameters = self.calling_positional_parameters
         calling_keyword_parameters = self.calling_keyword_parameters
         
         if calling_positional_parameters is None:
             if calling_keyword_parameters:
@@ -557,33 +510,33 @@
     
     def returning_itself(self):
         """
         Creates a new retuning wrapper checking for whether the input value matches the returned one.
         
         Returns
         -------
-        new : ``WrapperCall``
+        new : `instance<type<self>>`
         
         Raises
         ------
         ValueError
             The wrapper is not parameterised, or incorrect amount parameters registered.
         """
-        if not self.is_call_with:
+        if not self.is_call_with():
             raise ValueError(
-                f'Call wrapper cannot check for return value if it has no parameters added; self={self!r}.'
+                f'Call wrapper cannot check for return value if it has no parameters added; self = {self!r}.'
             )
         
         calling_positional_parameters = self.calling_positional_parameters
         calling_keyword_parameters = self.calling_keyword_parameters
         
         if len(calling_positional_parameters) + len(calling_keyword_parameters) != 1:
             raise ValueError(
-                f'``.returning_itself`` is only applicable if the wrapper has 1 parameter added; '
-                f'self={self!r}.'
+                f'`returning_itself` is only applicable if the wrapper has 1 parameter added; '
+                f'self = {self!r}.'
             )
         
         if calling_positional_parameters:
             returning_value = calling_positional_parameters[0]
         else:
             returning_value = next(iter(calling_keyword_parameters.values()))
         
@@ -598,42 +551,75 @@
     @classmethod
     def call_with_constructor(cls, *calling_positional_parameters, **calling_keyword_parameters):
         """
         Creates new parameterised wrapper.
         
         Parameters
         ----------
-        *calling_positional_parameters : `tuple` of `Any`
+        *calling_positional_parameters : `tuple` of `object`
             Positional parameter to call the test with.
-        **calling_keyword_parameters : `dict` of (`str`, `Any`) items
+        **calling_keyword_parameters : `dict` of (`str`, `object`) items
             Keyword parameters to call the test with.
         
         Returns
         -------
-        self : ``WrapperCall``
+        self : `instance<cls>`
         """
         return cls(
             call_with = (calling_positional_parameters, calling_keyword_parameters),
         )
     
     
     def call_with(self, *calling_positional_parameters, **calling_keyword_parameters):
         """
         Creates a new parameterised wrapper extending self.
         
         Parameters
         ----------
-        *calling_positional_parameters : `tuple` of `Any`
+        *calling_positional_parameters : `tuple` of `object`
             Positional parameter to call the test with.
-        **calling_keyword_parameters : `dict` of (`str`, `Any`) items
+        **calling_keyword_parameters : `dict` of (`str`, `object`) items
             Keyword parameters to call the test with.
         
         Returns
         -------
-        new : ``WrapperCall``
+        new : `instance<type<self>>`
         """
         return type(self)(
             self.wrapped,
             raising = self.raising_key,
             returning = self.returning_key,
             call_with = (calling_positional_parameters, calling_keyword_parameters),
         )
+    
+    
+    def is_raising(self):
+        """
+        Returns whether raised exceptions of the test should be checked.
+        
+        Returns
+        -------
+        is_raising : `bool`
+        """
+        return True if self.mode & MODE_RAISING else False
+    
+    
+    def is_returning(self):
+        """
+        Returns whether returned value of the test should be checked.
+        
+        Returns
+        -------
+        is_returning : `bool`
+        """
+        return True if self.mode & MODE_RETURNING else False
+    
+    
+    def is_call_with(self):
+        """
+        Returns whether the test should be called with specific parameters.
+        
+        Returns
+        -------
+        is_call_with : `bool`
+        """
+        return True if self.mode & MODE_CALL_WITH else False
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_chainer.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_chainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 __all__ = ('WrapperChainer',)
 
 from scarletio import copy_docs, export
 
-from ..helpers import hash_set
+from ..helpers.hashing import hash_set
 
 from .wrapper_base import WrapperBase
 
 
 @export
 class WrapperChainer(WrapperBase):
     """
     Attributes
     ----------
-    wrapped : `None`, `Any`
+    wrapped : `None`, `object`
         The wrapped test.
     wrappers : `set` of ``WrapperBase``
         The applied wrappers.
     """
     __slots__ = ('wrappers',)
     
-    def __new__(cls, wrapped=None):
+    def __new__(cls, wrapped = None):
         """
         Creates a new combined wrapper containing more wrappers.
         
         Parameters
         ----------
-        wrapped : `None`, `Any` = `None`, Optional
+        wrapped : `None`, `object` = `None`, Optional
             The wrapped test if any.
         """
         self = object.__new__(cls)
         self.wrapped = wrapped
         self.wrappers = set()
         return self
     
@@ -38,27 +38,27 @@
     def __call__(self, to_wrap):
         if isinstance(to_wrap, WrapperBase):
             self.append(to_wrap)
             return self
         
         
         if (self.wrapped is not None):
-            raise RuntimeError(f'Wrapped already wrapped; self={self!r}, to_wrap={to_wrap!r}.')
+            raise RuntimeError(f'Wrapped already wrapped; self = {self!r}, to_wrap = {to_wrap!r}.')
         
         self.wrapped = to_wrap
         return self
     
     
     @copy_docs(WrapperBase.__repr__)
     def __repr__(self):
         for field_added, repr_parts in self._cursed_repr_builder():
             if field_added:
                 repr_parts.append(',')
             
-            repr_parts.append(' wrappers=')
+            repr_parts.append(' wrappers = ')
             repr_parts.append(repr(self.wrappers))
         
         return ''.join(repr_parts)
     
     
     @copy_docs(WrapperBase.__hash__)
     def __hash__(self):
@@ -83,18 +83,18 @@
         for wrapper in self.wrappers:
             if wrapper.do_skip():
                 return True
         
         return False
     
     
-    @copy_docs(WrapperBase.do_revert)
-    def do_revert(self):
+    @copy_docs(WrapperBase.do_reverse)
+    def do_reverse(self):
         for wrapper in self.wrappers:
-            if wrapper.do_revert():
+            if wrapper.do_reverse():
                 return True
         
         return False
     
     @copy_docs(WrapperBase.check_conflicts)
     def check_conflicts(self):
         wrappers = list(self.wrappers)
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_conflict.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_conflict.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,73 +5,73 @@
 
 class WrapperConflict(RichAttributeErrorBaseType):
     """
     Raised when 2 wrappers have conflict with each other.
     
     Attributes
     ----------
-    wrapper_1 : ``WrapperBase``
+    wrapper_0 : ``WrapperBase``
         The wrapper 1 with the conflict.
     reason : `None`, `str`
         The reason why the two wrappers are incompatible.
-    wrapper_2 : `None`, ``WrapperBase``
+    wrapper_1 : `None`, ``WrapperBase``
         The wrapper 2 with the conflict.
     """
-    __slots__ = ('reason', 'wrapper_1', 'wrapper_2')
+    __slots__ = ('reason', 'wrapper_0', 'wrapper_1')
     
-    def __new__(cls, wrapper_1, wrapper_2 = None, *, reason = None):
+    def __new__(cls, wrapper_0, wrapper_1 = None, *, reason = None):
         """
         Creates a new wrapper conflict.
         
         Parameters
         ----------
-        wrapper_1 : ``WrapperBase``
+        wrapper_0 : ``WrapperBase``
             Wrapper one with the conflict.
-        wrapper_2 : `None`, ``WrapperBase`` = `None`, Optional
+        wrapper_1 : `None`, ``WrapperBase`` = `None`, Optional
             Wrapper two with the conflict.
         reason : `None`, `str` = `None`, Optional (Keyword only)
             The reason why the two wrappers are incompatible.
         """
         self = object.__new__(cls)
+        self.wrapper_0 = wrapper_0
         self.wrapper_1 = wrapper_1
-        self.wrapper_2 = wrapper_2
         self.reason = reason
         return self
     
     
     def __repr__(self):
         """Returns the wrapper conflict's representation."""
         repr_parts = ['<', self.__class__.__name__]
         
-        repr_parts.append(' wrapper_1=')
-        repr_parts.append(repr(self.wrapper_1))
+        repr_parts.append(' wrapper_0=')
+        repr_parts.append(repr(self.wrapper_0))
         
-        wrapper_2 = self.wrapper_2
-        if (wrapper_2 is not None):
-            repr_parts.append(', wrapper_2=')
-            repr_parts.append(repr(self.wrapper_2))
+        wrapper_1 = self.wrapper_1
+        if (wrapper_1 is not None):
+            repr_parts.append(', wrapper_1=')
+            repr_parts.append(repr(self.wrapper_1))
         
         reason = self.reason
         if (reason is not None):
             repr_parts.append(', reason = ')
             repr_parts.append(repr(self.reason))
         
         repr_parts.append('>')
         return ''.join(repr_parts)
     
     
     def __hash__(self):
         """Returns the wrapper conflict's hash value."""
         hash_value = 0
         
-        hash_value ^= hash(self.wrapper_1)
+        hash_value ^= hash(self.wrapper_0)
         
-        wrapper_2 = self.wrapper_2
-        if (wrapper_2 is not None):
-            hash_value ^= hash(wrapper_2)
+        wrapper_1 = self.wrapper_1
+        if (wrapper_1 is not None):
+            hash_value ^= hash(wrapper_1)
         
         reason = self.reason
         if (reason is not None):
             hash_value ^= hash(reason)
         
         return hash_value
     
@@ -95,40 +95,14 @@
         """
         Returns the collective wrappers of the conflict.
         
         Returns
         -------
         wrappers : `frozenset` of ``WrapperBase``
         """
-        wrappers = [self.wrapper_1]
+        wrappers = [self.wrapper_0]
         
-        wrapper_2 = self.wrapper_2
-        if (wrapper_2 is not None):
-            wrappers.append(wrapper_2)
+        wrapper_1 = self.wrapper_1
+        if (wrapper_1 is not None):
+            wrappers.append(wrapper_1)
         
         return frozenset(wrappers)
-    
-    
-    def get_failure_message(self):
-        """
-        Returns the failure message of the wrapper conflict.
-        
-        Returns
-        -------
-        failure_message : `str`
-        """
-        failure_message_parts = ['Wrapper conflict']
-        
-        reason = self.reason
-        if (reason is not None):
-            failure_message_parts.append(': ')
-            failure_message_parts.append(reason)
-        
-        failure_message_parts.append('Between wrappers:\n')
-        failure_message_parts.append(repr(self.wrapper_1))
-        
-        wrapper_2 = self.wrapper_2
-        if (wrapper_2 is not None):
-            failure_message_parts.append('\n')
-            failure_message_parts.append(repr(wrapper_2))
-        
-        return ''.join(failure_message_parts)
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_environment.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class WrapperEnvironment(WrapperBase):
     """
     Uses a specific environment for the wrapped test.
 
     Attributes
     ----------
-    wrapped : `None`, `Any`
+    wrapped : `None`, `object`
         The wrapped test.
     environment : ``DefaultEnvironment``
         Environment to use while running the test.
     """
     __slots__ = ('environment',)
     
     def __new__(cls, environment):
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_garbage_collect.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_garbage_collect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 __all__ = ('WrapperGarbageCollect',)
 
-from gc import collect as gc_collect
+from scarletio import copy_docs
 
-from .wrapper_base import WrapperBase
+from ..contexts import ContextGarbageCollect
 
-from scarletio import copy_docs
+from .wrapper_base import WrapperBase
 
 
 class WrapperGarbageCollect(WrapperBase):
     """
     Collects garbage before and (or) after the test as configured.
     
     Attributes
     ----------
-    wrapped : `None`, `Any`
+    wrapped : `None`, `object`
         The wrapped test.
     after : `bool`
         Whether garbage should be collected after the test.
     before : `bool`
         Whether garbage should be collected before the test.
     """
     __slots__ = ('after', 'before')
@@ -59,30 +59,17 @@
         
         self = object.__new__(cls)
         self.after = after
         self.before = before
         return self
     
     
-    @copy_docs(WrapperBase.context)
-    def context(self):
-        call_state = yield None
-        
-        if self.before:
-            gc_collect()
-            gc_collect()
-        
-        try:
-            result_state = yield call_state
-        finally:
-            if self.after:
-                gc_collect()
-                gc_collect()
-        
-        yield result_state
+    @copy_docs(WrapperBase.get_context)
+    def get_context(self, handle):
+        return ContextGarbageCollect(self)
     
     
     @copy_docs(WrapperBase.__repr__)
     def __repr__(self):
         return f'<{self.__class__.__name__} before = {self.before!r}, after = {self.after!r}>'
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_revert.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_reverse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-__all__ = ('WrapperRevert',)
+__all__ = ('WrapperReverse',)
 
 from scarletio import copy_docs
 
 from .wrapper_base import WrapperBase
 
 
-class WrapperRevert(WrapperBase):
+class WrapperReverse(WrapperBase):
     """
-    Reverts the test's result.
+    Reverses the test's result.
 
     Attributes
     ----------
-    wrapped : `None`, `Any`
+    wrapped : `None`, `object`
         The wrapped test.
     """
     __slots__ = ()
     
     @copy_docs(WrapperBase.__repr__)
     def __repr__(self):
         """Returns the conditional skip wrapper's representation."""
@@ -32,10 +32,10 @@
     
     
     @copy_docs(WrapperBase.__hash__)
     def __hash__(self):
         return (1 << 4)
     
     
-    @copy_docs(WrapperBase.do_revert)
-    def do_revert(self):
+    @copy_docs(WrapperBase.do_reverse)
+    def do_reverse(self):
         return True
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_skip.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class WrapperSkip(WrapperBase):
     """
     Skips the test.
 
     Attributes
     ----------
-    wrapped : `None`, `Any`
+    wrapped : `None`, `object`
         The wrapped test.
     """
     __slots__ = ()
     
     @copy_docs(WrapperBase.__repr__)
     def __repr__(self):
         return f'<{self.__class__.__name__}'
```

### Comparing `vampytest-0.0.7/vampytest/core/wrappers/wrapper_skip_conditional.py` & `vampytest-0.0.8/vampytest/core/wrappers/wrapper_skip_conditional.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class WrapperSkipConditional(WrapperSkip):
     """
     Skips the test.
 
     Attributes
     ----------
-    wrapped : `None`, `Any`
+    wrapped : `None`, `object`
         The wrapped test.
     skip : `bool`
         Whether the test should be skipped.
     """
     __slots__ = ('skip', )
     
     def __new__(cls, skip):
```

### Comparing `vampytest-0.0.7/vampytest/main/__init__.py` & `vampytest-0.0.8/vampytest/main/__init__.py`

 * *Files identical despite different names*

### Comparing `vampytest-0.0.7/vampytest.egg-info/PKG-INFO` & `vampytest-0.0.8/vampytest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vampytest
-Version: 0.0.7
+Version: 0.0.8
 Summary: A vampy test framework
 Home-page: https://github.com/HuyaneMatsu/vampytest
 Author: HuyaneMatsu
 Author-email: re.ism.tm@gmail.com
 License: DBAD
 Description: <h1 align="center">
             Vampytest
@@ -22,20 +22,20 @@
         
         *The library currently is in alpha stage. It can run tests but many features might be missing.*
         
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `vampytest-0.0.7/vampytest.egg-info/SOURCES.txt` & `vampytest-0.0.8/vampytest.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 vampytest.egg-info/PKG-INFO
 vampytest.egg-info/SOURCES.txt
 vampytest.egg-info/dependency_links.txt
 vampytest.egg-info/requires.txt
 vampytest.egg-info/top_level.txt
 vampytest/core/__init__.py
 vampytest/core/handle.py
-vampytest/core/helpers.py
 vampytest/core/run_state.py
 vampytest/core/test_case.py
-vampytest/core/utils.py
 vampytest/core/assertions/__init__.py
+vampytest/core/assertions/aliases.py
 vampytest/core/assertions/assertion_base.py
 vampytest/core/assertions/assertion_conditional_base.py
 vampytest/core/assertions/assertion_contains.py
 vampytest/core/assertions/assertion_equals.py
 vampytest/core/assertions/assertion_false.py
 vampytest/core/assertions/assertion_identical.py
 vampytest/core/assertions/assertion_instance.py
@@ -25,26 +24,36 @@
 vampytest/core/assertions/assertion_not_equals.py
 vampytest/core/assertions/assertion_not_identical.py
 vampytest/core/assertions/assertion_raising.py
 vampytest/core/assertions/assertion_states.py
 vampytest/core/assertions/assertion_subtype.py
 vampytest/core/assertions/assertion_true.py
 vampytest/core/assertions/exceptions.py
+vampytest/core/contexts/__init__.py
+vampytest/core/contexts/base.py
+vampytest/core/contexts/calling.py
+vampytest/core/contexts/garbage_collect.py
+vampytest/core/contexts/output_capturing.py
 vampytest/core/environment/__init__.py
 vampytest/core/environment/configuration.py
 vampytest/core/environment/constants.py
 vampytest/core/environment/default.py
 vampytest/core/environment/helpers.py
 vampytest/core/environment/manager.py
 vampytest/core/environment/scarletio_coroutine.py
 vampytest/core/event_handling/__init__.py
 vampytest/core/event_handling/base.py
+vampytest/core/event_handling/colors.py
 vampytest/core/event_handling/default.py
 vampytest/core/event_handling/default_output_writer.py
 vampytest/core/event_handling/text_styling.py
+vampytest/core/event_handling/rendering_helpers/__init__.py
+vampytest/core/event_handling/rendering_helpers/result_modifier_parameters.py
+vampytest/core/event_handling/rendering_helpers/result_rendering.py
+vampytest/core/event_handling/rendering_helpers/writers.py
 vampytest/core/events/__init__.py
 vampytest/core/events/base.py
 vampytest/core/events/constants.py
 vampytest/core/events/file_load_done.py
 vampytest/core/events/file_registration.py
 vampytest/core/events/file_registration_done.py
 vampytest/core/events/file_testing_done.py
@@ -52,31 +61,41 @@
 vampytest/core/events/testing_end.py
 vampytest/core/events/testing_start.py
 vampytest/core/file/__init__.py
 vampytest/core/file/collection.py
 vampytest/core/file/file_system_entry.py
 vampytest/core/file/load_failure.py
 vampytest/core/file/test_file.py
+vampytest/core/helpers/__init__.py
+vampytest/core/helpers/exception_matching.py
+vampytest/core/helpers/hashing.py
+vampytest/core/helpers/merging.py
+vampytest/core/helpers/path_repr.py
+vampytest/core/helpers/un_nesting.py
 vampytest/core/result/__init__.py
 vampytest/core/result/result.py
-vampytest/core/result/result_group.py
-vampytest/core/result/failures/__init__.py
-vampytest/core/result/failures/asserting.py
-vampytest/core/result/failures/base.py
-vampytest/core/result/failures/helpers.py
-vampytest/core/result/failures/raising.py
-vampytest/core/result/failures/returning.py
-vampytest/core/result/failures/reverted.py
+vampytest/core/result/reports/__init__.py
+vampytest/core/result/reports/asserting.py
+vampytest/core/result/reports/base.py
+vampytest/core/result/reports/output.py
+vampytest/core/result/reports/raising.py
+vampytest/core/result/reports/returning.py
 vampytest/core/runner/__init__.py
 vampytest/core/runner/context.py
 vampytest/core/runner/runner.py
+vampytest/core/utils/__init__.py
+vampytest/core/utils/aliases.py
+vampytest/core/utils/capture_output_context_manager.py
+vampytest/core/utils/wrap_nothing.py
 vampytest/core/wrappers/__init__.py
+vampytest/core/wrappers/aliases.py
 vampytest/core/wrappers/wrapper_base.py
 vampytest/core/wrappers/wrapper_call.py
+vampytest/core/wrappers/wrapper_call_from.py
 vampytest/core/wrappers/wrapper_chainer.py
 vampytest/core/wrappers/wrapper_conflict.py
 vampytest/core/wrappers/wrapper_environment.py
 vampytest/core/wrappers/wrapper_garbage_collect.py
-vampytest/core/wrappers/wrapper_revert.py
+vampytest/core/wrappers/wrapper_reverse.py
 vampytest/core/wrappers/wrapper_skip.py
 vampytest/core/wrappers/wrapper_skip_conditional.py
 vampytest/main/__init__.py
```

