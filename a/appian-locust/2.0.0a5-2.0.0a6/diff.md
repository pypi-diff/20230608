# Comparing `tmp/appian-locust-2.0.0a5.tar.gz` & `tmp/appian-locust-2.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0a5.tar", last modified: Wed May 24 15:50:10 2023, max compression
+gzip compressed data, was "appian-locust-2.0.0a6.tar", last modified: Thu Jun  8 19:11:07 2023, max compression
```

## Comparing `appian-locust-2.0.0a5.tar` & `appian-locust-2.0.0a6.tar`

### file list

```diff
@@ -1,88 +1,57 @@
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.885844 appian-locust-2.0.0a5/
--rw-r--r--   0 harry.wilton   (502) staff       (20)    11358 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/LICENSE
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-24 15:50:10.885990 appian-locust-2.0.0a5/PKG-INFO
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4829 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/README.rst
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.858313 appian-locust-2.0.0a5/appian_locust/
--rw-r--r--   0 harry.wilton   (502) staff       (20)      775 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/__init__.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     9541 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_actions.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      786 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_admin.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2479 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_base.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6282 2023-05-23 17:47:36.000000 appian-locust-2.0.0a5/appian_locust/_design.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6206 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_feature_toggle_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7830 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_grid_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    53252 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5171 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_locust_error_handler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7765 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_news.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1025 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_portals.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    16297 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_records.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7380 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_records_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7185 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_reports.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     3016 2023-04-27 17:42:07.000000 appian-locust-2.0.0a5/appian_locust/_save_request_builder.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     9934 2023-05-23 18:03:22.000000 appian-locust-2.0.0a5/appian_locust/_sites.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4514 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_task_opener.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7644 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/_tasks.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2365 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/appian_locust/_ui_reconciler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1372 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/actions_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    14485 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/appianclient.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      354 2023-05-23 17:55:37.000000 appian-locust-2.0.0a5/appian_locust/application.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     3950 2023-05-24 15:47:33.000000 appian-locust-2.0.0a5/appian_locust/application_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      358 2023-05-23 17:55:55.000000 appian-locust-2.0.0a5/appian_locust/design_object.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      205 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/design_object_type.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1068 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/design_object_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6234 2023-05-23 17:47:36.000000 appian-locust-2.0.0a5/appian_locust/design_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      859 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/appian_locust/exceptions.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1792 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/feature_flag.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    16278 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/helper.py
--rwxr-xr-x   0 harry.wilton   (502) staff       (20)     1431 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/loadDriverUtils.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      862 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/logger.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2749 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/news_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1941 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/record_list_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1320 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/record_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      547 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/records_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1546 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/reports_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1364 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/site_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      990 2023-05-23 17:57:12.000000 appian-locust-2.0.0a5/appian_locust/site_objects.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1261 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/sites_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1406 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/tasks_info.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2504 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/tempo_navigator.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    73573 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/appian_locust/uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    13980 2023-05-23 18:00:11.000000 appian-locust-2.0.0a5/appian_locust/visitor.py
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.863019 appian-locust-2.0.0a5/appian_locust.egg-info/
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5403 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2293 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)        1 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)       15 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/requires.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)       14 2023-05-24 15:50:10.000000 appian-locust-2.0.0a5/appian_locust.egg-info/top_level.txt
--rw-r--r--   0 harry.wilton   (502) staff       (20)      100 2023-02-28 19:42:15.000000 appian-locust-2.0.0a5/pyproject.toml
--rw-r--r--   0 harry.wilton   (502) staff       (20)      595 2023-05-24 15:50:10.886654 appian-locust-2.0.0a5/setup.cfg
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1088 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/setup.py
-drwxr-xr-x   0 harry.wilton   (502) staff       (20)        0 2023-05-24 15:50:10.885221 appian-locust-2.0.0a5/tests/
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6106 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_actions.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1053 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_admin.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6785 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_app_importer.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    11018 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_appianclient.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1667 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_application_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2981 2023-05-23 17:50:15.000000 appian-locust-2.0.0a5/tests/test_design.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1632 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_design_object_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2596 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_design_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    12722 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_feature_toggle_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     7834 2022-06-20 13:00:59.000000 appian-locust-2.0.0a5/tests/test_grid_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2936 2022-06-08 19:05:09.000000 appian-locust-2.0.0a5/tests/test_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    19580 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_interactor.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1458 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_libraries_utils.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      891 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_locust_error_handler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4727 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_news.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2391 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_portals.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     1844 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_record_list_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4349 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_record_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    13429 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_records.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2334 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_records_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     5554 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_reports.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     3664 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_save_request_builder.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2257 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_site_helper.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     6304 2023-05-23 18:01:25.000000 appian-locust-2.0.0a5/tests/test_sites.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     4184 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_tasks.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)     2360 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_ui_reconciler.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    61599 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_uiform.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)      784 2022-02-17 16:44:14.000000 appian-locust-2.0.0a5/tests/test_utils.py
--rw-r--r--   0 harry.wilton   (502) staff       (20)    22517 2023-05-22 19:20:22.000000 appian-locust-2.0.0a5/tests/test_visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:11:07.367953 appian-locust-2.0.0a6/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-06-08 19:11:07.367953 appian-locust-2.0.0a6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4829 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:11:07.366952 appian-locust-2.0.0a6/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9573 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6282 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    53252 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5171 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7789 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    16614 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7464 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9934 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4514 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    14940 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/appianclient.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     3950 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_object_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/feature_flag.py
+-rw-rw-rw-   0 root         (0) root         (0)    16346 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1431 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/site_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/site_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/tasks_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2211 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/tempo_navigator.py
+-rw-rw-rw-   0 root         (0) root         (0)    73573 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    15051 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:11:07.367953 appian-locust-2.0.0a6/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 19:11:07.000000 appian-locust-2.0.0a6/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-08 19:11:07.368953 appian-locust-2.0.0a6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-08 19:10:58.000000 appian-locust-2.0.0a6/setup.py
```

### Comparing `appian-locust-2.0.0a5/LICENSE` & `appian-locust-2.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/PKG-INFO` & `appian-locust-2.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a5
+Version: 2.0.0a6
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a5/README.rst` & `appian-locust-2.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/__init__.py` & `appian-locust-2.0.0a6/appian_locust/__init__.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_actions.py` & `appian-locust-2.0.0a6/appian_locust/_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,21 +54,22 @@
         if self.interactor.url_pattern_version == 1:
             uri += "p."
         uri += ACTIONS_NAV_PATH[1] + ACTIONS_NAV_PATH[2]
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Nav')
         return resp.json()
 
