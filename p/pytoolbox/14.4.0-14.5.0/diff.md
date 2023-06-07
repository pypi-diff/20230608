# Comparing `tmp/pytoolbox-14.4.0.tar.gz` & `tmp/pytoolbox-14.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoolbox-14.4.0.tar", last modified: Fri Dec  9 11:25:59 2022, max compression
+gzip compressed data, was "pytoolbox-14.5.0.tar", last modified: Wed Jun  7 22:11:06 2023, max compression
```

## Comparing `pytoolbox-14.4.0.tar` & `pytoolbox-14.5.0.tar`

### file list

```diff
@@ -1,194 +1,216 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.747899 pytoolbox-14.4.0/
--rw-rw-r--   0 david     (1000) david     (1000)      233 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/AUTHORS
--rw-r--r--   0 david     (1000) david     (1000)     5747 2018-11-12 11:04:46.000000 pytoolbox-14.4.0/LICENSE.rst
--rw-r--r--   0 david     (1000) david     (1000)       48 2018-11-12 11:04:46.000000 pytoolbox-14.4.0/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     7591 2022-12-09 11:25:59.747899 pytoolbox-14.4.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     6011 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/README.rst
--rw-rw-r--   0 david     (1000) david     (1000)    29372 2022-12-09 11:04:16.000000 pytoolbox-14.4.0/changelog.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/
--rw-rw-r--   0 david     (1000) david     (1000)       23 2022-12-09 11:04:41.000000 pytoolbox-14.4.0/pytoolbox/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/ai/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/ai/vision/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/ai/vision/face/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/face/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/ai/vision/face/detect/
--rw-rw-r--   0 david     (1000) david     (1000)       67 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/face/detect/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8863 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/face/detect/dlib.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/ai/vision/face/recognize/
--rw-rw-r--   0 david     (1000) david     (1000)       97 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/face/recognize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11379 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py
--rw-rw-r--   0 david     (1000) david     (1000)      603 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/ai/vision/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     3178 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1703 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/atlassian.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/aws/
--rw-rw-r--   0 david     (1000) david     (1000)       35 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/aws/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2712 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/aws/s3.py
--rw-rw-r--   0 david     (1000) david     (1000)    10233 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     4013 2022-12-09 10:51:31.000000 pytoolbox-14.4.0/pytoolbox/comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)     5248 2022-12-09 10:58:11.000000 pytoolbox-14.4.0/pytoolbox/console.py
--rw-rw-r--   0 david     (1000) david     (1000)     5763 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/crypto.py
--rw-rw-r--   0 david     (1000) david     (1000)    10583 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)     4411 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox/django/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/core/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/core/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       77 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/core/constants.py
--rw-rw-r--   0 david     (1000) david     (1000)     2592 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/core/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     2536 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/core/validators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/forms/
--rw-rw-r--   0 david     (1000) david     (1000)       20 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/forms/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      693 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/forms/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      528 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/forms/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     5334 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/forms/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     3518 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/forms/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      752 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/forms/widgets.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/models/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      377 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1623 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/models/fields/
--rw-rw-r--   0 david     (1000) david     (1000)       20 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/fields/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4162 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/fields/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1264 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/fields/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/models/managers/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/models/managers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      738 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/managers/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      433 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/metaclass.py
--rw-rw-r--   0 david     (1000) david     (1000)    15199 2022-12-09 07:17:03.000000 pytoolbox-14.4.0/pytoolbox/django/models/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/models/query/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/models/query/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2555 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/query/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1482 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/models/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/signals/
--rw-rw-r--   0 david     (1000) david     (1000)       48 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/signals/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      825 2022-12-09 07:17:03.000000 pytoolbox-14.4.0/pytoolbox/django/signals/dispatch.py
--rw-rw-r--   0 david     (1000) david     (1000)     3731 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/signals/handlers.py
--rw-rw-r--   0 david     (1000) david     (1000)     1390 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/storage.py
--rw-rw-r--   0 david     (1000) david     (1000)    10669 2022-10-01 14:38:11.000000 pytoolbox-14.4.0/pytoolbox/django/templatetags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/test/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4761 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/test/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.735899 pytoolbox-14.4.0/pytoolbox/django/test/runner/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/test/runner/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      843 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/test/runner/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      579 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/urls.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django/utils/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django/utils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2339 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/utils/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     1624 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/utils/logging.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django/views/
--rw-rw-r--   0 david     (1000) david     (1000)       20 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      476 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/views/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     4890 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      282 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django/views/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django_datatable_view/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django_datatable_view/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django_datatable_view/views/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django_datatable_view/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1732 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django_datatable_view/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django_filter/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django_filter/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django_filter/filterset/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django_filter/filterset/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      718 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django_filter/filterset/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django_formtools/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django_formtools/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/django_formtools/views/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/django_formtools/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3056 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/django_formtools/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1448 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/enum.py
--rw-rw-r--   0 david     (1000) david     (1000)     3633 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    21424 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     3096 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/flask.py
--rw-rw-r--   0 david     (1000) david     (1000)     6120 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/humanize.py
--rw-rw-r--   0 david     (1000) david     (1000)     2321 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/itertools.py
--rw-rw-r--   0 david     (1000) david     (1000)    49289 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/juju.py
--rw-rw-r--   0 david     (1000) david     (1000)      936 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/linux.py
--rw-rw-r--   0 david     (1000) david     (1000)     3946 2022-12-09 10:52:45.000000 pytoolbox-14.4.0/pytoolbox/logging.py
--rw-rw-r--   0 david     (1000) david     (1000)      281 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/module.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/multimedia/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/multimedia/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/multimedia/exif/
--rw-rw-r--   0 david     (1000) david     (1000)      344 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1555 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/brand.py
--rw-rw-r--   0 david     (1000) david     (1000)      530 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/camera.py
--rw-rw-r--   0 david     (1000) david     (1000)     1021 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/equipment.py
--rw-rw-r--   0 david     (1000) david     (1000)     1664 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/image.py
--rw-rw-r--   0 david     (1000) david     (1000)      754 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/lens.py
--rw-rw-r--   0 david     (1000) david     (1000)     2180 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/metadata.py
--rw-rw-r--   0 david     (1000) david     (1000)     1069 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/photo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3762 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/exif/tag.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.739899 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/
--rw-rw-r--   0 david     (1000) david     (1000)      235 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7144 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/encode.py
--rw-rw-r--   0 david     (1000) david     (1000)     5639 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)     8289 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/ffprobe.py
--rw-rw-r--   0 david     (1000) david     (1000)     6895 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py
--rw-rw-r--   0 david     (1000) david     (1000)     1419 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/multimedia/image/
--rw-rw-r--   0 david     (1000) david     (1000)     2231 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/image/PIL.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/image/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1663 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/multimedia/x264.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/network/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/network/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     6975 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/http.py
--rw-rw-r--   0 david     (1000) david     (1000)     1113 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/ip.py
--rw-rw-r--   0 david     (1000) david     (1000)    15618 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/rtp.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/network/smpte2022/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/network/smpte2022/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    27705 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/smpte2022/base.py
--rw-rw-r--   0 david     (1000) david     (1000)    10798 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/smpte2022/generator.py
--rw-rw-r--   0 david     (1000) david     (1000)    28039 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/smpte2022/receiver.py
--rw-rw-r--   0 david     (1000) david     (1000)      925 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/network/url.py
--rw-rw-r--   0 david     (1000) david     (1000)      479 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/pandas.py
--rw-rw-r--   0 david     (1000) david     (1000)      370 2022-12-09 10:18:59.000000 pytoolbox-14.4.0/pytoolbox/private.py
--rw-rw-r--   0 david     (1000) david     (1000)     3099 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/regex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/rest_framework/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/rest_framework/metadata/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/metadata/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1084 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/metadata/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      825 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/permissions.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/rest_framework/serializers/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/serializers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      742 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/serializers/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     2329 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/serializers/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/rest_framework/views/
--rw-r--r--   0 david     (1000) david     (1000)        0 2022-09-13 21:04:52.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1666 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/rest_framework/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.743899 pytoolbox-14.4.0/pytoolbox/selenium/
--rw-rw-r--   0 david     (1000) david     (1000)      113 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3042 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/client.py
--rw-rw-r--   0 david     (1000) david     (1000)     1137 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/common.py
--rw-rw-r--   0 david     (1000) david     (1000)      428 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)      230 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/select.py
--rw-rw-r--   0 david     (1000) david     (1000)     2535 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/test.py
--rw-rw-r--   0 david     (1000) david     (1000)      779 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/webdrivers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.747899 pytoolbox-14.4.0/pytoolbox/selenium/webelements/
--rw-rw-r--   0 david     (1000) david     (1000)      150 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/webelements/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1090 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/webelements/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      948 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/webelements/bootstrap_slider.py
--rw-rw-r--   0 david     (1000) david     (1000)      427 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/selenium/webelements/bootstrap_switch.py
--rw-rw-r--   0 david     (1000) david     (1000)    19717 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)      410 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/setuptools.py
--rw-rw-r--   0 david     (1000) david     (1000)     1371 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     2520 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/states.py
--rw-rw-r--   0 david     (1000) david     (1000)     4513 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/string.py
--rw-rw-r--   0 david     (1000) david     (1000)    13904 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)     3381 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/throttles.py
--rw-rw-r--   0 david     (1000) david     (1000)     7767 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/types.py
--rw-rw-r--   0 david     (1000) david     (1000)    10245 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)     8898 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/validation.py
--rw-rw-r--   0 david     (1000) david     (1000)     1169 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/virtualenv.py
--rw-rw-r--   0 david     (1000) david     (1000)     2118 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/pytoolbox/voluptuous.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-12-09 11:25:59.731899 pytoolbox-14.4.0/pytoolbox.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     7591 2022-12-09 11:25:59.000000 pytoolbox-14.4.0/pytoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     4949 2022-12-09 11:25:59.000000 pytoolbox-14.4.0/pytoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2022-12-09 11:25:59.000000 pytoolbox-14.4.0/pytoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      845 2022-12-09 11:25:59.000000 pytoolbox-14.4.0/pytoolbox.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       10 2022-12-09 11:25:59.000000 pytoolbox-14.4.0/pytoolbox.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      144 2022-12-09 11:25:59.747899 pytoolbox-14.4.0/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     8102 2022-10-01 14:38:05.000000 pytoolbox-14.4.0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/
+-rw-rw-r--   0 david     (1000) david     (1000)      208 2023-06-07 22:02:37.000000 pytoolbox-14.5.0/AUTHORS.md
+-rw-rw-r--   0 david     (1000) david     (1000)    27931 2023-06-07 22:08:36.000000 pytoolbox-14.5.0/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5747 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/LICENSE.rst
+-rw-rw-r--   0 david     (1000) david     (1000)       27 2023-06-07 22:02:59.000000 pytoolbox-14.5.0/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     7617 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     6034 2023-06-07 22:09:15.000000 pytoolbox-14.5.0/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/
+-rw-rw-r--   0 david     (1000) david     (1000)       23 2023-06-07 22:09:59.000000 pytoolbox-14.5.0/pytoolbox/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/face/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/
+-rw-rw-r--   0 david     (1000) david     (1000)       67 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8907 2023-06-07 20:22:05.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/dlib.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/
+-rw-rw-r--   0 david     (1000) david     (1000)       97 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11379 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py
+-rw-rw-r--   0 david     (1000) david     (1000)      603 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3213 2023-06-07 15:17:33.000000 pytoolbox-14.5.0/pytoolbox/argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1703 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/atlassian.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/aws/
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/aws/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2716 2023-06-07 17:56:24.000000 pytoolbox-14.5.0/pytoolbox/aws/s3.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10233 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3826 2023-06-07 17:29:11.000000 pytoolbox-14.5.0/pytoolbox/comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5380 2023-06-07 17:33:45.000000 pytoolbox-14.5.0/pytoolbox/console.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5749 2023-06-07 17:52:13.000000 pytoolbox-14.5.0/pytoolbox/crypto.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10583 2023-06-07 17:59:59.000000 pytoolbox-14.5.0/pytoolbox/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4457 2023-06-07 19:19:11.000000 pytoolbox-14.5.0/pytoolbox/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/core/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/core/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       77 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/core/constants.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2592 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/core/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2541 2023-06-07 14:42:58.000000 pytoolbox-14.5.0/pytoolbox/django/core/validators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/forms/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/forms/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      693 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      528 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5314 2023-06-07 14:44:46.000000 pytoolbox-14.5.0/pytoolbox/django/forms/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3518 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      752 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/widgets.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      377 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/fields/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/models/fields/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4116 2023-06-07 14:44:04.000000 pytoolbox-14.5.0/pytoolbox/django/models/fields/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1264 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/fields/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/managers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/managers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      738 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/managers/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/metaclass.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15157 2023-06-07 17:58:01.000000 pytoolbox-14.5.0/pytoolbox/django/models/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/query/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/query/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2555 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/query/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1484 2023-06-07 17:58:17.000000 pytoolbox-14.5.0/pytoolbox/django/models/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/signals/
+-rw-rw-r--   0 david     (1000) david     (1000)       64 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/signals/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      505 2023-06-07 14:38:31.000000 pytoolbox-14.5.0/pytoolbox/django/signals/dispatch.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3745 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/signals/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1390 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/storage.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10640 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/templatetags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4761 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/test/runner/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/runner/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      843 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/runner/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      579 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/urls.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2339 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/utils/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1624 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/utils/logging.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      476 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/views/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4892 2023-06-07 17:58:25.000000 pytoolbox-14.5.0/pytoolbox/django/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      282 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/views/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_datatable_view/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_datatable_view/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1732 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_filter/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_filter/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_filter/filterset/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_filter/filterset/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      718 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_filter/filterset/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_formtools/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_formtools/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_formtools/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_formtools/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3056 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_formtools/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1448 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/enum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3639 2023-06-07 17:52:48.000000 pytoolbox-14.5.0/pytoolbox/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21371 2023-06-07 19:22:04.000000 pytoolbox-14.5.0/pytoolbox/filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3096 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/flask.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6177 2023-06-07 19:22:27.000000 pytoolbox-14.5.0/pytoolbox/humanize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2272 2023-06-07 19:30:05.000000 pytoolbox-14.5.0/pytoolbox/itertools.py
+-rw-rw-r--   0 david     (1000) david     (1000)    49285 2023-06-07 19:46:20.000000 pytoolbox-14.5.0/pytoolbox/juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)      936 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/linux.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3720 2023-06-07 19:53:25.000000 pytoolbox-14.5.0/pytoolbox/logging.py
+-rw-rw-r--   0 david     (1000) david     (1000)      322 2023-06-07 19:31:43.000000 pytoolbox-14.5.0/pytoolbox/module.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/exif/
+-rw-rw-r--   0 david     (1000) david     (1000)      344 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1593 2023-06-07 20:32:28.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/brand.py
+-rw-rw-r--   0 david     (1000) david     (1000)      530 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/camera.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1021 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/equipment.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1664 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/image.py
+-rw-rw-r--   0 david     (1000) david     (1000)      740 2023-06-07 18:06:30.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/lens.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2180 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/metadata.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/photo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3811 2023-06-07 20:36:20.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/tag.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/
+-rw-rw-r--   0 david     (1000) david     (1000)      235 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7221 2023-06-07 20:56:06.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/encode.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5617 2023-06-07 19:17:58.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8291 2023-06-07 17:58:50.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffprobe.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6987 2023-06-07 20:56:16.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1401 2023-06-07 18:05:36.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/image/
+-rw-rw-r--   0 david     (1000) david     (1000)     2233 2023-06-07 17:58:12.000000 pytoolbox-14.5.0/pytoolbox/multimedia/image/PIL.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/image/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1663 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/network/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7006 2023-06-07 19:15:02.000000 pytoolbox-14.5.0/pytoolbox/network/http.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1115 2023-06-07 17:58:57.000000 pytoolbox-14.5.0/pytoolbox/network/ip.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15618 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/rtp.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/network/smpte2022/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27680 2023-06-07 20:38:57.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10383 2023-06-07 20:42:14.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/generator.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27905 2023-06-07 20:56:35.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/receiver.py
+-rw-rw-r--   0 david     (1000) david     (1000)      925 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/url.py
+-rw-rw-r--   0 david     (1000) david     (1000)      479 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/pandas.py
+-rw-rw-r--   0 david     (1000) david     (1000)      370 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3069 2023-06-07 19:51:38.000000 pytoolbox-14.5.0/pytoolbox/regex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 14:26:46.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1075 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      682 2023-06-07 14:48:10.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/permissions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      742 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2203 2023-06-07 14:48:30.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1536 2023-06-07 14:48:58.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/selenium/
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3042 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1137 2023-06-07 19:25:15.000000 pytoolbox-14.5.0/pytoolbox/selenium/common.py
+-rw-rw-r--   0 david     (1000) david     (1000)      428 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)      230 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2563 2023-06-07 19:27:45.000000 pytoolbox-14.5.0/pytoolbox/selenium/test.py
+-rw-rw-r--   0 david     (1000) david     (1000)      779 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/webdrivers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/selenium/webelements/
+-rw-rw-r--   0 david     (1000) david     (1000)      150 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1073 2023-06-07 17:39:23.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      994 2023-06-07 19:26:22.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/bootstrap_slider.py
+-rw-rw-r--   0 david     (1000) david     (1000)      473 2023-06-07 19:29:01.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/bootstrap_switch.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19719 2023-06-07 17:55:15.000000 pytoolbox-14.5.0/pytoolbox/serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)      410 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/setuptools.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1373 2023-06-07 17:55:23.000000 pytoolbox-14.5.0/pytoolbox/signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2506 2023-06-07 19:48:35.000000 pytoolbox-14.5.0/pytoolbox/states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4513 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/string.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13946 2023-06-07 20:57:00.000000 pytoolbox-14.5.0/pytoolbox/subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3381 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/throttles.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7808 2023-06-07 19:47:09.000000 pytoolbox-14.5.0/pytoolbox/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10314 2023-06-07 17:48:00.000000 pytoolbox-14.5.0/pytoolbox/unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8945 2023-06-07 20:19:20.000000 pytoolbox-14.5.0/pytoolbox/validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1169 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/virtualenv.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2118 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/voluptuous.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     7617 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5436 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      827 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-07 22:11:06.678008 pytoolbox-14.5.0/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     8067 2023-06-07 15:14:14.000000 pytoolbox-14.5.0/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)      959 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1193 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4605 2023-06-07 15:32:54.000000 pytoolbox-14.5.0/tests/test_comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)      772 2023-06-07 14:38:27.000000 pytoolbox-14.5.0/tests/test_console.py
+-rw-rw-r--   0 david     (1000) david     (1000)      416 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      624 2023-06-07 15:33:50.000000 pytoolbox-14.5.0/tests/test_django_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      909 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17588 2023-06-07 15:33:08.000000 pytoolbox-14.5.0/tests/test_ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)      983 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2843 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)      677 2023-06-07 15:33:10.000000 pytoolbox-14.5.0/tests/test_module.py
+-rw-rw-r--   0 david     (1000) david     (1000)      632 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1629 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2563 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4025 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2805 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_string.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4121 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)      294 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5699 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)      577 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      389 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_x264.py
```

### Comparing `pytoolbox-14.4.0/LICENSE.rst` & `pytoolbox-14.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/PKG-INFO` & `pytoolbox-14.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.4.0
+Version: 14.5.0
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 Provides-Extra: smpte2022
 Provides-Extra: vision
 Provides-Extra: voluptuous
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE.rst
-License-File: AUTHORS
+License-File: AUTHORS.md
 
 =========
 Pytoolbox
 =========
 
 .. image:: https://badge.fury.io/py/pytoolbox.png
    :target: http://badge.fury.io/py/pytoolbox
@@ -155,14 +155,15 @@
 How to check coverage ?
 -----------------------
 
 ::
 
     $ source /some/python3/venv/bin/activate
     $ pip install -e .[all,test]
+    $ flake8 pytoolbox
     $ pytest
     $ xdg-open htmlcov/index.html
 
 Remarks:
 
 * All Django related modules are excluded from tests!
 * However I am using them with Django 1.8 up to 3.1.0.
```

### Comparing `pytoolbox-14.4.0/README.rst` & `pytoolbox-14.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 How to check coverage ?
 -----------------------
 
 ::
 
     $ source /some/python3/venv/bin/activate
     $ pip install -e .[all,test]
+    $ flake8 pytoolbox
     $ pytest
     $ xdg-open htmlcov/index.html
 
 Remarks:
 
 * All Django related modules are excluded from tests!
 * However I am using them with Django 1.8 up to 3.1.0.
```

### Comparing `pytoolbox-14.4.0/changelog.rst` & `pytoolbox-14.5.0/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,1178 +1,971 @@
-=========
-changelog
-=========
+# Changelog
 
 Roadmap ? Not so, but you can check this: https://github.com/davidfischer-ch/pytoolbox/issues
 
---------------------
-v14.4.0 (2022-12-09)
---------------------
+## v14.5.0 (2023-06-07)
+
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.5.0...14.4.0
+
+### Minor compatibility breaks
+
+- Bye bye Django 3 and less
+
+### Features
+
+- Make code compatible with Django 4+
+
+### Fix and enhancements
+
+- Usage of `super()` magic
+- Upgrade testing stack especially pylint with its dozen tests
+- Apply recommendations from linters (or silent it...)
+- Convert Changelog and Authors in Markdown
+
+## v14.4.0 (2022-12-09)
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.4.0...14.3.0
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
 - Replace `comparison.parse_version` by `comparison.try_parse_version` with a fallback behavior
 
-Features
-========
+### Features
 
 - Add function `humanize.naturalweight`
 - Add function `console.toggle_colors`
 - Module `comparison`: Add `unified_diff`, `compare_versions` and `satisfy_version_constraints`
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
 - Compatibility with latest Django releases
 - Compatibility with latest `packaging` module (`LegacyVersion` was dropped)
 
---------------------
-v14.3.0 (2022-09-09)
---------------------
+## v14.3.0 (2022-09-09)
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.3.0...14.2.0
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
 - Drop Python 3.7 & 3.8 compatibility
 - Drop `logging` extra (`termcolor` is now installed by default)
 
-Features
-========
+### Features
 
