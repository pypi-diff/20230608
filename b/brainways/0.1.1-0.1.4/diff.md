# Comparing `tmp/brainways-0.1.1.tar.gz` & `tmp/brainways-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainways-0.1.1.tar", last modified: Fri May 26 13:54:23 2023, max compression
+gzip compressed data, was "brainways-0.1.4.tar", last modified: Thu Jun  8 07:42:29 2023, max compression
```

## Comparing `brainways-0.1.1.tar` & `brainways-0.1.4.tar`

### file list

```diff
@@ -1,175 +1,182 @@
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/
--rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.1/.editorconfig
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.938592 brainways-0.1.1/.github/
--rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.1/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.1/.gitignore
--rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.1/.travis.yml
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.1/AUTHORS.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.1/HISTORY.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.1/LICENSE
--rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.1/MANIFEST.in
--rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.1/Makefile
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-05-26 13:54:23.958592 brainways-0.1.1/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.1/README.rst
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/data/
--rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.1/data/test_data.npz
--rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.1/data/test_image.jpg
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/docs/
--rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/Makefile
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.934592 brainways-0.1.1/docs/_build/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.934592 brainways-0.1.1/docs/_build/html/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/docs/_build/html/_static/
--rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/authors.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.elastix.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.pipeline.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.project.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.1/docs/brainways.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.scripts.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.transforms.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.atlas.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.cell_detection_importer.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.czi.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.io_utils.file_iterators.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.io_utils.readers.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.io_utils.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.1/docs/brainways.utils.rst
--rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.1/docs/conf.py
--rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/contributing.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/history.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/index.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/installation.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/make.bat
--rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.1/docs/modules.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/readme.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.1/docs/usage.rst
--rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.1/pyproject.toml
--rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.1/requirements_dev.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-05-26 13:54:23.958592 brainways-0.1.1/setup.cfg
--rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.1/setup.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.934592 brainways-0.1.1/src/
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.942592 brainways-0.1.1/src/brainways/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.1/src/brainways/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways/_version.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7068 2022-11-30 13:46:38.000000 brainways-0.1.1/src/brainways/conftest.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/elastix/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.1/src/brainways/elastix/Par0033bspline.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.1/src/brainways/elastix/Par0033similarity.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.1/src/brainways/elastix/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/elastix/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.1/src/brainways/elastix/_tests/test_elastix.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.1/src/brainways/elastix/elastix.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/pipeline/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/pipeline/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/pipeline/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.1/src/brainways/pipeline/_tests/test_atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.1/src/brainways/pipeline/_tests/test_brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.1/src/brainways/pipeline/affine_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.1/src/brainways/pipeline/atlas_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1231 2023-01-25 12:05:30.000000 brainways-0.1.1/src/brainways/pipeline/brainways_params.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.1/src/brainways/pipeline/brainways_pipeline.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4123 2023-04-30 11:04:32.000000 brainways-0.1.1/src/brainways/pipeline/cell_detector.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.1/src/brainways/pipeline/tps.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways/project/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/project/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/project/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.1/src/brainways/project/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      615 2022-11-23 13:20:41.000000 brainways-0.1.1/src/brainways/project/_tests/conftest.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1951 2022-11-24 12:49:33.000000 brainways-0.1.1/src/brainways/project/_tests/test_brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8844 2022-11-23 13:20:41.000000 brainways-0.1.1/src/brainways/project/_tests/test_brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     8262 2023-05-18 10:57:16.000000 brainways-0.1.1/src/brainways/project/brainways_project.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    18817 2023-05-07 14:18:30.000000 brainways-0.1.1/src/brainways/project/brainways_subject.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1277 2023-05-17 07:54:03.000000 brainways-0.1.1/src/brainways/project/info_classes.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/scripts/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.1/src/brainways/scripts/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/scripts/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.1/src/brainways/scripts/_tests/test_cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.1/src/brainways/scripts/batch_create_thumbnails.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.1/src/brainways/scripts/cell_detection.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.1/src/brainways/scripts/cli.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.1/src/brainways/scripts/create_excel.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.1/src/brainways/scripts/create_excel_colabelling.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.1/src/brainways/scripts/create_reg_model_data.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.1/src/brainways/scripts/display_area.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.1/src/brainways/scripts/import_cell_detections_keren.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.1/src/brainways/scripts/import_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.1/src/brainways/scripts/move_images.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/transforms/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.1/src/brainways/transforms/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.950592 brainways-0.1.1/src/brainways/transforms/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.1/src/brainways/transforms/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/_tests/test_tps_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.1/src/brainways/transforms/affine_transform_2d.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.1/src/brainways/transforms/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.1/src/brainways/transforms/compose.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/transforms/depth_registration.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.1/src/brainways/transforms/image_to_atlas_transform.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.1/src/brainways/transforms/tps_transform.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.1/src/brainways/utils/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.1/src/brainways/utils/_imports.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.1/src/brainways/utils/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.1/src/brainways/utils/_tests/test_cell_count_summary.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.1/src/brainways/utils/_tests/test_cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/utils/_tests/test_image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/atlas/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.1/src/brainways/utils/atlas/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/atlas/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.1/src/brainways/utils/atlas/_tests/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.1/src/brainways/utils/atlas/_tests/test_slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1.1/src/brainways/utils/atlas/brainways_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.1/src/brainways/utils/atlas/slice_atlas.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.1/src/brainways/utils/cell_count_summary.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.954592 brainways-0.1.1/src/brainways/utils/cell_detection_importer/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.1/src/brainways/utils/cell_detection_importer/utils.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.1/src/brainways/utils/cells.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.1/src/brainways/utils/config.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/czi/
--rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.1/src/brainways/utils/czi/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/utils/czi/czi_to_jpg.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.1/src/brainways/utils/dataclasses.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.1/src/brainways/utils/image.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/
--rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.1/src/brainways/utils/io_utils/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/
--rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/__init__.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/image_entry.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/path.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.1/src/brainways/utils/io_utils/image_path.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/readers/
--rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/__init__.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.958592 brainways-0.1.1/src/brainways/utils/io_utils/readers/_tests/
--rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/base.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/czi_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.1/src/brainways/utils/io_utils/readers/qupath_reader.py
--rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.1/src/brainways/utils/paths.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.1/src/brainways/utils/preprocess.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.1/src/brainways/utils/qupath.py
--rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.1/src/brainways/utils/test_utils.py
-drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-05-26 13:54:23.946592 brainways-0.1.1/src/brainways.egg-info/
--rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1001) ben       (1001)     5332 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/entry_points.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/requires.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-05-26 13:54:23.000000 brainways-0.1.1/src/brainways.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.1/tox.ini
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      292 2022-07-13 13:47:58.000000 brainways-0.1.4/.editorconfig
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.532988 brainways-0.1.4/.github/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      320 2022-07-13 13:47:58.000000 brainways-0.1.4/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1248 2022-07-13 14:46:16.000000 brainways-0.1.4/.gitignore
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1194 2022-07-14 13:50:01.000000 brainways-0.1.4/.pre-commit-config.yaml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      681 2022-07-13 13:47:58.000000 brainways-0.1.4/.travis.yml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2022-07-13 13:47:58.000000 brainways-0.1.4/AUTHORS.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3523 2022-07-13 13:47:58.000000 brainways-0.1.4/CONTRIBUTING.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       89 2022-07-13 13:47:58.000000 brainways-0.1.4/HISTORY.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)    35148 2022-08-24 08:26:24.000000 brainways-0.1.4/LICENSE
+-rw-rw-r--   0 ben       (1001) ben       (1001)      262 2022-07-13 13:47:58.000000 brainways-0.1.4/MANIFEST.in
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2430 2023-05-26 08:21:13.000000 brainways-0.1.4/Makefile
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-08 07:42:29.548988 brainways-0.1.4/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)      962 2023-05-26 08:25:05.000000 brainways-0.1.4/README.rst
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.532988 brainways-0.1.4/data/
+-rw-rw-r--   0 ben       (1001) ben       (1001)   269441 2022-03-11 09:30:01.000000 brainways-0.1.4/data/test_data.npz
+-rw-rw-r--   0 ben       (1001) ben       (1001)    47973 2022-06-30 11:17:43.000000 brainways-0.1.4/data/test_image.jpg
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/docs/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      610 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/Makefile
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/docs/_build/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/docs/_build/html/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/docs/_build/html/_static/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      286 2022-10-06 11:03:00.000000 brainways-0.1.4/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.4/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       90 2022-10-06 11:03:00.000000 brainways-0.1.4/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/authors.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      361 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.elastix.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1317 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.pipeline.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      770 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.project.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      500 2023-05-26 08:26:43.000000 brainways-0.1.4/docs/brainways.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2137 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.scripts.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1387 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.transforms.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      601 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.atlas.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1405 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.cell_detection_importer.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      386 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.czi.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      971 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.io_utils.file_iterators.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1145 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.io_utils.readers.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      553 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.io_utils.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1833 2023-05-26 08:18:55.000000 brainways-0.1.4/docs/brainways.utils.rst
+-rwxrwxr-x   0 ben       (1001) ben       (1001)     4967 2023-05-26 08:17:55.000000 brainways-0.1.4/docs/conf.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)       33 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/contributing.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       28 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/history.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      306 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/index.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1118 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/installation.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      807 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/make.bat
+-rw-rw-r--   0 ben       (1001) ben       (1001)       64 2023-05-26 08:26:43.000000 brainways-0.1.4/docs/modules.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       27 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/readme.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)       73 2022-07-13 13:47:58.000000 brainways-0.1.4/docs/usage.rst
+-rw-rw-r--   0 ben       (1001) ben       (1001)      383 2023-05-26 08:03:19.000000 brainways-0.1.4/pyproject.toml
+-rw-rw-r--   0 ben       (1001) ben       (1001)      165 2022-07-13 14:08:33.000000 brainways-0.1.4/requirements_dev.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1967 2023-06-08 07:42:29.548988 brainways-0.1.4/setup.cfg
+-rw-rw-r--   0 ben       (1001) ben       (1001)       60 2023-05-26 07:59:05.000000 brainways-0.1.4/setup.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/src/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-13 14:28:10.000000 brainways-0.1.4/src/brainways/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      160 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways/_version.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7168 2023-06-07 15:59:32.000000 brainways-0.1.4/src/brainways/conftest.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/elastix/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2596 2022-07-14 13:40:58.000000 brainways-0.1.4/src/brainways/elastix/Par0033bspline.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2316 2022-07-14 13:40:58.000000 brainways-0.1.4/src/brainways/elastix/Par0033similarity.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-12-09 12:20:50.000000 brainways-0.1.4/src/brainways/elastix/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/elastix/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      592 2022-10-27 09:03:02.000000 brainways-0.1.4/src/brainways/elastix/_tests/test_elastix.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2649 2022-09-08 14:32:33.000000 brainways-0.1.4/src/brainways/elastix/elastix.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/pipeline/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/pipeline/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways/pipeline/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      430 2022-10-27 09:03:02.000000 brainways-0.1.4/src/brainways/pipeline/_tests/test_atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      552 2022-11-23 11:34:52.000000 brainways-0.1.4/src/brainways/pipeline/_tests/test_brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1097 2022-11-30 13:23:46.000000 brainways-0.1.4/src/brainways/pipeline/affine_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2339 2023-05-24 12:27:57.000000 brainways-0.1.4/src/brainways/pipeline/atlas_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1165 2023-06-07 14:11:19.000000 brainways-0.1.4/src/brainways/pipeline/brainways_params.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3712 2022-11-30 13:35:53.000000 brainways-0.1.4/src/brainways/pipeline/brainways_pipeline.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5186 2023-06-07 15:47:46.000000 brainways-0.1.4/src/brainways/pipeline/cell_detector.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1596 2022-11-30 13:25:23.000000 brainways-0.1.4/src/brainways/pipeline/tps.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/project/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.4/src/brainways/project/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1003 2023-06-07 11:33:52.000000 brainways-0.1.4/src/brainways/project/_tests/conftest.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2598 2023-06-08 07:32:26.000000 brainways-0.1.4/src/brainways/project/_tests/test_brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8619 2023-06-07 11:26:16.000000 brainways-0.1.4/src/brainways/project/_tests/test_brainways_subject.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.528988 brainways-0.1.4/src/brainways/project/_tests/test_projects/
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       38 2023-06-07 15:59:39.000000 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/subject1/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2155 2023-06-07 10:30:28.000000 brainways-0.1.4/src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
+-rw-rw-r--   0 ben       (1001) ben       (1001)      388 2023-06-07 11:49:25.000000 brainways-0.1.4/src/brainways/project/_tests/test_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1493 2023-06-08 07:35:04.000000 brainways-0.1.4/src/brainways/project/_utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     8792 2023-06-07 15:29:27.000000 brainways-0.1.4/src/brainways/project/brainways_project.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    18458 2023-06-07 13:06:53.000000 brainways-0.1.4/src/brainways/project/brainways_subject.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1388 2023-06-07 15:59:32.000000 brainways-0.1.4/src/brainways/project/info_classes.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/scripts/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.4/src/brainways/scripts/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/scripts/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2023-05-26 08:21:13.000000 brainways-0.1.4/src/brainways/scripts/_tests/test_cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3031 2022-09-08 14:06:58.000000 brainways-0.1.4/src/brainways/scripts/batch_create_thumbnails.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3053 2023-05-07 14:18:30.000000 brainways-0.1.4/src/brainways/scripts/cell_detection.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1142 2023-05-04 08:18:52.000000 brainways-0.1.4/src/brainways/scripts/cli.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1588 2023-05-07 14:18:29.000000 brainways-0.1.4/src/brainways/scripts/create_excel.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4944 2022-11-30 14:10:59.000000 brainways-0.1.4/src/brainways/scripts/create_excel_colabelling.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4023 2022-11-23 12:26:10.000000 brainways-0.1.4/src/brainways/scripts/create_reg_model_data.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5253 2022-11-23 12:35:34.000000 brainways-0.1.4/src/brainways/scripts/display_area.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1618 2022-12-08 14:20:04.000000 brainways-0.1.4/src/brainways/scripts/import_cell_detections_keren.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1192 2022-11-23 12:26:10.000000 brainways-0.1.4/src/brainways/scripts/import_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      920 2022-12-11 10:14:02.000000 brainways-0.1.4/src/brainways/scripts/move_images.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.540988 brainways-0.1.4/src/brainways/transforms/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.4/src/brainways/transforms/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/transforms/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.4/src/brainways/transforms/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2173 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1813 2022-11-23 11:35:37.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2034 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2667 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/_tests/test_tps_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4104 2022-11-30 13:34:33.000000 brainways-0.1.4/src/brainways/transforms/affine_transform_2d.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      436 2022-07-14 12:46:19.000000 brainways-0.1.4/src/brainways/transforms/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      623 2022-07-14 13:40:58.000000 brainways-0.1.4/src/brainways/transforms/compose.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2594 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/transforms/depth_registration.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2205 2022-09-08 13:13:42.000000 brainways-0.1.4/src/brainways/transforms/image_to_atlas_transform.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2185 2022-11-30 13:46:38.000000 brainways-0.1.4/src/brainways/transforms/tps_transform.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 08:14:53.000000 brainways-0.1.4/src/brainways/utils/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1674 2022-07-17 07:51:20.000000 brainways-0.1.4/src/brainways/utils/_imports.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-07-14 12:32:42.000000 brainways-0.1.4/src/brainways/utils/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7710 2023-05-26 08:21:13.000000 brainways-0.1.4/src/brainways/utils/_tests/test_cell_count_summary.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2715 2023-05-07 14:18:30.000000 brainways-0.1.4/src/brainways/utils/_tests/test_cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2412 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/utils/_tests/test_image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/atlas/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-21 11:07:35.000000 brainways-0.1.4/src/brainways/utils/atlas/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/atlas/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-04-27 09:13:34.000000 brainways-0.1.4/src/brainways/utils/atlas/_tests/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3708 2022-07-14 13:40:59.000000 brainways-0.1.4/src/brainways/utils/atlas/_tests/test_slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4263 2022-12-11 16:13:39.000000 brainways-0.1.4/src/brainways/utils/atlas/brainways_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2280 2023-05-04 09:01:16.000000 brainways-0.1.4/src/brainways/utils/atlas/slice_atlas.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5751 2023-05-14 15:00:03.000000 brainways-0.1.4/src/brainways/utils/cell_count_summary.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.544988 brainways-0.1.4/src/brainways/utils/cell_detection_importer/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2022-10-06 09:31:17.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     7465 2022-10-06 10:12:40.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1240 2022-11-23 12:23:47.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1722 2022-12-08 14:20:04.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1343 2022-11-23 12:26:10.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      507 2022-11-27 15:04:03.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2438 2022-12-11 10:33:01.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      731 2022-12-08 14:20:04.000000 brainways-0.1.4/src/brainways/utils/cell_detection_importer/utils.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4985 2023-05-02 09:29:03.000000 brainways-0.1.4/src/brainways/utils/cells.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     4270 2022-09-11 13:34:36.000000 brainways-0.1.4/src/brainways/utils/config.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/czi/
+-rw-rw-r--   0 ben       (1001) ben       (1001)        0 2021-07-15 08:31:32.000000 brainways-0.1.4/src/brainways/utils/czi/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1112 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/utils/czi/czi_to_jpg.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      793 2022-07-14 12:49:34.000000 brainways-0.1.4/src/brainways/utils/dataclasses.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     9025 2023-05-26 13:51:47.000000 brainways-0.1.4/src/brainways/utils/image.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/
+-rw-rw-r--   0 ben       (1001) ben       (1001)       42 2022-07-17 07:44:03.000000 brainways-0.1.4/src/brainways/utils/io_utils/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      379 2022-09-08 08:38:22.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/__init__.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      230 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/image_entry.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      407 2022-07-07 09:39:04.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/path.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      914 2022-11-23 12:29:43.000000 brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      630 2022-07-07 09:39:09.000000 brainways-0.1.4/src/brainways/utils/io_utils/image_path.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/readers/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1041 2022-09-11 12:16:49.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/__init__.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.548988 brainways-0.1.4/src/brainways/utils/io_utils/readers/_tests/
+-rw-rw-r--   0 ben       (1001) ben       (1001)      218 2022-09-22 07:42:16.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/_tests/test_qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1419 2022-09-08 08:38:21.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/aicsimageio_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      649 2022-07-14 12:39:58.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/base.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1364 2022-09-08 08:38:21.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/czi_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)    15748 2023-05-21 10:26:48.000000 brainways-0.1.4/src/brainways/utils/io_utils/readers/qupath_reader.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)      108 2022-09-11 13:34:36.000000 brainways-0.1.4/src/brainways/utils/paths.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1181 2022-07-14 13:48:40.000000 brainways-0.1.4/src/brainways/utils/preprocess.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     3183 2022-09-11 10:47:30.000000 brainways-0.1.4/src/brainways/utils/qupath.py
+-rw-rw-r--   0 ben       (1001) ben       (1001)     1083 2022-07-14 13:48:39.000000 brainways-0.1.4/src/brainways/utils/test_utils.py
+drwxrwxr-x   0 ben       (1001) ben       (1001)        0 2023-06-08 07:42:29.536988 brainways-0.1.4/src/brainways.egg-info/
+-rw-rw-r--   0 ben       (1001) ben       (1001)     2343 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/PKG-INFO
+-rw-rw-r--   0 ben       (1001) ben       (1001)     5542 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/SOURCES.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)        1 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/dependency_links.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       57 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/entry_points.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      413 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/requires.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)       10 2023-06-08 07:42:29.000000 brainways-0.1.4/src/brainways.egg-info/top_level.txt
+-rw-rw-r--   0 ben       (1001) ben       (1001)      540 2022-07-13 13:47:58.000000 brainways-0.1.4/tox.ini
```

### Comparing `brainways-0.1.1/.gitignore` & `brainways-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/.pre-commit-config.yaml` & `brainways-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/.travis.yml` & `brainways-0.1.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/CONTRIBUTING.rst` & `brainways-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/LICENSE` & `brainways-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/Makefile` & `brainways-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/PKG-INFO` & `brainways-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.1
+Version: 0.1.4
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.1/README.rst` & `brainways-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/data/test_data.npz` & `brainways-0.1.4/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/data/test_image.jpg` & `brainways-0.1.4/data/test_image.jpg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/Makefile` & `brainways-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.pipeline.rst` & `brainways-0.1.4/docs/brainways.pipeline.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.project.rst` & `brainways-0.1.4/docs/brainways.project.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.scripts.rst` & `brainways-0.1.4/docs/brainways.scripts.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.transforms.rst` & `brainways-0.1.4/docs/brainways.transforms.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.utils.atlas.rst` & `brainways-0.1.4/docs/brainways.utils.atlas.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.utils.cell_detection_importer.rst` & `brainways-0.1.4/docs/brainways.utils.cell_detection_importer.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.utils.io_utils.file_iterators.rst` & `brainways-0.1.4/docs/brainways.utils.io_utils.file_iterators.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.utils.io_utils.readers.rst` & `brainways-0.1.4/docs/brainways.utils.io_utils.readers.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.utils.io_utils.rst` & `brainways-0.1.4/docs/brainways.utils.io_utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/brainways.utils.rst` & `brainways-0.1.4/docs/brainways.utils.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/conf.py` & `brainways-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/installation.rst` & `brainways-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/docs/make.bat` & `brainways-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/setup.cfg` & `brainways-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/conftest.py` & `brainways-0.1.4/src/brainways/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from PIL import Image
 from pytest import fixture
 
 from brainways.pipeline.brainways_params import (
     AffineTransform2DParams,
     AtlasRegistrationParams,
     BrainwaysParams,
+    CellDetectorParams,
     TPSTransformParams,
 )
 from brainways.project.brainways_subject import BrainwaysSubject
 from brainways.project.info_classes import ProjectSettings, SliceInfo
 from brainways.utils.atlas.brainways_atlas import AtlasSlice, BrainwaysAtlas
 from brainways.utils.image import ImageSizeHW
 from brainways.utils.io_utils import ImagePath
