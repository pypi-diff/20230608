# Comparing `tmp/linktest-2.0.8.tar.gz` & `tmp/linktest-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.0.8.tar", last modified: Thu May 11 10:52:08 2023, max compression
+gzip compressed data, was "linktest-2.1.0.tar", last modified: Thu Jun  8 09:20:10 2023, max compression
```

## Comparing `linktest-2.0.8.tar` & `linktest-2.1.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-11 10:52:08.942080 linktest-2.0.8/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-11 10:52:08.941239 linktest-2.0.8/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-11 10:52:08.863377 linktest-2.0.8/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-05-11 10:51:05.000000 linktest-2.0.8/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-04-26 05:36:37.000000 linktest-2.0.8/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-04-25 07:00:45.000000 linktest-2.0.8/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-04-26 05:52:13.000000 linktest-2.0.8/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-04-26 05:58:55.000000 linktest-2.0.8/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-04-26 06:07:11.000000 linktest-2.0.8/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-04-26 06:20:46.000000 linktest-2.0.8/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-04-26 06:23:55.000000 linktest-2.0.8/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-04-26 06:27:01.000000 linktest-2.0.8/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-04-25 07:00:45.000000 linktest-2.0.8/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-04-26 06:27:01.000000 linktest-2.0.8/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-04-25 12:18:59.000000 linktest-2.0.8/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-04-26 06:28:34.000000 linktest-2.0.8/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-04-25 13:06:43.000000 linktest-2.0.8/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8706 2023-05-09 07:09:35.000000 linktest-2.0.8/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100661 2023-05-09 07:25:32.000000 linktest-2.0.8/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-04-25 12:18:59.000000 linktest-2.0.8/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      423 2023-05-11 10:50:59.000000 linktest-2.0.8/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-04-25 12:18:59.000000 linktest-2.0.8/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:57:24.000000 linktest-2.0.8/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-04-26 06:29:23.000000 linktest-2.0.8/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-11 10:52:08.872252 linktest-2.0.8/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-05-11 10:52:08.000000 linktest-2.0.8/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2190 2023-05-11 10:52:08.000000 linktest-2.0.8/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-05-11 10:52:08.000000 linktest-2.0.8/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-05-11 10:52:08.000000 linktest-2.0.8/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-05-11 10:52:08.000000 linktest-2.0.8/linktest.egg-info/top_level.txt
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-05-11 10:52:08.939705 linktest-2.0.8/lintest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/auto_generate_test_suite.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/auto_organize_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/lintest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.0.8/lintest/xml_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-05-11 10:52:08.942264 linktest-2.0.8/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-05-11 10:51:55.000000 linktest-2.0.8/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-06-08 09:20:10.967037 linktest-2.1.0/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-06-08 09:20:10.966407 linktest-2.1.0/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-06-08 09:20:10.883711 linktest-2.1.0/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-06-08 09:15:22.000000 linktest-2.1.0/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2023-05-15 09:26:57.000000 linktest-2.1.0/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16834 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9712 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7110 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16356 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      916 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31803 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10033 2023-06-07 05:49:19.000000 linktest-2.1.0/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   100661 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8059 2023-06-08 03:00:07.000000 linktest-2.1.0/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      423 2023-06-08 09:15:17.000000 linktest-2.1.0/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3115 2023-06-08 03:18:42.000000 linktest-2.1.0/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2023-05-11 10:53:17.000000 linktest-2.1.0/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-06-08 09:20:10.891442 linktest-2.1.0/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      100 2023-06-08 09:20:10.000000 linktest-2.1.0/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2220 2023-06-08 09:20:10.000000 linktest-2.1.0/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2023-06-08 09:20:10.000000 linktest-2.1.0/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      116 2023-06-08 09:20:10.000000 linktest-2.1.0/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2023-06-08 09:20:10.000000 linktest-2.1.0/linktest.egg-info/top_level.txt
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2023-06-08 09:20:10.965205 linktest-2.1.0/lintest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      461 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10758 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2629 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/auto_generate_test_suite.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    30653 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    17741 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2130 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/auto_organize_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10929 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1786 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7062 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2511 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16348 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1481 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3135 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    31798 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      176 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/lintest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10159 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   111768 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1071 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7822 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      420 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      914 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3052 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3597 2023-04-25 06:29:43.000000 linktest-2.1.0/lintest/xml_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2023-06-08 09:20:10.967198 linktest-2.1.0/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      454 2023-06-08 09:19:49.000000 linktest-2.1.0/setup.py
```

### Comparing `linktest-2.0.8/linktest/appium_utils.py` & `linktest-2.1.0/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/auto_generate_testcase_list.py` & `linktest-2.1.0/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.1.0/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/base_testcase.py` & `linktest-2.1.0/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/clean_data.py` & `linktest-2.1.0/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/conver_xml_into_db.py` & `linktest-2.1.0/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/database_helper.py` & `linktest-2.1.0/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/date_utilities.py` & `linktest-2.1.0/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/doctor.py` & `linktest-2.1.0/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/framework_log.py` & `linktest-2.1.0/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/get_adb_devices.py` & `linktest-2.1.0/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/get_ios_devices_list.py` & `linktest-2.1.0/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/get_platform_info.py` & `linktest-2.1.0/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/get_project_info.py` & `linktest-2.1.0/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/html_report.py` & `linktest-2.1.0/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/logged_requests.py` & `linktest-2.1.0/linktest/logged_requests.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     return command.format(method=method, headers=headers, data=data, uri=uri)
 
 
 class LoggedRequests:
     """
         封装 requests module 的常用方法，自动log 每次 request 的参数 & response 内容
+        如果 api 有version字段 同时会log其版本信息
         @author: Wang Lin
         """
 
     def __init__(self, logger):
         self.logger = logger
 
     def log_curl(func):