-- Add `types.merge_annotations` class decorator
-- Module `comparison`: Add `unified_diff`, `compare_versions` and `satisfy_version_constraints`
+- Add [types.merge_annotations` class decorator
+- Module `comparison`: Add [unified_diff`,
+    [compare_versions` and
+    [satisfy_version_constraints`
 
---------------------
-v14.2.0 (2022-06-10)
---------------------
+## v14.2.0 (2022-06-10)
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.2.0...14.1.0
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
 - Drop Python 3.6 compatibility
 - Function `filesystem.from_template`: Make Jinja2 template strict with undefined values
 - Module `argparse`: Return `pathlib.Path` instead of `str` (See commit 6acf8d13e2739a6e564b325bc035e33676c9ff07)
 
-Features
-========
+### Features
 
 - Add some type hints (more to come)
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
 - Convert some FIXMEs to TODOs
 - Ensure Python 3.10 compatibility
 - Fix many linter issues
 
--------
-v14.1.0
--------
+## v14.1.0
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.1.0...14.0.2
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
-- Module dango.models.fields: Apply NullifyMixin to StripCharField and StripTextField
+- Module `dango.models.fields`: Apply `NullifyMixin` to `StripCharField` and `StripTextField`
 
-Features
-========
+### Features
 
-- Module django.models.fields: Add NullifyMixin, CharField and TextField
+- Module `django.models.fields`: Add `NullifyMixin`, `CharField` and `TextField`
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
-- Module django.signals: Fix strip_strings_and_validate_model not importable from django.signals
-- Module django.models.fields: Fix StripMixin not fair play with inheritance
+- Module `django.signals`: Fix `strip_strings_and_validate_model` not importable from `django.signals`
+- Module `django.models.fields`: Fix `StripMixin` not fair play with inheritance
 
--------
-v14.0.2
--------
+## v14.0.2
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.0.0...14.0.1
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
-- Fix Django deprecation warning (ugettext_lazy -> gettext_lazy)
+- Fix Django deprecation warning (`ugettext_lazy` -> `gettext_lazy`)
 
--------
-v14.0.1
--------
+## v14.0.1
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.0.0...14.0.1
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
-- Function filesystem.from_template: Add directories optional argument
+- Function `filesystem.from_template`: Add directories optional argument
 - Fix Keras imports (because they changed)
 - Fix newer pylint errors
 
--------
-v14.0.0
--------
+## v14.0.0
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/13.5.0...14.0.0
 
-Major compatibility breaks
-==========================
+## Major compatibility breaks
 
 - Drop Python 2.7 - 3.5 compatibility
-- Drop module encoding
-- Drop module mongo
-- Drop function network.http.get_request_data
-- Drop function unittest.{mock_cmd,runtests} (and dependency to nose)
+- Drop module `encoding`
+- Drop module `mongo`
+- Drop function `network.http.get_request_data`
+- Drop function `unittest.{mock_cmd,runtests}` (and dependency to nose)
 - Remove unused arguments on some functions
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
-- Function multimedia.exif.brand.Brand.clean: Raise exceptions.InvalidBrandError
+- Function `multimedia.exif.brand.Brand.clean`: Raise `exceptions.InvalidBrandError`
 
-Features
-========
+### Features
 
 - Rewrite code in Python 3 thanks to 2to3 and a lot of edits
 - Rewrite tests in Python 3 and with pytest in replacement to unittest (and nose)
 - Seamlessly download tests assets (small.mp4, ffmpeg, ffprobe) from S3
 - Test on recent Python releases from 3.6 to 3.8 (3.9 will come next)
-- Temporarily removed PyPy 3.6 from test matrix due to tensorflow (work in progress)
+- Temporarily removed PyPy 3.6 from test matrix due to `tensorflow` (work in progress)
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
-- setup.py an extra "all" one can install with pip install .[all]
+- setup.py an extra `all` one can install with pip install `.[all]`
 - Separate requirements in three major groups: features, test and docs
-- Make some functions compatible with pathlib.Path (work in progress)
+- Make some functions compatible with `pathlib.Path` (work in progress)
 - Check code quality with pylint and flake8 (they are top notch)
 - Remove doctests boilerplate code and make them more robust
 - Fix deprecation issues by reimplementing some functions
 - Fix code smells and silent irrelevant warnings
 - Update Travis CI configuration: Define distribution, update script, ...
-- Generate documentation with python setup.py docs
+- Generate documentation with `python setup.py docs`
 
--------
-v13.5.0
--------
+## v13.5.0
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
-- Class multimedia.exif.miscellaneous.VideoStream: Rename rotate to rotation
+- Class `multimedia.exif.miscellaneous.VideoStream`: Rename rotate to rotation
 
-Fix and enhancements
-====================
+## Fix and enhancements
 
-- Module multimedia.exif: Add Tamron brand
+- Module `multimedia.exif`: Add Tamron brand
 
--------
-v13.4.0
--------
+## v13.4.0
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
 - Drop Python 2.6 + Python 3.2 support (remove from Travis CI build)
-- Module multimedia.ffmpeg: Allow to pass input options (encoding)
-
-Fix and enhancements
-====================
-
-- Module multimedia.ffmpeg: Refresh metadata classes
-- Class multimedia.exif.Metadata: Allow to define path to save EXIF metadata
+- Module `multimedia.ffmpeg`: Allow to pass input options (encoding)
 
--------
-v13.3.5
--------
+## Fix and enhancements
 
-Fix and enhancements
-====================
+- Module `multimedia.ffmpeg`: Refresh metadata classes
+- Class `multimedia.exif.Metadata`: Allow to define path to save EXIF metadata
 
-* Module django: Django 2.0 compatibility
-* Module filesystem: Windows compatbility
-* Class django.models.fields.URLField: Set max_length to 8000 by default
-* Class django.models.fields.*: Use OptionsMixin on all fields
-* Add requests to requirements
+## v13.3.5
 
--------
-v13.3.0
--------
+## Fix and enhancements
 
-Fix and enhancements
-====================
+- Module `django`: Django 2.0 compatibility
+- Module `filesystem`: Windows compatbility
+- Class `django.models.fields.URLField`: Set max_length to 8000 by default
+- Class `django.models.fields.\*`: Use `OptionsMixin` on all fields
+- Add `requests` to requirements
 
-* Function filesystem.file_mime: Convert to unicode only if required.
+## v13.3.0
 
-Features
-========
+## Fix and enhancements
 
-* Add module pandas
+- Function `filesystem.file_mime`: Convert to unicode only if required.
 
--------
-v13.2.0
--------
+### Features
 
-Fix and enhancements
-====================
+- Add module `pandas`
 
-* Module multimedia.exif: Add Huawei.
+## v13.2.0
 
-Features
-========
+## Fix and enhancements
 
-* Add function console.shell
+- Module `multimedia.exif`: Add Huawei.
 
--------
-v13.1.3
--------
+### Features
 
-Fix and enhancements
-====================
+- Add function `console.shell`
 
-* Module mutlimedia.exif: Make classes swappable + importable from exif module.
-* Module smpte2022: Fixed wraparound sequence number calculations for RTP and FEC.
+## v13.1.3
 
-Thanks to @TobbeEdgeware!
+## Fix and enhancements
 
--------
-v13.1.1
--------
+- Module `mutlimedia.exif`: Make classes swappable + importable from exif module.
+- Module `smpte2022`: Fixed wraparound sequence number calculations for RTP and FEC.
 
-Minor compatibility breaks
-==========================
+Thanks to \@TobbeEdgeware!
 
-* Function serialization.object_to_dict: Rely almost only on schema to produce output structure (hint: use list in schema)
+## v13.1.1
 
-Fix and enhancements
-====================
+### Minor compatibility breaks
 
-* Function collections.swap_dict_of_values: Implement simple key-value swap.
+- Function `serialization.object_to_dict`: Rely almost only on schema to produce output structure (hint: use list in schema)
 
--------
-v13.0.4
--------
+## Fix and enhancements
 
-Fix and enhancements
-====================
+- Function `collections.swap_dict_of_values`: Implement simple key-value swap.
 
-* Function aws.s3.remove_objects: Add callback argument to make it more flexible.
-* Function multimedia.image.remove_transparency: Enhance code (remove force_rgb arg from 13.0.2).
-* Function serialization.object_to_dict: Add iterable_callback to customize container type of iterables.
+## v13.0.4
 
--------
-v13.0.0
--------
+## Fix and enhancements
 
-Compatibility breaks
-====================
+- Function `aws.s3.remove_objects`: Add callback argument to make it more flexible.
+- Function `multimedia.image.remove_transparency`: Enhance code (remove `force_rgb arg` from 13.0.2).
+- Function `serialization.object_to_dict`: Add `iterable_callback` to customize container type of iterables.
 
-* Remove fake bson ObjectId (private module) when library not available.
-* Function filesystem.find_recursive is now matching patterns against the whole path.
-* Function aws.s3.list_objects: Handle multiple patterns like filesystem.find_recursive.
-* Function aws.s3.remove_objects: Handle multiple patterns like filesystem.find_recursive.
+## v13.0.0
 
-Features
-========
+## Compatibility breaks
 
-* Add function filesystem.to_user_id
-* Add function filesystem.to_group_id
-* Add function regex.from_path_patterns
+- Remove fake bson's `ObjectId` (`private` module) when library not available.
+- Function `filesystem.find_recursive` is now matching patterns against the whole path.
+- Function `aws.s3.list_objects`: Handle multiple patterns like `filesystem.find_recursive`.
+- Function `aws.s3.remove_objects`: Handle multiple patterns like `filesystem.find_recursive`.
 
-Fix and enhancements
-====================
+### Features
 
-* Replace relative imports of len(.) > 1 by absolute imports
+- Add function `filesystem.to_user_id`
+- Add function `filesystem.to_group_id`
+- Add function `regex.from_path_patterns`
 
--------
-v12.2.3
--------
+## Fix and enhancements
 
-Features
-========
+- Replace relative imports of `len(.) > 1` by absolute imports
 
-* Add module aws.s3
+## v12.2.3
 
--------
-v12.1.2
--------
+### Features
 
-Compatibility breaks
-====================
+- Add module `aws.s3`
 
-* Remove object_to_dict and object_to_dictV2
-* Rename object_to_dictV3 to object_to_dict
+## v12.1.2
 
-Fix and enhancements
-====================
+## Compatibility breaks
 
-* Move AI data to S3 (own account).
-* Function serialization.object_to_dict: Also authorize to tweak obj (not only schema).
-* Function serialization.object_to_dict: Also add depth information.
-* Function serialization.to_file: Fix to_file ot using makedirs properly
+- Remove `object_to_dict` and `object_to_dictV2`
+- Rename `object_to_dictV3` to `object_to_dict`
 
---------
-v11.10.0
---------
+## Fix and enhancements
 
-Fix and enhancements
-====================
+- Move AI data to S3 (own account).
+- Function `serialization.object_to_dict`: Also authorize to tweak obj (not only schema).
+- Function `serialization.object_to_dict`: Also add depth information.
+- Function `serialization.to_file`: Fix `to_file` not using `makedirs` properly
 
-* Fix PEP-8 issue
-* Class django.models.fields.base.MoneyField: Make decimal_places tweakable
+## v11.10.0
 
-Features
-========
+## Fix and enhancements
 
-* Add class django.models.fields.mixins.LowercaseMixin
-* Add function serialization.object_to_dictV3
+- Fix PEP-8 issue
+- Class `django.models.fields.base.MoneyField`: Make decimal_places tweakable
 
--------
-v11.9.1
--------
+### Features
 
-Fix and enhancements
-====================
+- Add class `django.models.fields.mixins.LowercaseMixin`
+- Add function `serialization.object_to_dictV3`
 
-* Set line size to 100 chars and cleanup code
-* Fix Travis build (remove django modules when testing)
-* Always install pillow when installing with -e imaging
-* Update README to reflect newer options
+## v11.9.1
 
-* Class multimedia.exif.brand.Brand: Add more brands
-* Class multimedia.exif.image.Orientation: Use standard Enum, or object if not available
+## Fix and enhancements
 
-Features
-========
+- Set line size to 100 chars and cleanup code
+- Fix Travis build (remove `django` modules when testing)
+- Always install pillow when installing with -e imaging
+- Update README to reflect newer options
+- Class `multimedia.exif.brand.Brand`: Add more brands
+- Class `multimedia.exif.image.Orientation`: Use standard Enum, or object if not available
 
-* Add module ai
+### Features
 
--------
-v11.8.6
--------
+- Add module `ai`
 
-Fixes and enhancements
-======================
+## v11.8.6
 
-* Add functions multimedia.image.PIL.{apply,get}_orientation
-* Add constant ORIENTATION_TO_ROTATION to multimedia.exif.image.Image
-* Make function multimedia.image.PIL.apply_orientation more generic
-* Make function multimedia.image.PIL.apply_orientation defaulting to nothing if orientation is crazy
-* Make function multimedia.image.PIL.get_orientation more robust
-* Class exceptions.MessageMixin: Fix pickle recursion error
+### Fixes and enhancements
 
-Features
-========
+- Add `functions multimedia.image.PIL.{apply,get}_orientation`
+- Add constant `ORIENTATION_TO_ROTATION` to `multimedia.exif.image.Image`
+- Make function `multimedia.image.PIL.apply_orientation` more generic
+- Make function `multimedia.image.PIL.apply_orientation` defaulting to nothing if orientation is crazy
+- Make function `multimedia.image.PIL.get_orientation` more robust
+- Class `exceptions.MessageMixin`: Fix pickle recursion error
 
-* Add module multimedia.image.PIL
-* Add function types.merge_base_attribute
+### Features
 
--------
-v11.7.6
--------
+- Add module `multimedia.image.PIL`
+- Add function `types.merge_base_attribute`
 
-Minor compatibility breaks
-==========================
+## v11.7.6
 
-* Remove jinja2 from packages installed by default
+### Minor compatibility breaks
 
-Fixes and enhancements
-======================
+- Remove jinja2 from packages installed by default
 
-* Support more Python versions (3.5, 3.6)
-* Function filesystem.makedirs: Add parent argument
-* Module logging: Update logging color scheme + make it overridable
-* Module django.templatetags:
-    - Implement TEMPLATE_STRING_IF_INVALID for Django >= 1.8
-    - Implement include_is_allowed for Django >= 1.10
-* Class multimedia.exif.Metadata: Can also read EXIF metadata from buffer
-* Function argparse.password: Add it
+### Fixes and enhancements
 
--------
-v11.7.1
--------
+- Support more Python versions (3.5, 3.6)
+- Function `filesystem.makedirs`: Add parent argument
+- Module `logging`: Update logging color scheme + make it overridable
+- Module django.templatetags:
+  - Implement `TEMPLATE_STRING_IF_INVALID` for Django \>= 1.8
+  - Implement `include_is_allowed` for Django \>= 1.10
+- `Class multimedia.exif.Metadata`: Can also read EXIF metadata from buffer
+- Function `argparse.password`: Add it
 
-Minor compatibility breaks
-==========================
+## v11.7.1
 
-* Remove unnecessary dependencies + put some as extra
+### Minor compatibility breaks
 
-Fixes and enhancements
-======================
+- Remove unnecessary dependencies + put some as extra
 
-* Module filesystem: Add walk_kwargs to some functions
-* Function logging.setup_logging: make possible to setup an instance of logger
+### Fixes and enhancements
 
--------
-v11.6.4
--------
+- Module `filesystem`: Add `walk_kwargs` to some functions
+- Function `logging.setup_logging`: make possible to setup an instance of logger
 
-Fixes and enhancements
-======================
+## v11.6.4
 
-* Module argparse: Set columns to a value or auto-detected
-* Module exif: Fix orientation is not value from Orientation
-* Module smpte2022: Various fixes by @AbdulTheProgrammer
-* Enhance function logging.setup_logging:
-    - Add optional colorized mode
-    - Always setup log level and return logger
-* Enhance module multimedia.exif:
-    - Add optional orientation override
-    - Add rotation property based on orientation
-    - Add rewrite method to fix issues with exif tags
-    - Allow to specify gexiv2 version
-* Use iteritems because its still a Python 2 (and 3) library
+### Fixes and enhancements
 
--------
-v11.6.0
--------
+- Module `argparse`: Set columns to a value or auto-detected
+- Module `exif`: Fix orientation is not value from Orientation
+- Module `smpte2022`: Various fixes by @AbdulTheProgrammer
+- Enhance function `logging.setup_logging`:
+  - Add optional colorized mode
+  - Always setup log level and return logger
+- Enhance module `multimedia.exif`:
+  - Add optional orientation override
+  - Add rotation property based on orientation
+  - Add rewrite method to fix issues with exif tags
+  - Allow to specify gexiv2 version
+- Use iteritems because its still a Python 2 (and 3) library
 
-Fixes and enhancements
-======================
+## v11.6.0
 
-* Add method get_frames_md5_checksum to FFmpeg class
-* Update exif brands
+### Fixes and enhancements
 
-Features
-========
+- Add method `get_frames_md5_checksum` to `FFmpeg` class
+- Update exif brands
 
-* Support Python 3.6
-* Add function itertools.chunk
+### Features
 
--------
-v11.5.4
--------
+- Support Python 3.6
+- Add function `itertools.chunk`
 
-Fixes and enhancements
-======================
+## v11.5.4
 
-* Fix syntax error in multimedia.exif.lens at line 22
-* Prevent AppRegistryNotReady when importing django.models.utils
-* Add {pre,post}_func arguments to filesystem.from_template
-* Function filesystem.from_template: Make destination optional + allow to set template to content
+### Fixes and enhancements
 
-Features
-========
+- Fix syntax error in `multimedia.exif.lens` at line 22
+- Prevent `AppRegistryNotReady` when importing `django.models.utils`
+- Add `{pre,post}_func` arguments to `filesystem.from_template`
+- Function `filesystem.from_template`: Make destination optional + allow to set template to content
 
-* Add function crypto.get_password_generator
+### Features
 
--------
-v11.5.0
--------
+- Add function `crypto.get_password_generator`
 
-Fixes and enhancements
-======================
+## v11.5.0
 
-* Improve code quality
-* Remove try_ prefix from filesystem functions (retro compat: try_ functions still defined)
+### Fixes and enhancements
 
--------
-v11.4.3
--------
+- Improve code quality
+- Remove `try_` prefix from `filesystem` functions (retro compat: `try_` functions still defined)
 
-Features
-========
+## v11.4.3
 
-* Add constant encoding.integer_types
-* Add function subprocess.su
-* Add function types.get_arguments_names
+### Features
 
-Fixes and enhancements
-======================
+- Add constant `encoding.integer_types`
+- Add function `subprocess.su`
+- Add function `types.get_arguments_names`
 
-* Add bare argument to subprocess.git_clone_or_pull
+### Fixes and enhancements
 
--------
-v11.4.0
--------
+- Add bare argument to `subprocess.git_clone_or_pull`
 
-Features
-========
+## v11.4.0
 
-* Add module linux
-* Add module setuptools
+### Features
 
--------
-v11.2.0
--------
+- Add module `linux`
+- Add module `setuptools`
 
-Features
-========
+## v11.2.0
 
-* Add classes types.Echo{Object,Dict}
-* Add classes argparse.Help{ArgumentParser,Formatter}
+### Features
 
-Fixes and enhancements
-======================
+- Add classes `types.Echo{Object,Dict}`
+- Add classes `argparse.Help{ArgumentParser,Formatter}`
 
-* Add docstrings and fix doctests
-* Fix django.forms.utils.get_instance
-* Update FromPrivateKeyMixin to fix call to fail with recent DRF
+### Fixes and enhancements
 
--------
-v11.1.0
--------
+- Add docstrings and fix doctests
+- Fix `django.forms.utils.get_instance`
+- Update `FromPrivateKeyMixin` to fix call to fail with recent DRF
 
-Minor compatibility breaks
-==========================
+## v11.1.0
 
-* Update git_clone_or_pull to full clone by default
+### Minor compatibility breaks
 
-Features
-========
+- Update `git_clone_or_pull` to full clone by default
 
-* Add module network.url
-* Add mixin django.forms.mixins.CreatedByMixin
-* Add mixin django.forms.mixins.StaffOnlyFieldsMixin
+### Features
 
-Fixes and enhancements
-======================
+- Add module `network.url`
+- Add mixin `django.forms.mixins.CreatedByMixin`
+- Add mixin `django.forms.mixins.StaffOnlyFieldsMixin`
 
-* Add/fix docstrings and unit-tests
-* Use xrange and iter{items,keys,values} under Python 2
-* Replace nose.tools by pytoolbox.unittest.asserts
-* Make RequestMixin more transparent
-* network.http.download_ext: Pass kwargs to iter_download_to_file
-* django.views.mixins.AddRequestToFormKwargsMixin: Check form "handles" request as kwarg based on its class
+### Fixes and enhancements
 
--------
-v11.0.0
--------
+- Add/fix docstrings and unit-tests
+- Use `xrange` and `iter{items,keys,values}` under Python 2
+- Replace `nose.tools` by `pytoolbox.unittest.asserts`
+- Make `RequestMixin` more transparent
+- `network.http.download_ext`: Pass `kwargs` to `iter_download_to_file`
+- `django.views.mixins.AddRequestToFormKwargsMixin`: Check form "handles" request as `kwarg` based on its class
 
-Compatibility breaks
-====================
+## v11.0.0
 
-* Remove ming module to cleanup build
-* Remove django.models.mixins.PublishedMixin (not generic enough neither powerful enough)
+## Compatibility breaks
 
-Minor compatibility breaks
-==========================
+- Remove ming module to cleanup build
+- Remove `django.models.mixins.PublishedMixin` (not generic enough neither powerful enough)
 
-* Prefer path over filename (arguments convention)
-* Replace MapUniqueTogetherMixin + MapUniqueTogetherIntegrityErrorToValidationErrorMixin by BetterUniquenessErrorsMixin.
-* Move CancellableDeleteView to django.views.base
+### Minor compatibility breaks
 
-Features
-========
+- Prefer path over filename (arguments convention)
+- Replace `MapUniqueTogetherMixin` + `MapUniqueTogetherIntegrityErrorToValidationErrorMixin` by `BetterUniquenessErrorsMixin`.
+- Move `CancellableDeleteView` to `django.views.base`
 
-* Generate documentation and publish on readthedocs.org
-* Add mixin django.models.mixins.BetterUniquenessErrorsMixin
+### Features
 
-Fixes and enhancements
-======================
+- Generate documentation and publish on readthedocs.org
+- Add mixin `django.models.mixins.BetterUniquenessErrorsMixin`
 
-* Add/fix docstrings
-* Update modules headers
-* Make django.views.mixins.ValidationErrorsMixin more "generic"
-* Too many to be listed here, https://github.com/davidfischer-ch/pytoolbox/compare/10.4.0...11.0.0
+### Fixes and enhancements
 
--------
-v10.4.0
--------
+- Add/fix docstrings
+- Update modules headers
+- Make `django.views.mixins.ValidationErrorsMixin` more "generic"
+- Too many to be listed here, https://github.com/davidfischer-ch/pytoolbox/compare/10.4.0...11.0.0
 
-Features
-========
+## v10.4.0
 
-* Add module django.models.metaclass
-* Add module django.views.utils
-* Add module enum
-* Add modules in multimedia.exif:
-    - brand
-    - camera
-    - equipement
-    - image
-    - lens
-    - photo
-    - tag
-* Add module rest_framework.metadata.mixins
-* Add mixin django.models.mixins.PublicMetaMixin
-* Add decorator decorators.cached_property
-* Add decorator decorators.hybridmethod
-* Add functions in django.models.utils:
-    - get_related_manager
-    - get_related_model
-    - try_get_field
-* Add function types.get_properties
+### Features
 
-Fixes and enhancements
-======================
+- Add module `django.models.metaclass`
+- Add module `django.views.utils`
+- Add module `enum`
+- Add modules in `multimedia.exif`:
+  - `brand`
+  - `camera`
+  - `equipement`
+  - `image`
+  - `lens`
+  - `photo`
+  - `tag`
+- Add module `rest_framework.metadata.mixins`
+- Add mixin `django.models.mixins.PublicMetaMixin`
+- Add decorator `decorators.cached_property`
+- Add decorator `decorators.hybridmethod`
+- Add functions in `django.models.utils`:
+  - `get_related_manager`
+  - `get_related_model`
+  - `try_get_field`
+- Add function `types.get_properties`
 
-* Handle 24h+ hour format in datetime.str_to_datetime
-* Module django.forms.utils imports from django.forms.utils module
-* Fix ReloadMixin popping update_fields!
-* Refactor class multimedia.exif.metadata.Metadata (use newest classes)
-* Split module multimedia.ffmpeg
-* Fix ffmpeg mock class
+### Fixes and enhancements
 
--------
-v10.3.0
--------
+- Handle 24h+ hour format in `datetime.str_to_datetime`
+- Module `django.forms.utils` imports from `django.forms.utils` module
+- Fix `ReloadMixin` popping update_fields!
+- Refactor class `multimedia.exif.metadata.Metadata` (use newest classes)
+- Split module `multimedia.ffmpeg`
+- Fix `ffmpeg`'s' `mock` class
 
-Compatibility breaks
-====================
+## v10.3.0
 
-* Remove module rest_framework.v2
-* Refactor (optimize) unittest.FilterByTagsMixin
+## Compatibility breaks
 
-Minor compatibility breaks
-==========================
+- Remove module `rest_framework.v2`
+- Refactor (optimize) `unittest.FilterByTagsMixin`
 
-* Rename module exception to exceptions
-* Rename module rest_framework.v3 to rest_framework
-* Rename some attributes of multimedia.ffmpeg classes
+### Minor compatibility breaks
 
-Features
-========
+- Rename module `exception` to `exceptions`
+- Rename module `rest_framework.v3` to `rest_framework`
+- Rename some attributes of `multimedia.ffmpeg` classes
 
-* Add many modules:
-    - atlassian
-    - itertools
-    - module (yes!)
-    - selenium
-    - signals
-    - states
-    - string
-    - voluptuous
-* Add functions:
-* Add class argparse.Range
-* Add function argparse.multiple
-* Add function collections.{merge_dicts, swap_dict_of_values}
-* Add decorator decorators.run_once
-* Add modules and mixins in django* module
-* Add value encoding.binary_type
-* Add function humanize.naturalfrequency
-* Add function types.isiterable
-* Add classes types.{DummyObject,MissingType}
-* Add object types.Missing instance of MissingType
-* Add mixins unittest.{InMixin,InspectMixin}
-* Add class unittest.Asserts
-* Add object unittest.asserts
+### Features
 
-Fixes and enhancements
-======================
+- Add many modules:
+  - `atlassian`
+  - `itertools`
+  - `module` (yes!)
+  - `selenium`
+  - `signals`
+  - `states`
+  - `string`
+  - `voluptuous`
+- Add class `argparse.Range`
+- Add function `argparse.multiple`
+- Add function `collections.{merge_dicts, swap_dict_of_values}`
+- Add decorator `decorators.run_once`
+- Add modules and mixins in `django\*` module
+- Add value `encoding.binary_type`
+- Add function `humanize.naturalfrequency`
+- Add function `types.isiterable`
+- Add classes `types.{DummyObject,MissingType}`
+- Add object `types.Missing instance of MissingType`
+- Add mixins `unittest.{InMixin,InspectMixin}`
+- Add class `unittest.Asserts`
+- Add object `unittest.asserts`
 
-* Countless fixes and enhancements
-* Follow os.path import best practices
-* Make multimedia.ffmpeg private functions public
+### Fixes and enhancements
 
--------
-v10.2.0
--------
+- Countless fixes and enhancements
+- Follow `os.path` import best practices
+- Make `multimedia.ffmpeg` private functions public
 
-Compatibility breaks
-====================
+## v10.2.0
 
-* Add EncodeStatistics and refactor FFmpeg.encode()
+## Compatibility breaks
 
-Minor compatibility breaks
-==========================
+- Add `EncodeStatistics` and refactor `FFmpeg.encode()`
 
-* Merge django.template tags & filters into 1 file
-* Split FFmpeg class to FFmpeg + FFprobe classes
+### Minor compatibility breaks
 
-Features
-========
+- Merge `django.template` tags & filters into 1 file
+- Split `FFmpeg` class to `FFmpeg` + `FFprobe` classes
 
-* Add module django.exceptions
-* Add static_abspath Django template tag
-* Add class django.forms.mixins.EnctypeMixin
-* Add class django.models.mixins.AlwaysUpdateFieldsMixin
-* Add class django.models.mixins.AutoForceInsertMixin
-* Add class django.models.mixins.AutoUpdateFieldsMixin
-* Add class django.models.mixins.MapUniqueTogetherIntegrityErrorToValidationErrorMixin
-* Add class django.models.mixins.RelatedModelMixin
-* Add class django.models.mixins.UpdatePreconditionsMixin
-* Add class django.storage.ExpressTemporaryFileMixin
-* Add class django.test.mixins.FormWizardMixin
-* Add class django.views.mixins.InitialMixin
-* Add class logging.ColorizeFilter
-* Add function collections.flatten_dict
-* Add function datetime.multiply_time
+### Features
 
-Fixes and enhancements
-======================
+- Add module `django.exceptions`
+- Add `static_abspath` Django template tag
+- Add class `django.forms.mixins.EnctypeMixin`
+- Add class `django.models.mixins.AlwaysUpdateFieldsMixin`
+- Add class `django.models.mixins.AutoForceInsertMixin`
+- Add class `django.models.mixins.AutoUpdateFieldsMixin`
+- Add class `django.models.mixins.MapUniqueTogetherIntegrityErrorToValidationErrorMixin`
+- Add class `django.models.mixins.RelatedModelMixin`
+- Add class `django.models.mixins.UpdatePreconditionsMixin`
+- Add class `django.storage.ExpressTemporaryFileMixin`
+- Add class `django.test.mixins.FormWizardMixin`
+- Add class `django.views.mixins.InitialMixin`
+- Add class `logging.ColorizeFilter`
+- Add function `collections.flatten_dict`
+- Add function `datetime.multiply_time`
 
-* Avoid hardcoding \n
-* Module console: Write to given stream
-* Module datetime: Make API more consistent
-* Module multimedia.ffmpeg:
-    - Split FFmpeg class in FFmpeg and FFprobe
-    - Add EncodeState & EncodeStatistics classes
-    - Do some analysis before launching ffmpeg subprocess
-    - Fix progress if sub-clipping
-    - Improve handling of media argument
-    - Miscellaneous improvements
-* Module subprocess: Import Popen from psutil if available
-* Refactor function django.signals.create_site
+### Fixes and enhancements
 
--------
-v10.0.0
--------
+- Avoid hardcoding `\n`
+- Module `console`: Write to given stream
+- Module `datetime`: Make API more consistent
+- Module `multimedia.ffmpeg`:
+  - Split `FFmpeg` class in `FFmpeg` and `FFprobe`
+  - Add `EncodeState` & `EncodeStatistics` classes
+  - Do some analysis before launching `ffmpeg` subprocess
+  - Fix progress if sub-clipping
+  - Improve handling of `media` argument
+  - Miscellaneous improvements
+- Module `subprocess`: Import Popen from psutil if available
+- Refactor function `django.signals.create_site`
 
-Compatibility breaks
-====================
+## v10.0.0
 
-* Method multimedia.ffmpeg.FFmpeg.encode always yields at start
+## Compatibility breaks
 
-Features
-========
+- Method `multimedia.ffmpeg.FFmpeg.encode` always yields at start
 
-* Add some mixins in rest_framework.v*.views.mixins
+### Features
 
-Fixes and enhancements
-======================
+- Add some mixins in `rest_framework.v*.views.mixins`
 
-* Add class multimedia.ffmpeg.EncodingState
+### Fixes and enhancements
 
-------
-v9.7.2
-------
+- Add class `multimedia.ffmpeg.EncodingState`
 
-Minor compatibility breaks
-==========================
+## v9.7.2
 
-* Function filesystem.get_bytes returns a generator
-* Rename all functions with _to_ instead of 2 (e.g. str2time -> str_to_time)
-* Rename some methods of the class ffmpeg.FFmpeg
-* Change signature of console module functions
+### Minor compatibility breaks
 
-Features
-========
+- Function `filesystem.get_bytes` returns a generator
+- Rename all functions with `_to_` instead of `2` (e.g. `str2time` -> `str_to_time`)
+- Rename some methods of the class `ffmpeg.FFmpeg`
+- Change signature of `console` module's functions
 
-* Add module comparison
-* Add module regex
-* Add module types
-* Add class filesystem.TempStorage
-* Add function exception.get_exception_with_traceback
-* Add function humanize.natural_int_key
-* Add function console.progress_bar
+### Features
 
-Fixes and enhancements
-======================
+- Add module `comparison`
+- Add module `regex`
+- Add module `types`
+- Add class `filesystem.TempStorage`
+- Add function `exception.get_exception_with_traceback`
+- Add function `humanize.natural_int_key`
+- Add function `console.progress_bar`
 
-* Add *streams* methods to ffmpeg.FFmpeg
-* Improve ffmpeg module (add Media class for inputs/outputs)
-* Improve network.http.download_ext (Can download in chunks + progress callback)
-* Improve filesystem.get_bytes + crypto.* to read a file in chunks (if chunk_size is set)
+### Fixes and enhancements
 
-------
-v9.4.2
-------
+- Add `streams` methods to `ffmpeg.FFmpeg`
+- Improve `ffmpeg` module (add `Media` class for inputs/outputs)
+- Improve `network.http.download_ext` (Can download in chunks + progress callback)
+- Improve `filesystem.get_bytes` + `crypto.*` to read a file in chunks (if `chunk_size` is set)
 
-Features
-========
+## v9.4.2
 
-* Add module humanize
-* Add module django.models.query.mixins
-* Add module django.test.runner.mixins
+### Features
 
-Fixes and enhancements
-======================
+- Add module `humanize`
+- Add module `django.models.query.mixins`
+- Add module `django.test.runner.mixins`
 
-* Add __all__ to make the API explicit
-* Add method get_media_framerate to FFmpeg class
-* Add module private (with _parse_kwargs_string)
-* network module: Cleaner usage of string.format()
-* Refactor module humanize + add naturalfilesize
-* Improve humanize functions to handle [0-1] range + big numbers
+### Fixes and enhancements
 
------------
-v9.3.0-beta
------------
+- Add `__all__` to make the API explicit
+- Add method `get_media_framerate` to `FFmpeg` class
+- Add module `private` (with `_parse_kwargs_string`)
+- `network` module: Cleaner usage of `string.format()`
+- Refactor module `humanize` + add `naturalfilesize`
+- Improve `humanize` functions to handle `[0-1]` range + big numbers
 
-Compatibility breaks
-====================
+## v9.3.0-beta
 
-* Refactor multimedia modules
-* Rename module django.templatetags.pytoolbox_tags to _filters
+## Compatibility breaks
 
-Minor compatibility breaks
-==========================
+- Refactor `multimedia` modules
+- Rename module `django.templatetags.pytoolbox_tags` to `_filters`
 
-* Rename django.forms -> django.forms.mixins
-* Rename django.views -> django.views.mixins
+### Minor compatibility breaks
 
-Features
-========
+- Rename `django.forms` -> `django.forms.mixins`
+- Rename `django.views` -> `django.views.mixins`
 
-* Add module django.templatetags.pytoolbox_tags
-* Add module multimedia.exif
-* Add some django mixins
+### Features
 
-Fixes and enhancements
-======================
+- Add module `django.templatetags.pytoolbox_tags`
+- Add module `multimedia.exif`
+- Add some `django mixins`
 
-* Fix unicode handling
-* Function datetime.total_seconds now accept instance of timedelta
-* Function filesystem.from_template can now use jinja2 to generate the content
-* timedelta & to_filesize Django template filters now handle empty string input
-* Add argument create_out_directory to method multimedia.ffmpeg.FFmpeg.encode
-* Fix multimedia.ffmpeg.FFmpeg.encode: Create output directory before the subprocess
-* Improve multimedia.ffmpeg.FFmpeg.encode: Handle process missing + simplify mocking
+### Fixes and enhancements
 
------------
-v8.6.1-beta
------------
+- Fix unicode handling
+- Function `datetime.total_seconds` now accept instance of `timedelta`
+- Function `filesystem.from_template` can now use jinja2 to generate the content
+- `timedelta` & `to_filesize` Django template filters now handle empty string input
+- Add argument `create_out_directory` to method `multimedia.ffmpeg.FFmpeg.encode`
+- Fix `multimedia.ffmpeg.FFmpeg.encode`: Create output directory before the subprocess
+- Improve `multimedia.ffmpeg.FFmpeg.encode`: Handle process missing + simplify mocking
 
-Fixes and enhancements
-======================
+## v8.6.1-beta
 
-* Add function multimedia.ffmpeg.get_subprocess
+### Fixes and enhancements
 
------------
-v8.6.0-beta
------------
+- Add function `multimedia.ffmpeg.get_subprocess`
 
-Minor compatibility breaks
-==========================
+## v8.6.0-beta
 
-* Rename module django.models -> django.models.mixins
+### Minor compatibility breaks
 
-Features
-========
+- Rename module `django.models` -> `django.models.mixins`
 
-* Add module django.models.fields
-* Add class validation.CleanAttributesMixin
-* Add class validation.StrongTypedMixin
-* Add class django.forms.RequestMixin
-* Add class django.views.AddRequestToFormKwargsMixin
-* Add class django.views.LoggedCookieMixin
-* Add class unittest.AwareTearDownMixin
-* Add function subprocess.git_add_submodule
-* Add function network.http.download_ext
-* Add function datetime.parts_to_time
+### Features
 
-Fixes and enhancements
-======================
+- Add module `django.models.fields`
+- Add class `validation.CleanAttributesMixin`
+- Add class `validation.StrongTypedMixin`
+- Add class `django.forms.RequestMixin`
+- Add class `django.views.AddRequestToFormKwargsMixin`
+- Add class `django.views.LoggedCookieMixin`
+- Add class `unittest.AwareTearDownMixin`
+- Add function `subprocess.git_add_submodule`
+- Add function `network.http.download_ext`
+- Add function `datetime.parts_to_time`
 
-* Add some classes in module exception
-* Add module django.urls with utility regular expressions
-* Improve crypto.githash to handle reading data from a file
-* Fix SaveInstanceFilesMixin (use .pk instead of .id)
-* Improve datetime.str2time to handle microseconds
-* Improve filesystem.try_remove to handle directories (when recursive=True)
-* Improve multimedia.ffprobe.get_media_duration (return None in case of error)
-* StrongTypedMixin: Allow setting arg to the default value (if set)
-* Split HelpTextToPlaceholderMixin logic to allow modify behavior by inheritance
-* Fix multimedia.ffmpeg.encode (convert default_in_duration to time)
-* Fix multimedia.ffmpeg.encode (may return None - out_duration)
-* Fix multimedia.ffmpeg.encode (skip broken out duration)
-* Improve multimedia.ffprobe.get_media_duration to handle media info dict
+### Fixes and enhancements
 
------------
-v8.0.0-beta
------------
+- Add some classes in module `exception`
+- Add module `django.urls` with utility regular expressions
+- Improve `crypto.githash` to handle reading data from a file
+- Fix `SaveInstanceFilesMixin` (use .pk instead of .id)
+- Improve `datetime.str2time` to handle microseconds
+- Improve `filesystem.try_remove` to handle directories (when `recursive=True`)
+- Improve `multimedia.ffprobe.get_media_duration` (return None in case of error)
+- `StrongTypedMixin`: Allow setting arg to the default value (if set)
+- Split `HelpTextToPlaceholderMixin` logic to allow modify behavior by inheritance
+- Fix `multimedia.ffmpeg.encode` (convert default_in_duration to time)
+- Fix `multimedia.ffmpeg.encode` (may return None - out_duration)
+- Fix `multimedia.ffmpeg.encode` (skip broken out duration)
+- Improve `multimedia.ffprobe.get_media_duration` to handle media info dict
 
-Compatibility breaks
-====================
+## v8.0.0-beta
 
-* Move ffmpeg and x264 modules into multimedia
-* Replace unreliable ffmpeg.get_media_* functions by multimedia.ffprobe.get_media_*
+## Compatibility breaks
 
-Features
-========
+- Move `ffmpeg` and `x264` modules into `multimedia`
+- Replace unreliable `ffmpeg.get_media_*` functions by `multimedia.ffprobe.get_media_*`
 
-* Add module multimedia.ffprobe
-* Add function datetime.str2time
+### Features
 
-------------
-v7.1.17-beta
-------------
+- Add module `multimedia.ffprobe`
+- Add function `datetime.str2time`
 
-Compatibility breaks
-====================
+## v7.1.17-beta
 
-* Store command line arguments in args attribute, do not update __dict__ of the instance.
+## Compatibility breaks
 
-Features
-========
+- Store command line arguments in `args` attribute, do not update `__dict__` of the instance.
 
-* Add module argparse
+### Features
 
-Fixes and enhancements
-======================
+- Add module `argparse`
 
-* Add function argparse.is_file
-* Add cleanup argument to juju.boostrap
-* Add docstring to function juju.ensure_num_units
-* Add get_unit_public_address + properties methods to class juju.Environment (thanks @smarter)
-* Add args and namespace kwargs to juju.DeploymentScenario __init__ to allow bypassing sys.arv
-* Fix various bugs of juju module + various updates according to juju 1.18
-* Fix subprocess.rsync
-* Fix crypto.githash
-* Fix handling of juju bootstrap error message in Python 3
-* Default to something if key is missing in stats (x264.encode)
-* Use sudo with juju status (to work around https://bugs.launchpad.net/juju-core/+bug/1237259)
-* Add timeout to valid_uri
+### Fixes and enhancements
 
------------
-v6.6.0-beta
------------
+- Add function `argparse.is_file`
+- Add `cleanup` argument to `juju.boostrap`
+- Add docstring to function `juju.ensure_num_units`
+- Add `get_unit_public_address` + `properties` methods to class `juju.Environment` (thanks @smarter)
+- Add args and namespace kwargs to `juju.DeploymentScenario.__init__` to allow bypassing `sys.arv`
+- Fix various bugs of `juju` module + various updates according to juju 1.18
+- Fix `subprocess.rsync`
+- Fix `crypto.githash`
+- Fix handling of juju bootstrap error message in Python 3
+- Default to something if key is missing in stats (x264.encode)
+- Use sudo with juju status (to work around https://bugs.launchpad.net/juju-core/+bug/1237259)
+- Add timeout to valid_uri
 
-Compatibility breaks
-====================
+## v6.6.0-beta
 
-* Improve errors and time-outs handling in juju module (for the best)
-* Move socket & twisted fec generators to pytoolbox_bin
+## Compatibility breaks
 
-Minor compatibility breaks
-==========================
+- Improve errors and time-outs handling in `juju` module (for the best)
+- Move socket & twisted fec generators to `pytoolbox_bin`
 
-* Remove deprecated flask.get_request_data (replaced by network.http.get_requests_data)
-* SmartJSONEncoderV2 now filter the class attributes
-* Fix SmartJSONEncoderV2!
+### Minor compatibility breaks
 
-Features
-========
+- Remove deprecated `flask.get_request_data` (replaced by `network.http.get_requests_data`)
+- `SmartJSONEncoderV2` now filter the class attributes
+- Fix `SmartJSONEncoderV2`!
 
-* Add module decorators
-* Add module django.utils
-* Add module x264
-* Add function datetime.secs_to_time
-* Add function datetime.time_ratio
-* Add function ffmpeg.get_media_resolution
-* Add function mongo.mongo_do
-* Add function network.http.download
-* Add function subprocess.git_clone_or_pull
+### Features
 
-Fixes and enhancements
-======================
+- Add module `decorators`
+- Add module `django.utils`
+- Add module `x264`
+- Add function `datetime.secs_to_time`
+- Add function `datetime.time_ratio`
+- Add function `ffmpeg.get_media_resolution`
+- Add function `mongo.mongo_do`
+- Add function `network.http.download`
+- Add function `subprocess.git_clone_or_pull`
 
-* Fix test_ensure_num_units, str2datetime
-* Fix computation of FecReceiver.lostogram
-* Fix usage of time_ratio by ffmpeg and x264 modules
-* Use renamed IP class (previously IPAddress) fallback import to IPAddress
-* Accept None to leave owner or group unchanged (filesystem.chown)
-* Set default time-outs to None and update juju module (fixes)
-* Add some arguments to recursive_copy and rsync
-* Append sudo to juju bootstrap
-* Add juju.Environment.wait_unit
-* Improve ffmpeg module
+### Fixes and enhancements
 
------------
-v5.6.3-beta
------------
+- Fix `test_ensure_num_units`, `str2datetime`
+- Fix computation of `FecReceiver.lostogram`
+- Fix usage of `time_ratio` by `ffmpeg` and `x264` modules
+- Use renamed IP class (previously `IPAddress`) fallback import to `IPAddress`
+- Accept None to leave owner or group unchanged (`filesystem.chown`)
+- Set default time-outs to None and update juju module (fixes)
+- Add some arguments to `recursive_copy` and `rsync`
+- Append sudo to juju bootstrap
+- Add `juju.Environment.wait_unit`
+- Improve `ffmpeg` module
 
-Fixes and enhancements
-======================
+## v5.6.3-beta
 
-* Add timeout argument to cmd()
-* Remove symlink first, to avoid boring exceptions
-* Add timeout to juju status !
+### Fixes and enhancements
 
------------
-v5.6.0-beta
------------
+- Add timeout argument to `cmd()`
+- Remove symlink first, to avoid boring exceptions
+- Add timeout to juju status !
 
-Features
-========
+## v5.6.0-beta
 
-* Add function validation.valid_int()
+### Features
 
-Fixes and enhancements
-======================
+- Add function `validation.valid_int()`
 
-* Add constants to juju module
-* Juju bootstrap will print time as int
-* Add makedirs argument to some methods of the objects of serialization
-* Add user argument to function subprocess.cmd
-* Add path argument to subprocess.make
-* Add extra_args (list) to function subprocess.rsync
+### Fixes and enhancements
 
-* Fix juju, serialization, subprocess modules, update tests
-* Function subprocess.cmd : Handle logging.Logger as log, improve docstring, add retry loop
-* Upgrade relation_ methods
+- Add constants to `juju` module
+- Juju bootstrap will print time as int
+- Add `makedirs` argument to some methods of the objects of `serialization`
+- Add user argument to function `subprocess.cmd`
+- Add path argument to `subprocess.make`
+- Add extra_args (list) to function `subprocess.rsync`
+- Fix `juju`, `serialization`, `subprocess` modules, update tests
+- Function subprocess.cmd : Handle `logging.Logger` as log, improve docstring, add retry loop
+- Upgrade `relation_` methods
 
-------------
-v5.5.0-beta
-------------
+## v5.5.0-beta
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
-* Move all django template tags into module pytooblox_tags
-* Move juju functions to the Environment class
+- Move all django template tags into module `pytooblox_tags`
+- Move `juju` functions to the `Environment` class
 
-Features
-========
+### Features
 
-* Add console.choice() (by kyouko-taiga)
-* Add function serialization.to_file and use it to improve PickeableObject and JsoneableObject write methods.
+- Add `console.choice()` (by kyouko-taiga)
+- Add function `serialization.to_file` and use it to improve `PickeableObject` and `JsoneableObject` write methods.
 
-Fixes and enhancements
-======================
+### Fixes and enhancements
 
-* Add missing MANIFEST.in
-* Add new django-related modules
-* Add some django mixins + template tags
-* Make class django.models.GoogleMapsMixin more generic
-* Add cli_output argument to subprocess.cmd
-* Add size_only argument to subprocess.rsync
-* Do not add hashlib to requirements if already part of the stdlib
-* Fix headers + rest markup + update title
-* Enhance function ffmpeg.encode
-* Call log more often
+- Add missing MANIFEST.in
+- Add new django-related modules
+- Add some django mixins + template tags
+- Make class `django.models.GoogleMapsMixin` more generic
+- Add cli_output argument to `subprocess.cmd`
+- Add size_only argument to `subprocess.rsync`
+- Do not add hashlib to requirements if already part of the stdlib
+- Fix headers + rest markup + update title
+- Enhance function `ffmpeg.encode`
+- Call log more often
 
-------------
-v5.4.19-beta
-------------
+## v5.4.19-beta
 
-Deprecated
-==========
+### Deprecated
 
-* flask.get_request_data replaced by network.http.get_request_data
+- `flask.get_request_data` replaced by `network.http.get_request_data`
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
-* Split django module into submodules
-* Rename SmartModel to AbsoluteUrlMixin
+- Split `django` module into submodules
+- Rename `SmartModel` to `AbsoluteUrlMixin`
 
-Features
-========
+### Features
 
-* Embed smpte2022lib
-* Add entry points (socket-fec-generator + twisted-fec-generator)
-* Add commit and release scripts to make it more securely (run tests before, check sphinx ...)
-* Add module network.http and classes juju.SimulatedUnit(s)
-* Add module django.templatetags with getattribute function
-* Add class django.models.SaveInstanceFilesMixin
-* Add function django.forms.update_widget_attributes
+- Embed `smpte2022lib
+- Add entry points (`socket-fec-generator` + ` twisted-fec-generator`)
+- Add commit and release scripts to make it more securely (run tests before, check sphinx ...)
+- Add module `network.http` and classes `juju.SimulatedUnit(s)`
+- Add module `django.templatetags` with getattribute function
+- Add class `django.models.SaveInstanceFilesMixin`
+- Add function `django.forms.update_widget_attributes`
 
-Fixes and enhancements
-======================
+### Fixes and enhancements
 
-* Lighter list of dependencies
-* Add --extra-... flags to install dependencies for the extra features/modules.
-* Filter packages to avoid installing tests module !
-* Fix setup.py to avoid removing tests from packages list if it did not exist.
-* Add kwargs to serialization.object2json -> json.dumps
-* map_marker : Convert to unicode sooner (to handle special field class)
-* django.forms.SmartModelForm : Attributes & replacement class applied depending of the form field's class
-* Add fill option to collections.pygal_deque.list()
-* Replace range by xrange, values by itervalues, ...
-* Handle datetime.date class (function datetime.dateime2epoch)
-* Add suffix parameter to AbsoluteUrlMixin.get_absolute_url
-* Ensure import from future of great things
-* Fix docstrings
+- Lighter list of dependencies
+- Add `--extra-...` flags to install dependencies for the extra features/modules.
+- Filter packages to avoid installing tests module !
+- Fix `setup.py` to avoid removing tests from packages list if it did not exist.
+- Add kwargs to `serialization.object2json` -> `json.dumps`
+- `map_marker` : Convert to unicode sooner (to handle special field class)
+- `django.forms.SmartModelForm` : Attributes & replacement class applied depending of the form field's class
+- Add fill option to `collections.pygal_deque.list()`
+- Replace range by xrange, values by itervalues, ...
+- Handle `datetime.date` class (function `datetime.dateime2epoch`)
+- Add suffix parameter to `AbsoluteUrlMixin.get_absolute_url`
+- Ensure import from future of great things
+- Fix docstrings
 
-Example usage::
+Example usage:
 
-    sudo python setup.py install --help
-    sudo python setup.py install --extra-flask
+```
+sudo python setup.py install --help
+sudo python setup.py install --extra-flask
+```
 
------------
-v5.0.0-beta
------------
+## v5.0.0-beta
 
-Compatibility breaks
-====================
+## Compatibility breaks
 
-* Remove py_ prefix of all modules & paths
-* Change license (GNU GPLv3 -> EUPL 1.1)
+- Remove `py_` prefix of all modules & paths
+- Change license (GNU GPLv3 -> EUPL 1.1)
 
-Features
-========
+### Features
 
-* Add module mongo
+- Add module `mongo`
 
-Fixes and enhancements
-======================
+### Fixes and enhancements
 
-* Use absolute imports
-* Update classifiers
-* Update README.rst
+- Use absolute imports
+- Update classifiers
+- Update README.rst
 
------------
-v4.8.7-beta
------------
+## v4.8.7-beta
 
-Minor compatibility breaks
-==========================
+### Minor compatibility breaks
 
-* Rename duration2secs -> total_seconds
-* Rename get_request_json -> get_request_data
+- Rename `duration2secs` -> `total_seconds`
+- Rename `get_request_json` -> `get_request_data`
 
-Features
-========
+### Features
 
-* Python 3 support
-* Add module py_collections
-* Add module py_django
-* Add function json_response2dict
-* Add function make
-* Add function ssh
-* Greatly improve module py_juju
-* Greatly improve module py_serialization
+- Python 3 support
+- Add module `py_collections`
+- Add module `py_django`
+- Add function `json_response2dict`
+- Add function `make`
+- Add function `ssh`
+- Greatly improve module `py_juju`
+- Greatly improve module `py_serialization`
 
-Fixes and enhancements
-======================
+### Fixes and enhancements
 
-* Update README.rst
-* Update function get_request_data
-* Update function map_exceptions
-* Update function runtests
-* Update setup.py
+- Update README.rst
+- Update function `get_request_data`
+- Update function `map_exceptions`
+- Update function `runtests`
+- Update `setup.py`
 
-------------
-v4.0.0-beta
-------------
+## v4.0.0-beta
 
-Compatibility breaks
-====================
+## Compatibility breaks
 
-* Greatly improve module py_serialization
+- Greatly improve module `py_serialization`
 
-Features
-========
+### Features
 
-* Greatly improve module py_juju
-* Add class TimeoutError
-* Add function print_error
+- Greatly improve module `py_juju`
+- Add class `TimeoutError`
+- Add function `print_error`
 
-Fixes and enhancements
-======================
+### Fixes and enhancements
 
-* Fix setup.py
-* Update cmd
-* Update rsync
+- Fix `setup.py`
+- Update `cmd`
+- Update `rsync`
 
-------------
-v3.10.7-beta
-------------
+## v3.10.7-beta
 
-Compatibility breaks
-====================
+## Compatibility breaks
 
-* Rename module py_mock -> py_unittest
-* Remove function unicode_csv_reader
+- Rename module `py_mock` -> `py_unittest`
+- Remove function `unicode_csv_reader`
 
-Features
-========
+### Features
 
-* Add module py_console
-* Add module py_unicode
-* Add module and function runtests
-* Add class JsoneableObject
-* Add function assert_raises_item
-* Add function valid_uri
-* Add function validate_list
-* Greatly improve module py_juju
-* Greatly improve setup and unit-testing
+- Add module `py_console`
+- Add module `py_unicode`
+- Add module and function `runtests`
+- Add class `JsoneableObject`
+- Add function `assert_raises_item`
+- Add function `valid_uri`
+- Add function `validate_list`
+- Greatly improve module `py_juju`
+- Greatly improve setup and unit-testing
 
-Fixes and enhancements
-======================
+### Fixes and enhancements
 
-* Fix shebangs
-* Handle unicode
-* Use new string formatting
-* Update function map_exceptions
-* Add kwargs to functions of module py_subprocess
+- Fix shebangs
+- Handle unicode
+- Use new string formatting
+- Update function map_exceptions
+- Add kwargs to functions of module `py_subprocess`
```

### Comparing `pytoolbox-14.4.0/pytoolbox/ai/vision/face/detect/dlib.py` & `pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/dlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """
         if landmark_indices is None:
             landmark_indices = self.OUTER_EYES_AND_NOSE
         if landmarks is None:
             landmarks = self.find_landmarks(image, box)
 
         landmarks = np.float32(landmarks)
-        landmark_indices = np.array(landmark_indices)
+        landmark_indices = np.array(landmark_indices)  # pylint:disable=redefined-variable-type
 
         H = cv2.getAffineTransform(       # pylint:disable=invalid-name,no-member
             landmarks[landmark_indices],  # pylint:disable=unsubscriptable-object
             dimension * MINMAX_TEMPLATE[landmark_indices])
 
         return cv2.warpAffine(image, H, (dimension, dimension))  # pylint:disable=no-member
 
@@ -162,16 +162,16 @@
         :param image: RGB image to process. Shape: (height, width, 3)
         :type image: numpy.ndarray
         :return: All face bounding boxes in an image.
         :rtype: dlib.rectangles
         """
         try:
             return self.detector(image, 1)
-        except Exception as e:  # pylint:disable=broad-except
-            print(f"Warning: {e}")
+        except Exception as ex:  # pylint:disable=broad-except
+            print(f"Warning: {ex}")
             # In rare cases, exceptions are thrown.
             return []
 
     def get_largest_face_bounding_box(self, image, skip_multi=False):
         """
         Find the largest face bounding box in an image.
```

### Comparing `pytoolbox-14.4.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py` & `pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/ai/vision/utils.py` & `pytoolbox-14.5.0/pytoolbox/ai/vision/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/argparse.py` & `pytoolbox-14.5.0/pytoolbox/argparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,49 +14,50 @@
 >>> assert parser.parse_args(['.']).directory == Path(os.getcwd()).expanduser().resolve()
 >>> parser.parse_args(['/does_not_exist/'])
 Traceback (most recent call last):
     ...
 SystemExit: 2
 """
 
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Optional, Union
 import argparse, getpass, os, shutil
 
 from . import itertools, module
 
 _all = module.All(globals())
 
 # Credits https://gist.github.com/brantfaircloth/1443543
 
 
-def is_dir(path: Union[str, Path]) -> Path:
+def is_dir(path: str | Path) -> Path:
     """Check if `path` is an actual directory and return it."""
     path = Path(path)
     if path.is_dir():
         return path
     raise argparse.ArgumentTypeError(f'{path} is not a directory')
 
 
-def is_file(path: Union[str, Path]) -> Path:
+def is_file(path: str | Path) -> Path:
     """Check if `path` is an actual file and return it."""
     path = Path(path)
     if path.is_file():
         return path
     raise argparse.ArgumentTypeError(f'{path} is not a file')
 
 
-def multiple(f):
-    """Return a list with the result of `f`(value) for value in values."""
+def multiple(func):
+    """Return a list with the result of `func`(value) for value in values."""
     def _multiple(values):
-        return [f(v) for v in values] if isinstance(values, (list, tuple)) else f(values)
+        return [func(v) for v in values] if isinstance(values, (list, tuple)) else func(values)
     return _multiple
 
 
-def password(value: Optional[str]) -> str:
+def password(value: str | None) -> str:
     return value or getpass.getpass('Password: ')
 
 
 def set_columns(value=None, default=120):
     if value is None:
         try:
             value = shutil.get_terminal_size().columns
@@ -65,32 +66,32 @@
     os.environ['COLUMNS'] = str(value)
 
 
 class FullPaths(argparse.Action):
     """Expand user/relative paths."""
 
     def __call__(self, parser, namespace, values, option_string=None):
-        def fullpath(path: Union[str, Path]) -> Path:
+        def fullpath(path: str | Path) -> Path:
             return Path(path).expanduser().resolve()
         value = itertools.extract_single([fullpath(v) for v in itertools.chain(values)])
         setattr(namespace, self.dest, value)
 
 
-class Range(object):
+class Range(object):  # pylint:disable=too-few-public-methods
 
     def __init__(self, type, min, max):  # pylint:disable=redefined-builtin
         self.type = type
         self.min = min
         self.max = max
 
     def __call__(self, value):
         try:
             value = self.type(value)
-        except Exception as e:
-            raise argparse.ArgumentTypeError(f'Must be of type {self.type.__name__}') from e
+        except Exception as ex:
+            raise argparse.ArgumentTypeError(f'Must be of type {self.type.__name__}') from ex
         if not (self.min <= value <= self.max):  # pylint:disable=superfluous-parens
             raise argparse.ArgumentTypeError(f'Must be in range [{self.min}, {self.max}]')
         return value
 
 
 class HelpArgumentParser(argparse.ArgumentParser):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/atlassian.py` & `pytoolbox-14.5.0/pytoolbox/atlassian.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/aws/s3.py` & `pytoolbox-14.5.0/pytoolbox/aws/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,32 +34,32 @@
             if any(p.match(key) for p in patterns):
                 yield obj
 
 
 def load_object_meta(s3, bucket_name, path, fail=True):
     try:
         return s3.head_object(Bucket=bucket_name, Key=path)
-    except ClientError as e:
-        if 'Not Found' in str(e) and not fail:
+    except ClientError as ex:
+        if 'Not Found' in str(ex) and not fail:
             return None
         raise
 
 
 def read_object(s3, bucket_name, path, file=None, fail=True):
     try:
         if file is None:
             with BytesIO() as f:
                 s3.download_fileobj(bucket_name, path, f)
                 return f.getvalue()
         else:
             s3.download_fileobj(bucket_name, path, file)
             file.seek(0)
             return file
-    except ClientError as e:
-        if 'Not Found' in str(e) and not fail:
+    except ClientError as ex:
+        if 'Not Found' in str(ex) and not fail:
             return None
         raise
 
 
 def remove_objects(
     s3,
     bucket_name,
```

### Comparing `pytoolbox-14.4.0/pytoolbox/collections.py` & `pytoolbox-14.5.0/pytoolbox/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/comparison.py` & `pytoolbox-14.5.0/pytoolbox/comparison.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Iterator, Optional, Type, Union
+from __future__ import annotations
+
+from collections.abc import Iterator
 import difflib, operator as op, os
 
 from packaging.version import (  # pylint:disable=ungrouped-imports
     parse as _parse_version,
     InvalidVersion,
     Version
 )
@@ -58,50 +60,43 @@
             yield termcolor.colored(line, 'blue')
         else:
             yield line
 
 
 # Versions -----------------------------------------------------------------------------------------
 
-def _eqn(a, b) -> Optional[bool]:  # pylint:disable=invalid-name
+def _eqn(a, b) -> bool | None:  # pylint:disable=invalid-name
     return True if a == b else None
 
 
-def _nen(a, b) -> Optional[bool]:  # pylint:disable=invalid-name
+def _nen(a, b) -> bool | None:  # pylint:disable=invalid-name
     return False if a == b else None
 
 
-VERSION_OPERATIONS: dict = {
+VERSION_OPERATIONS: dict = {  # pylint:disable=consider-using-namedtuple-or-dataclass
     Version: {'<': op.lt, '<=': op.le, '==': op.eq, '!=': op.ne, '>=': op.ge, '>': op.gt},
     str: {'<': _nen, '<=': _eqn, '==': op.eq, '!=': op.ne, '>=': _eqn, '>': _nen}
 }
 
-try:
-    from packaging.version import LegacyVersion
-    VERSION_OPERATIONS[LegacyVersion] = VERSION_OPERATIONS[str]
-    VersionType = Union[LegacyVersion, Version]
-except ImportError:
-    VersionType: Type = Version  # type: ignore[no-redef]
-
 
 def compare_versions(
     a: str,  # pylint:disable=invalid-name
     b: str,  # pylint:disable=invalid-name
     operator: str
-) -> Optional[bool]:
+) -> bool | None:
     version_a = try_parse_version(a)
     version_b = try_parse_version(b)
     if type(version_a) is type(version_b):
         operation = VERSION_OPERATIONS[type(version_a)][operator]
         return operation(version_a, version_b) if operation else None
     return None  # Will not try to compare Version to LegacyVersion
 
 
 def satisfy_version_constraints(
-    version: Optional[str],
+    version: str | None,
     constraints: tuple[str, ...], *,
     default='<undefined>',
 ) -> bool:
     """
     Ensure given version fulfill the constraints (if any).
 
     Constraints are given in the form '<operator> <version>', Exemple:
@@ -118,12 +113,12 @@
     True
     >>> satisfy_version_constraints(None, ['!= master'], default='master')
     False
     """
     return all(compare_versions(version or default, *c.split(' ')[::-1]) for c in constraints or [])
 
 
-def try_parse_version(version: str) -> Union[VersionType, str]:
+def try_parse_version(version: str) -> Version | str:
     try:
         return _parse_version(version)
     except InvalidVersion:
         return version
```

### Comparing `pytoolbox-14.4.0/pytoolbox/console.py` & `pytoolbox-14.5.0/pytoolbox/console.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional
+from __future__ import annotations
+
 import atexit, code, os, sys
 
 __all__ = ['confirm', 'choice', 'print_error', 'progress_bar', 'shell']
 
 
 def confirm(question=None, default=False, stream=sys.stdout):
     """
@@ -24,20 +25,19 @@
     """
     if question is None:
         question = 'Confirm'
     question = f"{question} ? [{'Y/n' if default else 'y/N'}]: "
     while True:
         stream.write(question)
         stream.flush()
-        answer = input()
-        if not answer:
+        if not (answer := input()):  # pylint:disable=bad-builtin
             return default
-        if answer.lower() in ('y', 'yes'):
+        if answer.lower() in ('y', 'yes'):  # pylint:disable=use-set-for-membership
             return True
-        if answer.lower() in ('n', 'no'):
+        if answer.lower() in ('n', 'no'):  # pylint:disable=use-set-for-membership
             return False
         stream.write(f'please enter y(es) or n(o).{os.linesep}')
         stream.flush()
 
 
 def choice(question='', choices=tuple(), stream=sys.stdout):
     """
@@ -60,17 +60,16 @@
     if question is None:
         question = f'[{choices_string}]? '
     else:
         question = f'{question} [{choices_string}]: '
 
     # loop until an acceptable choice has been answered
     while True:
-        ans = input(question)
-        if ans in choices:
-            return ans
+        if (answer := input(question)) in choices:  # pylint:disable=bad-builtin
+            return answer
         stream.write(f'Please choose between {choices_string}.{os.linesep}')
 
 
 def print_error(message, exit_code=1, stream=sys.stderr):
     """
     Print an error message and exit if `exit_code` is not None.
 
@@ -146,15 +145,15 @@
     else:
         print('You do not like my question')
 
     print(choice('Select a language', ['Italian', 'French']))
 
 
 def toggle_colors(
-    env: Optional[dict[str, str]] = None,
+    env: dict[str, str] | None = None,
     *,
     colorize: bool,
     disable_vars=('NO_COLOR', 'ANSI_COLORS_DISABLED'),
     enable_vars=('FORCE_COLOR', )
 ) -> dict[str, str]:
     """
     Return `env` (defaulting to `os.environ`) updated to enable or disable colors.
```

### Comparing `pytoolbox-14.4.0/pytoolbox/crypto.py` & `pytoolbox-14.5.0/pytoolbox/crypto.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     'd41d8cd98f00b204e9800998ecf8427e'
     >>> checksum('give me some hash please')
     'cebf462dd7771c78d3957446b1b4a2f5928731ca41eff66aa8817a6513ea1313'
     >>> checksum('et ça fonctionne !\\n')
     'ced3a2b067d105accb9f54c0b37eb79c9ec009a61fee5df7faa8aefdbff1ddef'
     >>> checksum('et ça fonctionne !\\n', algorithm='md5')
     '3ca34e7965fd59beaa13b6e7094f43e7'
-    >>> checksum(directory / '..' / 'setup.py', is_path=True)
-    '28ffad590e8d5cc888a6fcb77cab07252692d29802206ba81945afb69aab358d'
-    >>> checksum(directory / '..' / 'setup.py', is_path=True, chunk_size=997)
-    '28ffad590e8d5cc888a6fcb77cab07252692d29802206ba81945afb69aab358d'
+    >>> checksum(directory / '..' / 'LICENSE.rst', is_path=True)
+    '793b47e008d4261d4fdc5ed24d56eb8d879b9a2e72d37c24a6944558b87909f8'
+    >>> checksum(directory / '..' / 'LICENSE.rst', is_path=True, chunk_size=997)
+    '793b47e008d4261d4fdc5ed24d56eb8d879b9a2e72d37c24a6944558b87909f8'
     """
     hasher = new(algorithm)
     for data in filesystem.get_bytes(path_or_data, encoding, is_path, chunk_size):
         hasher.update(data)
     return hasher.hexdigest()
 
 
@@ -92,18 +92,18 @@
     >>>
     >>> githash('')
     'e69de29bb2d1d6434b8b29ae775ad8c2e48c5391'
     >>> githash('give me some hash please')
     'abdd1818289725c072eff0f5ce185457679650be'
     >>> githash('et ça fonctionne !\\n')
     '91de5baf6aaa1af4f662aac4383b27937b0e663d'
-    >>> githash(directory / '..' / 'setup.py', is_path=True)
-    '388b2b5ff8dc37a4f3f8997ff1ca47368a97d17b'
-    >>> githash(directory / '..' / 'setup.py', is_path=True, chunk_size=256)
-    '388b2b5ff8dc37a4f3f8997ff1ca47368a97d17b'
+    >>> githash(directory / '..' / 'LICENSE.rst', is_path=True)
+    'b699ab5e129290e7bce9cbbc70443bf1cdede4ea'
+    >>> githash(directory / '..' / 'LICENSE.rst', is_path=True, chunk_size=256)
+    'b699ab5e129290e7bce9cbbc70443bf1cdede4ea'
     """
     hasher = hashlib.sha1()
     if is_path:
         hasher.update((f'blob {os.path.getsize(path_or_data)}\0').encode('utf-8'))
         for data_bytes in filesystem.get_bytes(path_or_data, encoding, is_path, chunk_size):
             hasher.update(data_bytes)
     else:
@@ -115,24 +115,24 @@
 
 def guess_algorithm(checksum, algorithms=None, unique=False):  # pylint:disable=redefined-outer-name
     """
     Guess the algorithms that have produced the checksum, based on its size.
 
     **Example usage**
 
-    >>> algorithms = ('md4', 'md5', 'sha256', 'sha512', 'whirlpool')
+    >>> algorithms = ('md5', 'sha256', 'sha512')
     >>> long_checksum = '43d92a466b57e3744532eab7d760708028a7562d9678f6762bf341f29b921e42'
     >>> short_checksum = '2b31de8940dfd3286f70c316f701a54a'
     >>> guess_algorithm('', algorithms)
     set()
     >>> {a.name for a in guess_algorithm(long_checksum, algorithms)}
     {'sha256'}
     >>> guess_algorithm(long_checksum, algorithms, unique=True).name
     'sha256'
-    >>> guess_algorithm(short_checksum, algorithms, unique=True) is None
+    >>> guess_algorithm('toto', algorithms, unique=True) is None
     True
 
     Following examples depends of your system, so they are disabled::
 
     >> {a.name for a in guess_algorithm(short_checksum)}
     {'md4', 'md5'}
     >> {a.name for a in guess_algorithm(long_checksum))}
@@ -140,17 +140,17 @@
     """
     digest_size = len(checksum) / 2
     if algorithms:
         algorithms = [hashlib.new(a) if isinstance(a, str) else a for a in algorithms]
     else:
         try:
             algorithms = [hashlib.new(a) for a in hashlib.algorithms_available if a.lower() == a]
-        except AttributeError as e:
+        except AttributeError as ex:
             raise NotImplementedError(
-                "Your version of hashlib doesn't implement algorithms_available") from e
+                "Your version of hashlib doesn't implement algorithms_available") from ex
     digest_size_to_algorithms = collections.defaultdict(set)
     for algorithm in algorithms:
         digest_size_to_algorithms[algorithm.digest_size].add(algorithm)
     possible_algorithms = digest_size_to_algorithms[digest_size]
     if unique:
         return possible_algorithms.pop() if len(possible_algorithms) == 1 else None
     return possible_algorithms
```

### Comparing `pytoolbox-14.4.0/pytoolbox/datetime.py` & `pytoolbox-14.5.0/pytoolbox/datetime.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/decorators.py` & `pytoolbox-14.5.0/pytoolbox/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools, os, warnings
 
 from . import console, module, subprocess as py_subprocess
 
 _all = module.All(globals())
 
 
-class cached_property(object):  # pylint:disable=invalid-name
+class cached_property(object):  # pylint:disable=invalid-name,too-few-public-methods
     """
     Decorator that converts a method with a single self argument into a property
     cached on the instance.
 
     Optional ``name`` argument allows you to make cached properties of other methods.
     For example ``url=cached_property(get_absolute_url, name='url')``.
 
@@ -41,15 +41,15 @@
             category=DeprecationWarning,
             filename=func.__code__.co_filename,
             lineno=func.__code__.co_firstlineno + 1)
         return func(*args, **kwargs)
     return _deprecated
 
 
-class hybridmethod(object):  # pylint:disable=invalid-name
+class hybridmethod(object):  # pylint:disable=invalid-name,too-few-public-methods
     """
     Decorator that allows a method to be both used as a class method and an instance method.
 
     Credits: http://stackoverflow.com/questions/18078744/#18078819
 
     **Example usage**
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/core/exceptions.py` & `pytoolbox-14.5.0/pytoolbox/django/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/core/validators.py` & `pytoolbox-14.5.0/pytoolbox/django/core/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
 @deconstructible
 class KeysValidator(object):
     """
     A validator designed for HStore to require, even restrict keys.
 
-    Code mostly borrowed from: https://github.com/django/django/blob/master/django/contrib/postgres/validators.py
+    Code mostly borrowed from:
+
+    https://github.com/django/django/blob/master/django/contrib/postgres/validators.py
     """
 
     messages = {
         'missing_keys': _('Some keys were missing: %(keys)s'),
         'extra_keys': _('Some unknown keys were provided: %(keys)s'),
     }
     strict = False
@@ -53,19 +55,19 @@
                 raise ValidationError(
                     self.messages['extra_keys'],
                     code='extra_keys',
                     params={'keys': ', '.join(extra_keys)})
 
     def __eq__(self, other):
         return (
-            isinstance(other, self.__class__) and
-            self.required_keys == other.required_keys and
-            self.optional_keys == other.optional_keys and
-            self.messages == other.messages and
-            self.strict == other.strict
+            isinstance(other, self.__class__)
+            and self.required_keys == other.required_keys
+            and self.optional_keys == other.optional_keys
+            and self.messages == other.messages
+            and self.strict == other.strict
         )
 
     def __ne__(self, other):
         return not self == other
 
 
 class MD5ChecksumValidator(validators.RegexValidator):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/forms/base.py` & `pytoolbox-14.5.0/pytoolbox/django/forms/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/forms/fields.py` & `pytoolbox-14.5.0/pytoolbox/django/forms/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/forms/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/forms/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     differently.
     """
 
     errors_map = {}
 
     def add_error(self, field, error):
         field = self.errors_map.get(field, field)
-        return super(MapErrorsMixin, self).add_error(field, error)
+        return super().add_error(field, error)
 
 
 class ModelBasedFormCleanupMixin(object):
     """
     Make possible the cleanup of the form by the model through a class method called `clean_form`.
     Useful to cleanup the form based on complex conditions, e.g. if two fields are inter-related
     (start/end dates, ...).
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/forms/utils.py` & `pytoolbox-14.5.0/pytoolbox/django/forms/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/forms/widgets.py` & `pytoolbox-14.5.0/pytoolbox/django/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/decorators.py` & `pytoolbox-14.5.0/pytoolbox/django/models/decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/fields/base.py` & `pytoolbox-14.5.0/pytoolbox/django/models/fields/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,24 @@
 class ExtraChoicesField(StripCharField):
 
     def __init__(self, verbose_name=None, extra_choices=None, **kwargs):
         self.extra_choices = extra_choices or []
         super().__init__(verbose_name=verbose_name, **kwargs)
 
     def deconstruct(self):
-        name, path, args, kwargs = super(ExtraChoicesField, self).deconstruct()
+        name, path, args, kwargs = super().deconstruct()
         if self.extra_choices:
             kwargs['extra_choices'] = self.extra_choices
         return name, path, args, kwargs
 
     def validate(self, value, model_instance):
         choices = self._choices
         try:
             self._choices = list(self.choices) + list(self.extra_choices)
-            return super(ExtraChoicesField, self).validate(value, model_instance)
+            return super().validate(value, model_instance)
         finally:
             self._choices = choices
 
 
 # Date and time
 
 class CreatedAtField(mixins.OptionsMixin, models.DateTimeField):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/fields/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/models/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/managers/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/models/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/models/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 - BetterUniquenessErrorsMixin
 - AutoForceInsertMixin
 - CallFieldsPreSaveMixin
 - AutoUpdateFieldsMixin
 - AlwaysUpdateFieldsMixin
 - AutoRemovePKFromUpdateFieldsMixin
-- ValidateOnSaveMixin (will defeat the detection method of AutoUpdateFieldsMixin if placed before it)
+- ValidateOnSaveMixin (will defeat the detection method of AutoUpdateFieldsMixin if put before it)
 - UpdatePreconditionsMixin
 - StateTransitionPreconditionMixin
 - StateTransitionEventsMixin
 
 Order for these does not matter:
 
 - PublicMetaMixin
@@ -106,15 +106,15 @@
     * Detect fields updated by the field's pre_save - CallFieldsPreSaveMixin before this mix-in.
     * Filter the primary key from the list of fields to update - AutoRemovePKFromUpdateFieldsMixin
       after this mix-in.
     """
     default_force_update = False
 
     def __init__(self, *args, **kwargs):
-        super(AutoUpdateFieldsMixin, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._setted_fields = set()
         self._fields_names = frozenset(f.attname for f in self._meta.fields)
 
     def __setattr__(self, name, value):
         # Check the instance is both initialized and already stored in DB
         if name in getattr(self, '_fields_names', set()) and not self._state.adding:
             self._setted_fields.add(name)
@@ -152,32 +152,32 @@
     """
     unique_from_integrity_error = True
     unique_together_hide_fields = ()
 
     def save(self, *args, **kwargs):
         try:
             super().save(*args, **kwargs)
-        except IntegrityError as e:
+        except IntegrityError as ex:
             if self.unique_from_integrity_error:
-                match = re.search(r'duplicate key[^\)]+\((?P<fields>[^\)]+)\)', e.args[0])
+                match = re.search(r'duplicate key[^\)]+\((?P<fields>[^\)]+)\)', ex.args[0])
                 if match:
                     fields = {
                         f.strip().replace('_id', '')
                         for f in match.groupdict()['fields'].split(',')
                     }
                     if fields in (set(u) for u in self._meta.unique_together):
                         fields = sorted(fields - set(self.unique_together_hide_fields))
                         if fields:
                             error = self.unique_error_message(self.__class__, fields)
                             raise ValidationError({fields[0]: error}) if len(fields) == 1 else error
-                        return self._handle_hidden_duplicate_key_error(e)
+                        return self._handle_hidden_duplicate_key_error(ex)
             raise
 
-    def _handle_hidden_duplicate_key_error(self, e):
-        raise e
+    def _handle_hidden_duplicate_key_error(self, ex):
+        raise ex
 
     def _perform_unique_checks(self, unique_checks):
         errors_by_field = super()._perform_unique_checks(unique_checks)
         hidden_fields = set(self.unique_together_hide_fields)
         if not hidden_fields:
             return errors_by_field
         filtered_errors_by_field = collections.defaultdict(list)
@@ -271,17 +271,17 @@
     def pop_preconditions(self, *args, **kwargs):
         self._preconditions = kwargs.pop('pre_excludes', {}), kwargs.pop('pre_filters', {})
         return args, kwargs, any(self._preconditions)
 
     def save(self, *args, **kwargs):
         args, kwargs, has_preconditions = self.pop_preconditions(*args, **kwargs)
         try:
-            super(UpdatePreconditionsMixin, self).save(*args, **kwargs)
-        except DatabaseError as e:
-            if has_preconditions and 'did not affect' in '{0}'.format(e):
+            super().save(*args, **kwargs)
+        except DatabaseError as ex:
+            if has_preconditions and 'did not affect' in str(ex):
                 raise self.precondition_error_class()
             raise
 
     def _do_update(self, base_qs, using, pk_val, values, update_fields, force_update):
         # FIXME _do_update is called once for each model in the inheritance hierarchy: Handle this!
         args = self.apply_preconditions(base_qs, using, pk_val, values, update_fields, force_update)
         updated = super()._do_update(*args)
@@ -294,15 +294,18 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.previous_state = self.state
 
     def on_post_state_transition(self, args, kwargs):
         signals.post_state_transition.send(
-            instance=self, previous_state=self.previous_state, args=args, kwargs=kwargs)
+            instance=self,
+            previous_state=self.previous_state,
+            args=args,
+            kwargs=kwargs)
 
     def save(self, *args, **kwargs):
         super().save(*args, **kwargs)
         if 'state' in kwargs.get('update_fields', ['state']):
             self.on_post_state_transition(args, kwargs)
             self.previous_state = self.state
 
@@ -335,18 +338,18 @@
             return False
         raise self.invalid_state_error_class(instance=self, states=states)
 
     def pop_preconditions(self, *args, **kwargs):
         """
         Add state precondition if state will be saved and state is not enforced by preconditions.
         """
-        args, kwargs, has_preconditions = super().pop_preconditions(*args, **kwargs)
+        args, kwargs, _ = super().pop_preconditions(*args, **kwargs)
         if (
-            kwargs.pop('check_state', self.check_state) and
-            'state' in kwargs.get('update_fields', ['state'])
+            kwargs.pop('check_state', self.check_state)
+            and 'state' in kwargs.get('update_fields', ['state'])
         ):
             pre_excludes, pre_filters = self._preconditions
             if not any(f.startswith('state') for f in itertools.chain(pre_excludes, pre_filters)):
                 states, valid = self.states.get_transit_from(self.state, auto_inverse=True)
                 assert states, (states, valid)
                 key, values = (
                     ('state__in', states) if len(states) > 1 else ('state', next(iter(states)))
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/query/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/models/query/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/models/utils.py` & `pytoolbox-14.5.0/pytoolbox/django/models/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     model = ct_models.ContentType.objects.get(app_label=app_label, model=model)
     return model.get_object_for_this_type(pk=pk)
 
 
 def try_get_field(instance, field_name):
     try:
         return getattr(instance, field_name)
-    except Exception as e:
-        if e.__class__.__name__ != 'RelatedObjectDoesNotExist':
+    except Exception as ex:
+        if ex.__class__.__name__ != 'RelatedObjectDoesNotExist':
             raise
 
 
 __all__ = _all.diff(globals())
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/signals/handlers.py` & `pytoolbox-14.5.0/pytoolbox/django/signals/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     """
     Ensure the site name and domain is well configured.
 
     Some alternative:
 
     * Loading an initial fixture with the values for the site
     * The application `django-defaultsite <https://github.com/oppian/django-defaultsite>`_
-    * Other options discussed `here <https://groups.google.com/forum/#!topic/django-developers/X-ef0C0V8Rk>`_
+    * Other options discussed here:
+        `here <https://groups.google.com/forum/#!topic/django-developers/X-ef0C0V8Rk>`_
     """
     from django.contrib.sites import models as site_app
     site_fields = {'domain': settings.SITE_DOMAIN, 'name': settings.SITE_NAME}
     site = site_app.Site.objects.update_or_create(pk=settings.SITE_ID, defaults=site_fields)[0]
     logger.info(
         f'Updated settings of Site "{site.name}" with ID {site.pk} and domain {site.domain}')
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/storage.py` & `pytoolbox-14.5.0/pytoolbox/django/storage.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/templatetags.py` & `pytoolbox-14.5.0/pytoolbox/django/templatetags.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,29 @@
 except Exception:
     try:  # Django < 1.8
         string_if_invalid = settings.TEMPLATE_STRING_IF_INVALID
     except Exception:
         pass  # Use default
 
 
-# ====================   =====================   ===============   ===============   =====================
-# description            decorator               arguments         input             output
-# ====================   =====================   ===============   ===============   =====================
-# only accept string     @stringfilter           -                 is a string [1]   return ...
-# do not add < > ' " &   is_safe=True            -                 of any type       return ...
-# add HTML < > ' " &     needs_autoescape=True   autoescape=None   esc(...) [2]      return mark_safe(...)
-# ====================   =====================   ===============   ===============   =====================
+# ==================== ===================== =============== =============== =====================
+# description          decorator             arguments       input           output
+# ==================== ===================== =============== =============== =====================
+# only accept string   @stringfilter         -               is a string [1] return ...
+# do not add < > ' " & is_safe=True          -               of any type     return ...
+# add HTML < > ' " &   needs_autoescape=True autoescape=None esc(...) [2]    return mark_safe(...)
+# ==================== ===================== =============== =============== =====================
 #
 # [1] Types of string passed to a template code:
-#     1. Raw str or unicode. They’re escaped on output if auto-escaping is in effect and presented unchanged, otherwise
-#     2. Already marker as safe (SafeBytes/Text, base: SafeData) commonly used for output that contains raw HTML to keep
-#     3. Marked as needing escaping, always escaped on output, regardless in autoescape block or not, EscapeBytes/Text
+#     1. Raw str or unicode. They’re escaped on output if auto-escaping is in effect and presented
+#        unchanged, otherwise
+#     2. Already marker as safe (SafeBytes/Text, base: SafeData) commonly used for output that
+#        contains raw HTML to keep
+#     3. Marked as needing escaping, always escaped on output, regardless in autoescape block or
+#        not, EscapeBytes/Text
 # [2]: esc = conditional_escape if autoescape else lambda x: x
 
 register = template.Library()
 
 NUMERIC_TEST = re.compile(r'^\d+$')
 LABEL_TO_CLASS = {
     'ERROR': 'label-important',
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django/test/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/test/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/test/runner/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/test/runner/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/urls.py` & `pytoolbox-14.5.0/pytoolbox/django/urls.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/utils/collections.py` & `pytoolbox-14.5.0/pytoolbox/django/utils/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/utils/logging.py` & `pytoolbox-14.5.0/pytoolbox/django/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django/views/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django/views/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,16 +128,16 @@
 
 
 class ValidationErrorsMixin(object):
 
     def form_valid(self, form):
         try:
             return super().form_valid(form)
-        except ValidationError as e:
-            for field, error in exceptions.iter_validation_errors(e):
+        except ValidationError as ex:
+            for field, error in exceptions.iter_validation_errors(ex):
                 if field:
                     form.add_error(field, error)
                 else:
                     self._handle_unknown_error(form, error)
             return self.form_invalid(form)
 
     def _handle_unknown_error(self, form, error):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/django_datatable_view/views/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django_filter/filterset/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django_filter/filterset/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/django_formtools/views/mixins.py` & `pytoolbox-14.5.0/pytoolbox/django_formtools/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/enum.py` & `pytoolbox-14.5.0/pytoolbox/enum.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/exceptions.py` & `pytoolbox-14.5.0/pytoolbox/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     try:
         if delete:
             del something[index]
         elif value is None:
             something[index]  # pylint:disable=pointless-statement
         else:
             something[index] = value
-    except Exception as e:  # pylint:disable=broad-except
-        if not isinstance(e, exception_cls):
+    except Exception as ex:  # pylint:disable=broad-except
+        if not isinstance(ex, exception_cls):
             raise ValueError(
-                f'Exception {e.__class__.__name__} is not '
-                f'an instance of {exception_cls.__name__}.') from e
+                f'Exception {ex.__class__.__name__} is not '
+                f'an instance of {exception_cls.__name__}.') from ex
         return
     raise AssertionError(f'Exception {exception_cls.__name__} not raised.')
 
 
 def get_exception_with_traceback(exception):
     """
     Return a string with the exception traceback.
@@ -113,16 +113,16 @@
     >>> get_exception_with_traceback(ValueError('yé'))
     'ValueError: yé\\n'
 
     If the exception was raised then there is a traceback:
 
     >>> try:
     ...     raise RuntimeError('yé')
-    ... except Exception as e:
-    ...     trace = get_exception_with_traceback(e)
+    ... except Exception as ex:
+    ...     trace = get_exception_with_traceback(ex)
     >>> 'Traceback' in trace
     True
     >>> "raise RuntimeError('yé')" in trace
     True
     """
     buf = io.StringIO()
     traceback.print_exception(type(exception), exception, exception.__traceback__, file=buf)
```

### Comparing `pytoolbox-14.4.0/pytoolbox/filesystem.py` & `pytoolbox-14.5.0/pytoolbox/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,18 +196,15 @@
     Yield the content read from the given `path` or the `data` converted to bytes.
 
     Remark: Value of `encoding` is used only if `data` is actually a string.
     """
     if is_path:
         with open(path_or_data, 'rb') as f:
             if chunk_size is not None:
-                while True:
-                    data = f.read(chunk_size)
-                    if not data:
-                        break
+                while data := f.read(chunk_size):
                     yield data
             else:
                 yield f.read()
     else:
         yield path_or_data.encode(encoding) if isinstance(path_or_data, str) else path_or_data
 
 
@@ -220,18 +217,18 @@
 
     **Example usage**
 
     >>> from pathlib import Path
     >>>
     >>> directory = Path(__file__).resolve().parent
     >>>
-    >>> get_size(directory / '..' / 'setup.py')
-    8102
-    >>> get_size(directory/ '..', '*.cfg')
-    105
+    >>> get_size(directory / '..' / 'LICENSE.rst')
+    5747
+    >>> get_size(directory / '..', '*.rst') > 1000
+    True
     >>> get_size(directory / '..', '.*/v[^/]+\\.py', regex=True) > 10000
     True
     """
     if os.path.isfile(path):
         return os.stat(path).st_size
     return sum(
         os.stat(f).st_size
@@ -271,17 +268,17 @@
     FileExistsError: ...
     """
     if parent:
         path = os.path.dirname(path)
     try:
         os.makedirs(path, mode=mode)
         return True
-    except OSError as e:
+    except OSError as ex:
         # Directory exists
-        if e.errno == errno.EEXIST and os.path.isdir(path):
+        if ex.errno == errno.EEXIST and os.path.isdir(path):
             return False
         raise  # Re-raise exception if a different error occurred
 
 
 def recursive_copy(  # pylint:disable=too-many-locals
     source_path,
     destination_path,
@@ -359,16 +356,15 @@
 
                 # FIXME maybe a finally block for that
                 src_file.close()
                 dst_file.close()
 
         # Output directory sanity check
         if check_size:
-            dst_size = get_size(destination_path)
-            if dst_size != src_size:
+            if (dst_size := get_size(destination_path)) != src_size:
                 raise IOError(f'Destination size does not match source ({src_size} vs {dst_size})')
 
         elapsed_time = time.time() - start_time
         return {'start_date': start_date, 'elapsed_time': elapsed_time, 'src_size': src_size}
     except Exception:
         if remove_on_error:
             shutil.rmtree(destination_path, ignore_errors=True)
@@ -407,26 +403,28 @@
     >>> remove('remove', recursive=True)
     True
     """
     try:
         try:
             os.remove(path)
             return True
-        except Exception as e:
+        except Exception as ex:
             # Is a directory and recursion is allowed
             if recursive and (
-                isinstance(e, OSError) and e.errno == errno.EISDIR  # pylint:disable=no-member
-                or PermissionError is not None and isinstance(e, PermissionError)
+                isinstance(ex, OSError)
+                and ex.errno == errno.EISDIR  # pylint:disable=no-member
+                or PermissionError is not None
+                and isinstance(ex, PermissionError)
             ):
                 shutil.rmtree(path)
                 return True
             raise  # Re-raise exception if a different error occurred
-    except OSError as e:
+    except OSError as ex:
         # File does not exist
-        if e.errno == errno.ENOENT:
+        if ex.errno == errno.ENOENT:
             return False
         raise  # Re-raise exception if a different error occurred
 
 
 def symlink(source, link_name):
     """
     Symlink a file/directory (which may already exists) without throwing an exception. Returns True
```

### Comparing `pytoolbox-14.4.0/pytoolbox/flask.py` & `pytoolbox-14.5.0/pytoolbox/flask.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/humanize.py` & `pytoolbox-14.5.0/pytoolbox/humanize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math, re
 
 from . import module
 
 _all = module.All(globals())
 
 DEFAULT_BITRATE_UNITS = ('bit/s', 'kb/s', 'Mb/s', 'Gb/s', 'Tb/s', 'Pb/s', 'Eb/s', 'Zb/s', 'Yb/s')
-DEFAULT_FILESIZE_ARGS = {
+DEFAULT_FILESIZE_ARGS = {  # pylint:disable=consider-using-namedtuple-or-dataclass
     'gnu': {'base': 1000, 'units': ('B', 'K', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y')},
     'nist': {'base': 1024, 'units': ('B', 'kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB')},
     'si': {'base': 1000, 'units': ('B', 'KiB', 'MiB', 'GiB', 'TiB', 'PiB', 'EiB', 'ZiB', 'YiB')},
 }
 DEFAULT_FREQUENCY_UNITS = ('Hz', 'kHz', 'MHz', 'GHz', 'THz', 'PHz', 'EHz', 'ZHz', 'YHz')
 DEFAULT_WEIGHT_UNITS = ('g', 'Kg', 'T', 'KT', 'MT', 'GT')
 DIGIT_REGEX = re.compile(r'(\d+)')
```

### Comparing `pytoolbox-14.4.0/pytoolbox/itertools.py` & `pytoolbox-14.5.0/pytoolbox/itertools.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,18 +36,15 @@
     [[0, 1, 2], [3, 4, 5], [6]]
     >>> list(chunk(iterable, 3))
     []
     >>> list(chunk((0, 1, (2, 3)), 1, of_type=set))
     [{0}, {1}, {(2, 3)}]
     """
     iterable = iter(objects)
-    while True:
-        data = of_type(itertools.islice(iterable, 0, length))
-        if not data:
-            break
+    while (data := of_type(itertools.islice(iterable, 0, length))):
         yield data
 
 
 def extract_single(objects):
     """
     Return the object from objects if there is only one object, else return objects unmodified.
```

### Comparing `pytoolbox-14.4.0/pytoolbox/juju.py` & `pytoolbox-14.5.0/pytoolbox/juju.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     seem to not work as expected. This happens the first time (and only the first time)
     juju connect to a freshly deployed environment.
 
     Solution : http://askubuntu.com/questions/123072/ssh-automatically-accept-keys::
 
         $ echo 'StrictHostKeyChecking no' >> ~/.ssh/config
     """
-    is_destroy = (command == 'destroy-environment')
+    is_destroy = command == 'destroy-environment'
     arguments = ['sudo', 'juju', command] if command in SUPER_COMMANDS else ['juju', command]
 
     if isinstance(environment, str) and environment != 'default':
         arguments += \
             [environment] if command in ENVIRONMENT_COMMANDS else ['--environment', environment]
 
     if isinstance(options, list):
@@ -111,15 +111,15 @@
         with open(config, encoding='utf-8') as f:
             options = yaml.safe_load(f)['options']
             config = {}
             for option in options:
                 config[option] = options[option]['default']
 
     for option, value in config.items():
-        if str(value).lower() in ('false', 'true'):
+        if str(value).lower() in ('false', 'true'):  # pylint:disable=use-set-for-membership
             config[option] = str(value).lower() == 'true'
             if hasattr(log, '__call__'):
                 log(f'Convert boolean option {option} {value} -> {config[option]}')
 
     return config
 
 
@@ -171,32 +171,32 @@
     environments_dict['environments'][environment] = environment_dict
 
     with open(environments, 'w', encoding='utf-8') as f:
         f.write(yaml.safe_dump(environments_dict))
 
     try:
         return juju_do('bootstrap', environment)
-    except RuntimeError as e:
-        if 'configuration error' in str(e):
+    except RuntimeError as ex:
+        if 'configuration error' in str(ex):
             del environments_dict['environments'][environment]
             with open(environments, 'w', encoding='utf-8') as f:
                 f.write(yaml.safe_dump(environments_dict))
-            raise ValueError(f'Cannot add environment {environment} ({e}).') from e
+            raise ValueError(f'Cannot add environment {environment} ({ex}).') from ex
         raise
 
 
 def get_environment(environment, environments=None, get_status=False, status_timeout=None):
     with open(environments or DEFAULT_ENVIRONMENTS_FILE, encoding='utf-8') as f:
         environments_dict = yaml.safe_load(f)
 
     environment = environments_dict['default'] if environment == 'default' else environment
     try:
         environment_dict = environments_dict['environments'][environment]
-    except KeyError as e:
-        raise ValueError(f'No environment with name {environment}.') from e
+    except KeyError as ex:
+        raise ValueError(f'No environment with name {environment}.') from ex
 
     if get_status:
         environment_dict['status'] = Environment(name=environment).status(timeout=status_timeout)
 
     return environment_dict
 
 
@@ -240,15 +240,15 @@
         host = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         host.connect(('8.8.8.8', 80))
         __get_ip = host.getsockname()[0]
         host.close()
     return __get_ip
 
 
-class CharmConfig(object):
+class CharmConfig(object):  # pylint:disable=too-few-public-methods
 
     def __init__(self):
         self.verbose = False
 
     def __repr__(self):
         return str(self.__dict__)
 
@@ -326,16 +326,16 @@
                 raise OSError('Disabled by user.')
             self.juju_ok = True
             self.load_config(json.loads(self.cmd(['config-get', '--format=json'])['stdout']))
             self.env_uuid = os.environ.get('JUJU_ENV_UUID')
             self.name = os.environ['JUJU_UNIT_NAME']
             self.private_address = socket.getfqdn(self.unit_get('private-address'))
             self.public_address = socket.getfqdn(self.unit_get('public-address'))
-        except (subprocess.CalledProcessError, OSError) as e:
-            reason = e
+        except (subprocess.CalledProcessError, OSError) as ex:
+            reason = ex
             self.juju_ok = False
             if default_config is not None:
                 self.load_config(default_config)
             self.env_uuid = default_os_env['JUJU_ENV_UUID']
             self.name = default_os_env['JUJU_UNIT_NAME']
             self.private_address = self.public_address = socket.getfqdn(get_ip())
         self.directory = os.getcwd()
@@ -367,23 +367,22 @@
     def is_leader(self):
         """
         Returns True if current unit is the leader of the peer-relation.
 
         By convention, the leader is the unit with the *smallest* id (the *oldest* unit).
         """
         try:
-            rel_ids = self.relation_ids('peer')
-            if not rel_ids:
+            if not (rel_ids := self.relation_ids('peer')):
                 return True  # no peer relation, so we're a leader that feels alone !
             assert len(rel_ids) == 1, f'Expect only 1 peer relation id: {rel_ids}'
             peers = self.relation_list(rel_ids[0])
             self.debug(f'us={self.name} peers={peers}')
             return len(peers) == 0 or self.name <= min(peers)
-        except Exception as e:  # pylint:disable=broad-except
-            self.remark(f'Bug during leader detection: {repr(e)}')
+        except Exception as ex:  # pylint:disable=broad-except
+            self.remark(f'Bug during leader detection: {repr(ex)}')
             return True
 
     # Maps calls to charm helpers functions and replace them if called in standalone ---------------
 
     def log(self, message):
         if self.juju_ok:
             return self.cmd(['juju-log', message], logging=False)  # Avoid infinite loop !
@@ -555,17 +554,17 @@
                 raise ValueError(f'Usage {sys.argv[0]} hook_name (e.g. config-changed)')
             hook_name = sys.argv[1]
 
         try:  # Call the function hooks_...
             self.hook(f'Execute {self.__class__.__name__} hook {hook_name}')
             getattr(self, f"hook_{hook_name.replace('-', '_')}")()
             self.save_local_config()
-        except subprocess.CalledProcessError as e:
+        except subprocess.CalledProcessError as ex:
             self.log('Exception caught:')
-            self.log(e.output)
+            self.log(ex.output)
             raise
         finally:
             self.hook(f'Exiting {self.__class__.__name__} hook {hook_name}')
 
 
 class Environment(object):  # pylint:disable=too-many-instance-attributes,too-many-public-methods
 
@@ -640,16 +639,14 @@
         timeout=600,
         status_timeout=15,
         polling_delay=30
     ):  # pylint:disable=too-many-branches,too-many-locals
         """
         Bootstrap an environment, (optional) terminate all machines and other associated resources
         before the bootstrap.
-
-        :param kwargs: Extra arguments for juju_do(), options is not allowed.
         """
         if cleanup:
             print(f'Cleanup and bootstrap environment {self.name}')
             print('[WARNING] This will terminate all units deployed into environment '
                   f'{self.name} by juju !')
         else:
             print(f'Bootstrap environment {self.name}')
@@ -659,17 +656,17 @@
 
         if cleanup:
             self.destroy(force=True, remove_default=True)
         if synchronize_tools:
             self.sync_tools(all_tools=True)
         try:
             result = juju_do('bootstrap', self.name)
-        except RuntimeError as e:
+        except RuntimeError as ex:
             result = None
-            if 'already' not in str(e):
+            if 'already' not in str(ex):
                 raise
 
         if not wait_started:
             return result
 
         start_time = time.time()
         while True:
@@ -733,23 +730,22 @@
 
     # Services
 
     def get_service_config(self, service, fail=True):
         return juju_do('get', self.name, options=[service], fail=fail)
 
     def get_service(self, service, default=None, fail=True, timeout=15):
-        status_dict = self.status(fail=fail, timeout=timeout)
-        if not status_dict:
+        if not (status_dict := self.status(fail=fail, timeout=timeout)):
             return default
         try:
             return status_dict['services'][service]  # pylint: disable=unsubscriptable-object
-        except KeyError as e:
+        except KeyError as ex:
             if fail:
                 raise RuntimeError(
-                    f'Service {service} not found in environment {self.name}.') from e
+                    f'Service {service} not found in environment {self.name}.') from ex
         return default
 
     def expose_service(self, service, fail=True):
         return juju_do('expose', self.name, options=[service], fail=fail)
 
     def unexpose_service(self, service, fail=True):
         return juju_do('unexpose', self.name, options=[service], fail=fail)
@@ -770,15 +766,15 @@
         release=None,
         repository=None,
         required=True,
         terminate=False,
         to=None,
         units_number_to_keep=None,
         timeout=None
-    ):  # pylint:disable=invalid-name,too-many-branches,too-many-locals
+    ):  # pylint:disable=invalid-name,too-many-arguments,too-many-branches,too-many-locals
         """
         Ensure `num_units` units of `service` into `environment` by adding new or destroying useless
         units first !
 
         At the end of this method, the number of running units can be greater as `num_units` because
         this algorithm will not destroy units with number in `units_number_to_keep`.
 
@@ -896,24 +892,22 @@
                         constraints=constraints,
                         local=local,
                         release=release,
                         repository=repository
                     )
 
             elif units_count < num_units:
-
-                num_units = num_units - units_count
-                if num_units:  # avoid to add units if number of units to add is 0
+                # avoid to add units if number of units to add is 0
+                if num_units := num_units - units_count:
                     results['add_units'] = self.add_units(
                         service or charm,
                         num_units=num_units,
                         to=to)
 
             elif units_count > num_units:
-
                 num_units = units_count - num_units
                 destroyed = {}
                 units_number_to_keep = \
                     [int(n) for n in units_number_to_keep] if units_number_to_keep else []
 
                 # TODO implement status comparison for sorting ??
                 for status in (ERROR, NOT_STARTED, PENDING, INSTALLED, STARTED):
@@ -959,33 +953,32 @@
     def get_unit(self, service, number, default=None, fail=True, timeout=None):
         # TODO maybe none if missing or something else
         name = f'{service}/{number}'
         service_dict = self.get_service(service, default=None, fail=fail, timeout=timeout)
         if service_dict is not None:
             try:
                 return service_dict['units'][name]
-            except KeyError as e:
+            except KeyError as ex:
                 if fail:
                     raise RuntimeError(
-                        f'No unit with name {name} on environment {self.name}.') from e
+                        f'No unit with name {name} on environment {self.name}.') from ex
         return default
 
     def get_unit_public_address(self, service, number):
         """
         Return the public address of a unit. Use the most reliable value available
         (dns-name of the machine).
         """
         if self.properties(cached=True)['type'] == 'local':
             return self.get_unit(service, number)['public-address']
 
         # public-address may report a private address (172.x.x.x) with non-local deployments see
         # OSCIED #132, so we need this workaround (which cannot be used for local deployments).
         machine_number = self.get_unit(service, number)['machine']
-        status_dict = self.status()
-        if status_dict:
+        if status_dict := self.status():
             return status_dict['machines'][machine_number]['dns-name']
         raise ValueError(f'Unable to get public address of unit {service}/{number}')
 
     def wait_unit(
         self,
         service,
         number,
@@ -1025,15 +1018,15 @@
         num_units=1,
         to=None,
         config=None,
         constraints=None,
         local=False,
         release=None,
         repository=None
-    ):  # pylint:disable=invalid-name
+    ):  # pylint:disable=invalid-name,too-many-arguments
         service = service or charm
         if not charm:
             raise ValueError('Charm is required.')
         options = ['--num-units', num_units]
         if to is not None:
             options += ['--to', to]
         if config is not None:
@@ -1086,33 +1079,33 @@
             return None
 
         member1 = service1 if relation1 is None else f'{service1}:{relation1}'
         member2 = service2 if relation2 is None else f'{service2}:{relation2}'
         result = None
         try:
             result = juju_do('add-relation', self.name, options=[member1, member2])
-        except RuntimeError as e:
+        except RuntimeError as ex:
             # TODO get status of service before adding relation may be cleaner.
-            if 'already exists' not in str(e):
+            if 'already exists' not in str(ex):
                 raise
         return result
 
     def remove_relation(self, service1, service2, relation1=None, relation2=None):
         """Remove a relation between 2 services. Knowing that the relation may not exists."""
         print(f'Remove relation between {service1} and {service2}')
         if not self.auto and not console.confirm('do it now', default=False):
             return None
 
         member1 = service1 if relation1 is None else f'{service1}:{relation1}'
         member2 = service2 if relation2 is None else f'{service2}:{relation2}'
         try:
             result = juju_do('remove-relation', self.name, options=[member1, member2])
-        except RuntimeError as e:
+        except RuntimeError as ex:
             # TODO get status of service before removing relation may be cleaner.
-            if 'exists' not in str(e):
+            if 'exists' not in str(ex):
                 raise
         return result
 
 
 class DeploymentScenario(object):
 
     def __init__(self, environments, args=None, namespace=None, **kwargs):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/linux.py` & `pytoolbox-14.5.0/pytoolbox/linux.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/logging.py` & `pytoolbox-14.5.0/pytoolbox/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,30 @@
+from __future__ import annotations
+
+from pathlib import Path
 import logging, sys
 
 from .collections import merge_dicts
 
 __all__ = ['setup_logging', 'ColorizeFilter']
 
 
 def setup_logging(
-    name_or_log='',
-    reset=False,
-    path=None,
-    console=False,
-    level=logging.DEBUG,
-    colorize=False,
-    color_by_level=None,
-    fmt='%(asctime)s %(levelname)-8s - %(message)s',
-    datefmt='%d/%m/%Y %H:%M:%S'
-):
+    name_or_log: str | logging.Logger = '',
+    reset: bool = False,
+    path: Path | str = None,
+    console: bool = False,
+    level: int | str = logging.DEBUG,
+    colorize: bool = False,
+    color_by_level: dict[int | str, str] = None,
+    fmt: str = '%(asctime)s %(levelname)-8s - %(message)s',
+    datefmt: str = '%d/%m/%Y %H:%M:%S'
+) -> logging.Logger:
     """
