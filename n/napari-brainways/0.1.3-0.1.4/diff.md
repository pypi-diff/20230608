# Comparing `tmp/napari_brainways-0.1.3.tar.gz` & `tmp/napari_brainways-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_brainways-0.1.3.tar", last modified: Fri May 26 15:40:39 2023, max compression
+gzip compressed data, was "napari_brainways-0.1.4.tar", last modified: Thu Jun  8 07:45:34 2023, max compression
```

## Comparing `napari_brainways-0.1.3.tar` & `napari_brainways-0.1.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.867291 napari_brainways-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/data/
--rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/data/test_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.867291 napari_brainways-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/src/napari_brainways/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/src/napari_brainways/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/brainways_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/affine_2d_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/annotation_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/cell_3d_viewer_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/cell_detector_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/registration_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/controllers/tps_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/napari_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.875290 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/affine_2d_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/cell_detector_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/cell_viewer_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/create_subject_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/registration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/tps_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/src/napari_brainways/widgets/workflow_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:40:39.871291 napari_brainways-0.1.3/src/napari_brainways.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:40:39.000000 napari_brainways-0.1.3/src/napari_brainways.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 15:40:21.000000 napari_brainways-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.299019 napari_brainways-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   269441 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/data/test_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.299019 napari_brainways-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/src/napari_brainways/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/src/napari_brainways/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/brainways_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/affine_2d_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/annotation_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/cell_3d_viewer_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/cell_detector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/registration_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/controllers/tps_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/napari_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   231054 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.307019 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_create_project_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/affine_2d_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/cell_detector_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/cell_viewer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/create_subject_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/registration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/tps_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22354 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/src/napari_brainways/widgets/workflow_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:45:34.303019 napari_brainways-0.1.4/src/napari_brainways.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 07:45:34.000000 napari_brainways-0.1.4/src/napari_brainways.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 07:45:11.000000 napari_brainways-0.1.4/tox.ini
```

### Comparing `napari_brainways-0.1.3/.github/workflows/test_and_deploy.yml` & `napari_brainways-0.1.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/.gitignore` & `napari_brainways-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/.napari/DESCRIPTION.md` & `napari_brainways-0.1.4/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/.pre-commit-config.yaml` & `napari_brainways-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/LICENSE` & `napari_brainways-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/PKG-INFO` & `napari_brainways-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_brainways
-Version: 0.1.3
+Version: 0.1.4
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.3/README.md` & `napari_brainways-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/data/test_data.npz` & `napari_brainways-0.1.4/data/test_data.npz`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/setup.cfg` & `napari_brainways-0.1.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 	Documentation = https://github.com/bkntr/napari-brainways#README.md
 	Source Code = https://github.com/bkntr/napari-brainways
 	User Support = https://github.com/bkntr/napari-brainways/issues
 
 [options]
 packages = find:
 install_requires = 
-	brainways
+	brainways==0.1.4
 	importlib-resources
 	napari
 	qtpy
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `napari_brainways-0.1.3/src/napari_brainways/_sample_data.py` & `napari_brainways-0.1.4/src/napari_brainways/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/_tests/test_reader.py` & `napari_brainways-0.1.4/src/napari_brainways/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/_tests/test_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/brainways_ui.py` & `napari_brainways-0.1.4/src/napari_brainways/brainways_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
             self.current_document, params=self.current_step.params
         )
 
     def save_subject(self, persist: bool = True) -> None:
         if persist:
             self.persist_current_params()
         self.current_subject.save()
