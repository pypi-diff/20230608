# Comparing `tmp/watchmen_rest_doll-16.5.7.tar.gz` & `tmp/watchmen_rest_doll-16.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_rest_doll-16.5.7.tar", max compression
+gzip compressed data, was "watchmen_rest_doll-16.5.8.tar", max compression
```

## Comparing `watchmen_rest_doll-16.5.7.tar` & `watchmen_rest_doll-16.5.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/LICENSE
--rw-r--r--   0        0        0     2257 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/__init__.py
--rw-r--r--   0        0        0      254 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/__init__.py
--rw-r--r--   0        0        0     9109 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/enumeration_router.py
--rw-r--r--   0        0        0     6875 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/pipeline_graphic_router.py
--rw-r--r--   0        0        0     9721 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/pipeline_router.py
--rw-r--r--   0        0        0    11907 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/space_router.py
--rw-r--r--   0        0        0     1029 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/synonym_topic_router.py
--rw-r--r--   0        0        0    14141 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/topic_router.py
--rw-r--r--   0        0        0     9733 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/topic_snapshot_scheduler_router.py
--rw-r--r--   0        0        0    14944 2023-06-07 11:34:15.635987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/user_group_router.py
--rw-r--r--   0        0        0    10118 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/user_router.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/analysis/__init__.py
--rw-r--r--   0        0        0     1868 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/analysis/pipeline_index_router.py
--rw-r--r--   0        0        0     3059 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/analysis/topic_index_router.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/auth/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/auth/authenticate_router.py
--rw-r--r--   0        0        0      158 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/connected_space_graphic_router.py
--rw-r--r--   0        0        0    22113 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/connected_space_router.py
--rw-r--r--   0        0        0    14467 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/dashboard_router.py
--rw-r--r--   0        0        0     5413 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/report_router.py
--rw-r--r--   0        0        0     7091 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/subject_router.py
--rw-r--r--   0        0        0     3559 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/doll.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/gui/__init__.py
--rw-r--r--   0        0        0     3503 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/gui/favorite_router.py
--rw-r--r--   0        0        0     3773 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/gui/last_snapshot_router.py
--rw-r--r--   0        0        0     3303 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/main.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/__init__.py
--rw-r--r--   0        0        0     3564 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/connected_space_import_router.py
--rw-r--r--   0        0        0     1517 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/dashboard_import_router.py
--rw-r--r--   0        0        0    40334 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/mix_import_router.py
--rw-r--r--   0        0        0     1879 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/pipeline_import_router.py
--rw-r--r--   0        0        0     1457 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/report_import_router.py
--rw-r--r--   0        0        0     1403 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/space_import_router.py
--rw-r--r--   0        0        0     1477 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/subject_import_router.py
--rw-r--r--   0        0        0     1806 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/topic_import_router.py
--rw-r--r--   0        0        0     1498 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/user_group_import_router.py
--rw-r--r--   0        0        0     1354 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/user_import_router.py
--rw-r--r--   0        0        0     3698 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/validator.py
--rw-r--r--   0        0        0      908 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/settings.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/saml/__init__.py
--rw-r--r--   0        0        0      998 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/saml/auth_saml_router.py
--rw-r--r--   0        0        0     3227 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/saml/saml_helper.py
--rw-r--r--   0        0        0      239 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/sso_router.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/__init__.py
--rw-r--r--   0        0        0     5697 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/data_source_router.py
--rw-r--r--   0        0        0     5054 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/external_writer_router.py
--rw-r--r--   0        0        0     2594 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/operation_router.py
--rw-r--r--   0        0        0     2632 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/package_version_router.py
--rw-r--r--   0        0        0     3010 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/pat_router.py
--rw-r--r--   0        0        0     4982 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/plugin_router.py
--rw-r--r--   0        0        0     4675 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/tenant_init_router.py
--rw-r--r--   0        0        0     5839 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/tenant_router.py
--rw-r--r--   0        0        0      881 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/utils.py
--rw-r--r--   0        0        0      131 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/util/__init__.py
--rw-r--r--   0        0        0      321 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/util/crypt.py
--rw-r--r--   0        0        0     2008 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/util/trans.py
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/webhook/__init__.py
--rw-r--r--   0        0        0     8121 2023-06-07 11:34:15.639987 watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/webhook/webhook_router.py
--rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 watchmen_rest_doll-16.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/LICENSE
+-rw-r--r--   0        0        0     2257 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/__init__.py
+-rw-r--r--   0        0        0     9109 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/enumeration_router.py
+-rw-r--r--   0        0        0     6875 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/pipeline_graphic_router.py
+-rw-r--r--   0        0        0     9721 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/pipeline_router.py
+-rw-r--r--   0        0        0    11907 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/space_router.py
+-rw-r--r--   0        0        0     1029 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/synonym_topic_router.py
+-rw-r--r--   0        0        0    14141 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/topic_router.py
+-rw-r--r--   0        0        0     9733 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/topic_snapshot_scheduler_router.py
+-rw-r--r--   0        0        0    14944 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/user_group_router.py
+-rw-r--r--   0        0        0    10118 2023-06-08 03:33:39.211630 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/user_router.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/analysis/__init__.py
+-rw-r--r--   0        0        0     1868 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/analysis/pipeline_index_router.py
+-rw-r--r--   0        0        0     3059 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/analysis/topic_index_router.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/auth/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/auth/authenticate_router.py
+-rw-r--r--   0        0        0      158 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/connected_space_graphic_router.py
+-rw-r--r--   0        0        0    22113 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/connected_space_router.py
+-rw-r--r--   0        0        0    14467 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/dashboard_router.py
+-rw-r--r--   0        0        0     5413 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/report_router.py
+-rw-r--r--   0        0        0     7091 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/subject_router.py
+-rw-r--r--   0        0        0     3559 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/doll.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/gui/__init__.py
+-rw-r--r--   0        0        0     3503 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/gui/favorite_router.py
+-rw-r--r--   0        0        0     3773 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/gui/last_snapshot_router.py
+-rw-r--r--   0        0        0     3303 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/main.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/__init__.py
+-rw-r--r--   0        0        0     3564 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/connected_space_import_router.py
+-rw-r--r--   0        0        0     1517 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/dashboard_import_router.py
+-rw-r--r--   0        0        0    40334 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/mix_import_router.py
+-rw-r--r--   0        0        0     1879 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/pipeline_import_router.py
+-rw-r--r--   0        0        0     1457 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/report_import_router.py
+-rw-r--r--   0        0        0     1403 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/space_import_router.py
+-rw-r--r--   0        0        0     1477 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/subject_import_router.py
+-rw-r--r--   0        0        0     1806 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/topic_import_router.py
+-rw-r--r--   0        0        0     1498 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/user_group_import_router.py
+-rw-r--r--   0        0        0     1354 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/user_import_router.py
+-rw-r--r--   0        0        0     3698 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/validator.py
+-rw-r--r--   0        0        0      908 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/settings.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/saml/__init__.py
+-rw-r--r--   0        0        0      998 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/saml/auth_saml_router.py
+-rw-r--r--   0        0        0     3227 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/saml/saml_helper.py
+-rw-r--r--   0        0        0      239 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/sso_router.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/__init__.py
+-rw-r--r--   0        0        0     5697 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/data_source_router.py
+-rw-r--r--   0        0        0     5054 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/external_writer_router.py
+-rw-r--r--   0        0        0     2594 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/operation_router.py
+-rw-r--r--   0        0        0     2632 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/package_version_router.py
+-rw-r--r--   0        0        0     3010 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/pat_router.py
+-rw-r--r--   0        0        0     4982 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/plugin_router.py
+-rw-r--r--   0        0        0     4675 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/tenant_init_router.py
+-rw-r--r--   0        0        0     5839 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/tenant_router.py
+-rw-r--r--   0        0        0      881 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/utils.py
+-rw-r--r--   0        0        0      131 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/util/__init__.py
+-rw-r--r--   0        0        0      321 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/util/crypt.py
+-rw-r--r--   0        0        0     2008 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/util/trans.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/webhook/__init__.py
+-rw-r--r--   0        0        0     8121 2023-06-08 03:33:39.215631 watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/webhook/webhook_router.py
+-rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 watchmen_rest_doll-16.5.8/PKG-INFO
```

### Comparing `watchmen_rest_doll-16.5.7/LICENSE` & `watchmen_rest_doll-16.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/pyproject.toml` & `watchmen_rest_doll-16.5.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "watchmen-rest-doll"
-version = "16.5.7"
+version = "16.5.8"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_rest_doll", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 passlib = "^1.7.4"
 bcrypt = "^3.2.0"
 python-multipart = "^0.0.5"