-    Setup logging (TODO).
-
-    :param name_or_log: TODO
-    :param reset: Unregister all previously registered handlers ?
-    :type reset: bool
-    :param path: TODO
-    :type name: str
-    :param console: Toggle console output (stdout)
-    :type console: bool
-    :param level: TODO
-    :type level: int
-    :param colorize: TODO
-    :type colorize: bool
-    :param color_by_level: TODO
-    :type color_by_level: dict
-    :param fmt: TODO
-    :type fmt: str
-    :param datefmt: TODO
-    :type datefmt: str
+    Setup logging.
 
     **Example usage**
 
     Setup a console output for logger with name *test*:
 
     >>> log = setup_logging('a', reset=True, console=True, fmt=None, datefmt=None)
     >>> log.info('this is my info')
@@ -92,21 +77,21 @@
     if colorize:
         log.addFilter(ColorizeFilter(color_by_level=color_by_level))
     if path:
         handler = logging.FileHandler(path)
         handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
         log.addHandler(handler)
     if console:
-        handler = logging.StreamHandler(sys.stdout)
+        handler = logging.StreamHandler(sys.stdout)  # pylint:disable=redefined-variable-type
         handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
         log.addHandler(handler)
     return log
 
 
-class ColorizeFilter(logging.Filter):
+class ColorizeFilter(logging.Filter):  # pylint:disable=too-few-public-methods
 
     color_by_level = {
         logging.DEBUG: 'cyan',
         logging.ERROR: 'red',
         logging.INFO: 'white',
         logging.WARNING: 'yellow'
     }