-    def get_actions_feed(self, locust_request_label: str = "Actions.Feed") -> Dict[str, Any]:
+    def get_actions_feed(self, locust_request_label: str = "Actions") -> Dict[str, Any]:
         uri = self.interactor.host + ACTIONS_FEED_PATH
         headers = self.interactor.setup_feed_headers()
-        resp = self.interactor.get_page(uri, headers, locust_request_label)
+        resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Feed')
         return resp.json()
 
-    def get_all(self, search_string: Optional[str] = None, locust_request_label: str = "Actions") -> Dict[str, Any]:
+    def get_all(self, search_string: Optional[str] = None,
+                locust_request_label: str = "Actions.MainMenu.AvailableActions") -> Dict[str, Any]:
         """
         Retrieves all the available "actions" and associated metadata from "Appian-Tempo-Actions"
 
         Note: All the retrieved data about actions is stored in the private variable self._actions
 
         Returns (dict): List of actions and associated metadata
 
@@ -84,15 +85,15 @@
             self.get_actions_feed(locust_request_label=locust_request_label)
         except Exception as e:
             log_locust_error(e, error_desc="Response Error", raise_error=False)
 
         headers = self.interactor.setup_request_headers(self.interactor.host + ACTIONS_ALL_PATH)
 
         resp = self.interactor.get_page(
-            self.interactor.host + ACTIONS_ALL_PATH, headers=headers, label="Actions.MainMenu.AvailableActions"
+            self.interactor.host + ACTIONS_ALL_PATH, headers=headers, label=locust_request_label
         )
         self._actions = dict()
         error_key_string = "ERROR::"
         error_key_count = 0
         try:
             json_resp = resp.json()[0]
             for current_action in json_resp["actions"]:
```

### Comparing `appian-locust-2.0.0a5/appian_locust/_admin.py` & `appian-locust-2.0.0a6/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_base.py` & `appian-locust-2.0.0a6/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_design.py` & `appian-locust-2.0.0a6/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.0a6/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_grid_interactor.py` & `appian-locust-2.0.0a6/appian_locust/_grid_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_interactor.py` & `appian-locust-2.0.0a6/appian_locust/_interactor.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.0a6/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_news.py` & `appian-locust-2.0.0a6/appian_locust/_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Examples:
 
             >>> self.appian.action.get_all()
 
         """
         if search_string:
             uri = NEWS_SEARCH_PATH + search_string
-            label = "News.Search." + search_string
+            label = locust_request_label or "News.Search." + search_string
         else:
             uri = NEWS_FEED_PATH
             label = locust_request_label or "News.Feed"
 
         self._news = dict()
         error_key_string = "ERROR::"
         error_key_count = 0
```

### Comparing `appian-locust-2.0.0a5/appian_locust/_portals.py` & `appian-locust-2.0.0a6/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_records.py` & `appian-locust-2.0.0a6/appian_locust/_records.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,21 +39,21 @@
         self.interactor = interactor
 
         # When Get All functions called, these variables will be used to cache the values
         self._record_types: Dict[str, Any] = dict()
         self._records: Dict[str, Any] = dict()
         self._errors: int = 0
 
