# Comparing `tmp/django-data-browser-4.2.1.tar.gz` & `tmp/django-data-browser-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-browser-4.2.1.tar", last modified: Sun May 21 17:28:36 2023, max compression
+gzip compressed data, was "django-data-browser-4.2.2.tar", last modified: Thu Jun  8 07:11:41 2023, max compression
```

## Comparing `django-data-browser-4.2.1.tar` & `django-data-browser-4.2.2.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.432530 django-data-browser-4.2.1/
--rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.2.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.2.1/LICENSE
--rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    62233 2023-05-21 17:28:36.431532 django-data-browser-4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    61104 2023-05-21 17:27:00.000000 django-data-browser-4.2.1/README.rst
--rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.2.1/build.sh
--rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.2.1/build_fe.sh
--rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.2.1/build_whl.sh
--rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.2.1/clean.sh
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.148696 django-data-browser-4.2.1/data_browser/
--rw-rw-rw-   0        0        0       18 2023-05-21 17:26:29.000000 django-data-browser-4.2.1/data_browser/__init__.py
--rw-rw-rw-   0        0        0     2417 2023-05-21 13:26:39.000000 django-data-browser-4.2.1/data_browser/admin.py
--rw-rw-rw-   0        0        0     5118 2023-05-20 11:07:43.000000 django-data-browser-4.2.1/data_browser/api.py
--rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.2.1/data_browser/apps.py
--rw-rw-rw-   0        0        0     3287 2023-05-07 09:17:35.000000 django-data-browser-4.2.1/data_browser/common.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.151677 django-data-browser-4.2.1/data_browser/fe_build/
--rw-rw-rw-   0        0        0      374 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/asset-manifest.json
--rw-rw-rw-   0        0        0     2400 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/index.html
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.068392 django-data-browser-4.2.1/data_browser/fe_build/static/
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.154672 django-data-browser-4.2.1/data_browser/fe_build/static/css/
--rw-rw-rw-   0        0        0     7170 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/static/css/main.a2cd42f2.css
--rw-rw-rw-   0        0        0    10320 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/static/css/main.a2cd42f2.css.map
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.159656 django-data-browser-4.2.1/data_browser/fe_build/static/js/
--rw-rw-rw-   0        0        0   328249 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/static/js/main.c57e8af0.js
--rw-rw-rw-   0        0        0     1447 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1220644 2023-05-21 17:28:25.000000 django-data-browser-4.2.1/data_browser/fe_build/static/js/main.c57e8af0.js.map
--rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.2.1/data_browser/format_csv.py
--rw-rw-rw-   0        0        0     5819 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/helpers.py
--rw-rw-rw-   0        0        0     2574 2023-05-01 18:51:44.000000 django-data-browser-4.2.1/data_browser/migration_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.191571 django-data-browser-4.2.1/data_browser/migrations/
--rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0002_auto_20200331_1842.py
--rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0003_remove_view_app.py
--rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0004_auto_20200501_0903.py
--rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0005_auto_20200516_1726.py
--rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0006_auto_20200531_1450.py
--rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0007_view_public_slug.py
--rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/migrations/0008_view_limit.py
--rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.2.1/data_browser/migrations/0009_migrate_saved_views.py
--rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/data_browser/migrations/0010_shared.py
--rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/data_browser/migrations/0011_folder.py
--rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.2.1/data_browser/migrations/0012_can_share.py
--rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.2.1/data_browser/migrations/__init__.py
--rw-rw-rw-   0        0        0     2657 2023-05-01 18:51:44.000000 django-data-browser-4.2.1/data_browser/models.py
--rw-rw-rw-   0        0        0    15088 2023-03-30 21:24:18.000000 django-data-browser-4.2.1/data_browser/orm_admin.py
--rw-rw-rw-   0        0        0     3923 2023-03-06 07:51:43.000000 django-data-browser-4.2.1/data_browser/orm_aggregates.py
--rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.2.1/data_browser/orm_debug.py
--rw-rw-rw-   0        0        0     8291 2023-04-30 12:59:04.000000 django-data-browser-4.2.1/data_browser/orm_fields.py
--rw-rw-rw-   0        0        0     5000 2023-05-21 13:30:07.000000 django-data-browser-4.2.1/data_browser/orm_functions.py
--rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.2.1/data_browser/orm_lookups.py
--rw-rw-rw-   0        0        0     9368 2023-05-21 16:12:12.000000 django-data-browser-4.2.1/data_browser/orm_results.py
--rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.2.1/data_browser/orm_types.py
--rw-rw-rw-   0        0        0     9970 2023-05-21 16:13:57.000000 django-data-browser-4.2.1/data_browser/query.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.069389 django-data-browser-4.2.1/data_browser/templates/
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.202542 django-data-browser-4.2.1/data_browser/templates/data_browser/
--rw-rw-rw-   0        0        0     2400 2023-05-21 17:28:26.000000 django-data-browser-4.2.1/data_browser/templates/data_browser/index.html
--rw-rw-rw-   0        0        0    16949 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/data_browser/types.py
--rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.2.1/data_browser/urls.py
--rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.2.1/data_browser/util.py
--rw-rw-rw-   0        0        0    13106 2023-05-21 15:01:36.000000 django-data-browser-4.2.1/data_browser/views.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.274857 django-data-browser-4.2.1/data_browser/web_root/
--rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.2.1/data_browser/web_root/android-chrome-192x192.png
--rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.2.1/data_browser/web_root/android-chrome-512x512.png
--rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.2.1/data_browser/web_root/apple-touch-icon.png
--rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.2.1/data_browser/web_root/favicon-16x16.png
--rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.2.1/data_browser/web_root/favicon-32x32.png
--rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.2.1/data_browser/web_root/favicon.ico
--rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/data_browser/web_root/site.webmanifest
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.305805 django-data-browser-4.2.1/django_data_browser.egg-info/
--rw-rw-rw-   0        0        0    62233 2023-05-21 17:28:35.000000 django-data-browser-4.2.1/django_data_browser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3438 2023-05-21 17:28:36.000000 django-data-browser-4.2.1/django_data_browser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 17:28:35.000000 django-data-browser-4.2.1/django_data_browser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-21 17:28:35.000000 django-data-browser-4.2.1/django_data_browser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-21 17:28:35.000000 django-data-browser-4.2.1/django_data_browser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.310791 django-data-browser-4.2.1/frontend/
--rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.2.1/frontend/README.md
--rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/frontend/package-lock.json
--rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.2.1/frontend/package.json
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.311789 django-data-browser-4.2.1/frontend/public/
--rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.2.1/frontend/public/index.html
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.337741 django-data-browser-4.2.1/frontend/src/
--rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/frontend/src/App.js
--rw-rw-rw-   0        0        0     7342 2023-05-21 17:10:18.000000 django-data-browser-4.2.1/frontend/src/App.scss
--rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.2.1/frontend/src/App.test.js
--rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/frontend/src/Config.js
--rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.2.1/frontend/src/ContextMenu.js
--rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/frontend/src/CurrentSavedView.js
--rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.2.1/frontend/src/HomePage.js
--rw-rw-rw-   0        0        0     9603 2023-05-21 17:07:43.000000 django-data-browser-4.2.1/frontend/src/Query.js
--rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.2.1/frontend/src/Query.test.js
--rw-rw-rw-   0        0        0    14930 2023-05-21 17:09:38.000000 django-data-browser-4.2.1/frontend/src/QueryPage.js
--rw-rw-rw-   0        0        0     9360 2023-05-21 16:43:53.000000 django-data-browser-4.2.1/frontend/src/Results.js
--rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.2.1/frontend/src/SavedViewPage.js
--rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.2.1/frontend/src/Tooltip.js
--rw-rw-rw-   0        0        0    12431 2023-05-21 14:02:17.000000 django-data-browser-4.2.1/frontend/src/Util.js
--rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.2.1/frontend/src/WindowDimensions.js
--rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.2.1/frontend/src/index.js
--rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.2.1/frontend/src/index.scss
--rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.2.1/frontend/src/logo.svg
--rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.2.1/frontend/src/setupTests.js
--rw-rw-rw-   0        0        0     2837 2023-05-01 18:51:44.000000 django-data-browser-4.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.2.1/requirements.txt
--rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.2.1/screenshot.png
--rw-rw-rw-   0        0        0       42 2023-05-21 17:28:36.432530 django-data-browser-4.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.2.1/setup.py
--rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.2.1/structure.svg
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.400594 django-data-browser-4.2.1/tests/
--rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.2.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.405582 django-data-browser-4.2.1/tests/array/
--rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.2.1/tests/array/__init__.py
--rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.2.1/tests/array/models.py
--rw-rw-rw-   0        0        0     2343 2023-05-07 09:14:15.000000 django-data-browser-4.2.1/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.408573 django-data-browser-4.2.1/tests/core/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.1/tests/core/__init__.py
--rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.2.1/tests/core/admin.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.413560 django-data-browser-4.2.1/tests/core/migrations/
--rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.2.1/tests/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.2.1/tests/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.2.1/tests/core/models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.414557 django-data-browser-4.2.1/tests/json/
--rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.1/tests/json/__init__.py
--rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.2.1/tests/json/models.py
-drwxrwxrwx   0        0        0        0 2023-05-21 17:28:36.418547 django-data-browser-4.2.1/tests/snapshots/
--rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.2.1/tests/snapshots/__init__.py
--rw-rw-rw-   0        0        0   439282 2023-05-21 15:04:07.000000 django-data-browser-4.2.1/tests/snapshots/snap_test_views.py
--rw-rw-rw-   0        0        0     5357 2023-05-21 13:26:39.000000 django-data-browser-4.2.1/tests/test_admin.py
--rw-rw-rw-   0        0        0    20582 2023-05-07 09:13:51.000000 django-data-browser-4.2.1/tests/test_api.py
--rw-rw-rw-   0        0        0     7267 2023-05-21 13:30:07.000000 django-data-browser-4.2.1/tests/test_array_field.py
--rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.2.1/tests/test_common.py
--rw-rw-rw-   0        0        0     3693 2022-05-03 21:04:24.000000 django-data-browser-4.2.1/tests/test_helpers.py
--rw-rw-rw-   0        0        0     6186 2023-05-21 13:30:07.000000 django-data-browser-4.2.1/tests/test_json_field.py
--rw-rw-rw-   0        0        0     4483 2021-12-12 21:09:42.000000 django-data-browser-4.2.1/tests/test_migrations.py
--rw-rw-rw-   0        0        0     1240 2020-07-06 07:50:49.000000 django-data-browser-4.2.1/tests/test_models.py
--rw-rw-rw-   0        0        0    35026 2023-03-30 22:40:08.000000 django-data-browser-4.2.1/tests/test_orm.py
--rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.2.1/tests/test_orm_debug.py
--rw-rw-rw-   0        0        0    25645 2023-05-21 16:31:25.000000 django-data-browser-4.2.1/tests/test_query.py
--rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.2.1/tests/test_tests.py
--rw-rw-rw-   0        0        0    18139 2023-05-01 18:59:45.000000 django-data-browser-4.2.1/tests/test_views.py
--rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.2.1/tests/urls.py
--rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.2.1/tests/util.py
--rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.2.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.544181 django-data-browser-4.2.2/
+-rw-rw-rw-   0        0        0     1885 2023-03-30 21:24:18.000000 django-data-browser-4.2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0    14913 2021-12-12 20:01:39.000000 django-data-browser-4.2.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1522 2020-03-29 21:09:45.000000 django-data-browser-4.2.2/LICENSE
+-rw-rw-rw-   0        0        0      605 2022-01-04 07:58:07.000000 django-data-browser-4.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    62499 2023-06-08 07:11:41.543185 django-data-browser-4.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    61368 2023-06-08 07:10:55.000000 django-data-browser-4.2.2/README.rst
+-rw-rw-rw-   0        0        0      508 2021-09-26 12:42:44.000000 django-data-browser-4.2.2/build.sh
+-rw-rw-rw-   0        0        0      243 2020-10-18 11:05:29.000000 django-data-browser-4.2.2/build_fe.sh
+-rw-rw-rw-   0        0        0      209 2020-11-28 10:32:50.000000 django-data-browser-4.2.2/build_whl.sh
+-rw-rw-rw-   0        0        0      105 2020-10-18 11:05:29.000000 django-data-browser-4.2.2/clean.sh
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.440459 django-data-browser-4.2.2/data_browser/
+-rw-rw-rw-   0        0        0       18 2023-06-08 07:11:01.000000 django-data-browser-4.2.2/data_browser/__init__.py
+-rw-rw-rw-   0        0        0     2009 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/admin.py
+-rw-rw-rw-   0        0        0     4818 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/api.py
+-rw-rw-rw-   0        0        0      206 2022-02-07 19:45:31.000000 django-data-browser-4.2.2/data_browser/apps.py
+-rw-rw-rw-   0        0        0     5645 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/common.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.442454 django-data-browser-4.2.2/data_browser/fe_build/
+-rw-rw-rw-   0        0        0      374 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2400 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/index.html
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.392587 django-data-browser-4.2.2/data_browser/fe_build/static/
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.444448 django-data-browser-4.2.2/data_browser/fe_build/static/css/
+-rw-rw-rw-   0        0        0     7170 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/static/css/main.a2cd42f2.css
+-rw-rw-rw-   0        0        0    10320 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/static/css/main.a2cd42f2.css.map
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.447441 django-data-browser-4.2.2/data_browser/fe_build/static/js/
+-rw-rw-rw-   0        0        0   328249 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/static/js/main.c57e8af0.js
+-rw-rw-rw-   0        0        0     1447 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1220644 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/fe_build/static/js/main.c57e8af0.js.map
+-rw-rw-rw-   0        0        0     1741 2021-03-13 16:54:43.000000 django-data-browser-4.2.2/data_browser/format_csv.py
+-rw-rw-rw-   0        0        0     5819 2023-05-28 08:26:29.000000 django-data-browser-4.2.2/data_browser/helpers.py
+-rw-rw-rw-   0        0        0     2566 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/migration_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.468384 django-data-browser-4.2.2/data_browser/migrations/
+-rw-rw-rw-   0        0        0     1629 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      536 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0002_auto_20200331_1842.py
+-rw-rw-rw-   0        0        0      263 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0003_remove_view_app.py
+-rw-rw-rw-   0        0        0      325 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0004_auto_20200501_0903.py
+-rw-rw-rw-   0        0        0      463 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0005_auto_20200516_1726.py
+-rw-rw-rw-   0        0        0      592 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0006_auto_20200531_1450.py
+-rw-rw-rw-   0        0        0      440 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0007_view_public_slug.py
+-rw-rw-rw-   0        0        0      344 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/migrations/0008_view_limit.py
+-rw-rw-rw-   0        0        0      469 2020-12-01 19:24:08.000000 django-data-browser-4.2.2/data_browser/migrations/0009_migrate_saved_views.py
+-rw-rw-rw-   0        0        0      350 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/data_browser/migrations/0010_shared.py
+-rw-rw-rw-   0        0        0      502 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/data_browser/migrations/0011_folder.py
+-rw-rw-rw-   0        0        0      529 2023-05-01 18:51:44.000000 django-data-browser-4.2.2/data_browser/migrations/0012_can_share.py
+-rw-rw-rw-   0        0        0        0 2020-03-31 16:35:44.000000 django-data-browser-4.2.2/data_browser/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2646 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/models.py
+-rw-rw-rw-   0        0        0    15460 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/orm_admin.py
+-rw-rw-rw-   0        0        0     3923 2023-03-06 07:51:43.000000 django-data-browser-4.2.2/data_browser/orm_aggregates.py
+-rw-rw-rw-   0        0        0     2471 2021-12-31 10:44:42.000000 django-data-browser-4.2.2/data_browser/orm_debug.py
+-rw-rw-rw-   0        0        0     8339 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/orm_fields.py
+-rw-rw-rw-   0        0        0     4991 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/orm_functions.py
+-rw-rw-rw-   0        0        0     1729 2022-01-03 10:46:07.000000 django-data-browser-4.2.2/data_browser/orm_lookups.py
+-rw-rw-rw-   0        0        0     9234 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/orm_results.py
+-rw-rw-rw-   0        0        0     3525 2023-03-30 22:40:08.000000 django-data-browser-4.2.2/data_browser/orm_types.py
+-rw-rw-rw-   0        0        0     9969 2023-06-04 16:30:52.000000 django-data-browser-4.2.2/data_browser/query.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.393584 django-data-browser-4.2.2/data_browser/templates/
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.469381 django-data-browser-4.2.2/data_browser/templates/data_browser/
+-rw-rw-rw-   0        0        0     2400 2023-06-08 07:11:33.000000 django-data-browser-4.2.2/data_browser/templates/data_browser/index.html
+-rw-rw-rw-   0        0        0    16949 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/data_browser/types.py
+-rw-rw-rw-   0        0        0     1684 2021-12-31 10:46:26.000000 django-data-browser-4.2.2/data_browser/urls.py
+-rw-rw-rw-   0        0        0      349 2023-05-01 18:51:44.000000 django-data-browser-4.2.2/data_browser/util.py
+-rw-rw-rw-   0        0        0    12967 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/data_browser/views.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.476363 django-data-browser-4.2.2/data_browser/web_root/
+-rw-rw-rw-   0        0        0     5221 2020-07-01 20:11:06.000000 django-data-browser-4.2.2/data_browser/web_root/android-chrome-192x192.png
+-rw-rw-rw-   0        0        0    17683 2020-07-01 20:11:06.000000 django-data-browser-4.2.2/data_browser/web_root/android-chrome-512x512.png
+-rw-rw-rw-   0        0        0     4613 2020-07-01 20:11:06.000000 django-data-browser-4.2.2/data_browser/web_root/apple-touch-icon.png
+-rw-rw-rw-   0        0        0      333 2020-07-01 20:11:06.000000 django-data-browser-4.2.2/data_browser/web_root/favicon-16x16.png
+-rw-rw-rw-   0        0        0      648 2020-07-01 20:11:06.000000 django-data-browser-4.2.2/data_browser/web_root/favicon-32x32.png
+-rw-rw-rw-   0        0        0    15406 2020-07-01 20:11:06.000000 django-data-browser-4.2.2/data_browser/web_root/favicon.ico
+-rw-rw-rw-   0        0        0      424 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/data_browser/web_root/site.webmanifest
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.483344 django-data-browser-4.2.2/django_data_browser.egg-info/
+-rw-rw-rw-   0        0        0    62499 2023-06-08 07:11:41.000000 django-data-browser-4.2.2/django_data_browser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3438 2023-06-08 07:11:41.000000 django-data-browser-4.2.2/django_data_browser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 07:11:41.000000 django-data-browser-4.2.2/django_data_browser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-08 07:11:41.000000 django-data-browser-4.2.2/django_data_browser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 07:11:41.000000 django-data-browser-4.2.2/django_data_browser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.488331 django-data-browser-4.2.2/frontend/
+-rw-rw-rw-   0        0        0     2891 2020-04-22 19:19:40.000000 django-data-browser-4.2.2/frontend/README.md
+-rw-rw-rw-   0        0        0  1009738 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/frontend/package-lock.json
+-rw-rw-rw-   0        0        0     1000 2022-04-10 12:41:54.000000 django-data-browser-4.2.2/frontend/package.json
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.488331 django-data-browser-4.2.2/frontend/public/
+-rw-rw-rw-   0        0        0     3304 2023-03-06 21:38:15.000000 django-data-browser-4.2.2/frontend/public/index.html
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.511270 django-data-browser-4.2.2/frontend/src/
+-rw-rw-rw-   0        0        0     1298 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/frontend/src/App.js
+-rw-rw-rw-   0        0        0     7342 2023-05-21 17:10:18.000000 django-data-browser-4.2.2/frontend/src/App.scss
+-rw-rw-rw-   0        0        0      280 2020-04-22 19:19:40.000000 django-data-browser-4.2.2/frontend/src/App.test.js
+-rw-rw-rw-   0        0        0       85 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/frontend/src/Config.js
+-rw-rw-rw-   0        0        0     2678 2021-12-29 21:35:30.000000 django-data-browser-4.2.2/frontend/src/ContextMenu.js
+-rw-rw-rw-   0        0        0      551 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/frontend/src/CurrentSavedView.js
+-rw-rw-rw-   0        0        0     4278 2023-05-01 19:00:44.000000 django-data-browser-4.2.2/frontend/src/HomePage.js
+-rw-rw-rw-   0        0        0     9603 2023-05-21 17:07:43.000000 django-data-browser-4.2.2/frontend/src/Query.js
+-rw-rw-rw-   0        0        0      144 2020-06-27 10:10:01.000000 django-data-browser-4.2.2/frontend/src/Query.test.js
+-rw-rw-rw-   0        0        0    14930 2023-05-21 17:09:38.000000 django-data-browser-4.2.2/frontend/src/QueryPage.js
+-rw-rw-rw-   0        0        0     9360 2023-05-21 16:43:53.000000 django-data-browser-4.2.2/frontend/src/Results.js
+-rw-rw-rw-   0        0        0     6645 2023-05-01 19:01:07.000000 django-data-browser-4.2.2/frontend/src/SavedViewPage.js
+-rw-rw-rw-   0        0        0     1649 2021-12-30 00:35:29.000000 django-data-browser-4.2.2/frontend/src/Tooltip.js
+-rw-rw-rw-   0        0        0    12431 2023-05-21 14:02:17.000000 django-data-browser-4.2.2/frontend/src/Util.js
+-rw-rw-rw-   0        0        0      591 2021-12-12 20:01:39.000000 django-data-browser-4.2.2/frontend/src/WindowDimensions.js
+-rw-rw-rw-   0        0        0      733 2023-04-25 17:09:12.000000 django-data-browser-4.2.2/frontend/src/index.js
+-rw-rw-rw-   0        0        0      366 2020-04-22 19:19:40.000000 django-data-browser-4.2.2/frontend/src/index.scss
+-rw-rw-rw-   0        0        0     2671 2020-04-22 19:19:40.000000 django-data-browser-4.2.2/frontend/src/logo.svg
+-rw-rw-rw-   0        0        0      255 2020-04-22 19:19:40.000000 django-data-browser-4.2.2/frontend/src/setupTests.js
+-rw-rw-rw-   0        0        0     2837 2023-05-01 18:51:44.000000 django-data-browser-4.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      260 2023-03-06 20:00:37.000000 django-data-browser-4.2.2/requirements.txt
+-rw-rw-rw-   0        0        0   112598 2021-03-13 16:54:43.000000 django-data-browser-4.2.2/screenshot.png
+-rw-rw-rw-   0        0        0       42 2023-06-08 07:11:41.545179 django-data-browser-4.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-03-30 22:40:08.000000 django-data-browser-4.2.2/setup.py
+-rw-rw-rw-   0        0        0    35837 2020-06-27 10:10:01.000000 django-data-browser-4.2.2/structure.svg
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.531216 django-data-browser-4.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2019-07-20 09:57:44.000000 django-data-browser-4.2.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.532214 django-data-browser-4.2.2/tests/array/
+-rw-rw-rw-   0        0        0        0 2020-10-24 10:26:31.000000 django-data-browser-4.2.2/tests/array/__init__.py
+-rw-rw-rw-   0        0        0      617 2021-12-31 10:07:16.000000 django-data-browser-4.2.2/tests/array/models.py
+-rw-rw-rw-   0        0        0     2600 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.535206 django-data-browser-4.2.2/tests/core/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.2/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     4422 2021-12-31 10:49:19.000000 django-data-browser-4.2.2/tests/core/admin.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.537201 django-data-browser-4.2.2/tests/core/migrations/
+-rw-rw-rw-   0        0        0    10069 2023-03-06 08:08:57.000000 django-data-browser-4.2.2/tests/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2021-12-29 23:58:51.000000 django-data-browser-4.2.2/tests/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4303 2021-12-31 10:48:59.000000 django-data-browser-4.2.2/tests/core/models.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.539195 django-data-browser-4.2.2/tests/json/
+-rw-rw-rw-   0        0        0        0 2020-08-31 16:28:18.000000 django-data-browser-4.2.2/tests/json/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-03-30 22:40:08.000000 django-data-browser-4.2.2/tests/json/models.py
+drwxrwxrwx   0        0        0        0 2023-06-08 07:11:41.540192 django-data-browser-4.2.2/tests/snapshots/
+-rw-rw-rw-   0        0        0        0 2020-06-27 10:10:01.000000 django-data-browser-4.2.2/tests/snapshots/__init__.py
+-rw-rw-rw-   0        0        0   439282 2023-05-21 15:04:07.000000 django-data-browser-4.2.2/tests/snapshots/snap_test_views.py
+-rw-rw-rw-   0        0        0     6618 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_admin.py
+-rw-rw-rw-   0        0        0    20582 2023-06-04 21:17:05.000000 django-data-browser-4.2.2/tests/test_api.py
+-rw-rw-rw-   0        0        0     7227 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_array_field.py
+-rw-rw-rw-   0        0        0      919 2020-09-09 18:29:41.000000 django-data-browser-4.2.2/tests/test_common.py
+-rw-rw-rw-   0        0        0     3744 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     6156 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_json_field.py
+-rw-rw-rw-   0        0        0     4472 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_migrations.py
+-rw-rw-rw-   0        0        0     1392 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_models.py
+-rw-rw-rw-   0        0        0    34997 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_orm.py
+-rw-rw-rw-   0        0        0      878 2023-03-30 22:40:08.000000 django-data-browser-4.2.2/tests/test_orm_debug.py
+-rw-rw-rw-   0        0        0    25645 2023-05-21 16:31:25.000000 django-data-browser-4.2.2/tests/test_query.py
+-rw-rw-rw-   0        0        0      165 2020-10-22 20:32:07.000000 django-data-browser-4.2.2/tests/test_tests.py
+-rw-rw-rw-   0        0        0    18706 2023-06-08 07:10:28.000000 django-data-browser-4.2.2/tests/test_views.py
+-rw-rw-rw-   0        0        0      184 2020-10-22 18:16:38.000000 django-data-browser-4.2.2/tests/urls.py
+-rw-rw-rw-   0        0        0      366 2023-03-30 21:24:18.000000 django-data-browser-4.2.2/tests/util.py
+-rw-rw-rw-   0        0        0      574 2023-03-30 22:40:08.000000 django-data-browser-4.2.2/tox.ini
```

### Comparing `django-data-browser-4.2.1/.pre-commit-config.yaml` & `django-data-browser-4.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/CONTRIBUTING.rst` & `django-data-browser-4.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/LICENSE` & `django-data-browser-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/MANIFEST.in` & `django-data-browser-4.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/PKG-INFO` & `django-data-browser-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.2.1
+Version: 4.2.2
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -365,14 +365,16 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
 |         |            | | Fix small bug when removing filters with errors.                                                       |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.1   | 2023-05-07 | Fix bug with shared views when using multiple authentication backends.                                   |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.0   | 2023-05-01 | | Support sharing of saved views between users.                                                          |