-watchmen-lineage = "16.5.7"
-watchmen-data-surface = "16.5.7"
-watchmen-collector-surface = { version = "16.5.7", optional = true }
-watchmen-pipeline-surface = "16.5.7"
-watchmen-inquiry-surface = "16.5.7"
-watchmen-inquiry-trino = { version = "16.5.7", optional = true }
-watchmen-indicator-surface = "16.5.7"
-watchmen-storage-mysql = { version = "16.5.7", optional = true }
-watchmen-storage-oracle = { version = "16.5.7", optional = true }
-watchmen-storage-mongodb = { version = "16.5.7", optional = true }
-watchmen-storage-mssql = { version = "16.5.7", optional = true }
-watchmen-storage-postgresql = { version = "16.5.7", optional = true }
-watchmen-storage-oss = { version = "16.5.7", optional = true }
-watchmen-storage-s3 = { version = "16.5.7", optional = true }
+watchmen-lineage = "16.5.8"
+watchmen-data-surface = "16.5.8"
+watchmen-collector-surface = { version = "16.5.8", optional = true }
+watchmen-pipeline-surface = "16.5.8"
+watchmen-inquiry-surface = "16.5.8"
+watchmen-inquiry-trino = { version = "16.5.8", optional = true }
+watchmen-indicator-surface = "16.5.8"
+watchmen-storage-mysql = { version = "16.5.8", optional = true }
+watchmen-storage-oracle = { version = "16.5.8", optional = true }
+watchmen-storage-mongodb = { version = "16.5.8", optional = true }
+watchmen-storage-mssql = { version = "16.5.8", optional = true }
+watchmen-storage-postgresql = { version = "16.5.8", optional = true }
+watchmen-storage-oss = { version = "16.5.8", optional = true }
+watchmen-storage-s3 = { version = "16.5.8", optional = true }
 kafka-python = { version = "^2.0.2", optional = true }
 aiokafka = { version = "^0.7.2", optional = true }
 aio-pika = { version = "^7.1.2", optional = true }
 starlette-prometheus = { version = "^0.9.0", optional = true }
 requests = { version = "^2.27.1", optional = true }
 python3-saml = { version = "^1.14.0", optional = true }
 cryptography = { version = "^36.0.2", optional = true }