@@ -115,12 +100,11 @@
         self.color_by_level = merge_dicts(
             self.color_by_level,
             kwargs.pop('color_by_level', None) or {})
         super().__init__(*args, **kwargs)
 
     def filter(self, record):
         record.raw_msg = record.msg
-        color = self.color_by_level.get(record.levelno)
-        if color:
+        if color := self.color_by_level.get(record.levelno):
             import termcolor
             record.msg = termcolor.colored(record.msg, color)
         return True
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/brand.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/brand.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,13 +49,12 @@
 
     def __new__(cls, brand):
         return cls.clean(brand)
 
     @classmethod
     def clean(cls, brand):
         brand = brand.strip() if brand else brand
-        if not brand:
+        if not brand:  # pylint:disable=consider-using-assignment-expr
             return None
-        brand = cls.clean_map.get(brand.lower(), brand)
-        if brand not in cls.brands:
+        if (brand := cls.clean_map.get(brand.lower(), brand)) not in cls.brands:
             raise exceptions.InvalidBrandError(brand=brand, brands=cls.brands)
         return brand
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/camera.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/camera.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/equipment.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/equipment.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/image.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/image.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/lens.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/lens.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 class Lens(equipment.Equipement):
 
     brand_class = brand.Brand
 
     @property
     def brand(self):