```

### Comparing `django-data-browser-4.2.1/README.rst` & `django-data-browser-4.2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,16 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
 |         |            | | Fix small bug when removing filters with errors.                                                       |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.1   | 2023-05-07 | Fix bug with shared views when using multiple authentication backends.                                   |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.0   | 2023-05-01 | | Support sharing of saved views between users.                                                          |
```

### Comparing `django-data-browser-4.2.1/data_browser/admin.py` & `django-data-browser-4.2.2/data_browser/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from copy import copy
-
 from django.contrib import admin
-from django.contrib.admin.utils import flatten_fieldsets
 from django.utils.html import format_html
 
 from . import models
-from .common import PUBLIC_PERM, add_request_info, has_permission
+from .common import PUBLIC_PERM, has_permission, set_global_state
 from .helpers import AdminMixin, attributes
-from .orm_admin import get_models
 
 
 @admin.register(models.View)
 class ViewAdmin(AdminMixin, admin.ModelAdmin):
     fieldsets = [
         (
             None,
@@ -38,42 +34,35 @@
             },
         ),
         ("Query", {"fields": ["model_name", "fields", "query", "limit"]}),
         ("Internal", {"fields": ["id", "created_time", "shared"]}),
     ]
     list_display = ["__str__", "owner", "public"]
 
