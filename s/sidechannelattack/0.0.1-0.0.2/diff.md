# Comparing `tmp/sidechannelattack-0.0.1.tar.gz` & `tmp/sidechannelattack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sidechannelattack-0.0.1.tar", last modified: Tue Dec  6 12:49:42 2022, max compression
+gzip compressed data, was "dist\sidechannelattack-0.0.2.tar", last modified: Thu Jun  8 06:05:11 2023, max compression
```

## Comparing `sidechannelattack-0.0.1.tar` & `sidechannelattack-0.0.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/
--rw-rw-rw-   0        0        0      405 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        1 2022-12-06 12:44:19.000000 sidechannelattack-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      849 2022-12-06 12:48:38.000000 sidechannelattack-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/
--rw-rw-rw-   0        0        0     5993 2022-03-28 08:42:38.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/big_ttest.py
--rw-rw-rw-   0        0        0     4858 2021-12-24 02:13:28.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/cpa.py
--rw-rw-rw-   0        0        0     3050 2022-12-05 06:01:46.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/dpa.py
--rw-rw-rw-   0        0        0     3040 2022-12-06 11:35:04.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/modef_attack.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/aes/
--rw-rw-rw-   0        0        0    16073 2021-12-16 07:46:18.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/aes/funcs.py
--rw-rw-rw-   0        0        0     9036 2021-12-10 06:01:10.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/aes/key_schedule.py
--rw-rw-rw-   0        0        0        0 2021-05-04 06:23:44.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/aes/__init__.py
--rw-rw-rw-   0        0        0     5470 2021-12-16 08:04:30.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/base.py
--rw-rw-rw-   0        0        0    16044 2022-12-06 11:20:56.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/DES.py
--rw-rw-rw-   0        0        0     6523 2021-12-10 06:01:10.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/__init__.py
--rw-rw-rw-   0        0        0    24044 2022-11-21 04:48:02.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/model_attack.py
--rw-rw-rw-   0        0        0    10960 2021-12-24 10:20:14.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/new_math.py
--rw-rw-rw-   0        0        0     5276 2022-12-06 12:10:16.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/t_testlll.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/
--rw-rw-rw-   0        0        0     4275 2022-12-06 11:26:42.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/aes_cipher.py
--rw-rw-rw-   0        0        0    12470 2021-05-04 06:23:44.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/aes_tables.py
--rw-rw-rw-   0        0        0    39144 2022-12-06 11:26:42.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/parameter.py
--rw-rw-rw-   0        0        0    16912 2021-05-04 06:23:44.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/util.py
--rw-rw-rw-   0        0        0        0 2021-05-04 06:23:44.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/__init__.py
--rw-rw-rw-   0        0        0       64 2022-12-06 12:10:16.000000 sidechannelattack-0.0.1/sidechannelattack/attackmeasure/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/basetrace/
--rw-rw-rw-   0        0        0     2662 2022-12-06 11:26:42.000000 sidechannelattack-0.0.1/sidechannelattack/basetrace/base.py
--rw-rw-rw-   0        0        0     2100 2021-12-10 06:01:10.000000 sidechannelattack-0.0.1/sidechannelattack/basetrace/data_resolve.py
--rw-rw-rw-   0        0        0     1877 2021-12-24 10:38:18.000000 sidechannelattack-0.0.1/sidechannelattack/basetrace/get_intermediate_value.py
--rw-rw-rw-   0        0        0    10962 2022-12-06 11:31:51.000000 sidechannelattack-0.0.1/sidechannelattack/basetrace/new_math.py
--rw-rw-rw-   0        0        0      521 2021-10-12 09:12:06.000000 sidechannelattack-0.0.1/sidechannelattack/basetrace/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/data_visualization/
--rw-rw-rw-   0        0        0      504 2022-12-06 12:06:41.000000 sidechannelattack-0.0.1/sidechannelattack/data_visualization/plt_ttest.py
--rw-rw-rw-   0        0        0     7854 2022-12-06 11:43:50.000000 sidechannelattack-0.0.1/sidechannelattack/data_visualization/test.py
--rw-rw-rw-   0        0        0      168 2022-12-06 11:28:52.000000 sidechannelattack-0.0.1/sidechannelattack/data_visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/leakage_testing/
--rw-rw-rw-   0        0        0     4160 2022-12-06 12:24:43.000000 sidechannelattack-0.0.1/sidechannelattack/leakage_testing/correlation_test.py
--rw-rw-rw-   0        0        0     3214 2021-12-08 07:41:58.000000 sidechannelattack-0.0.1/sidechannelattack/leakage_testing/snr.py
--rw-rw-rw-   0        0        0     1211 2022-01-04 06:08:10.000000 sidechannelattack-0.0.1/sidechannelattack/leakage_testing/T_test.py
--rw-rw-rw-   0        0        0      168 2022-12-06 11:35:04.000000 sidechannelattack-0.0.1/sidechannelattack/leakage_testing/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/
--rw-rw-rw-   0        0        0     3854 2022-05-28 07:48:52.000000 sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/correlation.py
--rw-rw-rw-   0        0        0     2527 2022-05-28 09:10:46.000000 sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/pre_traces.py
--rw-rw-rw-   0        0        0     2257 2022-12-06 12:39:47.000000 sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/snr.py
--rw-rw-rw-   0        0        0     2871 2022-12-06 12:40:30.000000 sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/t-test.py
--rw-rw-rw-   0        0        0      154 2022-05-28 07:12:36.000000 sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/
--rw-rw-rw-   0        0        0     5501 2022-12-06 11:52:43.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/aligner.py
--rw-rw-rw-   0        0        0     1508 2022-12-06 11:26:42.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/base.py
--rw-rw-rw-   0        0        0        0 2021-12-06 12:59:48.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/demo.py
--rw-rw-rw-   0        0        0     1693 2022-12-06 11:47:39.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/fft.py
--rw-rw-rw-   0        0        0     4436 2022-12-06 12:13:34.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/filter.py
--rw-rw-rw-   0        0        0     1850 2021-12-01 13:19:02.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/find_peaks.py
--rw-rw-rw-   0        0        0     2148 2021-12-20 02:51:16.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/moving_average.py
--rw-rw-rw-   0        0        0     7518 2021-12-01 13:19:02.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/new_math.py
--rw-rw-rw-   0        0        0     7546 2022-05-02 03:30:08.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/pre_traces.py
--rw-rw-rw-   0        0        0     1311 2021-12-01 13:19:02.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/principal_component_analysis.py
--rw-rw-rw-   0        0        0     2481 2022-12-06 11:52:43.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/sample.py
--rw-rw-rw-   0        0        0     1097 2021-12-02 02:13:20.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/to_one.py
--rw-rw-rw-   0        0        0      230 2021-12-01 11:01:44.000000 sidechannelattack-0.0.1/sidechannelattack/pretrace/__init__.py
--rw-rw-rw-   0        0        0      275 2022-12-06 12:46:56.000000 sidechannelattack-0.0.1/sidechannelattack/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack.egg-info/
--rw-rw-rw-   0        0        0        1 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      405 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       62 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2463 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       18 2022-12-06 12:49:42.000000 sidechannelattack-0.0.1/sidechannelattack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:11.000000 sidechannelattack-0.0.2/
+-rw-rw-rw-   0        0        0     1076 2022-12-06 12:47:14.000000 sidechannelattack-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1001 2023-06-08 06:05:11.000000 sidechannelattack-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-06-08 05:49:55.000000 sidechannelattack-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 06:05:11.000000 sidechannelattack-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-06-08 03:48:44.000000 sidechannelattack-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/
+-rw-rw-rw-   0        0        0     5993 2022-03-28 08:42:38.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/big_ttest.py
+-rw-rw-rw-   0        0        0     4858 2021-12-24 02:13:28.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/cpa.py
+-rw-rw-rw-   0        0        0     3050 2022-12-05 06:01:46.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/dpa.py
+-rw-rw-rw-   0        0        0     3040 2022-12-06 11:35:06.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/modef_attack.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/aes/
+-rw-rw-rw-   0        0        0    16073 2021-12-16 07:46:18.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/aes/funcs.py
+-rw-rw-rw-   0        0        0     9036 2021-12-10 06:01:10.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/aes/key_schedule.py
+-rw-rw-rw-   0        0        0        0 2021-05-04 06:23:44.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/aes/__init__.py
+-rw-rw-rw-   0        0        0     5470 2021-12-16 08:04:30.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/base.py
+-rw-rw-rw-   0        0        0    16044 2022-12-06 11:20:58.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/DES.py
+-rw-rw-rw-   0        0        0     6523 2021-12-10 06:01:10.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/__init__.py
+-rw-rw-rw-   0        0        0    24044 2022-11-21 04:48:02.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/model_attack.py
+-rw-rw-rw-   0        0        0    10960 2021-12-24 10:20:14.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/new_math.py
+-rw-rw-rw-   0        0        0     5276 2022-12-06 12:10:18.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/t_testlll.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/
+-rw-rw-rw-   0        0        0     4275 2022-12-06 11:26:44.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/aes_cipher.py
+-rw-rw-rw-   0        0        0    12470 2021-05-04 06:23:44.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/aes_tables.py
+-rw-rw-rw-   0        0        0    39144 2022-12-06 11:26:44.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/parameter.py
+-rw-rw-rw-   0        0        0    16912 2021-05-04 06:23:44.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/util.py
+-rw-rw-rw-   0        0        0        0 2021-05-04 06:23:44.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/__init__.py
+-rw-rw-rw-   0        0        0       64 2022-12-06 12:10:18.000000 sidechannelattack-0.0.2/sidechannelattack/attackmeasure/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/basetrace/
+-rw-rw-rw-   0        0        0     2662 2022-12-06 11:26:44.000000 sidechannelattack-0.0.2/sidechannelattack/basetrace/base.py
+-rw-rw-rw-   0        0        0     2100 2021-12-10 06:01:10.000000 sidechannelattack-0.0.2/sidechannelattack/basetrace/data_resolve.py
+-rw-rw-rw-   0        0        0     1877 2021-12-24 10:38:18.000000 sidechannelattack-0.0.2/sidechannelattack/basetrace/get_intermediate_value.py
+-rw-rw-rw-   0        0        0    10962 2022-12-06 11:31:52.000000 sidechannelattack-0.0.2/sidechannelattack/basetrace/new_math.py
+-rw-rw-rw-   0        0        0      521 2021-10-12 09:12:06.000000 sidechannelattack-0.0.2/sidechannelattack/basetrace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/data_visualization/
+-rw-rw-rw-   0        0        0      504 2022-12-06 12:06:42.000000 sidechannelattack-0.0.2/sidechannelattack/data_visualization/plt_ttest.py
+-rw-rw-rw-   0        0        0     7854 2022-12-06 11:43:52.000000 sidechannelattack-0.0.2/sidechannelattack/data_visualization/test.py
+-rw-rw-rw-   0        0        0      168 2022-12-06 11:28:54.000000 sidechannelattack-0.0.2/sidechannelattack/data_visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack/leakage_testing/
+-rw-rw-rw-   0        0        0     4160 2022-12-06 12:24:44.000000 sidechannelattack-0.0.2/sidechannelattack/leakage_testing/correlation_test.py
+-rw-rw-rw-   0        0        0     3214 2021-12-08 07:41:58.000000 sidechannelattack-0.0.2/sidechannelattack/leakage_testing/snr.py
+-rw-rw-rw-   0        0        0     2647 2022-05-28 07:12:36.000000 sidechannelattack-0.0.2/sidechannelattack/leakage_testing/t-test.py
+-rw-rw-rw-   0        0        0     1211 2022-01-04 06:08:10.000000 sidechannelattack-0.0.2/sidechannelattack/leakage_testing/T_test.py
+-rw-rw-rw-   0        0        0      168 2022-12-06 11:35:06.000000 sidechannelattack-0.0.2/sidechannelattack/leakage_testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:11.000000 sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/
+-rw-rw-rw-   0        0        0     3854 2022-05-28 07:48:52.000000 sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/correlation.py
+-rw-rw-rw-   0        0        0     2527 2022-05-28 09:10:46.000000 sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/pre_traces.py
+-rw-rw-rw-   0        0        0     2257 2022-12-06 12:39:48.000000 sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/snr.py
+-rw-rw-rw-   0        0        0     2871 2023-05-15 09:34:11.000000 sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/t-test.py
+-rw-rw-rw-   0        0        0      154 2022-05-28 07:12:36.000000 sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:11.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/
+-rw-rw-rw-   0        0        0     5501 2022-12-06 11:52:44.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/aligner.py
+-rw-rw-rw-   0        0        0     1508 2022-12-06 11:26:44.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/base.py
+-rw-rw-rw-   0        0        0        0 2021-12-06 12:59:48.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/demo.py
+-rw-rw-rw-   0        0        0     1693 2022-12-06 11:47:40.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/fft.py
+-rw-rw-rw-   0        0        0     4436 2022-12-06 12:13:36.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/filter.py
+-rw-rw-rw-   0        0        0     1850 2021-12-01 13:19:02.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/find_peaks.py
+-rw-rw-rw-   0        0        0     2148 2021-12-20 02:51:16.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/moving_average.py
+-rw-rw-rw-   0        0        0     7518 2021-12-01 13:19:02.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/new_math.py
+-rw-rw-rw-   0        0        0     7546 2022-05-02 03:30:08.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/pre_traces.py
+-rw-rw-rw-   0        0        0     1311 2021-12-01 13:19:02.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/principal_component_analysis.py
+-rw-rw-rw-   0        0        0     2481 2022-12-06 11:52:44.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/sample.py
+-rw-rw-rw-   0        0        0     1097 2021-12-02 02:13:20.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/to_one.py
+-rw-rw-rw-   0        0        0      230 2021-12-01 11:01:44.000000 sidechannelattack-0.0.2/sidechannelattack/pretrace/__init__.py
+-rw-rw-rw-   0        0        0      275 2022-12-06 12:46:58.000000 sidechannelattack-0.0.2/sidechannelattack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1001 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2515 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 06:05:10.000000 sidechannelattack-0.0.2/sidechannelattack.egg-info/top_level.txt
```

### Comparing `sidechannelattack-0.0.1/setup.py` & `sidechannelattack-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md",'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "sidechannelattack",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "yangsu ",
     author_email = "1152036203@qq.com",
     description = "sidechannelattack",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     # url="https://github.com/tqthooo2021/Create-Own-Python-Package",
     packages=setuptools.find_packages(),