@@ -145,14 +146,17 @@
     params = BrainwaysParams(
         atlas=AtlasRegistrationParams(ap=5),
         affine=AffineTransform2DParams(),
         tps=TPSTransformParams(
             points_src=tps_points,
             points_dst=tps_points,
         ),
+        cell=CellDetectorParams(
+            normalizer="clahe",
+        ),
     )
     documents = []
     for i in range(3):
         doc_image_filename_name = f"{Path(mock_image_path.filename).stem}_{i}.jpg"
         doc_image_filename = Path(mock_image_path.filename).with_name(
             doc_image_filename_name
         )
```

### Comparing `brainways-0.1.1/src/brainways/elastix/Par0033bspline.txt` & `brainways-0.1.4/src/brainways/elastix/Par0033bspline.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/elastix/Par0033similarity.txt` & `brainways-0.1.4/src/brainways/elastix/Par0033similarity.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/elastix/_tests/test_elastix.py` & `brainways-0.1.4/src/brainways/elastix/_tests/test_elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/elastix/elastix.py` & `brainways-0.1.4/src/brainways/elastix/elastix.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/pipeline/_tests/test_brainways_pipeline.py` & `brainways-0.1.4/src/brainways/pipeline/_tests/test_brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/pipeline/affine_2d.py` & `brainways-0.1.4/src/brainways/pipeline/affine_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/pipeline/atlas_registration.py` & `brainways-0.1.4/src/brainways/pipeline/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/pipeline/brainways_params.py` & `brainways-0.1.4/src/brainways/pipeline/brainways_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,19 +14,16 @@
     affine: Optional[AffineTransform2DParams] = None
     tps: Optional[TPSTransformParams] = None
     cell: Optional[CellDetectorParams] = None
 
 
 @dataclass
 class CellDetectorParams:
-    diameter: float
-    net_avg: bool
-    flow_threshold: float
-    mask_threshold: float
-    preview_bb: Optional[Tuple[float, float, float, float]] = None
+    normalizer: str = "quantile"
+    normalizer_range: Tuple[float, float] = (0.98, 0.997)
 
 
 @dataclass
 class AffineTransform2DParams:
     angle: float = 0.0
     tx: float = 0.0
     ty: float = 0.0
```

### Comparing `brainways-0.1.1/src/brainways/pipeline/brainways_pipeline.py` & `brainways-0.1.4/src/brainways/pipeline/brainways_pipeline.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/pipeline/tps.py` & `brainways-0.1.4/src/brainways/pipeline/tps.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/project/_tests/test_brainways_project.py` & `brainways-0.1.4/src/brainways/project/_tests/test_brainways_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     mock_project_settings: ProjectSettings,
     mock_atlas: BrainwaysAtlas,
 ) -> BrainwaysProject:
     brainways_project = BrainwaysProject(
         subjects=[brainways_subject], settings=mock_project_settings, lazy_init=True
     )
     brainways_project.atlas = mock_atlas
+    brainways_project.load_pipeline()
     return brainways_project
 
 
 def test_brainways_project_create_excel(brainways_project: BrainwaysProject, tmpdir):
     excel_path = Path(tmpdir / "excel.xlsx")
     cells_df = pd.DataFrame({"x": [0.5], "y": [0.5]})
     subject = brainways_project.subjects[0]