-    def get_readonly_fields(self, request, obj):
-        return flatten_fieldsets(self.get_fieldsets(request, obj))
+    def has_add_permission(self, request):
+        return False
+
+    def has_change_permission(self, request, obj=None):
+        return False
 
     def get_fieldsets(self, request, obj=None):
         res = super().get_fieldsets(request, obj)
         if not has_permission(request.user, PUBLIC_PERM):
             res = [fs for fs in res if fs[0] != "Public"]
         return res
 
-    def get_object(self, request, object_id, from_field=None):
-        res = super().get_object(request, object_id, from_field=from_field)
-
-        ddb_request = copy(request)
-        ddb_request.environ = request.environ
-        ddb_request.user = res.owner
-        add_request_info(ddb_request)
-        models.global_data.request = ddb_request
-
+    def changeform_view(self, request, *args, **kwargs):
+        with set_global_state(request=request, set_ddb=False):
+            res = super().changeform_view(request, *args, **kwargs)
+            res.render()
         return res
 
     @staticmethod
     def open_view(obj):
         if not obj.model_name:
-            return "N/A"
+            return "N/A"  # pragma: no cover
         return format_html(f'<a href="{obj.url}">view</a>')
 
     @attributes(boolean=True)
     def valid(self, obj):
-        orm_models = get_models(models.global_data.request)
-        return obj.get_query().is_valid(orm_models)
-
-    def get_changeform_initial_data(self, request):
-        get_results = super().get_changeform_initial_data(request)
-        get_results["owner"] = request.user.pk
-        return get_results
+        with set_global_state(user=obj.owner, public_view=False):
+            return obj.is_valid()
```

### Comparing `django-data-browser-4.2.1/data_browser/api.py` & `django-data-browser-4.2.2/data_browser/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from django.shortcuts import get_object_or_404
 from django.views.decorators import csrf
 
 from .common import (
     SHARE_PERM,
     HttpResponse,
     JsonResponse,
-    add_request_info,
+    global_state,
+    set_global_state,
     str_user,
     users_with_permission,
 )