-        brands = {t.brand for t in self.tags.values() if t.brand}
-        if brands:
+        if brands := {t.brand for t in self.tags.values() if t.brand}:
             assert len(brands) == 1, brands
             return next(iter(brands))
         # Extract brand from model
         return self.brand_class(self._model.split(' ')[0])
 
     @property
     def _model(self):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/metadata.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/metadata.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/photo.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/photo.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/exif/tag.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/exif/tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pytoolbox import decorators
 from pytoolbox.datetime import str_to_datetime, str_to_time
 from . import brand  # pylint:disable=unused-import
 
 __all__ = ['Tag', 'TagSet']
 
 
-class Tag(object):
+class Tag(object):  # pylint:disable=too-few-public-methods
 
     brand_class = brand.Brand
     date_formats = ['%Y%m%d %H%M%S', '%Y%m%d']
     date_clean_regex = re.compile(r'[:-]')
     group_to_brand_blacklist = frozenset(['aux', 'crs', 'exifEX', 'Image', 'Photo'])
     type_to_hook = {
         datetime.datetime: 'get_tag_string',  # clean method will convert to a date-time
@@ -47,20 +47,19 @@
         self.key = key
 
     def __repr__(self):
         return f'<{self.__class__.__name__} {self.key}: {str(self.data)[:20]}>'
 
     @property
     def data(self):
-        type_hook = self.get_type_hook()
-        if type_hook:
+        if type_hook := self.get_type_hook():
             try:
                 return self.clean(type_hook(self.key))
-            except UnicodeDecodeError as e:
-                return e
+            except UnicodeDecodeError as ex:
+                return ex
         return self.data_bytes
 
     @property
     def data_bytes(self):
         tag_raw = self.metadata.exiv2.get_tag_raw(self.key)
         return tag_raw.get_data() if tag_raw else None
 
@@ -87,40 +86,39 @@
         return self.metadata.exiv2.get_tag_raw(self.key).get_size()
 
     @decorators.cached_property
     def type(self):
         tag_type = self.metadata.exiv2.get_tag_type(self.key)
         try:
             return self.type_to_python[tag_type]
-        except KeyError as e:
+        except KeyError as ex:
             if tag_type:
-                raise KeyError(f'Unknow tag type {tag_type}') from e
+                raise KeyError(f'Unknow tag type {tag_type}') from ex
         return bytes
 
     def clean(self, data):
         if isinstance(data, str):
             data = data.strip()
         if self.type == datetime.time:
             return str_to_time(data)
         if self.type == datetime.datetime or isinstance(data, str):
             cleaned_data = self.date_clean_regex.sub('', data)
             for date_format in self.date_formats:
-                date = str_to_datetime(cleaned_data, date_format, fail=False)
-                if date:
+                if date := str_to_datetime(cleaned_data, date_format, fail=False):
                     return date
         assert not data or isinstance(data, self.type), \
             f'{self.key} {self.type} {data} {type(data)}'
         return data
 
     def get_type_hook(self):
         name = self.type_to_hook.get(self.type)
         return getattr(self.metadata.exiv2, name) if name else None
 
 
-class TagSet(object):
+class TagSet(object):  # pylint:disable=too-few-public-methods
 
     @staticmethod
     def clean_number(number):
         return number if number and number > 0 else None
 
     def __init__(self, metadata):
         self.metadata = metadata
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/encode.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     r'q=\s*(?P<qscale>\S+)\s+\S*.*'
     r'size=\s*(?P<size>\S+)\s+'
     r'time=\s*(?P<time>\S+)\s+'
     r'bitrate=\s*(?P<bit_rate>\S+)'
 )
 
 