@@ -49,7 +50,25 @@
     mock_project_settings: ProjectSettings,
     mock_subject_documents: List[SliceInfo],
 ):
     project = BrainwaysProject.open(project_path, lazy_init=True)
     assert project.settings == mock_project_settings
     assert len(project.subjects) == 1
     assert project.subjects[0].documents == mock_subject_documents
+
+
+def test_open_brainways_project_v0_1_1(
+    brainways_project_path_v0_1_1: Path,
+    mock_project_settings: ProjectSettings,
+    mock_subject_documents: List[SliceInfo],
+):
+    project = BrainwaysProject.open(brainways_project_path_v0_1_1, lazy_init=True)
+    assert project.settings.atlas == mock_project_settings.atlas
+    assert len(project.subjects) == 1
+    assert (
+        project.subjects[0].documents[0].params.atlas
+        == mock_subject_documents[0].params.atlas
+    )
+    assert (
+        project.subjects[0].documents[0].params.affine
+        == mock_subject_documents[0].params.affine
+    )
```

### Comparing `brainways-0.1.1/src/brainways/project/_tests/test_brainways_subject.py` & `brainways-0.1.4/src/brainways/project/_tests/test_brainways_subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,20 +215,14 @@
 ):
     mock_atlas = Mock()
     mock_atlas.brainglobe_atlas.atlas_name = "test"
     with pytest.raises(ValueError):
         BrainwaysSubject(settings=mock_project_settings, documents=[], atlas=mock_atlas)
 
 