-    def get_records_interface(self, locust_request_label: str = "Records") -> Dict[str, Any]:
+    def get_records_interface(self, locust_request_label: Optional[str] = "Records") -> Dict[str, Any]:
         uri = self.interactor.host + RECORDS_INTERFACE_PATH
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Interface')
         return resp.json()
 
-    def get_records_nav(self, locust_request_label: str = "Records") -> Dict[str, Any]:
+    def get_records_nav(self, locust_request_label: Optional[str] = "Records") -> Dict[str, Any]:
         uri = self.interactor.host + RECORDS_NAV_PATH[0]
         if self.interactor.url_pattern_version == 1:
             uri += "p."
         uri += RECORDS_NAV_PATH[1] + RECORDS_NAV_PATH[2]
         headers = self.interactor.setup_sail_headers()
         resp = self.interactor.get_page(uri, headers, f'{locust_request_label}.Nav')
         return resp.json()
@@ -93,16 +93,14 @@
 
         Returns (dict): List of record types and associated metadata
         """
 
         json_response = self.fetch_all_records_json(locust_request_label)
 
         self._record_types = get_all_record_types_from_json(json_response)
-        for title in self._record_types.keys():
-            self._records[title] = dict()
 
         return self._record_types
 
     def fetch_all_records_json(self, locust_request_label: str = "Records") -> Dict[str, Any]:
         uri = RECORDS_ALL_PATH
 
         headers = self.interactor.setup_request_headers()
@@ -123,14 +121,15 @@
 
         Returns (dict): List of records and associated metadata
 
         Examples:
 
             >>> self.appian.records.get_all_records_of_record_type("record_type_name")
         """
+        self._records[record_type] = dict()
 
         json_response = self._record_type_list_request(record_type, search_string=search_string)
 
         if column_index is not None:
             self._records[record_type], self._errors = get_records_from_json_by_column(json_response, column_index)
         else:
             self._records[record_type], self._errors = get_all_records_from_json(json_response)
@@ -228,15 +227,15 @@
 
         """
         _, current_record_type = super().get(self._record_types, record_type, exact_match)
         if not current_record_type:
             raise Exception(f"There is no record type with name {record_type} in the system under test (Exact match = {exact_match})")
         return current_record_type
 
-    def visit_record_instance(self, record_type: str = "", record_name: str = "", view_url_stub: str = "", exact_match: bool = True, locust_request_label: str = "") -> Dict[str, Any]:
+    def visit_record_instance(self, record_type: str = "", record_name: str = "", view_url_stub: str = "", exact_match: bool = True, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
         """
         This function calls the API for the specific record view/instance to get its response data.
 
         Note: This function is meant to only traverse to Record forms, not to interact with them. For that, use visit_record_instance_and_get_form()
 
         Args:
             record_type (str): Record Type Name. If not specified, a random record type will be selected.
@@ -291,15 +290,15 @@
         uri = f"{RECORD_VIEW_PATH[0]}{tempo_site_url_stub}{RECORD_VIEW_PATH[1]}{opaque_id}{RECORD_VIEW_PATH[2]}{view_url_stub}"
         resp = self.interactor.get_page(uri=uri, headers=headers, label=locust_label)
         return resp.json()
 
     # Alias for the above function to allow backwards compatability
     visit = visit_record_instance
 