-class EncodeState(object):
+class EncodeState(object):  # pylint:disable=too-few-public-methods
     NEW = 'NEW'
     STARTED = 'STARTED'
     PROCESSING = 'PROCESSING'
     SUCCESS = 'SUCCESS'
     FAILURE = 'FAILURE'
 
     ALL_STATES = frozenset([NEW, STARTED, PROCESSING, SUCCESS, FAILURE])
@@ -93,16 +93,15 @@
         self.frame = 0
         self._update_ratio()
         return self
 
     def progress(self, chunk):
         self.state = self.states.PROCESSING
         self.elapsed_time = datetime.timedelta(seconds=time.time() - self.start_time)
-        ffmpeg_statistics = self._parse_chunk(chunk)
-        if ffmpeg_statistics:
+        if ffmpeg_statistics := self._parse_chunk(chunk):
             self.output.duration = ffmpeg_statistics['time']
             self.frame = ffmpeg_statistics['frame']
             self.frame_rate = ffmpeg_statistics['frame_rate']
             self.qscale = ffmpeg_statistics['qscale']
             self.output.size = ffmpeg_statistics['size']
             self.bit_rate = ffmpeg_statistics['bit_rate']
         self._update_ratio()
@@ -149,16 +148,15 @@
             sub_position = zero
 
         sub_duration = max(zero, min(duration - sub_position, sub_duration))
         return sub_duration, int(size * time_ratio(sub_duration, duration))
 
     def _parse_chunk(self, chunk):
         self.process_output += chunk
-        match = self.encoding_regex.match(chunk.strip())
-        if not match:
+        if not (match := self.encoding_regex.match(chunk.strip())):
             return None
         ffmpeg_statistics = match.groupdict()
         try:
             ffmpeg_statistics['time'] = str_to_time(ffmpeg_statistics['time'], as_delta=True)
         except ValueError:
             return None  # Parsed statistics are broken, do not use them
         ffmpeg_statistics['frame'] = int(ffmpeg_statistics['frame'])
@@ -171,15 +169,16 @@
 
     @staticmethod
     def _to_time(value):
         method = str_to_time if ':' in value else secs_to_time
         return method(value, as_delta=True)
 
 