-def test_load_pipeline(brainways_subject: BrainwaysSubject, mock_atlas: BrainwaysAtlas):
-    assert brainways_subject.pipeline is None
-    brainways_subject.load_pipeline()
-    assert brainways_subject.pipeline is not None
-
-
 def test_init_subject_with_nonempty_directory(
     mock_project_settings: ProjectSettings, tmpdir
 ):
     (Path(tmpdir) / "test").touch()
     with pytest.raises(FileExistsError):
         BrainwaysSubject(settings=mock_project_settings, subject_path=Path(tmpdir))
```

### Comparing `brainways-0.1.1/src/brainways/project/brainways_project.py` & `brainways-0.1.4/src/brainways/project/brainways_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import dacite
 import pandas as pd
 from natsort import natsorted, ns
 from pandas import ExcelWriter
 
 from brainways.pipeline.brainways_pipeline import BrainwaysPipeline
 from brainways.pipeline.cell_detector import CellDetector
+from brainways.project._utils import update_project_from_previous_versions
 from brainways.project.brainways_subject import BrainwaysSubject
 from brainways.project.info_classes import ExcelMode, ProjectSettings, SliceInfo
 from brainways.utils.atlas.brainways_atlas import BrainwaysAtlas
 from brainways.utils.cell_detection_importer.cell_detection_importer import (
     CellDetectionImporter,
 )
 
@@ -52,15 +53,15 @@
         if path.suffix == ".bwp":
             project_dir = path.parent
         else:
             project_dir = path
             path = path / "brainways.bwp"
 
         if not force and project_dir.exists() and len(list(project_dir.glob("*"))) > 0:
-            raise FileExistsError(f"Directory is not empty: {path}")
+            raise FileExistsError(f"Directory is not empty: {project_dir}")
 
         project_dir.mkdir(parents=True, exist_ok=True)
 
         serialized_settings = asdict(settings)
         with open(path, "w") as f:
             json.dump(serialized_settings, f)
 
@@ -70,27 +71,36 @@
     def open(cls, path: Union[Path, str], lazy_init: bool = False):
         path = Path(path)
         if not path.exists():
             raise FileNotFoundError(f"BrainwaysProject file not found: {path}")
         if not path.suffix == ".bwp":
             raise FileNotFoundError(f"File is not a Brainways project file: {path}")
 
+        update_project_from_previous_versions(path)
+
         with open(path) as f:
             serialized_settings = json.load(f)
 
-        settings = dacite.from_dict(ProjectSettings, serialized_settings)
+        settings = dacite.from_dict(
+            ProjectSettings, serialized_settings, config=dacite.Config(cast=[tuple])
+        )
         subject_directories = [d for d in path.parent.glob("*") if d.is_dir()]
         subject_directories = natsorted(
             subject_directories, alg=ns.IGNORECASE, key=lambda x: x.name
         )
         subjects = [
             BrainwaysSubject.open(subject_path) for subject_path in subject_directories
         ]
         return cls(subjects=subjects, settings=settings, path=path, lazy_init=lazy_init)
 
+    def save(self):
+        serialized_settings = asdict(self.settings)
+        with open(self.path, "w") as f:
+            json.dump(serialized_settings, f)
+
     def add_subject(self, id: str) -> BrainwaysSubject:
         subject = BrainwaysSubject(
             settings=self.settings, subject_path=self.path.parent / id
         )
         self.subjects.append(subject)
         return subject
 
@@ -217,20 +227,24 @@
                 root=cell_detections_root,
                 cell_detection_importer=importer,
             )
 
     def run_cell_detector_iter(self) -> Iterator:
         cell_detector = CellDetector()
         for subject in self.subjects:
-            yield from subject.run_cell_detector_iter(cell_detector)
+            yield from subject.run_cell_detector_iter(
+                cell_detector, default_params=self.settings.default_cell_detector_params
+            )
 
     def run_cell_detector(self) -> None:
         cell_detector = CellDetector()
         for subject in self.subjects:
-            subject.run_cell_detector(cell_detector)
+            subject.run_cell_detector(
+                cell_detector, default_params=self.settings.default_cell_detector_params
+            )
 
     @property
     def n_valid_images(self):
         return sum(len(subject.valid_documents) for subject in self.subjects)
 
     def __len__(self) -> int:
         return len(self.subjects)
```

### Comparing `brainways-0.1.1/src/brainways/project/brainways_subject.py` & `brainways-0.1.4/src/brainways/project/brainways_subject.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import dacite
 import numpy as np
 import pandas as pd
 from PIL import Image
 
+from brainways.pipeline.brainways_params import CellDetectorParams
 from brainways.pipeline.brainways_pipeline import BrainwaysPipeline, PipelineStep