@@ -51,14 +52,42 @@
 
             instance.logger.info(
                 os.linesep + os.linesep + "================================ cURL Start ==========================")
             instance.logger.info(os.linesep + curlify.to_curl(res.request))
             instance.logger.info(
                 os.linesep + "================================ cURL End ============================" + os.linesep)
 
+            api_version = ""
+            # 检查响应头部中的各种可能的版本信息
+            api_version_keys = ["version", "Version", "VERSION",
+                                "API-Version", "API-VERSION","api-version",
+                                "API-Version-Header", "api-version-header", "API-VERSION-HEADER"]
+
+
+            # ===== log api's version =====
+            for key in api_version_keys:
+                if key in res.headers:
+                    api_version = f"API version found in headers: {res.headers[key]}"
+                    break
+
+            if not api_version:
+                # 如果未在响应头部中找到版本信息，请检查响应体中的各种可能的版本信息
+                try:
+                    response_body = res.json()
+                except json_func.JSONDecodeError:
+                    self.logger.info("Failed to decode JSON response body.")
+
+                for key in api_version_keys:
+                    if key in response_body:
+                        api_version = f"API version found in response body: {response_body[key]}"
+                        break
+
+            if not api_version:
+                instance.logger.info(os.linesep + "-------- API Version: %s" % api_version)
+
             return res
 
         return wrapper
 
     @log_curl
     def get(self, url, params=None, **kwargs):
         if hasattr(settings, "auto_log_request") and settings.auto_log_request is False:
```

### Comparing `linktest-2.0.8/linktest/main.py` & `linktest-2.1.0/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/memory_usage.py` & `linktest-2.1.0/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/run.py` & `linktest-2.1.0/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/run_testcase_thread.py` & `linktest-2.1.0/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/scp_report_to_specified_path.py` & `linktest-2.1.0/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/selenium_helper.py` & `linktest-2.1.0/lintest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/timeout_thread.py` & `linktest-2.1.0/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/ui_testcase.py` & `linktest-2.1.0/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/update_config.py` & `linktest-2.1.0/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest/xml_report.py` & `linktest-2.1.0/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/linktest.egg-info/SOURCES.txt` & `linktest-2.1.0/linktest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 linktest/set_run_flag_thread.py
 linktest/setup.py
 linktest/testcase_order.py
 linktest/testcase_timeout_exception.py
 linktest/timeout_thread.py
 linktest/ui_testcase.py
 linktest/update_config.py