-from .models import View, global_data
-from .orm_admin import get_models
+from .models import View
 from .util import group_by
 
 
 def clean_str(field, value):
     return value.strip()[: View._meta.get_field(field).max_length]
 
 
@@ -42,125 +42,118 @@
     ("query", "query", clean_noop),
     ("limit", "limit", clean_uint),
     ("folder", "folder", clean_str),
     ("shared", "shared", clean_noop),
 ]
 
 
-def deserialize(request):
-    data = json.loads(request.body)
-
+def deserialize(data):
     res = {
         model_field_name: clean(model_field_name, data[api_field_name])
         for model_field_name, api_field_name, clean in WRITABLE_FIELDS
         if api_field_name in data
     }
 
     return res
 
 
 def name_sort(entries):
     return sorted(entries, key=lambda entry: entry["name"].lower())
 
 
-def serialize(orm_models, view):
+def serialize(view):
     return {
         **{
             api_field_name: getattr(view, model_field_name)
             for model_field_name, api_field_name, clean in WRITABLE_FIELDS
         },
         "publicLink": view.public_link(),
         "googleSheetsFormula": view.google_sheets_formula(),
         "link": view.get_query().get_url("html"),
         "createdTime": f"{view.created_time:%Y-%m-%d %H:%M:%S}",
         "pk": view.pk,
         "shared": bool(view.shared and view.name),
-        "valid": view.get_query().is_valid(orm_models),
-        "can_edit": global_data.request.user == view.owner,
+        "valid": view.is_valid(),
+        "can_edit": global_state.request.user == view.owner,
         "type": "view",
     }
 
 
-def serialize_list(orm_models, views, *, include_invalid=False):
-    res = [serialize(orm_models, view) for view in views]
+def serialize_list(views, *, include_invalid=False):
+    res = [serialize(view) for view in views]
     if not include_invalid:
         res = [row for row in res if row["valid"]]
     return name_sort(res)
 
 
-def serialize_folders(orm_models, views, *, include_invalid=False):
+def serialize_folders(views, *, include_invalid=False):
     grouped_views = group_by(views, key=lambda v: v.folder.strip())
     flat_views = grouped_views.pop("", [])
 
-    res = serialize_list(orm_models, flat_views, include_invalid=include_invalid)
+    res = serialize_list(flat_views, include_invalid=include_invalid)
     for folder_name, views in sorted(grouped_views.items()):
-        entries = serialize_list(orm_models, views, include_invalid=include_invalid)
+        entries = serialize_list(views, include_invalid=include_invalid)
         if entries:
             res.append({"name": folder_name, "type": "folder", "entries": entries})
     return name_sort(res)
 
 
-def get_queryset(request):
-    return View.objects.filter(owner=request.user)
+def get_queryset(user):
+    return View.objects.filter(owner=user)
 
 
 @csrf.csrf_protect
 @admin_decorators.staff_member_required
+@set_global_state(public_view=False)
 def view_list(request):
-    add_request_info(request)
-    global_data.request = request
-    orm_models = get_models(request)
-
     if request.method == "GET":
         # saved
-        saved_views = get_queryset(request)
-        saved_views_serialized = serialize_folders(
-            orm_models, saved_views, include_invalid=True
-        )
+        saved_views = get_queryset(request.user)
+        saved_views_serialized = serialize_folders(saved_views, include_invalid=True)
 
         # shared
         shared_views = (
             View.objects.exclude(owner=request.user)
             .filter(owner__in=users_with_permission(SHARE_PERM), shared=True)
             .exclude(name="")
             .prefetch_related("owner")
         )
         shared_views_by_user = group_by(shared_views, lambda v: str_user(v.owner))
         shared_views_serialized = []
         for owner_name, shared_views in shared_views_by_user.items():
-            entries = serialize_folders(orm_models, shared_views)
+            entries = serialize_folders(shared_views)
             if entries:
                 shared_views_serialized.append(
                     {"name": owner_name, "type": "folder", "entries": entries}
                 )
 
         # response
         return JsonResponse(
             {"saved": saved_views_serialized, "shared": shared_views_serialized}
         )
     elif request.method == "POST":
-        view = View.objects.create(owner=request.user, **deserialize(request))
-        return JsonResponse(serialize(orm_models, view))
+        data = json.loads(request.body)
+        view = View.objects.create(owner=request.user, **deserialize(data))
+        return JsonResponse(serialize(view))
     else:
         return HttpResponse(status=400)
 
 
 @csrf.csrf_protect
 @admin_decorators.staff_member_required
+@set_global_state(public_view=False)
 def view_detail(request, pk):
-    add_request_info(request)
-    global_data.request = request
-    view = get_object_or_404(get_queryset(request), pk=pk)
-    orm_models = get_models(request)
+    view = get_object_or_404(get_queryset(request.user), pk=pk)
 
     if request.method == "GET":
-        return JsonResponse(serialize(orm_models, view))
+        return JsonResponse(serialize(view))
     elif request.method == "PATCH":
-        for k, v in deserialize(request).items():
+        data = json.loads(request.body)
+        for k, v in deserialize(data).items():
             setattr(view, k, v)
         view.save()
-        return JsonResponse(serialize(orm_models, view))
+        return JsonResponse(serialize(view))
     elif request.method == "DELETE":
         view.delete()
         return HttpResponse(status=204)
     else:
         return HttpResponse(status=400)
```

### Comparing `django-data-browser-4.2.1/data_browser/fe_build/index.html` & `django-data-browser-4.2.2/data_browser/fe_build/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/fe_build/static/css/main.a2cd42f2.css` & `django-data-browser-4.2.2/data_browser/fe_build/static/css/main.a2cd42f2.css`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/fe_build/static/css/main.a2cd42f2.css.map` & `django-data-browser-4.2.2/data_browser/fe_build/static/css/main.a2cd42f2.css.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/fe_build/static/js/main.c57e8af0.js` & `django-data-browser-4.2.2/data_browser/fe_build/static/js/main.c57e8af0.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt` & `django-data-browser-4.2.2/data_browser/fe_build/static/js/main.c57e8af0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/fe_build/static/js/main.c57e8af0.js.map` & `django-data-browser-4.2.2/data_browser/fe_build/static/js/main.c57e8af0.js.map`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/format_csv.py` & `django-data-browser-4.2.2/data_browser/format_csv.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/helpers.py` & `django-data-browser-4.2.2/data_browser/helpers.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/migration_helpers.py` & `django-data-browser-4.2.2/data_browser/migration_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from urllib.parse import parse_qsl, urlencode
 
 from django.contrib.auth import get_user_model
 from django.test import RequestFactory
 from django.urls import reverse
 
-from data_browser.orm_admin import get_models
 from data_browser.types import (
     IsNullType,
     NumberChoiceArrayType,
     NumberChoiceType,
     StringChoiceArrayType,
     StringChoiceType,
 )
 
+from .common import global_state, set_global_state
+
 
 def _fix_filter(models, field, parts, lookup, value):
     if lookup == "is_null":
         value = {"true": "IsNull", "false": "NotNull"}.get(value.lower(), value)
     elif field.type_ == IsNullType and lookup == "equals":
         value = {"true": "IsNull", "false": "NotNull"}.get(value.lower(), value)
     elif field.type_ in [StringChoiceType, NumberChoiceType]:
@@ -42,22 +43,19 @@
     else:
         pass
 
     return parts, lookup, value
 
 
 def forwards_0009(View):
-    from data_browser.views import add_request_info
-
     User = get_user_model()
-
+    user = User(is_superuser=True)
     request = RequestFactory().get(reverse("admin:index"))
-    request.user = User(is_superuser=True)
-    add_request_info(request)
-    models = get_models(request)
+    with set_global_state(request=request, user=user, public_view=False):
+        models = global_state.models
 
     for view in View.objects.all():
         filters = []
         for key, value in parse_qsl(view.query):
             *parts, lookup = key.split("__")
 
             model_name = view.model_name
```

### Comparing `django-data-browser-4.2.1/data_browser/migrations/0001_initial.py` & `django-data-browser-4.2.2/data_browser/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/migrations/0002_auto_20200331_1842.py` & `django-data-browser-4.2.2/data_browser/migrations/0002_auto_20200331_1842.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/migrations/0006_auto_20200531_1450.py` & `django-data-browser-4.2.2/data_browser/migrations/0006_auto_20200531_1450.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/migrations/0012_can_share.py` & `django-data-browser-4.2.2/data_browser/migrations/0012_can_share.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/orm_admin.py` & `django-data-browser-4.2.2/data_browser/orm_admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.forms.models import _get_foreign_key
 from django.urls import reverse
 from django.utils.html import format_html
 