+        self.project.save()
 
     def create_excel_async(
         self,
         path: Path,
         min_region_area_um2: Optional[int] = None,
         cells_per_area_um2: Optional[int] = None,
         min_cell_size_um: Optional[float] = None,
```

### Comparing `napari_brainways-0.1.3/src/napari_brainways/conftest.py` & `napari_brainways-0.1.4/src/napari_brainways/conftest.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/_tests/test_tps_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/_tests/test_tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/affine_2d_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/affine_2d_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/annotation_viewer_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/annotation_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/base.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/base.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/cell_3d_viewer_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/cell_3d_viewer_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/cell_detector_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/cell_detector_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from dataclasses import replace
 from typing import TYPE_CHECKING, Tuple
 
 import napari
 import napari.layers
 import numpy as np
 from brainways.pipeline.brainways_params import BrainwaysParams, CellDetectorParams
-from brainways.pipeline.cell_detector import ClaheNormalizer
-from napari.qt.threading import FunctionWorker, create_worker
 
 from napari_brainways.controllers.base import Controller
 from napari_brainways.utils import update_layer_contrast_limits
 from napari_brainways.widgets.cell_detector_widget import CellDetectorWidget
 
 if TYPE_CHECKING:
     from napari_brainways.brainways_ui import BrainwaysUI
@@ -27,15 +25,15 @@
 
         self.input_layer = None
         self.preview_box_layer: napari.layers.Points | None = None
         self.crop_layer: napari.layers.Image | None = None
         self.cell_mask_layer: napari.layers.Image | None = None
         self._run_lock = False
         self._params = None
-        self._worker = None
+        self._crop = None
 
     @property
     def name(self) -> str:
         return "Cell Detection"
 
     @staticmethod
     def has_current_step_params(params: BrainwaysParams) -> bool:
@@ -44,70 +42,67 @@
     @staticmethod
     def enabled(params: BrainwaysParams) -> bool:
         return True
 
     def default_params(
         self, image: np.ndarray, params: BrainwaysParams
     ) -> BrainwaysParams:
-        preview_bb = self.selected_bounding_box(
-            image, point=(0.5 * image.shape[0], 0.5 * image.shape[1])
-        )
-        return replace(
-            params,
-            cell=CellDetectorParams(
-                diameter=25.0,
-                net_avg=True,
-                flow_threshold=0.4,
-                mask_threshold=0.0,
-                preview_bb=preview_bb,
-            ),
-        )
+        return params
 
     def run_model(self, image: np.ndarray, params: BrainwaysParams) -> BrainwaysParams:
         return params
 
     def show(
         self,
         params: BrainwaysParams,
         image: np.ndarray | None = None,
         from_ui: bool = False,
     ) -> None:
         self._params = params
 
+        if self._params.cell is not None:
+            cell_detector_params = self._params.cell
+        else:
+            cell_detector_params = self.ui.project.settings.default_cell_detector_params
+
         if image is not None:
             self.input_layer.data = image
             update_layer_contrast_limits(self.input_layer)
 
-        params_widget = self.widget.cell_detector_params_widget
-        params_widget.diameter.value = params.cell.diameter
-        params_widget.net_avg.value = params.cell.net_avg
-        params_widget.flow_threshold.value = params.cell.flow_threshold
-        params_widget.mask_threshold.value = params.cell.mask_threshold
-
-        x0 = params.cell.preview_bb[0]
-        y0 = params.cell.preview_bb[1]
-        x1 = params.cell.preview_bb[0] + params.cell.preview_bb[2]
-        y1 = params.cell.preview_bb[1] + params.cell.preview_bb[3]
-        self.preview_box_layer.data = (
-            np.array([[y0, x0], [y0, x1], [y1, x1], [y1, x0]])
-            * self.input_layer.data.shape
-        )
+            x0, y0, w, h = self.selected_bounding_box(
+                image, point=(0.5 * image.shape[0], 0.5 * image.shape[1])
+            )
+            x1 = x0 + w
+            y1 = y0 + h
+            self.preview_box_layer.data = (
+                np.array([[y0, x0], [y0, x1], [y1, x1], [y1, x0]])
+                * self.input_layer.data.shape
+            )
+
+        if not from_ui:
+            self.widget.set_cell_detector_params(
+                normalizer=cell_detector_params.normalizer,
+                normalizer_range=cell_detector_params.normalizer_range,
+                unique=self._params.cell is not None,
+            )
+
         self.on_click()
         self.set_preview_affine()
 
         self.ui.viewer.reset_view()
 
     def load_model(self) -> None:
         from brainways.pipeline.cell_detector import CellDetector
 
         if self.model is None:
             self.model = CellDetector()
 
     def open(self) -> None:
-        self.widget.show()
+        if self._is_open:
+            return
 
         self.input_layer = self.ui.viewer.add_image(
             np.zeros((512, 512), np.uint8),
             name="Input",
         )
         self.input_layer.translate = (0, 0)
 
@@ -137,14 +132,15 @@
         self.ui.viewer.layers.remove(self.input_layer)
         self.ui.viewer.layers.remove(self.preview_box_layer)
         self.ui.viewer.layers.remove(self.crop_layer)
         self.ui.viewer.layers.remove(self.cell_mask_layer)
 
         self._image = None
         self._params = None
+        self._crop = None
 
         self.input_layer = None
         self.preview_box_layer = None
         self.crop_layer = None
         self.cell_mask_layer = None
         self._image_reader = None
         self._is_open = False
@@ -165,73 +161,94 @@
     def set_preview_affine(self):
         self.crop_layer.translate = self._preview_translate
         self.cell_mask_layer.translate = self._preview_translate
         self.crop_layer.scale = self._preview_scale
         self.cell_mask_layer.scale = self._preview_scale
 
     def _on_cell_detector_returned(self, mask: np.ndarray):
+        if self._params.cell is not None:
+            cell_detector_params = self._params.cell
+        else:
+            cell_detector_params = self.ui.project.settings.default_cell_detector_params
+        normalizer = self.model.get_normalizer(cell_detector_params)
+        if normalizer is not None:
+            self.crop_layer.data = normalizer.before(self._crop, axes=None).squeeze()
+            update_layer_contrast_limits(
+                self.crop_layer, contrast_limits_quantiles=(0.0, 1.0)
+            )
         self.cell_mask_layer.data = mask
         self.cell_mask_layer.visible = True
         self.ui.viewer.layers.selection = {self.preview_box_layer}
+        self.ui.widget.hide_progress_bar()
 
-    def _on_cell_detector_started(self):
-        self._run_lock = True
-        self.widget.show_progress_bar()
-
-    def _on_cell_detector_finished(self):
-        self._run_lock = False
-        self.widget.hide_progress_bar()
-
-    def run_cell_detector_preview_async(
+    def on_params_changed(
         self,
-        diameter: float,
-        net_avg: bool,
-        flow_threshold: float,
-        mask_threshold: float,
+        normalizer: str,
+        min_value: float,
+        max_value: float,
+        unique: bool = False,
     ):
-        self._check_is_open()
+        if max_value <= min_value:
+            max_value = min(1, min_value + 0.001)
+        normalizer_range = (min_value / 1000, max_value / 1000)
+        cell_detector_params = CellDetectorParams(
+            normalizer=normalizer, normalizer_range=normalizer_range
+        )
+        if unique:
+            # in unique mode, set cell detector params unique to current slice
+            self._params = replace(self._params, cell=cell_detector_params)
+        elif self._params.cell is not None:
+            # if changing from unique mode to non-unique mode, remove unique and set
+            # default params
+            self._params = replace(self._params, cell=None)
+            p = self.ui.project.settings.default_cell_detector_params
+            self.widget.set_cell_detector_params(
+                normalizer=p.normalizer,
+                normalizer_range=p.normalizer_range,
+                unique=False,
+            )
+        else:
+            # in default mode, change project default settings
+            self.ui.project.settings = replace(
+                self.ui.project.settings,
+                default_cell_detector_params=cell_detector_params,
+            )
 
+    def _run_cell_detector_on_preview(self):
         self.load_model()
-        self._worker: FunctionWorker = create_worker(
-            self.model.run_cell_detector,
-            self.crop_layer.data,
-            normalizer=ClaheNormalizer(),
-            # diameter=diameter,
-            # net_avg=net_avg,
-            # flow_threshold=flow_threshold,
-            # mask_threshold=mask_threshold,
+        self.ui.save_subject()
+
+        if self._params.cell is not None:
+            cell_detector_params = self._params.cell
+        else:
+            cell_detector_params = self.ui.project.settings.default_cell_detector_params
+        return self.model.run_cell_detector(
+            image=self._crop, params=cell_detector_params
+        )
+
+    def run_cell_detector_preview_async(self):
+        self._check_is_open()
+
+        self.ui.do_work_async(
+            self._run_cell_detector_on_preview,
+            return_callback=self._on_cell_detector_returned,
+            progress_label="Running cell detector on preview...",
         )
-        self._worker.returned.connect(self._on_cell_detector_returned)
-        self._worker.started.connect(self._on_cell_detector_started)
-        self._worker.finished.connect(self._on_cell_detector_finished)
-        self._worker.start()
 
     @property
     def params(self) -> BrainwaysParams:
-        params_widget = self.widget.cell_detector_params_widget
-        params = replace(
-            self._params,
-            cell=CellDetectorParams(
-                diameter=params_widget.diameter.value,
-                net_avg=params_widget.net_avg.value,
-                flow_threshold=params_widget.flow_threshold.value,
-                mask_threshold=params_widget.mask_threshold.value,
-                preview_bb=self.selected_bounding_box(),
-            ),
-        )
-        return params
+        return self._params
 
     def selected_bounding_box(
         self, image: np.ndarray | None = None, point: Tuple[float, float] | None = None
     ):
         """
 
         :return: x, y, w, h
         """
-        # TODO: convert points layer to shapes
         if image is None:
             image = self.input_layer.data
 
         if point is None:
             box = self.preview_box_layer.data[-1] / image.shape
             x = box[0, 1]
             y = box[0, 0]
@@ -282,13 +299,24 @@
                 "YX",
                 X=slice(x0, x1),
                 Y=slice(y0, y1),
                 C=self.ui.current_subject.settings.channel,
             )
             .compute()
         )
-        self.crop_layer.data = highres_crop
-        update_layer_contrast_limits(
-            self.crop_layer, contrast_limits_quantiles=(0, 0.98)
-        )
-        self.cell_mask_layer.data = np.zeros_like(self.crop_layer.data, dtype=np.uint8)
+
+        # if self._params.cell is not None:
+        #     cell_detector_params = self._params.cell
+        # else:
+        #     cell_detector_params = self.ui.project.settings.default_cell_detector_params
+        # normalizer = get_normalizer(
+        #     name=cell_detector_params.normalizer,
+        #     range=cell_detector_params.normalizer_range,
+        # )
+        # if normalizer is not None:
+        #     highres_crop = normalizer.before(highres_crop).squeeze()
+
+        self._crop = highres_crop
+        self.crop_layer.data = self._crop
+        update_layer_contrast_limits(self.crop_layer)
+        self.cell_mask_layer.data = np.zeros_like(self._crop, dtype=np.uint8)
         self.set_preview_affine()
```

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/registration_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/registration_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/controllers/tps_controller.py` & `napari_brainways-0.1.4/src/napari_brainways/controllers/tps_controller.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/napari.yaml` & `napari_brainways-0.1.4/src/napari_brainways/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/napari_reader.py` & `napari_brainways-0.1.4/src/napari_brainways/napari_reader.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/resources/logo.png` & `napari_brainways-0.1.4/src/napari_brainways/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/test_utils.py` & `napari_brainways-0.1.4/src/napari_brainways/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/utils.py` & `napari_brainways-0.1.4/src/napari_brainways/utils.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_create_project_dialog.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_create_project_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/_tests/test_registration_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/_tests/test_registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/affine_2d_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/affine_2d_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/cell_viewer_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/cell_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/create_subject_dialog.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/create_subject_dialog.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/registration_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/registration_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/tps_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/tps_widget.py`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/src/napari_brainways/widgets/workflow_widget.py` & `napari_brainways-0.1.4/src/napari_brainways/widgets/workflow_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,18 @@
             self,
             "New Brainways Project",
             self._prev_path,
             "Brainways Project File (*.bwp)",
         )
         if path == "":
             return