-    def visit_record_type(self, record_type: str = "", exact_match: bool = True, is_mobile: bool = False) -> Dict[str, Any]:
+    def visit_record_type(self, record_type: str = "", exact_match: bool = True, is_mobile: bool = False, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
         """
         Navigate into desired record type and retrieve all metadata for associated list of record views.
 
         Returns (dict): List of records and associated metadata
 
         Examples:
 
@@ -310,15 +309,17 @@
         if not self._records or not self._record_types:
             self.get_all()
 
         # If no record_type is specified, a random one will be assigned
         if not record_type:
             record_type = self._get_random_record_type()
 
-        return self._record_type_list_request(record_type, is_mobile=is_mobile)
+        locust_request_label = locust_request_label or f'Records.{record_type}.ListView'
+
+        return self._record_type_list_request(record_type, is_mobile=is_mobile, locust_request_label=locust_request_label)
 
     # ----- Private Functions ----- #
 
     def _is_response_good(self, response_text: str) -> bool:
         return ('"rel":"x-web-bookmark"' in response_text or '"#t":"CardLayout"' in response_text)
 
     def _get_random_record_instance(self, record_type: str = "") -> Tuple[str, str]:
@@ -330,20 +331,22 @@
         return record_type, record_name
 
     def _get_random_record_type(self) -> str:
         if not self._records or not self._record_types:
             self.get_all()
         return random.choice(list(self._records.keys()))
 
-    def _record_type_list_request(self, record_type: str, is_mobile: bool = False, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def _record_type_list_request(self, record_type: str, is_mobile: bool = False, search_string: Optional[str] = None,
+                                  locust_request_label: Optional[str] = None) -> Dict[str, Any]:
         if record_type not in self._record_types:
             raise Exception(f"There is no record type with name {record_type} in the system under test")
         record_type_component = self._record_types[record_type]
         record_type_url_stub = record_type_component['link']['value']['urlstub']
-        return self.fetch_record_type_json(record_type_url_stub, is_mobile, search_string, f"Records.{record_type}")
+        locust_request_label = locust_request_label or f"Records.{record_type}"
+        return self.fetch_record_type_json(record_type_url_stub, is_mobile, search_string, locust_request_label)
 
     def fetch_record_type_json(self, record_type_url_stub: str, is_mobile: bool = False, search_string: Optional[str] = None, label: Optional[str] = None) -> Dict[str, Any]:
         if not label:
             label = f"Records.{record_type_url_stub}"
         if is_mobile:
             uri = self._get_mobile_records_uri(record_type_url_stub)
         else:
```

### Comparing `appian-locust-2.0.0a5/appian_locust/_records_helper.py` & `appian-locust-2.0.0a6/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_reports.py` & `appian-locust-2.0.0a6/appian_locust/_reports.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,21 +130,22 @@
         if not current_report:
             _, current_report = super().get(self._reports, report_name, exact_match, search_string=report_name)
         if not current_report:
             raise (Exception("There is no report with name {} in the system under test (Exact match = {})".format(
                 report_name, exact_match)))
         return current_report
 
-    def fetch_report_json(self, report_name: str, exact_match: bool = True) -> Dict[str, Any]:
+    def fetch_report_json(self, report_name: str, exact_match: bool = True, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
         """
         This function calls the API for the specific report to get its "form" data
 
         Args:
             report_name (str): Name of the report to be called.
             exact_match (bool, optional): Should report name match exactly or to be partial match. Default : True
+            locust_request_label (str, optional): Label locust should associate this request with
 
         Returns (dict): Response of report's Get UI call in dictionary
 
         Examples:
 
             If full name of report is known,
 
@@ -160,14 +161,17 @@
         headers["Accept"] = "application/vnd.appian.tv.ui+json"
 
         # navigation request
         uri = REPORTS_NAV_PATH[0]
         if self.interactor.url_pattern_version == 1:
             uri += "p."
         uri += REPORTS_NAV_PATH[1] + REPORTS_NAV_PATH[2]
-        label = "Reports.Nav." + format_label(report_name, "::", 0)
-        self.interactor.get_page(uri=uri, headers=headers, label=label)  # report request
-        label = "Reports.GetUi." + format_label(report_name, "::", 0)
+        if locust_request_label:
+            nav_label = f"{locust_request_label}.Nav"
+        else:
+            nav_label = "Reports.Nav." + format_label(report_name, "::", 0)
+        self.interactor.get_page(uri=uri, headers=headers, label=nav_label)  # report request
+        label = locust_request_label or "Reports.GetUi." + format_label(report_name, "::", 0)
         resp = self.interactor.get_page(uri=form_uri, headers=headers, label=label)
         test_response_for_error(resp)
         resp.raise_for_status()
         return resp.json()
```

### Comparing `appian-locust-2.0.0a5/appian_locust/_save_request_builder.py` & `appian-locust-2.0.0a6/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_sites.py` & `appian-locust-2.0.0a6/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_task_opener.py` & `appian-locust-2.0.0a6/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_tasks.py` & `appian-locust-2.0.0a6/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.0a6/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/actions_info.py` & `appian-locust-2.0.0a6/appian_locust/actions_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 
 
 class ActionsInfo:
 
     def __init__(self, actions: _Actions):
         self.__actions = actions
 
-    def get_all_available_actions(self) -> Dict[str, Any]:
+    def get_all_available_actions(self, locust_request_label_breadcrumb: str = "Actions.MainMenu.AvailableActions") -> Dict[str, Any]:
         """
         Retrieves all the available "actions" and associated metadata from "Appian-Tempo-Actions"
 
+        Args:
+            locust_request_label_breadcrumb (str): Base label used for each of the multiple requests made by this method
+
         Returns (dict): List of actions and associated metadata
 
         Examples:
 
             >>> actions_info.get_all_available_actions()
 
         """
-        return self.__actions.get_all()
+        return self.__actions.get_all(locust_request_label=locust_request_label_breadcrumb)
 
     def get_action_info(self, action_name: str, exact_match: bool = False) -> Dict[str, Any]:
         """
         Get the information about specific action by name.
 
         Args:
             action_name (str): Name of the action
```

### Comparing `appian-locust-2.0.0a5/appian_locust/appianclient.py` & `appian-locust-2.0.0a6/appian_locust/appianclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from .feature_flag import FeatureFlag
 from ._feature_toggle_helper import (get_client_feature_toggles,
                                      override_default_feature_flags,
                                      set_mobile_feature_flags)
 from ._interactor import _Interactor
 from ._locust_error_handler import log_locust_error
 from .exceptions import MissingConfigurationException
+from ._actions import _Actions
+from ._records import _Records
+from ._reports import _Reports
+from ._sites import _Sites
+from ._tasks import _Tasks
 from .tempo_navigator import TempoNavigator
 from .visitor import Visitor
 from .site_helper import SiteHelper
 
 log = logger.getLogger(__name__)
 
 
@@ -140,18 +145,23 @@
             host (str): Host URL
 
         """
         self.client = session
         self.portals_mode = portals_mode
         self.host = _trim_trailing_slash(host)
         self._interactor = _Interactor(self.client, self.host, portals_mode=portals_mode)
-
-        self._visitor = Visitor(self._interactor)
-        self._site_helper = SiteHelper(self._interactor)
-        self._tempo_navigator = TempoNavigator(self._interactor)
+        actions = _Actions(self._interactor)
+        tasks = _Tasks(self._interactor)
+        reports = _Reports(self._interactor)
+        records = _Records(self._interactor)
+        sites = _Sites(self._interactor)
+
+        self._visitor = Visitor(self._interactor, tasks, reports, actions, records, sites)
+        self._site_helper = SiteHelper(self._interactor, actions)
+        self._tempo_navigator = TempoNavigator(self._interactor, tasks, reports, actions, records, sites)
 
         # Adding a few session specific attributes to self.client to that it can be carried and handled by session
         # in case of having multiple sessions in the future.
         setattr(self.client, "feature_flag", "")
         setattr(self.client, "feature_flag_extended", "")
 
         # Used for sites where /suite is not in the URL, i.e. local builds
```

### Comparing `appian-locust-2.0.0a5/appian_locust/application_uiform.py` & `appian-locust-2.0.0a6/appian_locust/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/design_object_uiform.py` & `appian-locust-2.0.0a6/appian_locust/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/design_uiform.py` & `appian-locust-2.0.0a6/appian_locust/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/exceptions.py` & `appian-locust-2.0.0a6/appian_locust/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/feature_flag.py` & `appian-locust-2.0.0a6/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/helper.py` & `appian-locust-2.0.0a6/appian_locust/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,16 @@
 
     Returns:
         List with filtered values
 
     """
     # Exact Matches gets priority even when exact match is set to false
     return_list = list(filter(lambda current_item: (
-        current_item.split("::")[0] == filter_string), list_var))
+        current_item == filter_string if "::" in filter_string else current_item.split("::")[0] == filter_string),
+        list_var))
     if not exact_match:
         return_list.extend(list(filter(lambda current_item: (
             bool(re.search(".*" + re.escape(filter_string) + ".*", current_item)) and current_item not in return_list),
             list_var)))
     return return_list
```

### Comparing `appian-locust-2.0.0a5/appian_locust/loadDriverUtils.py` & `appian-locust-2.0.0a6/appian_locust/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/logger.py` & `appian-locust-2.0.0a6/appian_locust/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/news_info.py` & `appian-locust-2.0.0a6/appian_locust/news_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+from requests.models import Response
 from typing import Any, Dict, Optional, Tuple
 
 from ._interactor import _Interactor
 from ._news import _News
 
 
 class NewsInfo:
     """
     Class which provides metadata about news entries from the Tempo News tab
     """
 
-    def __init__(self, interactor: _Interactor):
-        self.__news = _News(interactor)
+    def __init__(self, news: _News):
+        self.__news = news
 
-    def get_all_available_entries(self, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def get_all_available_entries(self, search_string: Optional[str] = None,
+                                  locust_request_label: str = "News.AllAvailableEntries") -> Dict[str, Any]:
         """
         Retrieves all the available "news" and associated metadata from "Appian-Tempo-News"
 
         Args:
             search_string(str, optional): results will be filtered based on the search string.
+            locust_request_label (str): Label locust should associate with the request
 
         Returns (dict): List of news and associated metadata
 
         Examples:
 
             >>> news_info.get_all()
         """
-        return self.__news.get_all(search_string=search_string)
+        return self.__news.get_all(search_string=search_string, locust_request_label=locust_request_label)
 
     def get_news(self, news_name: str, exact_match: bool = True, search_string: Optional[str] = None) -> Dict[str, Any]:
         """
         Get the information about specific news by name.
 
         Args:
             news_name (str): name of the news entry
@@ -71,7 +74,28 @@
             >>> news_info.visit_news_entry("news_name")
 
             If only partial name is known,
 
             >>> news_info.visit_news_entry("news_n", exact_match=False)
         """
         return self.__news.visit_news_entry(news_name, exact_match, search_string)
+
+    def get_news_entry_related_records(self, news_name: str, exact_match: bool = True,
+                                       search_string: Optional[str] = None,
+                                       locust_request_label: Optional[str] = None) -> Optional[Response]:
+        """
+        Request related records information for a news entry
+        Args:
+            news_name (str): name of the news entry
+            exact_match (bool, optional): Should news name match exactly or to be partial match. Default : True
+            search_string (str, optional): results will be filtered based on the search string.
+            locust_request_label (str, optional): Label locust should associate with the request for related records
+
+        Returns: Response object with related records information, if any exists
+
+        """
+        locust_request_label = locust_request_label or f"News.Entry.{news_name}.RelatedRecords"
+        news_entry = self.__news.get_news(news_name, exact_match, search_string)
+        for link in news_entry['links']:
+            if 'newsRelatedRecords' in link['href']:
+                return self.__news.interactor.get_page(link['href'], label=locust_request_label)
+        return None
```

### Comparing `appian-locust-2.0.0a5/appian_locust/record_list_uiform.py` & `appian-locust-2.0.0a6/appian_locust/record_list_uiform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 from urllib.parse import quote
 
 from ._interactor import _Interactor
-from ._records_helper import get_all_records_from_json
+from ._records_helper import get_all_records_from_json, get_records_from_json_by_column
 from .uiform import SailUiForm
 
 
 class RecordListUiForm(SailUiForm):
     """
     UiForm representing a Record List from Tempo Records
     """
@@ -35,10 +35,34 @@
         context_label = locust_request_label or f"{self.breadcrumb}.RecordType.SearchByText"
         search_uri = f"{self.form_url}?searchTerm={quote(search_term)}"
 
         headers = self._interactor.setup_sail_headers()
         response = self._interactor.get_page(uri=search_uri, headers=headers, label=context_label)
         return RecordListUiForm(self._interactor, response.json(), breadcrumb=context_label)
 
-    def get_visible_record_instances(self) -> Dict[str, Any]:
-        record_instances, _ = get_all_records_from_json(self._state)
+    def clear_records_search_filters(self) -> 'RecordListUiForm':
+        """
+        Clear any search filters on the records list
+
+        Returns: Unfiltered RecordsListUiForm
+        """
+        context_label = f"{self.breadcrumb}.RecordType.ClearFilters"
+        clear_uri = self.form_url
+
+        headers = self._interactor.setup_sail_headers()
+        response = self._interactor.get_page(uri=clear_uri, headers=headers, label=context_label)
+        return RecordListUiForm(self._interactor, response.json(), breadcrumb=context_label)
+
+    def get_visible_record_instances(self, column_index: Optional[int] = None) -> Dict[str, Any]:
+        """
+        Retrieve information about all visible records on the page.
+        Args:
+            column_index: Which column to retrieve record information for. If no column is selected, every record link
+                          in the UI will be retrieved
+
+        Returns: Dictionary with record instance information
+        """
+        if column_index is not None:
+            record_instances, _ = get_records_from_json_by_column(self._state, column_index)
+        else:
+            record_instances, _ = get_all_records_from_json(self._state)
         return record_instances
```

### Comparing `appian-locust-2.0.0a5/appian_locust/record_uiform.py` & `appian-locust-2.0.0a6/appian_locust/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/reports_info.py` & `appian-locust-2.0.0a6/appian_locust/reports_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,27 @@
     """
     Class which provides metadata about available reports from the Tempo Reports tab
     """
 
     def __init__(self, reports: _Reports):
         self.__reports = reports
 
-    def get_all_available_reports(self, search_string: Optional[str] = None) -> Dict[str, Any]:
+    def get_all_available_reports(self, search_string: Optional[str] = None, locust_request_label: Optional[str] = None) -> Dict[str, Any]:
         """
         Retrieves all the available "reports" and associated metadata from "Appian-Tempo-Reports"
 
         Returns (dict): List of reports and associated metadata
 
         Examples:
 
             >>> reports_info.get_all_available_reports()
 
         """
-        return self.__reports.get_all(search_string=search_string)
+        locust_request_label = locust_request_label or "Reports.Available.All"
+        return self.__reports.get_all(search_string=search_string, locust_request_label=locust_request_label)
 
     def get_report_info(self, report_name: str, exact_match: bool = True) -> Dict[str, Any]:
         """
         Get the information about specific report by name.
 
         Args:
             report_name (str): Name of the action
```

### Comparing `appian-locust-2.0.0a5/appian_locust/site_objects.py` & `appian-locust-2.0.0a6/appian_locust/site_objects.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/sites_info.py` & `appian-locust-2.0.0a6/appian_locust/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/tasks_info.py` & `appian-locust-2.0.0a6/appian_locust/tasks_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,26 +7,29 @@
     """
     Class which provides metadata about available tasks from the Tempo Tasks tab
     """
 
     def __init__(self, tasks: _Tasks):
         self.__tasks = tasks
 
-    def get_all_available_tasks(self) -> Dict[str, Any]:
+    def get_all_available_tasks(self, locust_request_label: str = "Tasks.MainMenu.GetAllAvailable") -> Dict[str, Any]:
         """
         Retrieves all the available "tasks" and associated metadata from "Appian-Tempo-Tasks"
 
+        Args:
+            locust_request_label (str): Label locust should associate with the request
+
         Returns (dict): List of tasks and associated metadata
 
         Examples:
 
             >>> tasks_info.get_all_available_tasks()
 
         """
-        return self.__tasks.get_all()
+        return self.__tasks.get_all(locust_request_label=locust_request_label)
 
     def get_task_info(self, task_name: str, exact_match: bool = True) -> Dict[str, Any]:
         """
         Get the information about specific task by name.
 
         Args:
             task_name (str): Name of the action
```

### Comparing `appian-locust-2.0.0a5/appian_locust/tempo_navigator.py` & `appian-locust-2.0.0a6/appian_locust/tempo_navigator.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,49 +2,46 @@
 from .actions_info import ActionsInfo
 from .records_info import RecordsInfo
 from .reports_info import ReportsInfo
 from .sites_info import SitesInfo
 from .tasks_info import TasksInfo
 from ._actions import _Actions
 from ._interactor import _Interactor
-from ._locust_error_handler import log_locust_error
+from ._news import _News
 from ._records import _Records
 from ._reports import _Reports
 from ._sites import _Sites
 from ._tasks import _Tasks
 
 
 class TempoNavigator:
     """
     Used for navigating the primary tabs on tempo to provide metadata on the content available for interaction.
     """
 
-    def __init__(self, interactor: _Interactor):
+    def __init__(self, interactor: _Interactor, tasks: _Tasks, reports: _Reports, actions: _Actions, records: _Records,
+                 sites: _Sites):
         self.__interactor = interactor
-        self.__actions = _Actions(self.__interactor)
-        self.__tasks = _Tasks(self.__interactor)
-        self.__reports = _Reports(self.__interactor)
-        self.__records = _Records(self.__interactor)
-        self.__sites = _Sites(self.__interactor)
+        self.__tasks = tasks
+        self.__reports = reports
+        self.__records = records
+        self.__sites = sites
+        self.__actions = actions
+        self.__news = _News(interactor)
 
     def navigate_to_news_and_get_info(self) -> NewsInfo:
         """
         Navigate to the News tab in Tempo and gather information about available news entries
         """
-        return NewsInfo(self.__interactor)
+        return NewsInfo(self.__news)
 
     def navigate_to_records_and_get_info(self) -> RecordsInfo:
         """
         Navigate to the records tab in Tempo and gather information about available record types
         """
-        try:
-            self.__records.get_records_interface(locust_request_label="Visit.Records.Tempo")
-            self.__records.get_records_nav(locust_request_label="Visit.Records.Tempo")
-        except Exception as e:
-            log_locust_error(e, error_desc="Response Error", raise_error=False)
         return RecordsInfo(records=self.__records)
 
     def navigate_to_actions_and_get_info(self) -> ActionsInfo:
         """
         Navigate to the actions tab in Tempo and gather information about available actions
         """
         return ActionsInfo(self.__actions)
```

### Comparing `appian-locust-2.0.0a5/appian_locust/uiform.py` & `appian-locust-2.0.0a6/appian_locust/uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/appian_locust/visitor.py` & `appian-locust-2.0.0a6/appian_locust/visitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 
 class Visitor:
     """
     Provides methods to get an interactable ``SailUiForm`` from an Appian instance. Each method will return the respected ``SailUiForm`` type for which it will allow
     interactions with the visited page.
     """
 
-    def __init__(self, interactor: _Interactor):
+    def __init__(self, interactor: _Interactor, tasks: _Tasks, reports: _Reports, actions: _Actions, records: _Records,
+                 sites: _Sites):
         self.__interactor = interactor
-        self.__tasks = _Tasks(self.__interactor)
-        self.__reports = _Reports(self.__interactor)
+        self.__tasks = tasks
+        self.__reports = reports
+        self.__records = records
+        self.__sites = sites
+        self.__actions = actions
         self.__design = _Design(self.__interactor)
-        self.__records = _Records(self.__interactor)
-        self.__sites = _Sites(self.__interactor)
-        self.__actions = _Actions(self.__interactor)
         self.__admin = _Admin(self.__interactor)
         self.__portals = _Portals(self.__interactor)
 
     def visit_task(self, task_name: str, exact_match: bool = True, locust_request_label: str = "") -> SailUiForm:
         """
         Gets the SailUiForm given a task name
 
@@ -55,27 +56,29 @@
 
         if not locust_request_label:
             breadcrumb = f"Tasks.{task_title}"
         else:
             breadcrumb = locust_request_label
         return SailUiForm(self.__interactor, self.__tasks.get_task_form_json(task_name=task_title, locust_request_label=breadcrumb, exact_match=False), breadcrumb=breadcrumb)
 
-    def visit_report(self, report_name: str, exact_match: bool = True) -> 'SailUiForm':
+    def visit_report(self, report_name: str, exact_match: bool = True, locust_request_label: Optional[str] = None) -> 'SailUiForm':
         """
         Navigate to a report and return a SailUiForm for that report's UI
 
         Args:
             report_name (str): Name of the report to be called.
             exact_match (bool, optional): Should report name match exactly or to be partial match. Default : True
+            locust_request_label (str, optional): Label locust should associate this request with
 
         Returns (SailUiForm): Response of report's Get UI call in SailUiForm
 
         """
         breadcrumb = f'Reports.SailUi.{format_label(report_name, "::", 0)}'
-        return SailUiForm(self.__interactor, self.__reports.fetch_report_json(report_name, exact_match), breadcrumb=breadcrumb)
+        locust_request_label = locust_request_label or f"Visit.Report.{report_name}"
+        return SailUiForm(self.__interactor, self.__reports.fetch_report_json(report_name, exact_match, locust_request_label=locust_request_label), breadcrumb=breadcrumb)
 
     def visit_design(self) -> DesignUiForm:
         """
         Navigate to /design
         Returns (DesignUiForm): UiForm representing /design
 
         """
@@ -137,43 +140,53 @@
         designUiForm: DesignUiForm = self.visit_design()
         designUiForm.select_nav_card_by_index(nav_group_label="leftNavbar", is_test_label=True, index=1)
         designUiForm.check_checkbox_by_test_label(test_label="object-type-checkbox", indices=[object_type.value])
         designUiForm.search_objects(object_name)
         design_object_opaque_id = self.__design.find_design_object_opaque_id_in_grid(object_name, designUiForm.get_latest_state())
         return self.visit_design_object_by_id(design_object_opaque_id)
 
-    def visit_record_instance(self, record_type: str = "", record_name: str = "", view_url_stub: str = "", exact_match: bool = False, summary_view: bool = True) -> RecordInstanceUiForm:
+    def visit_record_instance(self, record_type: str = "", record_name: str = "", view_url_stub: str = "",
+                              exact_match: bool = False, summary_view: bool = True,
+                              locust_request_label: Optional[str] = None) -> RecordInstanceUiForm:
         """
         Navigate to a specific record and return a RecordUiForm
 
         Args:
             record_type (str): Record Type Name. If not specified, a random record type will be selected.
             record_name (str): Name of the record to be called. If not specified, a random record will be selected.
             view_url_stub (str, optional): page/tab to be visited in the record. If not specified, "summary" dashboard will be selected.
             exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
             summary_view (bool, optional): Should the Record UI be returned in Summary View, if false will return Header View
+            locust_request_label (str, optional): Label locust should associate this request with
 
         Returns (RecordUiForm): The UI for the record instance
 
         """
-        form_json = self.__records.visit_record_instance(record_type, record_name, view_url_stub=view_url_stub, exact_match=exact_match)
+        self.__records.get_records_nav(locust_request_label=locust_request_label)
+        form_json = self.__records.visit_record_instance(record_type, record_name, view_url_stub=view_url_stub,
+                                                         exact_match=exact_match, locust_request_label=locust_request_label)
         breadcrumb = f'Records.{record_type}.{format_label(record_name, "::", 0)}.SailUi'
         return RecordInstanceUiForm(self.__interactor, form_json, summary_view=summary_view, breadcrumb=breadcrumb)
 
-    def visit_record_type(self, record_type: str = "", exact_match: bool = False, is_mobile: bool = False) -> RecordListUiForm:
+    def visit_record_type(self, record_type: str = "", exact_match: bool = False, is_mobile: bool = False,
+                          locust_request_label: Optional[str] = None) -> RecordListUiForm:
         """
         This function calls the API for the specific record type and returns a SAIL form representing the list of records for that record type.
 
         Args:
             record_type (str): Record Type Name. If not specified, a random record type will be selected.
             exact_match (bool, optional): Should record type and record name matched exactly as it is or partial match.
+            is_mobile (bool, optional): If this is a mobile record
+            locust_request_label (str, optional): Label locust should associate this request with
 
         Returns (SailUiForm): UI representing list of records for that record type
         """
-        form_json = self.__records.visit_record_type(record_type, exact_match=exact_match, is_mobile=is_mobile)
+        self.__records.get_records_nav(locust_request_label=locust_request_label)
+        form_json = self.__records.visit_record_type(record_type, exact_match=exact_match, is_mobile=is_mobile,
+                                                     locust_request_label=locust_request_label)
         breadcrumb = f'Records.{record_type}.RecordListUi'
         return RecordListUiForm(self.__interactor, form_json, breadcrumb=breadcrumb)
 
     def visit_site(self, site_name: str, page_name: str) -> 'SailUiForm':
         """
         Get a SailUiForm for a Task, Report or Action
```

### Comparing `appian-locust-2.0.0a5/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.0a6/appian_locust.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0a5
+Version: 2.0.0a6
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `appian-locust-2.0.0a5/setup.cfg` & `appian-locust-2.0.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0a5/setup.py` & `appian-locust-2.0.0a6/setup.py`

 * *Files identical despite different names*