```

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/enumeration_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/enumeration_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/pipeline_graphic_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/pipeline_graphic_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/pipeline_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/pipeline_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/space_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/space_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/synonym_topic_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/synonym_topic_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/topic_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/topic_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/topic_snapshot_scheduler_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/topic_snapshot_scheduler_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/user_group_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/user_group_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/admin/user_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/admin/user_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/analysis/pipeline_index_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/analysis/pipeline_index_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/analysis/topic_index_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/analysis/topic_index_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/auth/authenticate_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/auth/authenticate_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/connected_space_graphic_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/connected_space_graphic_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/connected_space_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/connected_space_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/dashboard_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/dashboard_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/report_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/report_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/console/subject_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/console/subject_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/doll.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/doll.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/gui/favorite_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/gui/favorite_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/gui/last_snapshot_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/gui/last_snapshot_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/main.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/connected_space_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/connected_space_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/dashboard_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/dashboard_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/mix_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/mix_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/pipeline_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/pipeline_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/report_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/report_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/space_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/space_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/subject_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/subject_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/topic_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/topic_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/user_group_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/user_group_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/user_import_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/user_import_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/meta_import/validator.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/meta_import/validator.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/settings.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/saml/auth_saml_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/saml/auth_saml_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/sso/saml/saml_helper.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/sso/saml/saml_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/data_source_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/data_source_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/external_writer_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/external_writer_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/operation_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/operation_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/package_version_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/package_version_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/pat_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/pat_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/plugin_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/plugin_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/tenant_init_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/tenant_init_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/tenant_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/tenant_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/system/utils.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/system/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/util/trans.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/util/trans.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/src/watchmen_rest_doll/webhook/webhook_router.py` & `watchmen_rest_doll-16.5.8/src/watchmen_rest_doll/webhook/webhook_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_doll-16.5.7/PKG-INFO` & `watchmen_rest_doll-16.5.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-rest-doll
-Version: 16.5.7
+Version: 16.5.8
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,21 +32,21 @@
 Requires-Dist: cryptography (>=36.0.2,<37.0.0) ; extra == "mysql" or extra == "sso"
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0) ; extra == "kafka"
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: python3-saml (>=1.14.0,<2.0.0) ; extra == "sso"
 Requires-Dist: requests (>=2.27.1,<3.0.0) ; extra == "standard-ext-writer"
 Requires-Dist: starlette-prometheus (>=0.9.0,<0.10.0) ; extra == "prometheus"
-Requires-Dist: watchmen-collector-surface (==16.5.7) ; extra == "collector"
-Requires-Dist: watchmen-data-surface (==16.5.7)
-Requires-Dist: watchmen-indicator-surface (==16.5.7)
-Requires-Dist: watchmen-inquiry-surface (==16.5.7)
-Requires-Dist: watchmen-inquiry-trino (==16.5.7) ; extra == "trino"
-Requires-Dist: watchmen-lineage (==16.5.7)
-Requires-Dist: watchmen-pipeline-surface (==16.5.7)
-Requires-Dist: watchmen-storage-mongodb (==16.5.7) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.7) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.7) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.7) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.7) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.7) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.7) ; extra == "s3"
+Requires-Dist: watchmen-collector-surface (==16.5.8) ; extra == "collector"
+Requires-Dist: watchmen-data-surface (==16.5.8)
+Requires-Dist: watchmen-indicator-surface (==16.5.8)
+Requires-Dist: watchmen-inquiry-surface (==16.5.8)
+Requires-Dist: watchmen-inquiry-trino (==16.5.8) ; extra == "trino"
+Requires-Dist: watchmen-lineage (==16.5.8)
+Requires-Dist: watchmen-pipeline-surface (==16.5.8)
+Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.8) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.8) ; extra == "s3"
```