+
+        if Path(path).suffix == "":
+            path += ".bwp"
+
         self._prev_path = str(Path(path).parent)
 
         available_atlases = list(get_all_atlases_lastversions().keys())
         user_values = request_values(
             title="New Brainways Project",
             atlas=dict(
                 value="whs_sd_rat_39um",
@@ -510,15 +514,15 @@
     @property
     def max(self):
         return self.selector_widget.value.max
 
     @max.setter
     def max(self, value: int):
         self.selector_widget.value.max = value
-        self.selector_max_label.value = f"/ {value}"
+        self.selector_max_label.setText(f"/ {value}")
 
     @property
     def visible(self) -> bool:
         return self.isVisible()
 
     @visible.setter
     def visible(self, value: bool):
```

### Comparing `napari_brainways-0.1.3/src/napari_brainways.egg-info/PKG-INFO` & `napari_brainways-0.1.4/src/napari_brainways.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-brainways
-Version: 0.1.3
+Version: 0.1.4
 Summary: Brainways UI
 Home-page: https://github.com/bkntr/napari-brainways
 Author: Ben Kantor
 Author-email: benkantor@mail.tau.ac.il
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/bkntr/napari-brainways/issues
 Project-URL: Documentation, https://github.com/bkntr/napari-brainways#README.md
```

### Comparing `napari_brainways-0.1.3/src/napari_brainways.egg-info/SOURCES.txt` & `napari_brainways-0.1.4/src/napari_brainways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_brainways-0.1.3/tox.ini` & `napari_brainways-0.1.4/tox.ini`

 * *Files identical despite different names*