```

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/big_ttest.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/big_ttest.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/cpa.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/cpa.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/dpa.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/dpa.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/modef_attack.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/modef_attack.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/aes/funcs.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/aes/funcs.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/aes/key_schedule.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/aes/key_schedule.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/base.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/base.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/DES.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/DES.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/models/__init__.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/model_attack.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/model_attack.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/new_math.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/new_math.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/t_testlll.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/t_testlll.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/aes_cipher.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/aes_cipher.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/aes_tables.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/aes_tables.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/parameter.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/attackmeasure/utils/util.py` & `sidechannelattack-0.0.2/sidechannelattack/attackmeasure/utils/util.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/basetrace/base.py` & `sidechannelattack-0.0.2/sidechannelattack/basetrace/base.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/basetrace/data_resolve.py` & `sidechannelattack-0.0.2/sidechannelattack/basetrace/data_resolve.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/basetrace/get_intermediate_value.py` & `sidechannelattack-0.0.2/sidechannelattack/basetrace/get_intermediate_value.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/basetrace/new_math.py` & `sidechannelattack-0.0.2/sidechannelattack/basetrace/new_math.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/basetrace/__init__.py` & `sidechannelattack-0.0.2/sidechannelattack/basetrace/__init__.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/data_visualization/test.py` & `sidechannelattack-0.0.2/sidechannelattack/data_visualization/test.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/leakage_testing/correlation_test.py` & `sidechannelattack-0.0.2/sidechannelattack/leakage_testing/correlation_test.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/leakage_testing/snr.py` & `sidechannelattack-0.0.2/sidechannelattack/leakage_testing/snr.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/leakage_testing/T_test.py` & `sidechannelattack-0.0.2/sidechannelattack/leakage_testing/T_test.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/correlation.py` & `sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/correlation.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/pre_traces.py` & `sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/pre_traces.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/snr.py` & `sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/snr.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/n_leakage_testing/t-test.py` & `sidechannelattack-0.0.2/sidechannelattack/n_leakage_testing/t-test.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,26 +14,26 @@
     '''
     :instrctions:even  and  odd 间或采集
     :param n: blocks of traces
     :param N: sample numbers
     :return: result
     '''
     # arr = np.load(url_trace + r"2process_arrPart0.npy")
-    arr = np.load(url_trace + trace_name + r"0.npy")
+    arr = np.load(url_trace + trace_name + r".npy")
     count = 0
     N = arr.shape[1]
     old_var_even = np.zeros(N)
     old_mean_even = np.zeros(N)
     old_var_odd = np.zeros(N)
     old_mean_odd = np.zeros(N)
     oddcount = 0
     evencount = 0
     for j in trange(n):
         # arr = np.load(url_trace + r"2process_arrPart{0}.npy".format(j))
-        arr = np.load(url_trace + trace_name + r"{0}.npy".format(j))
+        arr = np.load(url_trace + trace_name + r".npy")
         for i in range(arr.shape[0]):
             if count % 2 == 0:
                 new_mean = old_mean_even + (arr[i] - old_mean_even) / (evencount + 1)
                 new_var = old_var_even + ((arr[i] - old_mean_even) * (arr[i] - new_mean) - old_var_even) / (
                         evencount + 1)
                 old_mean_even = new_mean
                 old_var_even = new_var
@@ -68,18 +68,18 @@
     result = t_test(num_file_blocks, url_trace, trace_name)
     ax.plot(result)
     plt.show()
 
 if __name__ == '__main__':
 
     # 文件路径
-    # url_trace = r"H:/zhoujiayun1/"
+    url_trace = r"C:/Users/DELL/Desktop/"
     # 文件块数
-    num_file_blocks = 100
+    num_file_blocks = 1
     # 文件名字
-    trace_name = "arrPart"
+    trace_name = "AES_DPA_ATTACK_trace"
     # 运行函数
-    # ttest_function(num_file_blocks, url_trace, trace_name)
+    ttest_function(num_file_blocks, url_trace, trace_name)
```

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/aligner.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/aligner.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/base.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/base.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/fft.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/fft.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/filter.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/filter.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/find_peaks.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/find_peaks.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/moving_average.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/moving_average.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/new_math.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/new_math.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/pre_traces.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/pre_traces.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/principal_component_analysis.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/principal_component_analysis.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/sample.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/sample.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack/pretrace/to_one.py` & `sidechannelattack-0.0.2/sidechannelattack/pretrace/to_one.py`

 * *Files identical despite different names*

### Comparing `sidechannelattack-0.0.1/sidechannelattack.egg-info/SOURCES.txt` & `sidechannelattack-0.0.2/sidechannelattack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 sidechannelattack/__init__.py
 sidechannelattack.egg-info/PKG-INFO
 sidechannelattack.egg-info/SOURCES.txt
 sidechannelattack.egg-info/dependency_links.txt
 sidechannelattack.egg-info/requires.txt
@@ -33,14 +34,15 @@
 sidechannelattack/data_visualization/__init__.py
 sidechannelattack/data_visualization/plt_ttest.py
 sidechannelattack/data_visualization/test.py
 sidechannelattack/leakage_testing/T_test.py
 sidechannelattack/leakage_testing/__init__.py
 sidechannelattack/leakage_testing/correlation_test.py
 sidechannelattack/leakage_testing/snr.py
+sidechannelattack/leakage_testing/t-test.py
 sidechannelattack/n_leakage_testing/__init__.py
 sidechannelattack/n_leakage_testing/correlation.py
 sidechannelattack/n_leakage_testing/pre_traces.py
 sidechannelattack/n_leakage_testing/snr.py
 sidechannelattack/n_leakage_testing/t-test.py
 sidechannelattack/pretrace/__init__.py
 sidechannelattack/pretrace/aligner.py
```

