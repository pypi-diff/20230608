# Comparing `tmp/pytoolbox-14.5.0.tar.gz` & `tmp/pytoolbox-14.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoolbox-14.5.0.tar", last modified: Wed Jun  7 22:11:06 2023, max compression
+gzip compressed data, was "pytoolbox-14.5.1.tar", last modified: Thu Jun  8 10:21:28 2023, max compression
```

## Comparing `pytoolbox-14.5.0.tar` & `pytoolbox-14.5.1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/
--rw-rw-r--   0 david     (1000) david     (1000)      208 2023-06-07 22:02:37.000000 pytoolbox-14.5.0/AUTHORS.md
--rw-rw-r--   0 david     (1000) david     (1000)    27931 2023-06-07 22:08:36.000000 pytoolbox-14.5.0/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)     5747 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/LICENSE.rst
--rw-rw-r--   0 david     (1000) david     (1000)       27 2023-06-07 22:02:59.000000 pytoolbox-14.5.0/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     7617 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     6034 2023-06-07 22:09:15.000000 pytoolbox-14.5.0/README.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/
--rw-rw-r--   0 david     (1000) david     (1000)       23 2023-06-07 22:09:59.000000 pytoolbox-14.5.0/pytoolbox/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/face/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/
--rw-rw-r--   0 david     (1000) david     (1000)       67 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8907 2023-06-07 20:22:05.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/dlib.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/
--rw-rw-r--   0 david     (1000) david     (1000)       97 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11379 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py
--rw-rw-r--   0 david     (1000) david     (1000)      603 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/ai/vision/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     3213 2023-06-07 15:17:33.000000 pytoolbox-14.5.0/pytoolbox/argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1703 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/atlassian.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/aws/
--rw-rw-r--   0 david     (1000) david     (1000)       35 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/aws/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2716 2023-06-07 17:56:24.000000 pytoolbox-14.5.0/pytoolbox/aws/s3.py
--rw-rw-r--   0 david     (1000) david     (1000)    10233 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     3826 2023-06-07 17:29:11.000000 pytoolbox-14.5.0/pytoolbox/comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)     5380 2023-06-07 17:33:45.000000 pytoolbox-14.5.0/pytoolbox/console.py
--rw-rw-r--   0 david     (1000) david     (1000)     5749 2023-06-07 17:52:13.000000 pytoolbox-14.5.0/pytoolbox/crypto.py
--rw-rw-r--   0 david     (1000) david     (1000)    10583 2023-06-07 17:59:59.000000 pytoolbox-14.5.0/pytoolbox/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)     4457 2023-06-07 19:19:11.000000 pytoolbox-14.5.0/pytoolbox/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/core/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/core/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       77 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/core/constants.py
--rw-rw-r--   0 david     (1000) david     (1000)     2592 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/core/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     2541 2023-06-07 14:42:58.000000 pytoolbox-14.5.0/pytoolbox/django/core/validators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/forms/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/forms/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      693 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      528 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     5314 2023-06-07 14:44:46.000000 pytoolbox-14.5.0/pytoolbox/django/forms/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     3518 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      752 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/forms/widgets.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      377 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/fields/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/models/fields/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4116 2023-06-07 14:44:04.000000 pytoolbox-14.5.0/pytoolbox/django/models/fields/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1264 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/fields/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/managers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/managers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      738 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/managers/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      433 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/metaclass.py
--rw-rw-r--   0 david     (1000) david     (1000)    15157 2023-06-07 17:58:01.000000 pytoolbox-14.5.0/pytoolbox/django/models/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox/django/models/query/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/query/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2555 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/models/query/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1484 2023-06-07 17:58:17.000000 pytoolbox-14.5.0/pytoolbox/django/models/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/signals/
--rw-rw-r--   0 david     (1000) david     (1000)       64 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/signals/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      505 2023-06-07 14:38:31.000000 pytoolbox-14.5.0/pytoolbox/django/signals/dispatch.py
--rw-rw-r--   0 david     (1000) david     (1000)     3745 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/signals/handlers.py
--rw-rw-r--   0 david     (1000) david     (1000)     1390 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/storage.py
--rw-rw-r--   0 david     (1000) david     (1000)    10640 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/templatetags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/test/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4761 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/test/runner/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/runner/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      843 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/test/runner/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      579 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/urls.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/utils/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/utils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2339 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/utils/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     1624 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/utils/logging.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django/views/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/django/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      476 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/views/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     4892 2023-06-07 17:58:25.000000 pytoolbox-14.5.0/pytoolbox/django/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      282 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django/views/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_datatable_view/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_datatable_view/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1732 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_filter/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_filter/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_filter/filterset/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_filter/filterset/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      718 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_filter/filterset/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_formtools/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_formtools/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/django_formtools/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_formtools/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3056 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/django_formtools/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1448 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/enum.py
--rw-rw-r--   0 david     (1000) david     (1000)     3639 2023-06-07 17:52:48.000000 pytoolbox-14.5.0/pytoolbox/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    21371 2023-06-07 19:22:04.000000 pytoolbox-14.5.0/pytoolbox/filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     3096 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/flask.py
--rw-rw-r--   0 david     (1000) david     (1000)     6177 2023-06-07 19:22:27.000000 pytoolbox-14.5.0/pytoolbox/humanize.py
--rw-rw-r--   0 david     (1000) david     (1000)     2272 2023-06-07 19:30:05.000000 pytoolbox-14.5.0/pytoolbox/itertools.py
--rw-rw-r--   0 david     (1000) david     (1000)    49285 2023-06-07 19:46:20.000000 pytoolbox-14.5.0/pytoolbox/juju.py
--rw-rw-r--   0 david     (1000) david     (1000)      936 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/linux.py
--rw-rw-r--   0 david     (1000) david     (1000)     3720 2023-06-07 19:53:25.000000 pytoolbox-14.5.0/pytoolbox/logging.py
--rw-rw-r--   0 david     (1000) david     (1000)      322 2023-06-07 19:31:43.000000 pytoolbox-14.5.0/pytoolbox/module.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/exif/
--rw-rw-r--   0 david     (1000) david     (1000)      344 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1593 2023-06-07 20:32:28.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/brand.py
--rw-rw-r--   0 david     (1000) david     (1000)      530 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/camera.py
--rw-rw-r--   0 david     (1000) david     (1000)     1021 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/equipment.py
--rw-rw-r--   0 david     (1000) david     (1000)     1664 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/image.py
--rw-rw-r--   0 david     (1000) david     (1000)      740 2023-06-07 18:06:30.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/lens.py
--rw-rw-r--   0 david     (1000) david     (1000)     2180 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/metadata.py
--rw-rw-r--   0 david     (1000) david     (1000)     1069 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/photo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3811 2023-06-07 20:36:20.000000 pytoolbox-14.5.0/pytoolbox/multimedia/exif/tag.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/
--rw-rw-r--   0 david     (1000) david     (1000)      235 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7221 2023-06-07 20:56:06.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/encode.py
--rw-rw-r--   0 david     (1000) david     (1000)     5617 2023-06-07 19:17:58.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)     8291 2023-06-07 17:58:50.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffprobe.py
--rw-rw-r--   0 david     (1000) david     (1000)     6987 2023-06-07 20:56:16.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py
--rw-rw-r--   0 david     (1000) david     (1000)     1401 2023-06-07 18:05:36.000000 pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/multimedia/image/
--rw-rw-r--   0 david     (1000) david     (1000)     2233 2023-06-07 17:58:12.000000 pytoolbox-14.5.0/pytoolbox/multimedia/image/PIL.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/image/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1663 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/multimedia/x264.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/network/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7006 2023-06-07 19:15:02.000000 pytoolbox-14.5.0/pytoolbox/network/http.py
--rw-rw-r--   0 david     (1000) david     (1000)     1115 2023-06-07 17:58:57.000000 pytoolbox-14.5.0/pytoolbox/network/ip.py
--rw-rw-r--   0 david     (1000) david     (1000)    15618 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/rtp.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/network/smpte2022/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    27680 2023-06-07 20:38:57.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/base.py
--rw-rw-r--   0 david     (1000) david     (1000)    10383 2023-06-07 20:42:14.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/generator.py
--rw-rw-r--   0 david     (1000) david     (1000)    27905 2023-06-07 20:56:35.000000 pytoolbox-14.5.0/pytoolbox/network/smpte2022/receiver.py
--rw-rw-r--   0 david     (1000) david     (1000)      925 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/network/url.py
--rw-rw-r--   0 david     (1000) david     (1000)      479 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/pandas.py
--rw-rw-r--   0 david     (1000) david     (1000)      370 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/private.py
--rw-rw-r--   0 david     (1000) david     (1000)     3069 2023-06-07 19:51:38.000000 pytoolbox-14.5.0/pytoolbox/regex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 14:26:46.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1075 2023-06-07 14:42:00.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      682 2023-06-07 14:48:10.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/permissions.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      742 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     2203 2023-06-07 14:48:30.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/rest_framework/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1536 2023-06-07 14:48:58.000000 pytoolbox-14.5.0/pytoolbox/rest_framework/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/selenium/
--rw-rw-r--   0 david     (1000) david     (1000)      113 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3042 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/client.py
--rw-rw-r--   0 david     (1000) david     (1000)     1137 2023-06-07 19:25:15.000000 pytoolbox-14.5.0/pytoolbox/selenium/common.py
--rw-rw-r--   0 david     (1000) david     (1000)      428 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)      230 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/select.py
--rw-rw-r--   0 david     (1000) david     (1000)     2563 2023-06-07 19:27:45.000000 pytoolbox-14.5.0/pytoolbox/selenium/test.py
--rw-rw-r--   0 david     (1000) david     (1000)      779 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/webdrivers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/pytoolbox/selenium/webelements/
--rw-rw-r--   0 david     (1000) david     (1000)      150 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1073 2023-06-07 17:39:23.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      994 2023-06-07 19:26:22.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/bootstrap_slider.py
--rw-rw-r--   0 david     (1000) david     (1000)      473 2023-06-07 19:29:01.000000 pytoolbox-14.5.0/pytoolbox/selenium/webelements/bootstrap_switch.py
--rw-rw-r--   0 david     (1000) david     (1000)    19719 2023-06-07 17:55:15.000000 pytoolbox-14.5.0/pytoolbox/serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)      410 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/setuptools.py
--rw-rw-r--   0 david     (1000) david     (1000)     1373 2023-06-07 17:55:23.000000 pytoolbox-14.5.0/pytoolbox/signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     2506 2023-06-07 19:48:35.000000 pytoolbox-14.5.0/pytoolbox/states.py
--rw-rw-r--   0 david     (1000) david     (1000)     4513 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/string.py
--rw-rw-r--   0 david     (1000) david     (1000)    13946 2023-06-07 20:57:00.000000 pytoolbox-14.5.0/pytoolbox/subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)     3381 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/throttles.py
--rw-rw-r--   0 david     (1000) david     (1000)     7808 2023-06-07 19:47:09.000000 pytoolbox-14.5.0/pytoolbox/types.py
--rw-rw-r--   0 david     (1000) david     (1000)    10314 2023-06-07 17:48:00.000000 pytoolbox-14.5.0/pytoolbox/unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)     8945 2023-06-07 20:19:20.000000 pytoolbox-14.5.0/pytoolbox/validation.py
--rw-rw-r--   0 david     (1000) david     (1000)     1169 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/virtualenv.py
--rw-rw-r--   0 david     (1000) david     (1000)     2118 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/pytoolbox/voluptuous.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.670008 pytoolbox-14.5.0/pytoolbox.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     7617 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5436 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      827 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       10 2023-06-07 22:11:06.000000 pytoolbox-14.5.0/pytoolbox.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-07 22:11:06.678008 pytoolbox-14.5.0/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     8067 2023-06-07 15:14:14.000000 pytoolbox-14.5.0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-07 22:11:06.674008 pytoolbox-14.5.0/tests/
--rw-rw-r--   0 david     (1000) david     (1000)      959 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1193 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     4605 2023-06-07 15:32:54.000000 pytoolbox-14.5.0/tests/test_comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)      772 2023-06-07 14:38:27.000000 pytoolbox-14.5.0/tests/test_console.py
--rw-rw-r--   0 david     (1000) david     (1000)      416 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)      624 2023-06-07 15:33:50.000000 pytoolbox-14.5.0/tests/test_django_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      909 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    17588 2023-06-07 15:33:08.000000 pytoolbox-14.5.0/tests/test_ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)      983 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     2843 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_juju.py
--rw-rw-r--   0 david     (1000) david     (1000)      677 2023-06-07 15:33:10.000000 pytoolbox-14.5.0/tests/test_module.py
--rw-rw-r--   0 david     (1000) david     (1000)      632 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_private.py
--rw-rw-r--   0 david     (1000) david     (1000)     1629 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)     2563 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     4025 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_states.py
--rw-rw-r--   0 david     (1000) david     (1000)     2805 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_string.py
--rw-rw-r--   0 david     (1000) david     (1000)     4121 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)      294 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_types.py
--rw-rw-r--   0 david     (1000) david     (1000)     5699 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)      577 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_validation.py
--rw-rw-r--   0 david     (1000) david     (1000)      389 2023-06-07 08:19:48.000000 pytoolbox-14.5.0/tests/test_x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:28.055742 pytoolbox-14.5.1/
+-rw-rw-r--   0 david     (1000) david     (1000)      208 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/AUTHORS.md
+-rw-rw-r--   0 david     (1000) david     (1000)    28118 2023-06-08 09:51:38.000000 pytoolbox-14.5.1/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5747 2021-09-17 11:12:53.000000 pytoolbox-14.5.1/LICENSE.rst
+-rw-rw-r--   0 david     (1000) david     (1000)       27 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     7617 2023-06-08 10:21:28.055742 pytoolbox-14.5.1/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     6034 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/
+-rw-rw-r--   0 david     (1000) david     (1000)       23 2023-06-08 09:51:49.000000 pytoolbox-14.5.1/pytoolbox/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/ai/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:53.000000 pytoolbox-14.5.1/pytoolbox/ai/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/ai/vision/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/ai/vision/face/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/face/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/ai/vision/face/detect/
+-rw-rw-r--   0 david     (1000) david     (1000)       67 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/face/detect/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8907 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/face/detect/dlib.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/ai/vision/face/recognize/
+-rw-rw-r--   0 david     (1000) david     (1000)       97 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/face/recognize/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11379 2021-09-17 13:29:02.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/face/recognize/nn4_small2.py
+-rw-rw-r--   0 david     (1000) david     (1000)      603 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/ai/vision/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3213 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1703 2021-09-17 13:29:02.000000 pytoolbox-14.5.1/pytoolbox/atlassian.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/aws/
+-rw-rw-r--   0 david     (1000) david     (1000)       35 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/aws/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2716 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/aws/s3.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10233 2022-09-09 14:04:01.000000 pytoolbox-14.5.1/pytoolbox/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4127 2023-06-08 09:46:56.000000 pytoolbox-14.5.1/pytoolbox/comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5380 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/console.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5749 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/crypto.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10583 2021-09-17 13:29:02.000000 pytoolbox-14.5.1/pytoolbox/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4457 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/core/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/core/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       77 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/core/constants.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2592 2021-10-21 14:44:55.000000 pytoolbox-14.5.1/pytoolbox/django/core/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2541 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/core/validators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/forms/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/forms/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      693 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/forms/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      528 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/forms/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5314 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/forms/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3518 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/forms/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      752 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/forms/widgets.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/models/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      377 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1623 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/models/fields/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/models/fields/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4116 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/models/fields/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1264 2022-02-28 12:49:16.000000 pytoolbox-14.5.1/pytoolbox/django/models/fields/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/models/managers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/managers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      738 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/managers/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/metaclass.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15157 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/models/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/models/query/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/query/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2555 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/models/query/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1484 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/models/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/signals/
+-rw-rw-r--   0 david     (1000) david     (1000)       64 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/signals/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      505 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/signals/dispatch.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3745 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/signals/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1390 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/storage.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10640 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/templatetags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4761 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/test/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox/django/test/runner/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/test/runner/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      843 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/test/runner/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      579 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/urls.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.887791 pytoolbox-14.5.1/pytoolbox/django/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2339 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/utils/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1624 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/utils/logging.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.931779 pytoolbox-14.5.1/pytoolbox/django/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      476 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/views/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4892 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/django/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      282 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django/views/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.931779 pytoolbox-14.5.1/pytoolbox/django_datatable_view/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_datatable_view/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.931779 pytoolbox-14.5.1/pytoolbox/django_datatable_view/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_datatable_view/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1732 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_datatable_view/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.931779 pytoolbox-14.5.1/pytoolbox/django_filter/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_filter/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.931779 pytoolbox-14.5.1/pytoolbox/django_filter/filterset/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_filter/filterset/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      718 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_filter/filterset/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.939776 pytoolbox-14.5.1/pytoolbox/django_formtools/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_formtools/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.943775 pytoolbox-14.5.1/pytoolbox/django_formtools/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_formtools/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3056 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/django_formtools/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1448 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/enum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3639 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21371 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3096 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/flask.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6177 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/humanize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2272 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/itertools.py
+-rw-rw-r--   0 david     (1000) david     (1000)    49285 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)      936 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/pytoolbox/linux.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3720 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/logging.py
+-rw-rw-r--   0 david     (1000) david     (1000)      322 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/module.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.943775 pytoolbox-14.5.1/pytoolbox/multimedia/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.951773 pytoolbox-14.5.1/pytoolbox/multimedia/exif/
+-rw-rw-r--   0 david     (1000) david     (1000)      344 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1593 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/brand.py
+-rw-rw-r--   0 david     (1000) david     (1000)      530 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/camera.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1021 2021-09-17 13:29:02.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/equipment.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1664 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/image.py
+-rw-rw-r--   0 david     (1000) david     (1000)      740 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/lens.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2180 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/metadata.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1069 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/photo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3811 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/exif/tag.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.955772 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/
+-rw-rw-r--   0 david     (1000) david     (1000)      235 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7221 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/encode.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5617 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8291 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/ffprobe.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6987 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/miscellaneous.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1401 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.959770 pytoolbox-14.5.1/pytoolbox/multimedia/image/
+-rw-rw-r--   0 david     (1000) david     (1000)     2233 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/multimedia/image/PIL.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/image/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1663 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/multimedia/x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.967768 pytoolbox-14.5.1/pytoolbox/network/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/network/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7006 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/network/http.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1115 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/network/ip.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15618 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/network/rtp.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.967768 pytoolbox-14.5.1/pytoolbox/network/smpte2022/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/network/smpte2022/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27680 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/network/smpte2022/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10383 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/network/smpte2022/generator.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27905 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/network/smpte2022/receiver.py
+-rw-rw-r--   0 david     (1000) david     (1000)      925 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/network/url.py
+-rw-rw-r--   0 david     (1000) david     (1000)      479 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/pandas.py
+-rw-rw-r--   0 david     (1000) david     (1000)      370 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3069 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/regex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.971767 pytoolbox-14.5.1/pytoolbox/rest_framework/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.971767 pytoolbox-14.5.1/pytoolbox/rest_framework/metadata/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/metadata/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1075 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/metadata/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      682 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/permissions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.975766 pytoolbox-14.5.1/pytoolbox/rest_framework/serializers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      742 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/serializers/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2203 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/serializers/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.979765 pytoolbox-14.5.1/pytoolbox/rest_framework/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1536 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/rest_framework/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.995760 pytoolbox-14.5.1/pytoolbox/selenium/
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/selenium/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3042 2021-09-17 13:29:02.000000 pytoolbox-14.5.1/pytoolbox/selenium/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1137 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/selenium/common.py
+-rw-rw-r--   0 david     (1000) david     (1000)      428 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/selenium/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)      230 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/selenium/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2563 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/selenium/test.py
+-rw-rw-r--   0 david     (1000) david     (1000)      779 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/selenium/webdrivers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.999759 pytoolbox-14.5.1/pytoolbox/selenium/webelements/
+-rw-rw-r--   0 david     (1000) david     (1000)      150 2021-09-17 11:12:54.000000 pytoolbox-14.5.1/pytoolbox/selenium/webelements/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1073 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/selenium/webelements/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      994 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/selenium/webelements/bootstrap_slider.py
+-rw-rw-r--   0 david     (1000) david     (1000)      473 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/selenium/webelements/bootstrap_switch.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19719 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)      410 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/pytoolbox/setuptools.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1373 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2506 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4513 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/pytoolbox/string.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13946 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3381 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/pytoolbox/throttles.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7808 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10314 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8945 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/pytoolbox/validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1169 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/pytoolbox/virtualenv.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2118 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/pytoolbox/voluptuous.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:27.735835 pytoolbox-14.5.1/pytoolbox.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     7617 2023-06-08 10:21:26.000000 pytoolbox-14.5.1/pytoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5436 2023-06-08 10:21:27.000000 pytoolbox-14.5.1/pytoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-08 10:21:26.000000 pytoolbox-14.5.1/pytoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      827 2023-06-08 10:21:26.000000 pytoolbox-14.5.1/pytoolbox.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2023-06-08 10:21:26.000000 pytoolbox-14.5.1/pytoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2023-06-08 10:21:28.055742 pytoolbox-14.5.1/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     8067 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-08 10:21:28.055742 pytoolbox-14.5.1/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)      959 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/tests/test_argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1193 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4605 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/tests/test_comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)      772 2023-02-03 07:19:19.000000 pytoolbox-14.5.1/tests/test_console.py
+-rw-rw-r--   0 david     (1000) david     (1000)      416 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      624 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/tests/test_django_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      909 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17588 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/tests/test_ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)      983 2022-09-09 13:16:43.000000 pytoolbox-14.5.1/tests/test_filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2843 2022-09-09 13:16:31.000000 pytoolbox-14.5.1/tests/test_juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)      677 2023-06-08 07:35:27.000000 pytoolbox-14.5.1/tests/test_module.py
+-rw-rw-r--   0 david     (1000) david     (1000)      632 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1629 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2563 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/tests/test_signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4025 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2805 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_string.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4121 2022-09-09 13:15:51.000000 pytoolbox-14.5.1/tests/test_subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)      294 2022-09-09 13:36:33.000000 pytoolbox-14.5.1/tests/test_types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5699 2022-08-24 13:26:15.000000 pytoolbox-14.5.1/tests/test_unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)      577 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      389 2021-09-17 11:12:55.000000 pytoolbox-14.5.1/tests/test_x264.py
```

### Comparing `pytoolbox-14.5.0/CHANGELOG.md` & `pytoolbox-14.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 Roadmap ? Not so, but you can check this: https://github.com/davidfischer-ch/pytoolbox/issues
 