+linktest/webdriver_wrapper.py
 linktest/windows_helper.py
 linktest/xml_report.py
 linktest.egg-info/PKG-INFO
 linktest.egg-info/SOURCES.txt
 linktest.egg-info/dependency_links.txt
 linktest.egg-info/requires.txt
 linktest.egg-info/top_level.txt
```

### Comparing `linktest-2.0.8/lintest/appium_utils.py` & `linktest-2.1.0/lintest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/auto_generate_test_suite.py` & `linktest-2.1.0/lintest/auto_generate_test_suite.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/auto_generate_testcase_list.py` & `linktest-2.1.0/lintest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/auto_generate_testcase_list_from_csv.py` & `linktest-2.1.0/lintest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/auto_organize_testcase.py` & `linktest-2.1.0/lintest/auto_organize_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/base_testcase.py` & `linktest-2.1.0/lintest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/clean_data.py` & `linktest-2.1.0/lintest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/conver_xml_into_db.py` & `linktest-2.1.0/lintest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/database_helper.py` & `linktest-2.1.0/lintest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/date_utilities.py` & `linktest-2.1.0/lintest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/doctor.py` & `linktest-2.1.0/lintest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/framework_log.py` & `linktest-2.1.0/lintest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/get_adb_devices.py` & `linktest-2.1.0/lintest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/get_ios_devices_list.py` & `linktest-2.1.0/lintest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/get_platform_info.py` & `linktest-2.1.0/lintest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/get_project_info.py` & `linktest-2.1.0/lintest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/html_report.py` & `linktest-2.1.0/lintest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/logged_requests.py` & `linktest-2.1.0/lintest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/main.py` & `linktest-2.1.0/lintest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/memory_usage.py` & `linktest-2.1.0/lintest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/run.py` & `linktest-2.1.0/lintest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/run_testcase_thread.py` & `linktest-2.1.0/lintest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/scp_report_to_specified_path.py` & `linktest-2.1.0/lintest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/selenium_helper.py` & `linktest-2.1.0/linktest/selenium_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import platform
 import traceback
 import subprocess
 from selenium import webdriver
+from .webdriver_wrapper import WebDriverWrapper
+
 
 try:
     import settings
 except ImportError:
     traceback.print_exc()
 
 try:
@@ -94,15 +96,18 @@
                             raise Exception("settings.BROWSER_OPTION must be a string list!")
 
                 if ui_testcase is None:
                     browser = webdriver.Chrome(chrome_options=chrome_options)
                 else:
                     # TODO: remove below hardcode ".webrtc.", instead of providing the BROWSER_OPTION in setting/__init__.py
                     if ui_testcase.__module__.find(".webrtc.") == -1:
-                        browser = webdriver.Chrome(chrome_options=chrome_options)
+                        # browser = webdriver.Chrome(chrome_options=chrome_options)
+
+                        # 使用 WebDriverWrapper 替换原来的 webdriver 实例
+                        browser = WebDriverWrapper(ui_testcase.logger, chrome_options=chrome_options)
                     else:
                         chrome_options.add_argument("--use-fake-device-for-media-stream")
                         chrome_options.add_argument("--use-fake-ui-for-media-stream")
                         chrome_options.add_argument("--incognito")
 
                         if platform.system() == "Darwin":
                             pass
```

### Comparing `linktest-2.0.8/lintest/timeout_thread.py` & `linktest-2.1.0/lintest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/ui_testcase.py` & `linktest-2.1.0/lintest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/update_config.py` & `linktest-2.1.0/lintest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.0.8/lintest/xml_report.py` & `linktest-2.1.0/lintest/xml_report.py`

 * *Files identical despite different names*