-class FrameBasedRatioMixin(object):
+class FrameBasedRatioMixin(object):  # pylint:disable=too-few-public-methods
+    # pylint:disable=no-member
     """
     Compute ratio based on estimated input number of frames and current output number of frames.
     Fall-back to super's ratio computation method.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,24 +72,23 @@
         process = self._get_process(arguments, **(process_kwargs or {}))
         try:
             yield statistics.start(process)
             while True:
                 chunk = self._get_chunk(process)
                 yield statistics.progress(chunk or '')
                 if process_poll:
-                    returncode = process.poll()
-                    if returncode is not None:
+                    if (returncode := process.poll()) is not None:
                         break
                 if self.encode_poll_delay:
                     time.sleep(self.encode_poll_delay)
             yield statistics.end(returncode)
-        except Exception as e:
+        except Exception as ex:
             traceback = sys.exc_info()[2]
             py_subprocess.kill(process)
-            raise e.with_traceback(traceback) if hasattr(e, 'with_traceback') else e
+            raise ex.with_traceback(traceback) if hasattr(ex, 'with_traceback') else ex
 
     @staticmethod
     def get_frames_md5_checksum(filename):
         with filesystem.TempStorage() as tmp:
             checksum_filename = tmp.create_tmp_file(return_file=False)
             FFmpeg()('-y', '-i', filename, '-f', 'framemd5', checksum_filename).wait()
             with open(checksum_filename, encoding='utf-8') as f:
@@ -132,16 +131,16 @@
     def _get_chunk(self, process):
         select.select([process.stderr], [], [], self.chunk_read_timeout)
         try:
             chunk = process.stderr.read()
             if chunk is None or isinstance(chunk, str):
                 return chunk
             return chunk.decode(self.encoding)
-        except IOError as e:
-            if e.errno != errno.EAGAIN:
+        except IOError as ex:
+            if ex.errno != errno.EAGAIN:
                 raise
         return None
 
     @staticmethod
     def _get_process(arguments, **process_kwargs):
         """Return an encoding process with stderr made asynchronous."""
         process = py_subprocess.raw_cmd(
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/ffprobe.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffprobe.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
                     self.executable,
                     '-v', 'quiet',
                     '-print_format', 'json',
                     '-show_format',
                     '-show_streams',
                     media.path
                 ]).decode('utf-8'))
-        except OSError as e:
+        except OSError as ex:
             # Executable does not exist
-            if fail or e.errno == errno.ENOENT:
+            if fail or ex.errno == errno.ENOENT:
                 raise
         except Exception:  # pylint:disable=broad-except
             if fail:
                 raise
         return None
 
     def get_media_format(self, media, fail=False):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 from pytoolbox.subprocess import to_args_list
 from pytoolbox.types import get_slots
 from . import utils
 
 _all = module.All(globals())
 
 
-class BaseInfo(validation.CleanAttributesMixin, comparison.SlotsEqualityMixin):
+class BaseInfo(  # pylint:disable=too-few-public-methods
+    validation.CleanAttributesMixin,
+    comparison.SlotsEqualityMixin
+):
 
     defaults = {}
     attr_name_template = '{name}'
 
     def __init__(self, info):
         for attr in get_slots(self):
             self._set_attribute(attr, info)
 
     def _set_attribute(self, name, info):
         """Set attribute `name` value from the `info` or ``self.defaults`` dictionary."""
         value = info.get(self.attr_name_template.format(name=name), self.defaults.get(name))
         setattr(self, name, value)
 
 
-class Codec(BaseInfo):
+class Codec(BaseInfo):  # pylint:disable=too-few-public-methods
 
     __slots__ = ('long_name', 'name', 'tag', 'tag_string', 'time_base', 'type')
 
     attr_name_template = 'codec_{name}'
 
     @staticmethod
     def clean_time_base(value):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/ffmpeg/utils.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 
 def is_pipe(path):
     return isinstance(path, str) and bool(PIPE_REGEX.match(path))
 
 
 def to_bit_rate(bit_rate):
-    match = BIT_RATE_REGEX.match(bit_rate)
-    if match:
+    if match := BIT_RATE_REGEX.match(bit_rate):
         match = match.groupdict()
         return int(float(match['value']) * BIT_RATE_COEFFICIENT_FOR_UNIT[match['units'][0]])
     if bit_rate == 'N/A':
         return None
     raise ValueError(bit_rate)
 
 
@@ -35,15 +34,14 @@
             return float(num) / float(denom)
         except ZeroDivisionError:
             return None
     return float(frame_rate)
 
 
 def to_size(size):
-    match = SIZE_REGEX.match(size)
-    if match:
+    if match := SIZE_REGEX.match(size):
         match = match.groupdict()
         return int(float(match['value']) * SIZE_COEFFICIENT_FOR_UNIT[match['units'][0].lower()])
     raise ValueError(size)
 
 
 __all__ = _all.diff(globals())
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/image/PIL.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/image/PIL.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     return functools.reduce(lambda i, op: i.transpose(op), sequences.get(orientation, []), image)
 
 
 def open(file_or_path):  # pylint:disable=redefined-builtin
     image = Image.open(file_or_path)
     try:
         image.load()
-    except IOError as e:
-        if 'truncated' not in str(e):
+    except IOError as ex:
+        if 'truncated' not in str(ex):
             raise
     return image
 
 
 def remove_metadata(image, keys=('exif', ), inplace=False):
     image = image if inplace else image.copy()
     for key in keys:
```

### Comparing `pytoolbox-14.4.0/pytoolbox/multimedia/x264.py` & `pytoolbox-14.5.0/pytoolbox/multimedia/x264.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/network/http.py` & `pytoolbox-14.5.0/pytoolbox/network/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 def download(url, path):
     """Read the content of given `url` and save it as a file `path`."""
     with open(path, 'wb') as target:
         with urllib.request.urlopen(url) as source:
             target.write(source.read())
 
 
-def iter_download_core(url, code=200, chunk_size=102400, **kwargs):
-    response = requests.get(url, stream=bool(chunk_size), **kwargs)
+def iter_download_core(url, code=200, chunk_size=102400, timeout=None, **kwargs):
+    response = requests.get(url, stream=bool(chunk_size), timeout=timeout, **kwargs)
     length = response.headers.get('content-length')
     if response.status_code != code:
         raise BadHTTPResponseCodeError(url=url, code=code, r_code=response.status_code)
     if response.status_code == 200:
         if chunk_size:
             position, length = 0, None if length is None else int(length)
             for chunk in response.iter_content(chunk_size):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/network/ip.py` & `pytoolbox-14.5.0/pytoolbox/network/ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,10 +27,10 @@
         TODO IPv6 ready : >>> IPSocket('[2001:0db8:0000:0000:0000:ff00:0042]:8329')
     """
     try:
         (address, port) = socket.rsplit(':', 1)
         # address = address.translate(None, '[]')
         ip_address(address)  # Seem not IPv6 ready
         port = int(port)
-    except Exception as e:
-        raise exceptions.InvalidIPSocketError(socket=socket) from e
+    except Exception as ex:
+        raise exceptions.InvalidIPSocketError(socket=socket) from ex
     return {'ip': address, 'port': port}
```

### Comparing `pytoolbox-14.4.0/pytoolbox/network/rtp.py` & `pytoolbox-14.5.0/pytoolbox/network/rtp.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/network/smpte2022/base.py` & `pytoolbox-14.5.0/pytoolbox/network/smpte2022/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,16 +543,15 @@
             # XOR LOOP     fec.payload_recovery[i] ^= packet.payload[i]
         return fec
 
     def compute_j(self, media_sequence):
         """
         TODO
         """
-        delta = media_sequence - self.snbase
-        if delta < 0:
+        if (delta := media_sequence - self.snbase) < 0:
             delta += RtpPacket.S_MASK + 1
         if delta % self.offset != 0:
             return None
         return int(delta / self.offset)
 
     def set_missing(self, media_sequence):
         """
@@ -633,27 +632,25 @@
         >>> fec.set_recovered(3)
         Traceback (most recent call last):
             ...
         ValueError: list.remove(x): x not in list
         >>> fec.missing
         [65533, 65530]
         """
-        j = self.compute_j(media_sequence)
-        if j is None:
+        if (j := self.compute_j(media_sequence)) is None:
             raise ValueError(self.ER_J)
         if media_sequence not in self.missing:
             self.missing.append(media_sequence)
         return j
 
     def set_recovered(self, media_sequence):
         """
         TODO
         """
-        j = self.compute_j(media_sequence)
-        if j is None:
+        if (j := self.compute_j(media_sequence)) is None:
             raise ValueError(self.ER_J)
         self.missing.remove(media_sequence)
         return j
 
     def __eq__(self, other):
         """
         Test equality field by field !
```

### Comparing `pytoolbox-14.4.0/pytoolbox/network/smpte2022/generator.py` & `pytoolbox-14.5.0/pytoolbox/network/smpte2022/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,102 +34,90 @@
         >>> print(FecGenerator(4, 5).D)
         5
         """
         return self._D
 
     # <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< Constructor >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 
-    def __init__(self, L, D):  # pylint:disable=invalid-name,too-many-instance-attributes
+    def __init__(self, L: int, D: int):  # pylint:disable=invalid-name,too-many-instance-attributes
         """
         Construct a FecGenerator.
 
         :param L: Horizontal size of the FEC matrix (columns)
-        :type L: int
         :param D: Vertical size of the FEC matrix (rows)
-        :type D: int
         """
         self._L, self._D = L, D  # pylint:disable=invalid-name
         self._col_sequence = self._row_sequence = 1
         self._media_sequence = None
         self._medias = []
         self._invalid = self._total = 0
 
     # <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< Functions >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 
     @staticmethod
-    def on_new_col(col):
+    def on_new_col(col: FecPacket):
         """
         Called by FecGenerator when a new column FEC packet is generated and available for output.
 
         By default this method only print a message to `stdout`.
 
         .. seealso::
 
             You can `monkey patch <http://stackoverflow.com/questions/5626193>`_ it.
 
         :param col: Generated column FEC packet
-        :type col: FecPacket
-        :param caller: The generator that fired this method / event
-        :type caller: FecGenerator
         """
         print(
             f'New COL FEC packet '
             f'seq={col.sequence} '
             f'snbase={col.snbase} '
             f'LxD={col.L}x{col.D} '
             f'trec={col.timestamp_recovery}')
 
     @staticmethod
-    def on_new_row(row):
+    def on_new_row(row: FecPacket):
         """
         Called by FecGenerator when a new row FEC packet is generated and available for output.
 
         By default this method only print a message to `stdout`.
 
         .. seealso::
 
             You can `monkey patch <http://stackoverflow.com/questions/5626193>`_ it.
 
         :param row: Generated row FEC packet
-        :type row: FecPacket
-        :param caller: The generator that fired this method / event
-        :type caller: FecGenerator
         """
         print(
             f'New ROW FEC packet '
             f'seq={row.sequence} '
             f'snbase={row.snbase} '
             f'LxD={row.L}x{row.D} '
             f'trec={row.timestamp_recovery}')
 
-    def on_reset(self, media):
+    def on_reset(self, media: RtpPacket):
         """
         Called by FecGenerator when the algorithm is reseted (an incoming media is out of sequence).
 
         By default this method only print a message to `stdout`.
 
         .. seealso::
 
             You can `monkey patch <http://stackoverflow.com/questions/5626193>`_ it.
 
         :param media: Out of sequence media packet
-        :type row: RtpPacket
-        :param caller: The generator that fired this method / event
-        :type caller: FecGenerator
         """
         print(
             f'Media seq={media.sequence} is out of sequence '
             f'(expected {self._media_sequence}) : FEC algorithm reseted !')
 
-    def put_media(self, media):
+    def put_media(self, media: RtpPacket):
         """
         Put an incoming media packet.
 
         :param media: Incoming media packet
-        :type media: RtpPacket
 
         **Example usage**
 
         Testing input of out of sequence medias:
 
         >>> g = FecGenerator(4, 5)
         >>> R = RtpPacket
```

### Comparing `pytoolbox-14.4.0/pytoolbox/network/smpte2022/receiver.py` & `pytoolbox-14.5.0/pytoolbox/network/smpte2022/receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import collections, os
+from __future__ import annotations
+
+import collections, io, os
 
 from pytoolbox.network.ip import IPSocket
 from pytoolbox.network.rtp import RtpPacket
 from .base import FecPacket
 
 __all__ = ['FecReceiver']
 
@@ -122,20 +124,19 @@
 
     DELAY_NAMES = ['packets', 'seconds']
     DELAY_RANGE = range(len(DELAY_NAMES))  # noqa
     PACKETS, SECONDS = DELAY_RANGE
 
     # <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< Constructors >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 
-    def __init__(self, output):
+    def __init__(self, output: io.StringIO):
         """
         Construct a new FecReceiver and register `output`.
 
         :param output: Where to output payload of the recovered stream.
-        :type output: IOBase
 
         **Example usage**
 
         Not yet an output:
 
         >>> FecReceiver(None)
         Traceback (most recent call last):
@@ -182,28 +183,28 @@
         self.max_row = 0       # Largest amount of stored elements in the rows buffer
         self.lostogram = collections.defaultdict(int)  # Statistics about lost medias
         self.lostogram_counter = 0  # Incremented while there are lost media packets
 
     # <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< Properties >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 
     @property
-    def current_delay(self):
+    def current_delay(self) -> int:
         """Return current delay based on the length of the media buffer."""
         if len(self.medias) == 0:
             return 0
         if self.delay_units == self.PACKETS:
             return len(self.medias)
         if self.delay_units == self.SECONDS:
             raise NotImplementedError()
         raise ValueError(self.ER_DELAY_UNITS.format(self.delay_units))
         # return medias.lastEntry().getValue().getTime() - medias.firstEntry().getValue().getTime()
 
     # <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<< Functions >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
 
-    def set_delay(self, value, units):
+    def set_delay(self, value, units) -> None:
         """Set desired size for the internal media buffer."""
         if units == self.PACKETS:
             self.delay_value = value
             self.delay_units = units
         elif units == self.SECONDS:
             raise NotImplementedError()
         else:
@@ -212,34 +213,35 @@
     def put_media(self, media, onlyMP2TS):  # pylint:disable=invalid-name
         """Put an incoming media packet."""
         if self.flushing:
             raise ValueError(self.ER_FLUSHING)
         if onlyMP2TS:
             if not media.validMP2T:
                 raise ValueError(self.ER_VALID_RTP_MP2TS)
-        else:
-            if not media.valid:
-                raise ValueError(self.ER_VALID_RTP)
+        elif not media.valid:
+            raise ValueError(self.ER_VALID_RTP)
 
         # Put the media packet into medias buffer
         if media.sequence in self.medias:
             self.media_overwritten += 1
         self.medias[media.sequence] = media
         if len(self.medias) > self.max_media:
             self.max_media = len(self.medias)
         self.media_received += 1
 
-        cross = self.crosses.get(media.sequence)
-        if cross:
+        if cross := self.crosses.get(media.sequence):
             # Simulate the recovery of a media packet to update buffers and potentially start
             self.recover_media_packet(media.sequence, cross, None)  # a recovery cascade !
 
         self.out()  # FIXME maybe better to call it from another thread
 
-    def put_fec(self, fec):  # pylint:disable=too-many-branches,too-many-statements
+    def put_fec(  # pylint:disable=too-many-branches,too-many-statements
+        self,
+        fec: FecPacket
+    ) -> None:
         """
         Put an incoming FEC packet, the algorithm will do the following according to these
         scenarios:
 
         1. The fec packet is useless if none of the protected media packets is missing
         2. Only on media packet missing, fec packet is able to recover it now !
         3. More than one media packet is missing, fec packet stored for future recovery
@@ -262,16 +264,15 @@
         media_test = fec.snbase
 
         while media_test != media_max:
             # If media packet is not in the medias buffer (is missing)
             if media_test not in self.medias:
                 media_lost = media_test
                 # TODO
-                cross = self.crosses.get(media_test)
-                if not cross:
+                if not (cross := self.crosses.get(media_test)):
                     cross = {'col_sequence': None, 'row_sequence': None}
                     self.crosses[media_test] = cross
                     if len(self.crosses) > self.max_cross:
                         self.max_cross = len(self.crosses)
 
                 # Register the fec packet able to recover the missing media packet
                 if fec.direction == FecPacket.COL:
@@ -297,15 +298,15 @@
         if fec.D:
             self.matrixD = fec.D
 
         # [1] The fec packet is useless if none of the protected media packets is missing
         if len(fec.missing) == 0:
             return
 
-        # FIXME check if 10*delay_value is a good way to avoid removing early fec packets !
+        # FIXME check if 10 * delay_value is a good way to avoid removing early fec packets !
         # The fec packet is useless if it needs an already output'ed media packet to do recovery
         drop = not self.validity_window(
             fec.snbase,
             self.position,
             (self.position + 10 * self.delay_value) & RtpPacket.S_MASK
         )
 
@@ -327,24 +328,24 @@
 
         # [2] Only on media packet missing, fec packet is able to recover it now !
         if len(fec.missing) == 1:
             self.recover_media_packet(media_lost, cross, fec)
             self.out()  # FIXME maybe better to call it from another thread
         # [3] More than one media packet is missing, fec packet stored for future recovery
 
-    def flush(self):
+    def flush(self) -> None:
         """Flush all buffers and output media packets to registered output (``self.output``)."""
         try:
             self.flushing = True
             self.out()
             self.output.flush()
         finally:
             self.flushing = False
 
-    def cleanup(self):
+    def cleanup(self) -> None:
         """Remove FEC packets that are stored / waiting but useless."""
         if self.flushing:
             raise ValueError(self.ER_FLUSHING)
 
         if self.startup:
             raise ValueError(self.ER_STARTUP)
 
@@ -356,20 +357,20 @@
                     del self.rows[cross['row_sequence']]
                     del self.crosses[media_sequence]
         elif self.delay_units == self.SECONDS:
             raise NotImplementedError()
 
         raise ValueError(self.ER_DELAY_UNITS.format(self.delay_units))
 
-    def recover_media_packet(
+    def recover_media_packet(  # pylint:disable=too-many-branches,too-many-statements
         self,
         media_sequence,
-        cross,
-        fec
-    ):  # pylint:disable=too-many-branches,too-many-locals,too-many-statements
+        cross: dict,
+        fec: FecPacket | None
+    ) -> None:
         """
         Recover a missing media packet helped by a FEC packet, this method is also called to
         register an incoming media packet if it is registered as missing.
         """
         recovered_by_fec = fec is not None
 
         # Read and remove "cross" it from the buffer
@@ -402,17 +403,16 @@
             aborted = False
             media_max = (fec.snbase + fec.na * fec.offset) & RtpPacket.S_MASK
             media_test = fec.snbase
             while media_test != media_max:
                 if media_test == media_sequence:
                     media_test = (media_test + fec.offset) & RtpPacket.S_MASK
                     continue
-                friend = self.medias[media_test]
                 # Unable to recover the media packet if any of the friend media packets is missing
-                if not friend:
+                if not (friend := self.medias[media_test]):
                     self.media_aborted_recovery += 1
                     aborted = True
                     break
                 media.payload_type ^= friend.payload_type
                 media.timestamp ^= friend.timestamp
                 payload_size ^= friend.payload_size
                 # TODO Optimize this
@@ -442,46 +442,42 @@
             fec_col.set_recovered(media_sequence)
         if fec_row:
             fec_row.set_recovered(media_sequence)
 
         if fec_col:
             if len(fec_col.missing) == 1:
                 # Cascade !
-                cascade_media_sequence = fec_col.missing[0]
-                if cascade_media_sequence:
-                    cascade_cross = self.crosses.get(cascade_media_sequence)
-                    if cascade_cross:
+                if cascade_media_sequence := fec_col.missing[0]:
+                    if cascade_cross := self.crosses.get(cascade_media_sequence):
                         self.recover_media_packet(cascade_media_sequence, cascade_cross, fec_col)
                     else:
                         raise NotImplementedError(
                             f'recover_media_packet({media_sequence}, {cross}, {fec}):{os.linesep}'
                             f'{self.ER_NULL_COL_CASCADE}{os.linesep}'
                             f'media sequence : {cascade_media_sequence}{os.linesep}'
                             f'{fec_col}{os.linesep}')
                 else:
                     raise NotImplementedError(self.ER_GET_COL_CASCADE.format(os.linesep, fec_col))
 
         if fec_row:
             if len(fec_row.missing) == 1:
                 # Cascade !
-                cascade_media_sequence = fec_row.missing[0]
-                if cascade_media_sequence:
-                    cascade_cross = self.crosses.get(cascade_media_sequence)
-                    if cascade_cross:
+                if cascade_media_sequence := fec_row.missing[0]:
+                    if cascade_cross := self.crosses.get(cascade_media_sequence):
                         self.recover_media_packet(cascade_media_sequence, cascade_cross, fec_row)
                     else:
                         raise NotImplementedError(
                             f'{self.ER_NULL_ROW_CASCADE}{os.linesep}'
                             f'recover_media_packet({media_sequence}, {cross}, {fec}):{os.linesep}'
                             f'media sequence : {cascade_media_sequence}{os.linesep}'
                             f'{fec_row}{os.linesep}')
                 else:
                     raise NotImplementedError(self.ER_GET_ROW_CASCADE.format(os.linesep, fec_row))
 
-    def out(self):
+    def out(self) -> None:
         """Extract packets to output in order to keep a 'certain' amount of them in the buffer."""
         units = self.PACKETS if self.flushing else self.delay_units
         value = 0 if self.flushing else self.delay_value
         lostogram_counter = 0
 
         # Extract packets to output in order to keep a 'certain' amount of them in the buffer
         if units == self.PACKETS:  # based on buffer size
@@ -490,28 +486,26 @@
                 if self.startup:
                     self.position = min(self.medias.keys()) & RtpPacket.S_MASK
                 else:
                     self.position = (self.position + 1) & RtpPacket.S_MASK
 
                 self.startup = False
 
-                media = self.medias.get(self.position)
-                if media:
+                if media := self.medias.get(self.position):
                     self.lostogram[lostogram_counter] += 1
                     lostogram_counter = 0
                     del self.medias[media.sequence]
                     if self.output:
                         self.output.write(media.payload)
                 else:
                     self.media_missing += 1
                     lostogram_counter += 1
 
                 # Remove any fec packet linked to current media packet
-                cross = self.crosses.get(self.position)
-                if cross:
+                if cross := self.crosses.get(self.position):
                     del self.crosses[self.position]
                     if cross['col_sequence'] and cross['col_sequence'] in self.cols:
                         del self.cols[cross['col_sequence']]
                     if cross['row_sequence'] and cross['row_sequence'] in self.rows:
                         del self.rows[cross['row_sequence']]
 
         # Extract packets to output in order to keep a 'certain' amount of them in the buffer
```

### Comparing `pytoolbox-14.4.0/pytoolbox/network/url.py` & `pytoolbox-14.5.0/pytoolbox/network/url.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/regex.py` & `pytoolbox-14.5.0/pytoolbox/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,17 @@
     >>> [embed_in_regex(s, r, i) for s, r, i in findall_partial('12:15:2', TIME_REGEX_PARTS)]
     [(0, '12:15:2[0-9]')]
     >>> [embed_in_regex(s, r, i) for s, r, i in findall_partial('18:2', TIME_REGEX_PARTS)]
     [(0, '18:2[0-9]:[0-5][0-9]'), (3, '[0-2][0-9]:18:2[0-9]')]
     >>> [embed_in_regex(s, r, i) for s, r, i in findall_partial('59:1', TIME_REGEX_PARTS)]
     [(3, '[0-2][0-9]:59:1[0-9]')]
     """
-    for index in range(0, len(regex_parts) - len(string) + 1):  # noqa
+    for index in range(0, len(regex_parts) - len(string) + 1):
         regex = regex_parts[index:index + len(string)]
-        match = re.search(''.join(regex), string)
-        if match:
+        if re.search(''.join(regex), string):
             yield string, regex_parts, index
 
 
 def from_path_patterns(patterns, regex=False):
     """
     Return patterns compiled to regular expressions, if necessary.
```

### Comparing `pytoolbox-14.4.0/pytoolbox/rest_framework/metadata/mixins.py` & `pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/mixins.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
-Mix-ins for building your own `Django REST Framework <https://github.com/tomchristie/django-rest-framework>`_
-powered API `metadata <https://github.com/tomchristie/django-rest-framework/blob/master/rest_framework/metadata.py>`_.
+Mix-ins for building your own
+`Django REST Framework <https://github.com/encode/django-rest-framework>`_ powered API
+`metadata <https://github.com/encode/django-rest-framework/blob/master/rest_framework/metadata.py>`_
+.
 """
 
 from rest_framework import serializers
 
 __all__ = ['ExcludeRelatedChoicesMixin']