-from brainways.pipeline.cell_detector import CellDetector, ClaheNormalizer
+from brainways.pipeline.cell_detector import CellDetector
 from brainways.project.info_classes import ExcelMode, ProjectSettings, SliceInfo
 from brainways.utils.atlas.brainways_atlas import BrainwaysAtlas
 from brainways.utils.cell_count_summary import cell_count_summary
 from brainways.utils.cell_detection_importer.cell_detection_importer import (
     CellDetectionImporter,
 )
 from brainways.utils.cells import (
@@ -106,32 +107,16 @@
 
     def read_highres_image(self, document: SliceInfo, level: Optional[int] = None):
         reader = QupathReader(document.path.filename)
         reader.set_scene(document.path.scene)
         if level:
             reader.set_level(level)
         image = reader.get_image_dask_data("YX", C=self.settings.channel).compute()
-        # image = slice_to_uint8(image)
         return image
 
-    def load_atlas(self, load_volumes: bool = True):
-        self.atlas = BrainwaysAtlas.load(
-            self.settings.atlas, exclude_regions=[76, 42, 41]
-        )  # TODO: from model
-        # load volumes to cache
-        if load_volumes:
-            _ = self.atlas.reference
-            _ = self.atlas.annotation
-            _ = self.atlas.hemispheres
-
-    def load_pipeline(self):
-        if self.atlas is None:
-            self.load_atlas()
-        self.pipeline = BrainwaysPipeline(self.atlas)
-
     def add_image(self, path: ImagePath, load_thumbnail: bool = True) -> SliceInfo:
         image_size = get_image_size(path)
         lowres_image_size = get_resize_size(
             input_size=image_size, output_size=(1024, 1024), keep_aspect=True
         )
         document = SliceInfo(
             path=path,
@@ -152,36 +137,32 @@
 
     @classmethod
     def open(
         cls,
         path: Union[Path, str],
         atlas: Optional[BrainwaysAtlas] = None,
         pipeline: Optional[BrainwaysPipeline] = None,
-        lazy_init: bool = True,
     ):
         subject_dir = BrainwaysSubject._get_subject_dir(path)
         if not subject_dir.exists():
             raise FileNotFoundError(f"subject path not found: {path}")
 
         with open(subject_dir / "brainways.bin", "rb") as f:
             serialized_settings, serialized_documents = pickle.load(f)
+
         settings = dacite.from_dict(ProjectSettings, serialized_settings)
         documents = [dacite.from_dict(SliceInfo, d) for d in serialized_documents]
         subject = BrainwaysSubject(
             settings=settings,
             documents=documents,
             subject_path=subject_dir,
             atlas=atlas,
             pipeline=pipeline,
         )
 
-        if not lazy_init:
-            subject.load_atlas()
-            subject.load_pipeline()
-
         return subject
 
     def save(self, path: Optional[Union[Path, str]] = None):
         if path is None:
             path = self.subject_path
         path = Path(path)
         subject_dir = self._get_subject_dir(path)
@@ -250,42 +231,49 @@
         cell_detection_importer: CellDetectionImporter,
     ) -> None:
         for _ in self.import_cell_detections_iter(
             root=root, cell_detection_importer=cell_detection_importer
         ):
             pass
 
-    def run_cell_detector_iter(self, cell_detector: CellDetector) -> Iterator:
+    def run_cell_detector_iter(
+        self, cell_detector: CellDetector, default_params: CellDetectorParams
+    ) -> Iterator:
         for i, document in self.valid_documents:
             try:
                 cell_detections_path = self.cell_detections_path(document.path)
                 if cell_detections_path.exists():
                     continue
                 reader = document.image_reader()
                 image = reader.get_image_dask_data(
                     "YX", C=self.settings.channel
                 ).compute()
-                # min_val, max_val = np.percentile(image, CFOS_CONTRAST_LIMITS)
-                # print(min_val, max_val)
-                # normalizer = MinMaxNormalizer(min=min_val, max=max_val)
-                normalizer = ClaheNormalizer()
-
-                labels = cell_detector.run_cell_detector(image, normalizer=normalizer)
+                if document.params.cell is not None:
+                    cell_detector_params = document.params.cell
+                else:
+                    cell_detector_params = default_params
+                labels = cell_detector.run_cell_detector(
+                    image, params=cell_detector_params
+                )
                 cells = cell_detector.cells(
                     labels=labels,
                     image=image,
                     physical_pixel_sizes=document.physical_pixel_sizes,
                 )
                 cells.to_csv(cell_detections_path, index=False)
             except Exception:
                 logging.exception(f"Cell detector on {document.path}")
             yield
 
-    def run_cell_detector(self, cell_detector: CellDetector) -> None:
-        for _ in self.run_cell_detector_iter(cell_detector):
+    def run_cell_detector(
+        self, cell_detector: CellDetector, default_params: CellDetectorParams
+    ) -> None:
+        for _ in self.run_cell_detector_iter(
+            cell_detector=cell_detector, default_params=default_params
+        ):
             pass
 
     def get_valid_cells(
         self, document: SliceInfo, annotation: Optional[np.ndarray] = None
     ) -> pd.DataFrame:
         if annotation is None:
             atlas_slice = self.pipeline.get_atlas_slice(document.params)
@@ -337,15 +325,17 @@
         min_region_area_um2: Optional[int] = None,
         cells_per_area_um2: Optional[int] = None,
         min_cell_size_um: Optional[float] = None,
         max_cell_size_um: Optional[float] = None,
         excel_mode: ExcelMode = ExcelMode.ROW_PER_SUBJECT,
     ):
         if self.pipeline is None:
-            self.load_pipeline()
+            raise RuntimeError(
+                "BrainwaysPipeline not loaded, run BrainwaysProject.load_pipeline()"
+            )
 
         all_region_areas = Counter()
         all_cells_on_atlas = []
         image_dfs = []
         for _, document in self.valid_documents:
             document: SliceInfo
             if (
```

### Comparing `brainways-0.1.1/src/brainways/project/info_classes.py` & `brainways-0.1.4/src/brainways/project/info_classes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Optional, Tuple, Union
 
 import brainways._version
-from brainways.pipeline.brainways_params import BrainwaysParams
+from brainways.pipeline.brainways_params import BrainwaysParams, CellDetectorParams
 from brainways.utils.dataclasses import dataclass_eq
 from brainways.utils.image import ImageSizeHW
 from brainways.utils.io_utils import ImagePath
 from brainways.utils.io_utils.readers import QupathReader
 
 
 @dataclass(frozen=True)
 class ProjectSettings:
     atlas: str
     channel: Union[int, str]
+    default_cell_detector_params: CellDetectorParams = CellDetectorParams()
+    version: str = brainways._version.version
 
 
 @dataclass(frozen=True)
 class SubjectSettings:
+    name: str
     condition: Optional[str] = None
-    ignore: bool = False
+    exclude: bool = False
 
 
 @dataclass(frozen=True, eq=False)
 class SliceInfo:
     path: ImagePath
     image_size: ImageSizeHW
     lowres_image_size: ImageSizeHW
     params: Optional[BrainwaysParams] = BrainwaysParams()
     ignore: bool = False
     physical_pixel_sizes: Optional[Tuple[float, float]] = None
-    version: str = brainways._version.version
 
     def image_reader(self) -> QupathReader:
         reader = QupathReader(self.path.filename)
         reader.set_scene(self.path.scene)
         return reader
 
     def __eq__(self, other):
```

### Comparing `brainways-0.1.1/src/brainways/scripts/_tests/test_cli.py` & `brainways-0.1.4/src/brainways/scripts/_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/batch_create_thumbnails.py` & `brainways-0.1.4/src/brainways/scripts/batch_create_thumbnails.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/cell_detection.py` & `brainways-0.1.4/src/brainways/scripts/cell_detection.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/cli.py` & `brainways-0.1.4/src/brainways/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/create_excel.py` & `brainways-0.1.4/src/brainways/scripts/create_excel.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/create_excel_colabelling.py` & `brainways-0.1.4/src/brainways/scripts/create_excel_colabelling.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/create_reg_model_data.py` & `brainways-0.1.4/src/brainways/scripts/create_reg_model_data.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/display_area.py` & `brainways-0.1.4/src/brainways/scripts/display_area.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/import_cell_detections_keren.py` & `brainways-0.1.4/src/brainways/scripts/import_cell_detections_keren.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/import_cells.py` & `brainways-0.1.4/src/brainways/scripts/import_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/scripts/move_images.py` & `brainways-0.1.4/src/brainways/scripts/move_images.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/_tests/test_affine_transform_2d.py` & `brainways-0.1.4/src/brainways/transforms/_tests/test_affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/_tests/test_depth_registration.py` & `brainways-0.1.4/src/brainways/transforms/_tests/test_depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/_tests/test_image_to_atlas_transform.py` & `brainways-0.1.4/src/brainways/transforms/_tests/test_image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/_tests/test_tps_transform.py` & `brainways-0.1.4/src/brainways/transforms/_tests/test_tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/affine_transform_2d.py` & `brainways-0.1.4/src/brainways/transforms/affine_transform_2d.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/compose.py` & `brainways-0.1.4/src/brainways/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/depth_registration.py` & `brainways-0.1.4/src/brainways/transforms/depth_registration.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/image_to_atlas_transform.py` & `brainways-0.1.4/src/brainways/transforms/image_to_atlas_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/transforms/tps_transform.py` & `brainways-0.1.4/src/brainways/transforms/tps_transform.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/_imports.py` & `brainways-0.1.4/src/brainways/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/_tests/test_cell_count_summary.py` & `brainways-0.1.4/src/brainways/utils/_tests/test_cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/_tests/test_cells.py` & `brainways-0.1.4/src/brainways/utils/_tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/_tests/test_image.py` & `brainways-0.1.4/src/brainways/utils/_tests/test_image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/atlas/_tests/test_slice_atlas.py` & `brainways-0.1.4/src/brainways/utils/atlas/_tests/test_slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/atlas/brainways_atlas.py` & `brainways-0.1.4/src/brainways/utils/atlas/brainways_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/atlas/slice_atlas.py` & `brainways-0.1.4/src/brainways/utils/atlas/slice_atlas.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_count_summary.py` & `brainways-0.1.4/src/brainways/utils/cell_count_summary.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt` & `brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/qupath_sample_file.txt`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py` & `brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py` & `brainways-0.1.4/src/brainways/utils/cell_detection_importer/_tests/test_qupath_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py` & `brainways-0.1.4/src/brainways/utils/cell_detection_importer/brainways_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py` & `brainways-0.1.4/src/brainways/utils/cell_detection_importer/keren_cell_detection_importer.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cell_detection_importer/utils.py` & `brainways-0.1.4/src/brainways/utils/cell_detection_importer/utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/cells.py` & `brainways-0.1.4/src/brainways/utils/cells.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/config.py` & `brainways-0.1.4/src/brainways/utils/config.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/czi/czi_to_jpg.py` & `brainways-0.1.4/src/brainways/utils/czi/czi_to_jpg.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/dataclasses.py` & `brainways-0.1.4/src/brainways/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/image.py` & `brainways-0.1.4/src/brainways/utils/image.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/file_iterators/qupath.py` & `brainways-0.1.4/src/brainways/utils/io_utils/file_iterators/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/image_path.py` & `brainways-0.1.4/src/brainways/utils/io_utils/image_path.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/readers/__init__.py` & `brainways-0.1.4/src/brainways/utils/io_utils/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/readers/aicsimageio_reader.py` & `brainways-0.1.4/src/brainways/utils/io_utils/readers/aicsimageio_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/readers/base.py` & `brainways-0.1.4/src/brainways/utils/io_utils/readers/base.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/readers/czi_reader.py` & `brainways-0.1.4/src/brainways/utils/io_utils/readers/czi_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/io_utils/readers/qupath_reader.py` & `brainways-0.1.4/src/brainways/utils/io_utils/readers/qupath_reader.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/preprocess.py` & `brainways-0.1.4/src/brainways/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/qupath.py` & `brainways-0.1.4/src/brainways/utils/qupath.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways/utils/test_utils.py` & `brainways-0.1.4/src/brainways/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `brainways-0.1.1/src/brainways.egg-info/PKG-INFO` & `brainways-0.1.4/src/brainways.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainways
-Version: 0.1.1
+Version: 0.1.4
 Summary: Brainways
 Home-page: https://github.com/bkntr/brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/brainways#README.md
```

### Comparing `brainways-0.1.1/src/brainways.egg-info/SOURCES.txt` & `brainways-0.1.4/src/brainways.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,25 @@
 src/brainways/pipeline/brainways_params.py
 src/brainways/pipeline/brainways_pipeline.py
 src/brainways/pipeline/cell_detector.py
 src/brainways/pipeline/tps.py
 src/brainways/pipeline/_tests/test_atlas_registration.py
 src/brainways/pipeline/_tests/test_brainways_pipeline.py
 src/brainways/project/__init__.py
+src/brainways/project/_utils.py
 src/brainways/project/brainways_project.py
 src/brainways/project/brainways_subject.py
 src/brainways/project/info_classes.py
 src/brainways/project/_tests/__init__.py
 src/brainways/project/_tests/conftest.py
 src/brainways/project/_tests/test_brainways_project.py
 src/brainways/project/_tests/test_brainways_subject.py
+src/brainways/project/_tests/test_utils.py
+src/brainways/project/_tests/test_projects/v0.1.1/project.bwp
+src/brainways/project/_tests/test_projects/v0.1.1/subject1/brainways.bin
 src/brainways/scripts/__init__.py
 src/brainways/scripts/batch_create_thumbnails.py
 src/brainways/scripts/cell_detection.py
 src/brainways/scripts/cli.py
 src/brainways/scripts/create_excel.py
 src/brainways/scripts/create_excel_colabelling.py
 src/brainways/scripts/create_reg_model_data.py
```

### Comparing `brainways-0.1.1/tox.ini` & `brainways-0.1.4/tox.ini`

 * *Files identical despite different names*