+## v14.5.1 (2023-06-08)
+
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.5.0...14.5.1
+
+### Fix and enhancements
+
+- Make code compatible with legacy versions of `packaging`
+
 ## v14.5.0 (2023-06-07)
 
-Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.5.0...14.4.0
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.4.0...14.5.0
 
 ### Minor compatibility breaks
 
 - Bye bye Django 3 and less
 
 ### Features
 
@@ -19,15 +27,15 @@
 - Usage of `super()` magic
 - Upgrade testing stack especially pylint with its dozen tests
 - Apply recommendations from linters (or silent it...)
 - Convert Changelog and Authors in Markdown
 
 ## v14.4.0 (2022-12-09)
 
-Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.4.0...14.3.0
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.3.0...14.4.0
 
 ### Minor compatibility breaks
 
 - Replace `comparison.parse_version` by `comparison.try_parse_version` with a fallback behavior
 
 ### Features
 
@@ -38,15 +46,15 @@
 ## Fix and enhancements
 
 - Compatibility with latest Django releases
 - Compatibility with latest `packaging` module (`LegacyVersion` was dropped)
 
 ## v14.3.0 (2022-09-09)
 
-Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.3.0...14.2.0
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.2.0...14.3.0
 
 ### Minor compatibility breaks
 
 - Drop Python 3.7 & 3.8 compatibility
 - Drop `logging` extra (`termcolor` is now installed by default)
 
 ### Features