-from .common import JsonResponse, debug_log, settings
+from .common import JsonResponse, debug_log, global_state, settings
 from .helpers import AdminMixin, _AnnotationDescriptor, _get_option, attributes
 from .orm_aggregates import get_aggregates_for_type
 from .orm_debug import DebugQS
 from .orm_fields import (
     OrmAnnotatedField,
     OrmCalculatedField,
     OrmConcreteField,
@@ -49,26 +49,26 @@
         default_filters = _get_option(self.admin, "default_filters")
         assert isinstance(default_filters, list)
         return [
             (f, l, v if isinstance(v, str) else json.dumps(v, cls=DjangoJSONEncoder))
             for (f, l, v) in default_filters
         ]
 
-    def get_queryset(self, request, fields=(), debug=False):
-        return admin_get_queryset(self.admin, request, fields, debug=debug)
+    def get_queryset(self, fields=(), debug=False):
+        return admin_get_queryset(global_state.request, self.admin, fields, debug=debug)
 
-    def get_http_request_for_action(self, request, action, pks):
-        actions = admin_get_actions(self.admin, request)
+    def get_http_request_for_action(self, action, pks):
+        actions = admin_get_actions(global_state.request, self.admin)
         if action not in actions:
             raise http.Http404(f"'{action}' unknown action")  # pragma: no cover
 
         return JsonResponse(
             {
                 "method": "post",
-                "url": _get_option(self.admin, "action_url", request),
+                "url": _get_option(self.admin, "action_url", global_state.request),
                 "data": [
                     ("action", action),
                     ("select_across", 0),
                     ("index", 0),
                     ("data_browser", 1),
                     *[(ACTION_CHECKBOX_NAME, pk) for pk in pks],
                 ],
@@ -99,29 +99,40 @@
 
     model_name = get_model_name(obj.__class__, "_")
     url_name = f"admin:{model_name}_change".lower()
     url = reverse(url_name, args=[obj.pk])
     return format_html('<a href="{}">{}</a>', url, obj)
 
 
-def admin_get_queryset(admin, request, fields=(), debug=False):
+def _admin_get_queryset(admin, request):
+    # this is just a hook for tests to see the request
+    return admin.get_queryset(request).using(settings.DATA_BROWSER_USING_DB)
+
+
+def admin_get_queryset(request, admin, fields=(), debug=False):
     if debug:
         klass = admin.__class__
         return DebugQS(
             f"{klass.__module__}.{klass.__name__}(model,"
             " admin_site).get_queryset(request)"
         )
     else:
-        request.data_browser.update(
-            {"calculated_fields": set(fields), "fields": set(fields)}
-        )
-        return admin.get_queryset(request).using(settings.DATA_BROWSER_USING_DB)
+        orig = request.data_browser
+        request.data_browser = {
+            **request.data_browser,
+            "calculated_fields": set(fields),
+            "fields": set(fields),
+        }
+        try:
+            return _admin_get_queryset(admin, request)
+        finally:
+            request.data_browser = orig
 
 
-def admin_get_actions(admin, request):
+def admin_get_actions(request, admin):
     assert hasattr(request, "data_browser"), request
 
     res = {}
     for func, name, desc in admin.get_actions(request).values():
         if not getattr(func, "ddb_hide", False):
             desc %= model_format_dict(admin.opts)
             res[name] = func, desc
@@ -133,30 +144,33 @@
         model._meta.get_field(field_name)
     except FieldDoesNotExist:
         return False
     return True
 
 
 def _get_all_admin_fields(request):
-    assert hasattr(request, "data_browser"), request
+    assert hasattr(request, "data_browser")
 
     def from_fieldsets(admin, include_calculated):
         auth_user_compat = settings.DATA_BROWSER_AUTH_USER_COMPAT
         if auth_user_compat and isinstance(admin, UserAdmin):
             obj = admin.model()  # get the change fieldsets, not the add ones
         else:
             obj = None
 
         fields = admin.get_fieldsets(request, obj)
         for f in flatten_fieldsets(fields):
             # skip calculated fields unless include_calculated given
             if include_calculated or _model_has_field(admin.model, f):
                 yield f
 
-    def visible(model_admin, request):
+    def visible(model_admin):
+        if not request.user:
+            return False  # pragma: no cover
+
         has_attrs = all(
             hasattr(model_admin, a) for a in ["get_fieldsets", "model", "get_queryset"]
         )
         if not has_attrs or not issubclass(model_admin.model, models.Model):
             debug_log(
                 f"{type(model_admin)} instance does not look like a ModelAdmin or"
                 " InlineModelAdmin"
@@ -174,23 +188,23 @@
     def get_common(admin, model):
         all_model_fields[model].update(from_fieldsets(admin, include_calculated=False))
         all_model_fields[model].update(_get_option(admin, "extra_fields", request))
         hidden_model_fields[model].update(_get_option(admin, "hide_fields", request))
 
     model_admins = {}
     for model, model_admin in site._registry.items():
-        if visible(model_admin, request):
+        if visible(model_admin):
             model_admins[model] = model_admin
             all_model_fields[model].update(model_admin.get_list_display(request))
             all_model_fields[model].add(open_in_admin)
             get_common(model_admin, model)
 
             # check the inlines, these are already filtered for access
             for inline in model_admin.get_inline_instances(request):
-                if visible(inline, request):
+                if visible(inline):
                     try:
                         fk_field = _get_foreign_key(model, inline.model, inline.fk_name)
                     except Exception as e:
                         debug_log(e)  # ignore things like GenericInlineModelAdmin
                     else:
                         if inline.model not in model_admins:  # pragma: no branch
                             model_admins[inline.model] = inline
@@ -250,15 +264,15 @@
         return None
 
     pretty_name = _make_pretty(
         getattr(field_func, "short_description", field_name.replace("_", " "))
     )
 
     if isinstance(field_func, _AnnotationDescriptor):
-        qs = admin_get_queryset(admin, request, [field_name])
+        qs = admin_get_queryset(request, admin, [field_name])
 
         annotation = qs.query.annotations.get(field_name)
         if not annotation:  # pragma: no cover
             raise Exception(
                 f"Can't find annotation '{field_name}' for {admin}.{field_name}"
             )
 
@@ -283,15 +297,15 @@
         if field_func is None:
 
             def field_func(obj):
                 value = getattr(obj, field_name)
                 return value() if callable(value) else value
 
         if field_func == open_in_admin and hasattr(admin, "get_actions"):
-            actions = admin_get_actions(admin, request)
+            actions = admin_get_actions(request, admin)
         else:
             actions = {}
 
         return OrmCalculatedField(
             model_name=model_name,
             name=field_name,
             pretty_name=pretty_name,
@@ -391,15 +405,15 @@
                 if json_fields:  # pragma: no branch
                     rel_name = f"{model_name}__{field_name}"
                     orm_models[rel_name] = _make_json_sub_module(
                         model_name, json_fields
                     )
 
             if field_name == model._meta.pk.name and hasattr(admin, "get_actions"):
-                actions = admin_get_actions(admin, request)
+                actions = admin_get_actions(request, admin)
             else:
                 actions = {}
 
             fields[field_name] = OrmConcreteField(
                 model_name=model_name,
                 name=field_name,
                 pretty_name=pretty_name,
```

### Comparing `django-data-browser-4.2.1/data_browser/orm_aggregates.py` & `django-data-browser-4.2.2/data_browser/orm_aggregates.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/orm_debug.py` & `django-data-browser-4.2.2/data_browser/orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/orm_fields.py` & `django-data-browser-4.2.2/data_browser/orm_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from typing import Sequence, Tuple
 
 from django.db import models
 from django.db.models import OuterRef, Subquery
 
+from .common import global_state
 from .orm_debug import DebugQS
 from .types import (
     ASC,
     BaseType,
     BooleanType,
     DateTimeType,
     DateType,
@@ -43,20 +44,20 @@
         return self.field.can_pivot
 
     def _lineage(self):
         if self.previous:
             return self.previous._lineage() + [self]
         return [self]
 
-    def annotate(self, request, qs, debug=False):
+    def annotate(self, qs, debug=False):
         for field in self._lineage():
-            qs = field._annotate(request, qs, debug=debug)
+            qs = field._annotate(qs, debug=debug)
         return qs
 
-    def _annotate(self, request, qs, debug=False):
+    def _annotate(self, qs, debug=False):
         return qs
 
     def _annotate_qs(self, qs, expression):
         assert "__" not in self.queryset_path_str
         return qs.annotate(**{self.queryset_path_str: expression})
 
     def __getattr__(self, name):
@@ -206,28 +207,30 @@
 
             return base_formatter(value)
 
         return format
 
 
 class OrmBoundAnnotatedField(OrmBoundField):
-    def _annotate(self, request, qs, debug=False):
+    def _annotate(self, qs, debug=False):
         from .orm_admin import admin_get_queryset
 
         if debug:
             subquery = DebugQS("Subquery")
             outer_ref = DebugQS("OuterRef")
         else:
             subquery = Subquery
             outer_ref = OuterRef
 
         return self._annotate_qs(
             qs,
             subquery(
-                admin_get_queryset(self.admin, request, [self.name], debug=debug)
+                admin_get_queryset(
+                    global_state.request, self.admin, [self.name], debug=debug
+                )
                 .filter(pk=outer_ref("__".join(self.previous.queryset_path + ["pk"])))
                 .values(self.name)[:1],
                 output_field=self.django_field,
             ),
         )
```

### Comparing `django-data-browser-4.2.1/data_browser/orm_functions.py` & `django-data-browser-4.2.2/data_browser/orm_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             ),
         }
     )
     return mapping[name]
 
 
 class OrmBoundFunctionField(OrmBoundField):
-    def _annotate(self, request, qs, debug=False):
+    def _annotate(self, qs, debug=False):
         func = _get_django_function(self.previous.type_, self.name, qs)[0](
             self.previous.queryset_path_str
         )
         return self._annotate_qs(qs, func)
 
     def parse_lookup(self, lookup, value):
         parsed, error_message = super().parse_lookup(lookup, value)
```

### Comparing `django-data-browser-4.2.1/data_browser/orm_lookups.py` & `django-data-browser-4.2.2/data_browser/orm_lookups.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/orm_results.py` & `django-data-browser-4.2.2/data_browser/orm_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,25 +54,25 @@
         bound_query.row_fields + body_fields,
         filters,
         bound_query.limit,
         bound_query.orm_model,
     )
 
 
-def get_result_queryset(request, bound_query, debug=False):
+def get_result_queryset(bound_query, debug=False):
     all_fields = {f.queryset_path_str: f for f in bound_query.bound_fields}
     all_fields.update({f.queryset_path_str: f for f in bound_query.bound_filters})
 
     qs = bound_query.orm_model.get_queryset(
-        request, {f.split("__")[0] for f in all_fields}, debug=debug
+        {f.split("__")[0] for f in all_fields}, debug=debug
     )
 
     # sql functions and qs annotations
     for field in all_fields.values():
-        qs = field.annotate(request, qs, debug=debug)
+        qs = field.annotate(qs, debug=debug)
 
     # filter normal and sql function fields (aka __date)
     for filter_ in bound_query.valid_filters:
         if filter_.orm_bound_field.filter_:
             qs = _filter(qs, filter_.orm_bound_field.queryset_path_str, filter_)
 
     # nothing to group on, early out with an aggregate
@@ -116,36 +116,34 @@
             # this comes up with impliclty ordered fields, which are neither
             sort_fields.append(field.orm_bound_field.queryset_path_str)
     qs = qs.order_by(*sort_fields)
 
     return qs[: bound_query.limit]
 
 
-def get_result_list(request, bound_query):
-    return list(get_result_queryset(request, bound_query))
+def get_result_list(bound_query):
+    return list(get_result_queryset(bound_query))
 
 
-def _get_objs_for_calculated_fields(request, bound_query, orm_models, res):
+def _get_objs_for_calculated_fields(bound_query, orm_models, res):
     # gather up all the objects to fetch for calculated fields
     to_load = defaultdict(set)
     loading_for = defaultdict(set)
     for field in bound_query.bound_fields:
         if field.model_name:
             loading_for[field.model_name].add(field.name)
             pks = to_load[field.model_name]
             for row in res:
                 pks.add(row[field.queryset_path_str])
 
     # fetch all the calculated field objects
     objs = {}
     for model_name, pks in to_load.items():
         objs[model_name] = (
-            orm_models[model_name]
-            .get_queryset(request, loading_for[model_name])
-            .in_bulk(pks)
+            orm_models[model_name].get_queryset(loading_for[model_name]).in_bulk(pks)
         )
 
     return objs
 
 
 # dump out the results
 def _format_table(fields, data, objs):
@@ -209,32 +207,32 @@
         table = []
         for row_key in row_keys:
             table.append(data[row_key].get(col_key))
         body_data.append(_format_table(fields, table, objs))
     return body_data
 
 
-def get_results(request, bound_query, orm_models, with_format_hints):
+def get_results(bound_query, orm_models, with_format_hints):
     if not bound_query.fields:
         return {"rows": [], "cols": [], "body": [], "length": 0}
 
-    res = get_result_list(request, bound_query)
+    res = get_result_list(bound_query)
 
     if not res:
         return {"rows": [], "cols": [], "body": [], "length": 0}
 
     if bound_query.bound_col_fields and bound_query.bound_row_fields:
         # need to fetch rows and col titles seperately to get correct sort
-        rows_res = get_result_list(request, _rows_sub_query(bound_query))
-        cols_res = get_result_list(request, _cols_sub_query(bound_query))
+        rows_res = get_result_list(_rows_sub_query(bound_query))
+        cols_res = get_result_list(_cols_sub_query(bound_query))
     else:
         rows_res = res
         cols_res = res
 
-    objs = _get_objs_for_calculated_fields(request, bound_query, orm_models, res)
+    objs = _get_objs_for_calculated_fields(bound_query, orm_models, res)
 
     if bound_query.bound_col_fields or bound_query.bound_body_fields:
         raw_body_data, raw_row_data, raw_col_data = _get_data_and_all_keys(
             bound_query, res
         )
 
         # the raw versions have the subset of correct results
```

### Comparing `django-data-browser-4.2.1/data_browser/orm_types.py` & `django-data-browser-4.2.2/data_browser/orm_types.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/query.py` & `django-data-browser-4.2.2/data_browser/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,10 +328,10 @@
         return _orm_fields(self.row_fields)
 
     @cached_property
     def bound_body_fields(self):
         return _orm_fields(self.body_fields)
 
     def all_valid(self):
-        fields_valid = all(f.is_valid for f in self.filters)
+        fields_valid = all(f.is_valid for f in self.fields)
         filters_valid = all(f.is_valid for f in self.filters)
         return fields_valid and filters_valid
```

### Comparing `django-data-browser-4.2.1/data_browser/templates/data_browser/index.html` & `django-data-browser-4.2.2/data_browser/templates/data_browser/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/types.py` & `django-data-browser-4.2.2/data_browser/types.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/urls.py` & `django-data-browser-4.2.2/data_browser/urls.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/views.py` & `django-data-browser-4.2.2/data_browser/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
 from . import version
 from .common import (
     PUBLIC_PERM,
     SHARE_PERM,
     HttpResponse,
     JsonResponse,
-    add_request_info,
+    global_state,
     has_permission,
+    set_global_state,
     settings,
 )
 from .format_csv import get_csv_rows
 from .models import View
-from .orm_admin import get_models
 from .orm_results import get_result_list, get_result_queryset, get_results
 from .query import BoundQuery, Query, QueryFilter
 from .types import TYPES
 from .util import str_to_field
 
 
 def _get_query_data(bound_query):
@@ -113,16 +113,16 @@
                 "value": filter_.value,
             }
             for filter_ in bq.filters
         ],
     }
 
 