```

### Comparing `pytoolbox-14.4.0/pytoolbox/rest_framework/serializers/fields.py` & `pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/rest_framework/serializers/mixins.py` & `pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
-Mix-ins for building your own `Django REST Framework <https://github.com/tomchristie/django-rest-framework>`_
-powered API `serializers <http://www.django-rest-framework.org/tutorial/1-serialization/>`_.
+Mix-ins for building your own Django REST Framework powered API serializers.
 """
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.encoding import smart_text
 from django.utils.translation import gettext_lazy as _
 
 from pytoolbox.django.models import utils
```

### Comparing `pytoolbox-14.4.0/pytoolbox/rest_framework/views/mixins.py` & `pytoolbox-14.5.0/pytoolbox/rest_framework/views/mixins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
-Mix-ins for building your own `Django REST Framework <https://github.com/tomchristie/django-rest-framework>`_
-powered API `views <http://www.django-rest-framework.org/tutorial/3-class-based-views/>`_.
+Mix-ins for building your own Django REST Framework powered API views.
 """
 
 from django.contrib.auth.views import redirect_to_login
 from rest_framework import renderers
 
 from pytoolbox import module
 
@@ -47,16 +46,16 @@
 
     redirected_classes = (renderers.BrowsableAPIRenderer, )
 
     def finalize_response(self, request, response, *args, **kwargs):
         response = super().finalize_response(request, response, *args, **kwargs)
         logged = request.user.is_authenticated
         if (
-            not (logged if isinstance(logged, bool) else logged()) and
-            isinstance(response.accepted_renderer, self.redirected_classes)
+            not (logged if isinstance(logged, bool) else logged())
+            and isinstance(response.accepted_renderer, self.redirected_classes)
         ):
             response = redirect_to_login(request.path)
             response.data = {}
         return response
 
 
 __all__ = _all.diff(globals())
```

### Comparing `pytoolbox-14.4.0/pytoolbox/selenium/client.py` & `pytoolbox-14.5.0/pytoolbox/selenium/client.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/selenium/common.py` & `pytoolbox-14.5.0/pytoolbox/selenium/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+# pylint:disable=no-member
+
 from . import exceptions
 
 __all__ = ['FindMixin']
 
 
 class FindMixin(object):
 
     @staticmethod
     def clean_elements(elements, criteria, force_list=False, fail=True):
         if elements:
             return elements if force_list or len(elements) > 1 else elements[0]
         if fail:
-            raise exceptions.NoSuchElementException(criteria)  # pylint:disable=no-member
+            raise exceptions.NoSuchElementException(criteria)
         return None
 
     def find_css(self, css_selector, prefix=True, force_list=False, fail=True):
         assert prefix  # Not implemented
         elements = self.find_elements_by_css_selector(css_selector)
         return self.clean_elements(elements, css_selector, force_list, fail)
```

### Comparing `pytoolbox-14.4.0/pytoolbox/selenium/test.py` & `pytoolbox-14.5.0/pytoolbox/selenium/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint:disable=no-member
+
 from . import client  # pylint:disable=unused-import
 
 __all__ = ['LiveTestCaseMixin']
 
 
 class LiveTestCaseMixin(object):
```

### Comparing `pytoolbox-14.4.0/pytoolbox/selenium/webdrivers.py` & `pytoolbox-14.5.0/pytoolbox/selenium/webdrivers.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/selenium/webelements/base.py` & `pytoolbox-14.5.0/pytoolbox/selenium/webelements/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,15 @@
         return value
 
     def get_attribute(self, name):
         value = super().get_attribute(name)
         return self.clean_value(value) if name == 'value' else value
 
     def _specialize(self):
-        component = self.get_attribute('data-component')
-        if component:
+        if component := self.get_attribute('data-component'):
             try:
                 self.__class__ = next(  # pylint: disable=invalid-class-object
                     c for c in type(self).__subclasses__() if c.component == component)
             except StopIteration:
                 self._specialize_default(component)
 
     @staticmethod
```

### Comparing `pytoolbox-14.4.0/pytoolbox/selenium/webelements/bootstrap_slider.py` & `pytoolbox-14.5.0/pytoolbox/selenium/webelements/bootstrap_slider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from pytoolbox.selenium import Keys
+# pylint:disable=no-member
+
+from pytoolbox.selenium import common, Keys
 
 __all__ = ['BootstrapSliderMixin']
 
 
-class BootstrapSliderMixin(object):
+class BootstrapSliderMixin(common.FindMixin):
 
     component = 'bootstrapSlider'
 
     @staticmethod
     def clean_value(value):
         return int(value)
```

### Comparing `pytoolbox-14.4.0/pytoolbox/serialization.py` & `pytoolbox-14.5.0/pytoolbox/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     """
     if makedirs:
         filesystem.makedirs(os.path.dirname(path))
     if backup:
         backup_path = f'{path}.bkp'
         try:
             shutil.copy2(path, backup_path)
-        except IOError as e:
-            if e.errno != errno.ENOENT:
+        except IOError as ex:
+            if ex.errno != errno.ENOENT:
                 raise
             backup_path = None
     write_path = f'{path}.tmp' if safe else path
     with open(write_path, 'wb' if binary else 'w') as f:
         if data is not None:
             f.write(data)
         if pickle_data is not None:
```

### Comparing `pytoolbox-14.4.0/pytoolbox/signals.py` & `pytoolbox-14.5.0/pytoolbox/signals.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 
 def propagate_handler(signum, frame):
     errors = {}
     for handler in reversed(handlers_by_signal[signum]):
         try:
             handler(signum, frame)
-        except Exception as e:  # pylint:disable=broad-except
-            errors[handler] = e
+        except Exception as ex:  # pylint:disable=broad-except
+            errors[handler] = ex
     if errors:
         raise RuntimeError(errors)
 
 
 def register_handler(signum, handler, append=True, reset=False):
     old_handler = signal.getsignal(signum)
     signal.signal(signum, propagate_handler)
```

### Comparing `pytoolbox-14.4.0/pytoolbox/states.py` & `pytoolbox-14.5.0/pytoolbox/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,15 @@
 
 
 class StateEnum(object, metaclass=StateEnumMetaclass):
 
     @classmethod
     def get(cls, name):
         if name.lower() == name:
-            name = name.upper()
-            if name in cls.ALL_STATES:
+            if (name := name.upper()) in cls.ALL_STATES:
                 return name
             return getattr(cls, name + '_STATES', None)
         return None
 
     @classmethod
     def get_transit_from(cls, state, auto_inverse=False):
         """
```

### Comparing `pytoolbox-14.4.0/pytoolbox/string.py` & `pytoolbox-14.5.0/pytoolbox/string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/subprocess.py` & `pytoolbox-14.5.0/pytoolbox/subprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from __future__ import annotations
+
+from collections.abc import Callable
 import errno, fcntl, grp, logging, multiprocessing, os, pwd, random, re
 import setuptools.archive_util, shlex, shutil, subprocess, threading, time
 
 from . import filesystem, module
 
 _all = module.All(globals())
 
@@ -19,19 +22,19 @@
 except ImportError:
     from pipes import quote
 
 
 def kill(process):
     try:
         process.kill()
-    except OSError as e:
-        if e.errno != errno.ESRCH:
+    except OSError as ex:
+        if ex.errno != errno.ESRCH:
             raise
-    except Exception as e:  # pylint:disable=broad-except
-        if not NoSuchProcess or not isinstance(e, NoSuchProcess):
+    except Exception as ex:  # pylint:disable=broad-except
+        if not NoSuchProcess or not isinstance(ex, NoSuchProcess):
             raise
 
 
 def su(user, group):  # pylint:disable=invalid-name
     """
     Return a function to change current user/group id.
 
@@ -54,16 +57,16 @@
 
 
 # http://stackoverflow.com/a/7730201/190597
 def read_async(fd):  # pylint:disable=invalid-name
     """Read some data from a file descriptor, ignoring EAGAIN errors."""
     try:
         return fd.read()
-    except IOError as e:
-        if e.errno == errno.EAGAIN:
+    except IOError as ex:
+        if ex.errno == errno.EAGAIN:
             return ''
         raise
 
 
 def to_args_list(args):
     if not args:
         return []
@@ -95,61 +98,51 @@
 
 
 # thanks http://stackoverflow.com/questions/1191374$
 def _communicate_with_timeout(*, data, process, input):  # pylint:disable=redefined-builtin
     data['stdout'], data['stderr'] = process.communicate(input=input)
 
 
-def cmd(  # pylint:disable=too-many-branches,too-many-locals,too-many-statements
-    command,
-    user=None,
-    input=None,  # pylint:disable=redefined-builtin
-    cli_input=None,
-    cli_output=False,
-    communicate=True,
-    timeout=None,
-    fail=True,
-    log=None,
-    tries=1,
-    delay_min=5,
-    delay_max=10,
+def cmd(  # pylint:disable=too-many-arguments,too-many-branches,too-many-locals,too-many-statements
+    command: str | list[str],
+    user: str | None = None,
+    input: str | None = None,  # pylint:disable=redefined-builtin
+    cli_input: str | None = None,
+    cli_output: bool = False,
+    communicate: bool = True,
+    timeout: float | None = None,
+    fail: bool = True,
+    log: Callable | logging.Logger | None = None,
+    tries: int = 1,
+    delay_min: float = 5,
+    delay_max: float = 10,
     **kwargs
 ):
     """
     Calls the `command` and returns a dictionary with process, stdout, stderr, and the returncode.
 
     Returned returncode, stdout and stderr will be None if `communicate` is set to False.
 
+    :param command: The command to execute.
     :param user: If set, this will use ``sudo -u <user> ...`` to execute `command` as `user`.
-    :type user: unicode
     :param input: If set, sended to stdin (if `communicate` is True).
-    :type input: unicode
     :param cli_input: If set, sended to stdin (no condition).
-    :type cli_input: unicode
     :param cli_output: Set to True to output (in real-time) stdout to stdout and stderr to stderr.
-    :type cli_output: bool
     :param fail: Set to False to avoid the exception `subprocess.CalledProcessError`.
-    :type fail: bool
     :param log: A function to log/print details about what is executed/any failure, can be a logger.
-    :type log: callable, logging.Logger
     :param communicate: Set to True to communicate with the process, this is a locking call
                         (if timeout is None).
-    :type communicate: bool
     :param timeout: Time-out for the communication with the process, in seconds.
-    :type timeout: float
     :param tries: How many times you want the command to be retried ?
-    :type tries: int
     :param delay_min: Minimum delay to sleep after every attempt communicate must be True.
-    :type delay: float, int
     :param delay_max: Maximum delay to sleep after every attempt communicate must be True.
-    :type delay: float, int
+    :param kwargs: Any argument of the :mod:`subprocess`.Popen constructor
+                   excepting stdin, stdout and stderr
 
-    * Delay will be a random number in range (`delay_min`, `delay_max`)
-    * Set kwargs with any argument of the :mod:`subprocess`.Popen constructor excepting
-      stdin, stdout and stderr.
+    The delay will be a random number in range (`delay_min`, `delay_max`).
 
     """
 
     # convert log argument to logging functions
     log_debug = log_warning = log_exception = None
     if isinstance(log, logging.Logger):
         log_debug, log_warning, log_exception = log.debug, log.warning, log.exception
@@ -180,21 +173,21 @@
         # create the sub-process
         try:
             process = Popen(
                 args_list,
                 stdin=subprocess.PIPE,
                 stdout=None if cli_output else subprocess.PIPE,
                 stderr=None if cli_output else subprocess.PIPE, **kwargs)
-        except OSError as e:
+        except OSError as ex:
             # unable to execute the program (e.g. does not exist)
             if log_exception:
-                log_exception(e)
+                log_exception(ex)
             if fail:
                 raise
-            return {'process': None, 'stdout': '', 'stderr': e, 'returncode': 2}
+            return {'process': None, 'stdout': '', 'stderr': ex, 'returncode': 2}
 
         # write to stdin (answer to questions, ...)
         if cli_input is not None:
             process.stdin.write(cli_input)
             process.stdin.flush()
 
         # interact with the process and wait for the process to terminate
@@ -206,18 +199,18 @@
                 kwargs={'data': data, 'input': input, 'process': process})
             thread.start()
             thread.join(timeout=timeout)
             if thread.is_alive():
                 try:
                     process.terminate()
                     thread.join()
-                except OSError as e:
+                except OSError as ex:
                     # Manage race condition with process that may terminate just after the call to
                     # thread.is_alive() !
-                    if e.errno != errno.ESRCH:
+                    if ex.errno != errno.ESRCH:
                         raise
             stdout, stderr = data['stdout'], data['stderr']
         else:
             # get a return code that may be None of course ...
             process.poll()
             stdout = stderr = None
 
@@ -311,15 +304,15 @@
     if remove_temporary:
         shutil.rmtree(path)
     return results
 
 
 # --------------------------------------------------------------------------------------------------
 
-def rsync(  # pylint:disable=too-many-locals
+def rsync(  # pylint:disable=too-many-arguments,too-many-locals
     source,
     destination,
     source_is_dir=False,
     destination_is_dir=False,
     makedest=False,
     archive=True,
     delete=False,
```

### Comparing `pytoolbox-14.4.0/pytoolbox/throttles.py` & `pytoolbox-14.5.0/pytoolbox/throttles.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/types.py` & `pytoolbox-14.5.0/pytoolbox/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     """
     value = init
     for base in cls.__mro__:
         value = merge_func(value, getattr(base, attr_name, default))
     return value
 
 
-class DummyObject(object):
+class DummyObject(object):  # pylint:disable=too-few-public-methods
     """
     Easy way to generate a dynamic object with the attributes defined at instantiation.
 
     **Example usage**
 
     >>> obj = DummyObject(foo=42, bar=None)
     >>> obj.foo
```

### Comparing `pytoolbox-14.4.0/pytoolbox/unittest.py` & `pytoolbox-14.5.0/pytoolbox/unittest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint:disable=no-member
+
 import functools, inspect, io, itertools, os, pprint, time, unittest
 
 from . import module
 from .multimedia import ffmpeg
 from .string import snake_to_camel
 from .types import Missing
 
@@ -258,15 +260,15 @@
     def assertIsMissing(self, value, *args, **kwargs):  # pylint:disable=invalid-name
         return self.assertIs(value, Missing, *args, **kwargs)
 
     def assertIsNotMissing(self, value, *args, **kwargs):  # pylint:disable=invalid-name
         return self.assertIsNot(value, Missing, *args, **kwargs)
 
 
-class SnakeCaseMixin(object):
+class SnakeCaseMixin(object):  # pylint:disable=too-few-public-methods
 
     def __getattr__(self, name):
         if name.lower() == name:
             attribute = snake_to_camel(name if name.startswith('assert_') else f'assert_{name}')
             return getattr(self, attribute)
         raise AttributeError
```

### Comparing `pytoolbox-14.4.0/pytoolbox/validation.py` & `pytoolbox-14.5.0/pytoolbox/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from . import module
 from .network.ip import ip_address
 from .private import InvalidId, ObjectId
 
 _all = module.All(globals())
 
 
-class CleanAttributesMixin(object):
+class CleanAttributesMixin(object):  # pylint:disable=too-few-public-methods
     """
     Put validation logic, cleanup code, ... into a method clean_<attribute_name> and this method
     will be called every time the attribute is set.
 
     **Example usage**
 
     >>> class Settings(CleanAttributesMixin):
@@ -30,21 +30,20 @@
     >>> assert isinstance(settings.locale, str)
     >>> settings = Settings(100, 'a string')
     Traceback (most recent call last):
         ...
     AssertionError
     """
     def __setattr__(self, name, value):
-        cleanup_method = getattr(self, 'clean_' + name, None)
-        if cleanup_method:
+        if cleanup_method := getattr(self, 'clean_' + name, None):
             value = cleanup_method(value)
         super().__setattr__(name, value)
 
 
-class StrongTypedMixin(object):
+class StrongTypedMixin(object):  # pylint:disable=too-few-public-methods
     """
     Annotate arguments of the class __init__ with types and then you'll get a class with type
     checking.
 
     **Example usage**
 
     >>> class Settings(StrongTypedMixin):
@@ -64,16 +63,15 @@
     >>> settings = Settings(locale=['en', 'fr'], broker={})
     >>> settings = Settings(locale=10, broker={})
     Traceback (most recent call last):
         ...
     AssertionError: Attribute locale must be set to an instance of (<class 'str'>, <class 'list'>)
     """
     def __setattr__(self, name, value):
-        the_type = self.__init__.__annotations__.get(name)
-        if the_type:
+        if the_type := self.__init__.__annotations__.get(name):
             default = inspect.signature(self.__init__).parameters[name].default
             if value != default:
                 assert isinstance(value, the_type), \
                     f'Attribute {name} must be set to an instance of {the_type}'
         super().__setattr__(name, value)
 
 
@@ -230,17 +228,17 @@
     if not url.netloc or scheme_mandatory and not url.scheme or port_mandatory and not url.port:
         return False
     if check_404:
         conn = http.client.HTTPConnection(url.netloc, url.port or default_port, timeout=timeout)
         try:
             conn.request('HEAD', url.path)
             return conn.getresponse().status != 404
-        except socket.error as e:
+        except socket.error as ex:
             # Resource does not exist
-            if isinstance(e, socket.timeout) or e.errno in excepted_errnos:
+            if isinstance(ex, socket.timeout) or ex.errno in excepted_errnos:
                 return False
             raise  # Re-raise exception if a different error occurred
         finally:
             conn.close()
     return True
```

### Comparing `pytoolbox-14.4.0/pytoolbox/virtualenv.py` & `pytoolbox-14.5.0/pytoolbox/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox/voluptuous.py` & `pytoolbox-14.5.0/pytoolbox/voluptuous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.4.0/pytoolbox.egg-info/PKG-INFO` & `pytoolbox-14.5.0/pytoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.4.0
+Version: 14.5.0
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
@@ -37,15 +37,15 @@
 Provides-Extra: smpte2022
 Provides-Extra: vision
 Provides-Extra: voluptuous
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE.rst
-License-File: AUTHORS
+License-File: AUTHORS.md
 
 =========
 Pytoolbox
 =========
 
 .. image:: https://badge.fury.io/py/pytoolbox.png
    :target: http://badge.fury.io/py/pytoolbox
@@ -155,14 +155,15 @@
 How to check coverage ?
 -----------------------
 
 ::
 
     $ source /some/python3/venv/bin/activate
     $ pip install -e .[all,test]
+    $ flake8 pytoolbox
     $ pytest
     $ xdg-open htmlcov/index.html
 
 Remarks:
 
 * All Django related modules are excluded from tests!
 * However I am using them with Django 1.8 up to 3.1.0.
```

### Comparing `pytoolbox-14.4.0/pytoolbox.egg-info/SOURCES.txt` & `pytoolbox-14.5.0/pytoolbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-AUTHORS
+AUTHORS.md
+CHANGELOG.md
 LICENSE.rst
 MANIFEST.in
 README.rst
-changelog.rst
 setup.cfg
 setup.py
 pytoolbox/__init__.py
 pytoolbox/argparse.py
 pytoolbox/atlassian.py
 pytoolbox/collections.py
 pytoolbox/comparison.py
@@ -147,8 +147,29 @@
 pytoolbox/selenium/exceptions.py
 pytoolbox/selenium/select.py
 pytoolbox/selenium/test.py
 pytoolbox/selenium/webdrivers.py
 pytoolbox/selenium/webelements/__init__.py
 pytoolbox/selenium/webelements/base.py
 pytoolbox/selenium/webelements/bootstrap_slider.py
-pytoolbox/selenium/webelements/bootstrap_switch.py
+pytoolbox/selenium/webelements/bootstrap_switch.py
+tests/test_argparse.py
+tests/test_collections.py
+tests/test_comparison.py
+tests/test_console.py
+tests/test_decorators.py
+tests/test_django_utils.py
+tests/test_exceptions.py
+tests/test_ffmpeg.py
+tests/test_filesystem.py
+tests/test_juju.py
+tests/test_module.py
+tests/test_private.py
+tests/test_serialization.py
+tests/test_signals.py
+tests/test_states.py
+tests/test_string.py
+tests/test_subprocess.py
+tests/test_types.py
+tests/test_unittest.py
+tests/test_validation.py
+tests/test_x264.py
```

### Comparing `pytoolbox-14.4.0/setup.py` & `pytoolbox-14.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 # **************************************************************************************************
 #                              PYTOOLBOX - TOOLBOX FOR PYTHON SCRIPTS
 #
 #  Main Developer : David Fischer (david.fischer.ch@gmail.com)
-#  Copyright      : Copyright (c) 2012-2020 David Fischer. All rights reserved.
+#  Copyright      : Copyright (c) 2012-2023 David Fischer. All rights reserved.
 #
 # **************************************************************************************************
 #
 # This file is part of David Fischer's pytoolbox Project.
 #
 # This project is free software: you can redistribute it and/or modify it under the terms of the
 # EUPL v. 1.1 as provided by the European Commission. This project is distributed in the hope that
@@ -19,17 +19,17 @@
 #
 # You should have received a copy of the EUPL General Public License along with this project.
 # If not, see he EUPL licence v1.1 is available in 22 languages:
 #     22-07-2013, <https://joinup.ec.europa.eu/software/page/eupl/licence-eupl>
 #
 # Retrieved from https://github.com/davidfischer-ch/pytoolbox.git
 
-import itertools, setuptools, subprocess, sys
 from pathlib import Path
 from setuptools.command import develop, install
+import itertools, setuptools, subprocess, sys
 
 import pytoolbox
 
 if sys.argv[-1] == 'test':
     sys.exit('Run pytest instead.')
 
 install_requires = [
@@ -134,23 +134,25 @@
 extras_require.update({
     'all': sorted(set(itertools.chain.from_iterable(extras_require.values()))),
     'doc': [
         'sphinx>=1.3.1',
         'sphinx_rtd_theme'
     ],
     'test': [
-        'coverage>=6.4.4<7',       # 01-09-2022 Released 16-08-2022
-        'flake8>=4,<5',            # 01-09-2022 Released 11-10-2021
-                                   # Bug https://github.com/tholo/pytest-flake8/issues/87
-                                   # Fix https://github.com/tholo/pytest-flake8/pull/88/files
-        'pylint>=2.15.0<3',        # 01-09-2022 Released 26-08-2022
-        'pytest>=7.1.2<8',         # 01-09-2022 Released 23-04-2022
-        'pytest-cov>=3.0.0<4',     # 01-09-2022 Released 04-10-2021
-        'pytest-flake8>=1.1.1<2',  # 01-09-2022 Released 18-03-2022
-        'pytest-pylint>=0.18.0<1'  # 01-09-2022 Released 09-11-2020
+        'coverage>=7.2.7,<8',        # 07-06-2023 Released 29-05-2023
+        'flake8>=6,<7',              # 07-06-2023 Released 23-11-2022
+        'pylint>=2.17.4,<3',         # 07-06-2023 Released 06-05-2023
+        'pytest>=7.3.1,<8',          # 07-06-2023 Released 14-04-2023
+        'pytest-cov>=4.1.0,<5',      # 07-06-2023 Released 24-05-2023
+        'pytest-pylint>=0.19.0,<1',  # 07-06-2023 Released 10-09-2022
+
+         # 07-06-2023 Bug still not resolved
+         # Bug https://github.com/tholo/pytest-flake8/issues/87
+         # Fix https://github.com/tholo/pytest-flake8/pull/88/files
+         # 'pytest-flake8'
     ]
 })
 
 
 def get_command_with_extras(cls):
 
     class WithExtra(cls):
```