@@ -54,15 +62,15 @@
 - Add [types.merge_annotations` class decorator
 - Module `comparison`: Add [unified_diff`,
     [compare_versions` and
     [satisfy_version_constraints`
 
 ## v14.2.0 (2022-06-10)
 
-Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.2.0...14.1.0
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.1.0...14.2.0
 
 ### Minor compatibility breaks
 
 - Drop Python 3.6 compatibility
 - Function `filesystem.from_template`: Make Jinja2 template strict with undefined values
 - Module `argparse`: Return `pathlib.Path` instead of `str` (See commit 6acf8d13e2739a6e564b325bc035e33676c9ff07)
 
@@ -74,15 +82,15 @@
 
 - Convert some FIXMEs to TODOs
 - Ensure Python 3.10 compatibility
 - Fix many linter issues
 
 ## v14.1.0
 
-Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.1.0...14.0.2
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.0.2...14.1.0
 
 ### Minor compatibility breaks
 
 - Module `dango.models.fields`: Apply `NullifyMixin` to `StripCharField` and `StripTextField`
 
 ### Features
 
@@ -91,15 +99,15 @@
 ## Fix and enhancements
 
 - Module `django.signals`: Fix `strip_strings_and_validate_model` not importable from `django.signals`
 - Module `django.models.fields`: Fix `StripMixin` not fair play with inheritance
 
 ## v14.0.2
 
-Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.0.0...14.0.1
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.0.1...14.0.2
 
 ## Fix and enhancements
 
 - Fix Django deprecation warning (`ugettext_lazy` -> `gettext_lazy`)
 
 ## v14.0.1
```

### Comparing `pytoolbox-14.5.0/LICENSE.rst` & `pytoolbox-14.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/PKG-INFO` & `pytoolbox-14.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.5.0
+Version: 14.5.1
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytoolbox-14.5.0/README.rst` & `pytoolbox-14.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/ai/vision/face/detect/dlib.py` & `pytoolbox-14.5.1/pytoolbox/ai/vision/face/detect/dlib.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/ai/vision/face/recognize/nn4_small2.py` & `pytoolbox-14.5.1/pytoolbox/ai/vision/face/recognize/nn4_small2.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/ai/vision/utils.py` & `pytoolbox-14.5.1/pytoolbox/ai/vision/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/argparse.py` & `pytoolbox-14.5.1/pytoolbox/argparse.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/atlassian.py` & `pytoolbox-14.5.1/pytoolbox/atlassian.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/aws/s3.py` & `pytoolbox-14.5.1/pytoolbox/aws/s3.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/collections.py` & `pytoolbox-14.5.1/pytoolbox/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/comparison.py` & `pytoolbox-14.5.1/pytoolbox/comparison.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,22 @@
 
 VERSION_OPERATIONS: dict = {  # pylint:disable=consider-using-namedtuple-or-dataclass
     Version: {'<': op.lt, '<=': op.le, '==': op.eq, '!=': op.ne, '>=': op.ge, '>': op.gt},
     str: {'<': _nen, '<=': _eqn, '==': op.eq, '!=': op.ne, '>=': _eqn, '>': _nen}
 }
 
 
+try:
+    from packaging.version import LegacyVersion
+    VERSION_OPERATIONS[LegacyVersion] = VERSION_OPERATIONS[str]
+    ParseVersionTypes = 'str | Version | LegacyVersion'  # pylint:disable=invalid-name
+except ImportError:
+    ParseVersionTypes = 'str | Version'  # pylint:disable=invalid-name
+
+
 def compare_versions(
     a: str,  # pylint:disable=invalid-name
     b: str,  # pylint:disable=invalid-name
     operator: str
 ) -> bool | None:
     version_a = try_parse_version(a)
     version_b = try_parse_version(b)
@@ -113,12 +121,12 @@
     True
     >>> satisfy_version_constraints(None, ['!= master'], default='master')
     False
     """
     return all(compare_versions(version or default, *c.split(' ')[::-1]) for c in constraints or [])
 
 
-def try_parse_version(version: str) -> Version | str:
+def try_parse_version(version: str) -> ParseVersionTypes:
     try:
         return _parse_version(version)
     except InvalidVersion:
         return version
```

### Comparing `pytoolbox-14.5.0/pytoolbox/console.py` & `pytoolbox-14.5.1/pytoolbox/console.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/crypto.py` & `pytoolbox-14.5.1/pytoolbox/crypto.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/datetime.py` & `pytoolbox-14.5.1/pytoolbox/datetime.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/decorators.py` & `pytoolbox-14.5.1/pytoolbox/decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/core/exceptions.py` & `pytoolbox-14.5.1/pytoolbox/django/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/core/validators.py` & `pytoolbox-14.5.1/pytoolbox/django/core/validators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/forms/base.py` & `pytoolbox-14.5.1/pytoolbox/django/forms/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/forms/fields.py` & `pytoolbox-14.5.1/pytoolbox/django/forms/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/forms/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/forms/utils.py` & `pytoolbox-14.5.1/pytoolbox/django/forms/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/forms/widgets.py` & `pytoolbox-14.5.1/pytoolbox/django/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/decorators.py` & `pytoolbox-14.5.1/pytoolbox/django/models/decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/fields/base.py` & `pytoolbox-14.5.1/pytoolbox/django/models/fields/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/fields/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/models/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/managers/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/models/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/models/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/query/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/models/query/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/models/utils.py` & `pytoolbox-14.5.1/pytoolbox/django/models/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/signals/handlers.py` & `pytoolbox-14.5.1/pytoolbox/django/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/storage.py` & `pytoolbox-14.5.1/pytoolbox/django/storage.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/templatetags.py` & `pytoolbox-14.5.1/pytoolbox/django/templatetags.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/test/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/test/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/test/runner/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/test/runner/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/urls.py` & `pytoolbox-14.5.1/pytoolbox/django/urls.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/utils/collections.py` & `pytoolbox-14.5.1/pytoolbox/django/utils/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/utils/logging.py` & `pytoolbox-14.5.1/pytoolbox/django/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django/views/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django_datatable_view/views/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django_datatable_view/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django_filter/filterset/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django_filter/filterset/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/django_formtools/views/mixins.py` & `pytoolbox-14.5.1/pytoolbox/django_formtools/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/enum.py` & `pytoolbox-14.5.1/pytoolbox/enum.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/exceptions.py` & `pytoolbox-14.5.1/pytoolbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/filesystem.py` & `pytoolbox-14.5.1/pytoolbox/filesystem.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/flask.py` & `pytoolbox-14.5.1/pytoolbox/flask.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/humanize.py` & `pytoolbox-14.5.1/pytoolbox/humanize.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/itertools.py` & `pytoolbox-14.5.1/pytoolbox/itertools.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/juju.py` & `pytoolbox-14.5.1/pytoolbox/juju.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/linux.py` & `pytoolbox-14.5.1/pytoolbox/linux.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/logging.py` & `pytoolbox-14.5.1/pytoolbox/logging.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/brand.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/brand.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/camera.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/camera.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/equipment.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/equipment.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/image.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/image.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/lens.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/lens.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/metadata.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/metadata.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/photo.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/photo.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/exif/tag.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/exif/tag.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/encode.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/encode.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffmpeg.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/ffprobe.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/ffprobe.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/miscellaneous.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/ffmpeg/utils.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/ffmpeg/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/image/PIL.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/image/PIL.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/multimedia/x264.py` & `pytoolbox-14.5.1/pytoolbox/multimedia/x264.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/http.py` & `pytoolbox-14.5.1/pytoolbox/network/http.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/ip.py` & `pytoolbox-14.5.1/pytoolbox/network/ip.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/rtp.py` & `pytoolbox-14.5.1/pytoolbox/network/rtp.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/smpte2022/base.py` & `pytoolbox-14.5.1/pytoolbox/network/smpte2022/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/smpte2022/generator.py` & `pytoolbox-14.5.1/pytoolbox/network/smpte2022/generator.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/smpte2022/receiver.py` & `pytoolbox-14.5.1/pytoolbox/network/smpte2022/receiver.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/network/url.py` & `pytoolbox-14.5.1/pytoolbox/network/url.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/regex.py` & `pytoolbox-14.5.1/pytoolbox/regex.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/rest_framework/metadata/mixins.py` & `pytoolbox-14.5.1/pytoolbox/rest_framework/metadata/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/rest_framework/permissions.py` & `pytoolbox-14.5.1/pytoolbox/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/fields.py` & `pytoolbox-14.5.1/pytoolbox/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/rest_framework/serializers/mixins.py` & `pytoolbox-14.5.1/pytoolbox/rest_framework/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/rest_framework/views/mixins.py` & `pytoolbox-14.5.1/pytoolbox/rest_framework/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/selenium/client.py` & `pytoolbox-14.5.1/pytoolbox/selenium/client.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/selenium/common.py` & `pytoolbox-14.5.1/pytoolbox/selenium/common.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/selenium/test.py` & `pytoolbox-14.5.1/pytoolbox/selenium/test.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/selenium/webdrivers.py` & `pytoolbox-14.5.1/pytoolbox/selenium/webdrivers.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/selenium/webelements/base.py` & `pytoolbox-14.5.1/pytoolbox/selenium/webelements/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/selenium/webelements/bootstrap_slider.py` & `pytoolbox-14.5.1/pytoolbox/selenium/webelements/bootstrap_slider.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/serialization.py` & `pytoolbox-14.5.1/pytoolbox/serialization.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/signals.py` & `pytoolbox-14.5.1/pytoolbox/signals.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/states.py` & `pytoolbox-14.5.1/pytoolbox/states.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/string.py` & `pytoolbox-14.5.1/pytoolbox/string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/subprocess.py` & `pytoolbox-14.5.1/pytoolbox/subprocess.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/throttles.py` & `pytoolbox-14.5.1/pytoolbox/throttles.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/types.py` & `pytoolbox-14.5.1/pytoolbox/types.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/unittest.py` & `pytoolbox-14.5.1/pytoolbox/unittest.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/validation.py` & `pytoolbox-14.5.1/pytoolbox/validation.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/virtualenv.py` & `pytoolbox-14.5.1/pytoolbox/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox/voluptuous.py` & `pytoolbox-14.5.1/pytoolbox/voluptuous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox.egg-info/PKG-INFO` & `pytoolbox-14.5.1/pytoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.5.0
+Version: 14.5.1
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytoolbox-14.5.0/pytoolbox.egg-info/SOURCES.txt` & `pytoolbox-14.5.1/pytoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/pytoolbox.egg-info/requires.txt` & `pytoolbox-14.5.1/pytoolbox.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/setup.py` & `pytoolbox-14.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_argparse.py` & `pytoolbox-14.5.1/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_collections.py` & `pytoolbox-14.5.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_comparison.py` & `pytoolbox-14.5.1/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_console.py` & `pytoolbox-14.5.1/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_django_utils.py` & `pytoolbox-14.5.1/tests/test_django_utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_exceptions.py` & `pytoolbox-14.5.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_ffmpeg.py` & `pytoolbox-14.5.1/tests/test_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_filesystem.py` & `pytoolbox-14.5.1/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_juju.py` & `pytoolbox-14.5.1/tests/test_juju.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_module.py` & `pytoolbox-14.5.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_private.py` & `pytoolbox-14.5.1/tests/test_private.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_serialization.py` & `pytoolbox-14.5.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_signals.py` & `pytoolbox-14.5.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_states.py` & `pytoolbox-14.5.1/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_string.py` & `pytoolbox-14.5.1/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_subprocess.py` & `pytoolbox-14.5.1/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_unittest.py` & `pytoolbox-14.5.1/tests/test_unittest.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.5.0/tests/test_validation.py` & `pytoolbox-14.5.1/tests/test_validation.py`

 * *Files identical despite different names*