-def _get_config(request):
-    orm_models = get_models(request)
+def _get_config():
+    orm_models = global_state.models
     types = {
         name: {
             "lookups": {
                 n: {"prettyName": tn, "type": t}
                 for n, (tn, t, _) in type_.lookups.items()
             },
             "sortedLookups": list(type_.lookups),
@@ -136,82 +136,81 @@
         model_name: _get_model_fields(model_name, orm_models)
         for model_name in orm_models
     }
 
     model_names_by_app = defaultdict(set)
     for name, model in orm_models.items():
         if model.root:
-            # todo why don't we get this in parts and then assemble it
+            # TODO why don't we get this in parts and then assemble it
             app_name, model_name = name.split(".")
             model_names_by_app[app_name].add(model_name)
 
     return {
         "baseUrl": reverse("data_browser:home"),
         "types": types,
         "allModelFields": all_model_fields,
         "sortedModels": [
             {"appName": app_name, "modelNames": sorted(model_names)}
             for app_name, model_names in sorted(model_names_by_app.items())
         ],
-        "canMakePublic": has_permission(request.user, PUBLIC_PERM),
-        "canShare": has_permission(request.user, SHARE_PERM),
+        "canMakePublic": has_permission(global_state.request.user, PUBLIC_PERM),
+        "canShare": has_permission(global_state.request.user, SHARE_PERM),
         "sentryDsn": settings.DATA_BROWSER_FE_DSN,
         "defaultRowLimit": settings.DATA_BROWSER_DEFAULT_ROW_LIMIT,
         "appsExpanded": settings.DATA_BROWSER_APPS_EXPANDED,
     }
 
 
 @admin_decorators.staff_member_required
+@set_global_state(public_view=False)
 def query_ctx(request, *, model_name="", fields=""):
-    add_request_info(request)
-    config = _get_config(request)
+    config = _get_config()
     return JsonResponse(config)
 
 
 def admin_action(request, model_name, fields):
     data = json.loads(request.body)
     action = data["action"]
     field = data["field"]
 
     if field not in fields:
         raise http.Http404(f"bad field '{field}'")  # pragma: no cover
 
     params = hyperlink.parse(request.get_full_path()).query
     query = Query.from_request(model_name, fields, params)
 
-    orm_models = get_models(request)
+    orm_models = global_state.models
     if query.model_name not in orm_models:
         raise http.Http404(f"'{query.model_name}' does not exist")  # pragma: no cover
 
     bound_query = BoundQuery.bind(query, orm_models)
     idx = [field.path_str for field in bound_query.fields].index(field)
     bound_field = bound_query.fields[idx].orm_bound_field
 
     if not bound_field.field.actions or action not in bound_field.field.actions:
         raise http.Http404(f"bad action '{action}'")  # pragma: no cover
 
-    results = get_result_list(request, bound_query)
+    results = get_result_list(bound_query)
 
     pks = {row[bound_field.queryset_path_str] for row in results}
     pks -= {None}
 
     model_name = bound_field.field.model_name
-    return orm_models[model_name].get_http_request_for_action(request, action, pks)
+    return orm_models[model_name].get_http_request_for_action(action, pks)
 
 
 @csrf.csrf_protect
 @csrf.ensure_csrf_cookie
 @admin_decorators.staff_member_required
+@set_global_state(public_view=False)
 def query_html(request, *, model_name="", fields=""):
-    add_request_info(request)
-
     if request.method == "POST":
         return admin_action(request, model_name, fields)
 
-    config = _get_config(request)
+    config = _get_config()
     config = json.dumps(config, cls=DjangoJSONEncoder)
     config = (
         config.replace("<", "\\u003C").replace(">", "\\u003E").replace("&", "\\u0026")
     )
 
     if settings.DATA_BROWSER_DEV:  # pragma: no cover
         try:
@@ -223,32 +222,31 @@
     else:
         template = loader.get_template("data_browser/index.html")
 
     return TemplateResponse(request, template, {"config": config, "version": version})
 
 
 @admin_decorators.staff_member_required
+@set_global_state(public_view=False)
 def query(request, *, model_name, fields="", media):
-    add_request_info(request)
-
     params = hyperlink.parse(request.get_full_path()).query
 
     if media.startswith("profile") or media.startswith("pstats"):
         if "_" in media:
             prof_media, media = media.split("_")
         else:
             prof_media = media
             media = "json"
 
         profiler = cProfile.Profile()
         try:
             profiler.enable()
 
             query = Query.from_request(model_name, fields, params)
-            for x in _data_response(request, query, media, privileged=True):
+            for x in _data_response(query, media, privileged=True):
                 pass
 
             profiler.disable()
 
             if prof_media == "profile":
                 buffer = io.StringIO()
                 stats = pstats.Stats(profiler, stream=buffer)
@@ -269,71 +267,68 @@
             else:
                 raise http.Http404(f"Bad file format {prof_media} requested")
         finally:
             if profiler:  # pragma: no branch
                 profiler.disable()
     else:
         query = Query.from_request(model_name, fields, params)
-        return _data_response(request, query, media, privileged=True)
+        return _data_response(query, media, privileged=True)
 
 
 def view(request, pk, media):
-    add_request_info(request, view=True)
-
     view = get_object_or_404(View.objects.filter(public=True), public_slug=pk)
-    if (
-        # some of these are checked by the admin but this is a good time to be paranoid
-        view.owner.is_active
-        and view.owner.is_staff
-        and has_permission(view.owner, PUBLIC_PERM)
-        and settings.DATA_BROWSER_ALLOW_PUBLIC
-    ):
-        request.user = view.owner  # public views are run as the person who owns them
-        query = view.get_query()
-        return _data_response(request, query, media, privileged=False, strict=True)
-    else:
-        raise http.Http404("No View matches the given query.")
+    with set_global_state(request=request, user=view.owner, public_view=True):
+        if (
+            # some of these are checked by the admin but this is a good time to be paranoid
+            view.owner
+            and view.owner.is_active
+            and view.owner.is_staff
+            and has_permission(view.owner, PUBLIC_PERM)
+            and settings.DATA_BROWSER_ALLOW_PUBLIC
+            and view.is_valid()
+        ):
+            query = view.get_query()
+            return _data_response(query, media, privileged=False)
+        else:
+            raise http.Http404("No View matches the given query.")
 
 
 class Echo:
     def write(self, value):
         return value
 
 
-def _data_response(request, query, media, privileged=False, strict=False):
-    orm_models = get_models(request)
+def _data_response(query, media, privileged=False):
+    orm_models = global_state.models
     if query.model_name not in orm_models:
         raise http.Http404(f"{query.model_name} does not exist")
     bound_query = BoundQuery.bind(query, orm_models)
 
-    if strict and not bound_query.all_valid():
-        return http.HttpResponseBadRequest()
-
     if media == "csv":
-        results = get_results(request, bound_query, orm_models, False)
+        results = get_results(bound_query, orm_models, False)
         csv_rows = get_csv_rows(bound_query, results)
 
         writer = csv.writer(Echo())
         response = http.StreamingHttpResponse(
             (writer.writerow(row) for row in csv_rows), content_type="text/csv"
         )
         response["Content-Disposition"] = (
             f"attachment; filename={query.model_name}-{timezone.now().isoformat()}.csv"
         )
         return response
     elif media == "json":
-        results = get_results(request, bound_query, orm_models, True)
+        results = get_results(bound_query, orm_models, True)
         resp = _get_query_data(bound_query) if privileged else {}
         resp.update(results)
         return JsonResponse(resp)
     elif privileged and media == "query":
         resp = _get_query_data(bound_query)
         return JsonResponse(resp)
     elif privileged and media in ["sql", "explain", "qs"]:
-        query_set = get_result_queryset(request, bound_query, media == "qs")
+        query_set = get_result_queryset(bound_query, media == "qs")
         if isinstance(query_set, list):
             res = "Not available for pure aggregates"
         else:
             if media == "sql":
                 res = (
                     "/* This is an approximation of the main query.\nPages with pivoted"
                     " or calculated data may do additional queries. */\n\n"
```

### Comparing `django-data-browser-4.2.1/data_browser/web_root/android-chrome-192x192.png` & `django-data-browser-4.2.2/data_browser/web_root/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/web_root/android-chrome-512x512.png` & `django-data-browser-4.2.2/data_browser/web_root/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/web_root/apple-touch-icon.png` & `django-data-browser-4.2.2/data_browser/web_root/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/web_root/favicon-32x32.png` & `django-data-browser-4.2.2/data_browser/web_root/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/data_browser/web_root/favicon.ico` & `django-data-browser-4.2.2/data_browser/web_root/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/django_data_browser.egg-info/PKG-INFO` & `django-data-browser-4.2.2/django_data_browser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-browser
-Version: 4.2.1
+Version: 4.2.2
 Summary: Interactive user-friendly database explorer.
 Home-page: https://github.com/tolomea/django-data-browser
 Author: Gordon Wrigley
 Author-email: gordon.wrigley@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -365,14 +365,16 @@
 
 Release History
 ---------------
 
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | Version | Date       | Summary                                                                                                  |
 +=========+============+==========================================================================================================+
+| 4.2.2   | 2023-06-08 | Fix various issues around saved view validity.                                                           |
++---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.2.1   | 2023-05-21 | | BREAKING: In JSON format move ``parsed`` and ``fitlerErrors`` onto the filters.                        |
 |         |            | | Display invalid fields (previously they were ignored).                                                 |
 |         |            | | Fix small bug when removing filters with errors.                                                       |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.1   | 2023-05-07 | Fix bug with shared views when using multiple authentication backends.                                   |
 +---------+------------+----------------------------------------------------------------------------------------------------------+
 | 4.1.0   | 2023-05-01 | | Support sharing of saved views between users.                                                          |
```

### Comparing `django-data-browser-4.2.1/django_data_browser.egg-info/SOURCES.txt` & `django-data-browser-4.2.2/django_data_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/README.md` & `django-data-browser-4.2.2/frontend/README.md`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/package-lock.json` & `django-data-browser-4.2.2/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/package.json` & `django-data-browser-4.2.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/public/index.html` & `django-data-browser-4.2.2/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/App.js` & `django-data-browser-4.2.2/frontend/src/App.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/App.scss` & `django-data-browser-4.2.2/frontend/src/App.scss`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/ContextMenu.js` & `django-data-browser-4.2.2/frontend/src/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/CurrentSavedView.js` & `django-data-browser-4.2.2/frontend/src/CurrentSavedView.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/HomePage.js` & `django-data-browser-4.2.2/frontend/src/HomePage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/Query.js` & `django-data-browser-4.2.2/frontend/src/Query.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/QueryPage.js` & `django-data-browser-4.2.2/frontend/src/QueryPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/Results.js` & `django-data-browser-4.2.2/frontend/src/Results.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/SavedViewPage.js` & `django-data-browser-4.2.2/frontend/src/SavedViewPage.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/Tooltip.js` & `django-data-browser-4.2.2/frontend/src/Tooltip.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/Util.js` & `django-data-browser-4.2.2/frontend/src/Util.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/WindowDimensions.js` & `django-data-browser-4.2.2/frontend/src/WindowDimensions.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/index.js` & `django-data-browser-4.2.2/frontend/src/index.js`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/frontend/src/logo.svg` & `django-data-browser-4.2.2/frontend/src/logo.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/pyproject.toml` & `django-data-browser-4.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/screenshot.png` & `django-data-browser-4.2.2/screenshot.png`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/setup.py` & `django-data-browser-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/structure.svg` & `django-data-browser-4.2.2/structure.svg`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/array/models.py` & `django-data-browser-4.2.2/tests/array/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/conftest.py` & `django-data-browser-4.2.2/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,27 +61,30 @@
     TIME_ZONE="UTC",
     SECRET_KEY="secret",
 )
 
 
 @pytest.fixture
 def ddb_request(rf):
-    from data_browser.common import add_request_info
+    from data_browser.common import global_state, set_global_state
 
     request = rf.get("/")
-    add_request_info(request)
-    return request
+    with set_global_state(request=request, public_view=False):
+        yield global_state.request
 
 
 @pytest.fixture
 def admin_ddb_request(ddb_request, admin_user):
-    ddb_request.user = admin_user
-    return ddb_request
+    from data_browser.common import global_state, set_global_state
+
+    with set_global_state(user=admin_user, public_view=False):
+        yield global_state.request
 
 
 @pytest.fixture
 def mock_admin_get_queryset(mocker):
-    from data_browser.orm_admin import admin_get_queryset
+    from data_browser.orm_admin import _admin_get_queryset
 
+    # TODO, I really want to patch ModelAdmin.get_queryset but can't work out how
     return mocker.patch(
-        "data_browser.orm_admin.admin_get_queryset", wraps=admin_get_queryset
+        "data_browser.orm_admin._admin_get_queryset", wraps=_admin_get_queryset
     )
```

### Comparing `django-data-browser-4.2.1/tests/core/admin.py` & `django-data-browser-4.2.2/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/core/migrations/0001_initial.py` & `django-data-browser-4.2.2/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/core/models.py` & `django-data-browser-4.2.2/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/snapshots/snap_test_views.py` & `django-data-browser-4.2.2/tests/snapshots/snap_test_views.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/test_api.py` & `django-data-browser-4.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/test_array_field.py` & `django-data-browser-4.2.2/tests/test_array_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from django.contrib import admin
 
 from data_browser import migration_helpers
+from data_browser.common import global_state
 from data_browser.models import View
-from data_browser.orm_admin import get_models
 from data_browser.orm_results import get_results
 from data_browser.query import BoundQuery, Query
 
 from .conftest import ARRAY_FIELD_SUPPORT
 
 if ARRAY_FIELD_SUPPORT:
     from .array.models import ArrayModel
@@ -30,20 +30,20 @@
     yield
     admin.site.unregister(ArrayModel)
 
 
 @pytest.fixture
 def get_results_flat(with_arrays, admin_ddb_request):
     def helper(*fields, **filters):
-        orm_models = get_models(admin_ddb_request)
+        orm_models = global_state.models
         query = Query.from_request(
             "array.ArrayModel", ",".join(fields), list(filters.items())
         )
         bound_query = BoundQuery.bind(query, orm_models)
-        data = get_results(admin_ddb_request, bound_query, orm_models, False)
+        data = get_results(bound_query, orm_models, False)
 
         for f in bound_query.filters:
             if f.error_message:
                 print(  # pragma: no cover
                     "filter error:",
                     f.path_str,
                     f.lookup,
@@ -191,15 +191,15 @@
         ("int_choice_array_field__wtf=1", "int_choice_array_field__wtf=1"),
         # regular array -> noop
         ("char_array_field__contains=a", "char_array_field__contains=a"),
         ("int_array_field__contains=1", "int_array_field__contains=1"),
     ],
 )
 def test_0009(admin_ddb_request, with_arrays, before, after):
-    orm_models = get_models(admin_ddb_request)
+    orm_models = global_state.models
     valid = int("wtf" not in before)
 
     view = View.objects.create(model_name="array.ArrayModel", query=before)
     migration_helpers.forwards_0009(View)
     view.refresh_from_db()
     assert view.query == after
     assert len(BoundQuery.bind(view.get_query(), orm_models).valid_filters) == valid
```

### Comparing `django-data-browser-4.2.1/tests/test_common.py` & `django-data-browser-4.2.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/test_helpers.py` & `django-data-browser-4.2.2/tests/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.contrib import admin
 
+from data_browser.common import global_state
 from data_browser.orm_admin import get_models
 
 from .core.admin import AddressAdmin, ProductAdmin
 from .core.models import Address, Producer, Product
 
 
 class TestAdminMixin:
@@ -84,10 +85,10 @@
     def test_ddb_url_ignored(self, admin_client):
         resp = admin_client.get("/admin/core/ignored/")
         assert resp.status_code == 200
         assert "ddb_url" not in resp.context
 
 
 def test_admin_options_setting(admin_ddb_request, settings):
-    assert "core.InAdmin" in get_models(admin_ddb_request)
+    assert "core.InAdmin" in get_models(global_state.request)
     settings.DATA_BROWSER_ADMIN_OPTIONS = {"tests.core.admin.InAdmin": {"ignore": True}}
-    assert "core.InAdmin" not in get_models(admin_ddb_request)
+    assert "core.InAdmin" not in get_models(global_state.request)
```

### Comparing `django-data-browser-4.2.1/tests/test_json_field.py` & `django-data-browser-4.2.2/tests/test_json_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from django.contrib import admin
 
+from data_browser.common import global_state
 from data_browser.helpers import AdminMixin
-from data_browser.orm_admin import get_models
 from data_browser.orm_results import get_results
 from data_browser.query import BoundQuery, Query
 
 from .json.models import JsonModel
 
 # Howto enable SQLite JSON support https://code.djangoproject.com/wiki/JSON1Extension
 
@@ -24,20 +24,20 @@
     yield
     admin.site.unregister(JsonModel)
 
 
 @pytest.fixture
 def get_results_flat(with_json, admin_ddb_request):
     def helper(*fields, **filters):
-        orm_models = get_models(admin_ddb_request)
+        orm_models = global_state.models
         query = Query.from_request(
             "json.JsonModel", ",".join(fields), list(filters.items())
         )
         bound_query = BoundQuery.bind(query, orm_models)
-        data = get_results(admin_ddb_request, bound_query, orm_models, False)
+        data = get_results(bound_query, orm_models, False)
 
         for f in bound_query.filters:
             if f.error_message:
                 print(
                     "filter error:",
                     f.path_str,
                     f.lookup,
```

### Comparing `django-data-browser-4.2.1/tests/test_migrations.py` & `django-data-browser-4.2.2/tests/test_migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
 from data_browser import migration_helpers
+from data_browser.common import global_state
 from data_browser.models import View
-from data_browser.orm_admin import get_models
 from data_browser.query import BoundQuery
 
 
 @pytest.fixture
 def models(admin_ddb_request):
-    return get_models(admin_ddb_request)
+    return global_state.models
 
 
 @pytest.mark.django_db
 @pytest.mark.parametrize(
     "before,after",
     [
         # is_null
```

### Comparing `django-data-browser-4.2.1/tests/test_models.py` & `django-data-browser-4.2.2/tests/test_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import pytest
 
-from data_browser.models import View, global_data
+from data_browser.common import global_state, set_global_state
+from data_browser.models import View
 
 
 @pytest.fixture
-def view():
-    return View(model_name="app.model", fields="+fa,-fd,fn", query="bob__equals=fred")
+def view(admin_user):
+    return View(
+        model_name="core.Product",
+        fields="name+0,size-1,size_unit",
+        query="name__equals=fred",
+        owner=admin_user,
+    )
 
 
 @pytest.fixture
 def global_request(rf):
     request = rf.get("/")
-    global_data.request = request
-    yield request
-    global_data.request = None
+    with set_global_state(request=request, public_view=False):
+        yield global_state.request
 
 
 def test_str(view):
     view.name = "bob"
-    assert str(view) == "app.model view: bob"
+    assert str(view) == "core.Product view: bob"
 
 
 def test_public_link(view, global_request, settings):
     assert view.public_link() == "N/A"
     view.public = True
     expected = f"http://testserver/data_browser/view/{view.public_slug}.csv"
     assert view.public_link() == expected
```

### Comparing `django-data-browser-4.2.1/tests/test_orm.py` & `django-data-browser-4.2.2/tests/test_orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import django
 import pytest
 from django.contrib.admin.options import BaseModelAdmin
 from django.contrib.auth.models import Permission, User
 from django.utils import timezone
 
-from data_browser.orm_admin import OrmModel, get_models
+from data_browser.common import global_state
+from data_browser.orm_admin import OrmModel
 from data_browser.orm_results import get_results
 from data_browser.query import BoundQuery, Query
 
 from .conftest import POSTGRES
 from .core import models
 from .util import ANY, KEYS, UTC
 
@@ -92,30 +93,30 @@
         models.Product.objects.create(
             created_time=dt, name=str(dt), size=i + 1, producer=producer
         )
 
 
 @pytest.fixture
 def get_orm_models(admin_ddb_request):
-    return lambda: get_models(admin_ddb_request)
+    return lambda: global_state.models
 
 
 @pytest.fixture
 def orm_models(get_orm_models):
     return get_orm_models()
 
 
 @pytest.fixture
 def get_product_pivot(admin_ddb_request, get_orm_models, django_assert_num_queries):
     def helper(queries, *args, **kwargs):
         orm_models = get_orm_models()
         query = Query.from_request("core.Product", *args, **kwargs)
         bound_query = BoundQuery.bind(query, orm_models)
         with django_assert_num_queries(queries):
-            data = get_results(admin_ddb_request, bound_query, orm_models, False)
+            data = get_results(bound_query, orm_models, False)
             return {
                 "cols": flatten_table(bound_query.col_fields, data["cols"]),
                 "rows": flatten_table(bound_query.row_fields, data["rows"]),
                 "body": [
                     flatten_table(bound_query.body_fields, row) for row in data["body"]
                 ],
             }
@@ -195,20 +196,20 @@
     def boom(*args, **kwargs):
         assert False
 
     monkeypatch.setattr(FileSystemStorage, "__init__", boom)
     default_storage._wrapped = empty
 
     # copy what the fixture does
-    orm_models = get_models(admin_ddb_request)
+    orm_models = global_state.models
 
     def get_product_flat(*args, **kwargs):
         query = Query.from_request("core.Product", *args)
         bound_query = BoundQuery.bind(query, orm_models)
-        data = get_results(admin_ddb_request, bound_query, orm_models, False)
+        data = get_results(bound_query, orm_models, False)
         return flatten_table(bound_query.fields, data["rows"])
 
     # some storage backends will hard fail if their underlying storage isn't
     # setup right https://github.com/tolomea/django-data-browser/issues/11
     producer = models.Producer.objects.create()
     models.Product.objects.create(name="a", producer=producer)
     models.Product.objects.create(name="b", producer=producer, image="bob.jpg")
@@ -782,15 +783,15 @@
 class TestPermissions:
     def get_fields_with_perms(self, ddb_request, perms):
         user = User.objects.create()
         for perm in perms:
             user.user_permissions.add(Permission.objects.get(codename=f"change_{perm}"))
 
         ddb_request.user = user
-        return get_models(ddb_request)
+        return global_state.models
 
     @pytest.mark.django_db
     def test_all_perms(self, ddb_request):
         orm_models = self.get_fields_with_perms(
             ddb_request, ["normal", "notinadmin", "inadmin", "inlineadmin"]
         )
```

### Comparing `django-data-browser-4.2.1/tests/test_orm_debug.py` & `django-data-browser-4.2.2/tests/test_orm_debug.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/test_query.py` & `django-data-browser-4.2.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-data-browser-4.2.1/tests/test_views.py` & `django-data-browser-4.2.2/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -374,25 +374,44 @@
 
     res = admin_client.get(f"/data_browser/view/{view.public_slug}.json")
     assert res.status_code == 200
 
     view.query = "sixe__lt=2&id__gt=0"
     view.save()
     res = admin_client.get(f"/data_browser/view/{view.public_slug}.json")
-    assert res.status_code == 400
+    assert res.status_code == 404
 
     view.query = "size__lx=2&id__gt=0"
     view.save()
     res = admin_client.get(f"/data_browser/view/{view.public_slug}.json")
-    assert res.status_code == 400
+    assert res.status_code == 404
 
     view.query = "size__lt=a&id__gt=0"
     view.save()
     res = admin_client.get(f"/data_browser/view/{view.public_slug}.json")
-    assert res.status_code == 400
+    assert res.status_code == 404
+
+
+@pytest.mark.usefixtures("products")
+def test_view_bad_field(admin_client):
+    view = data_browser.models.View.objects.create(
+        model_name="core.Product",
+        fields="size-0,name+1,size_unit",
+        query="size__lt=2&id__gt=0",
+        owner=User.objects.get(),
+        public=True,
+    )
+
+    res = admin_client.get(f"/data_browser/view/{view.public_slug}.json")
+    assert res.status_code == 200
+
+    view.fields = "invalid"
+    view.save()
+    res = admin_client.get(f"/data_browser/view/{view.public_slug}.json")
+    assert res.status_code == 404
 
 
 @pytest.mark.usefixtures("products")
 def test_action(admin_client):
     url = "/data_browser/query/core.Product/id.%s"
 
     ids = set(models.Product.objects.values_list("id", flat=True))
```

### Comparing `django-data-browser-4.2.1/tox.ini` & `django-data-browser-4.2.2/tox.ini`

 * *Files identical despite different names*

