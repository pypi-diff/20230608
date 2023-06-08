# Comparing `tmp/saenopy-1.0.0.tar.gz` & `tmp/saenopy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saenopy-1.0.0.tar", max compression
+gzip compressed data, was "saenopy-1.0.1.tar", max compression
```

## Comparing `saenopy-1.0.0.tar` & `saenopy-1.0.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     1065 2023-06-05 15:22:18.996823 saenopy-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2183 2023-06-05 15:22:18.996823 saenopy-1.0.0/README.md
--rw-r--r--   0        0        0     1307 2023-06-05 15:22:19.104823 saenopy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      348 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/__init__.py
--rw-r--r--   0        0        0     1347 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/build_beams.py
--rw-r--r--   0        0        0     1279 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/conjugate_gradient.py
--rw-r--r--   0        0        0     7716 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/examples.py
--rw-r--r--   0        0        0    15307 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/get_deformations.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/__init__.py
--rw-r--r--   0        0        0     3918 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/code_editor.py
--rw-r--r--   0        0        0     7389 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/gui_code.py
--rw-r--r--   0        0        0     4605 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/script_file.py
--rw-r--r--   0        0        0     7099 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/code/syntax.py
--rw-r--r--   0        0        0    19372 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/QExtendedGraphicsView.py
--rw-r--r--   0        0        0    46067 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/QtShortCuts.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/__init__.py
--rw-r--r--   0        0        0    21886 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/gui_classes.py
--rw-r--r--   0        0        0    33197 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/lif_reader.py
--rw-r--r--   0        0        0     6027 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/patch_lifreader.py
--rw-r--r--   0        0        0      282 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/resources.py
--rw-r--r--   0        0        0    15449 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/sigmoid_widget.py
--rw-r--r--   0        0        0     6583 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_preview.py
--rw-r--r--   0        0        0     3848 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector.py
--rw-r--r--   0        0        0     9342 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector_crop.py
--rw-r--r--   0        0        0     3096 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector_leica.py
--rw-r--r--   0        0        0    12078 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/common/stack_selector_tif.py
--rw-r--r--   0        0        0     7192 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/gui_master.py
--rw-r--r--   0        0        0    16079 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/material_fit/gui_fit.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/orientation/__init__.py
--rw-r--r--   0        0        0    51650 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/orientation/gui_orientation.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/solver/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/solver/analyze/__init__.py
--rw-r--r--   0        0        0    20577 2023-06-05 15:22:19.104823 saenopy-1.0.0/saenopy/gui/solver/analyze/plot_window.py
--rw-r--r--   0        0        0     1575 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/gui_solver.py
--rw-r--r--   0        0        0    16165 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/BatchEvaluate.py
--rw-r--r--   0        0        0    11795 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/DeformationDetector.py
--rw-r--r--   0        0        0     4203 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/FittedMesh.py
--rw-r--r--   0        0        0    11660 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/MeshCreator.py
--rw-r--r--   0        0        0    10563 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/PipelineModule.py
--rw-r--r--   0        0        0     1103 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/QTimeSlider.py
--rw-r--r--   0        0        0    14384 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/Regularizer.py
--rw-r--r--   0        0        0    11278 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/ResultView.py
--rw-r--r--   0        0        0    20033 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/StackDisplay.py
--rw-r--r--   0        0        0    12999 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/VTK_Toolbar.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/__init__.py
--rw-r--r--   0        0        0      541 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/code_export.py
--rw-r--r--   0        0        0     6645 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
--rw-r--r--   0        0        0    48390 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/Exporter.py
--rw-r--r--   0        0        0    13704 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
--rw-r--r--   0        0        0    17357 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
--rw-r--r--   0        0        0    18697 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/FiberViewer.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/exporter/__init__.py
--rw-r--r--   0        0        0    11681 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/load_measurement_dialog.py
--rw-r--r--   0        0        0     3868 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/path_editor.py
--rw-r--r--   0        0        0    12003 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/solver/modules/showVectorField.py
--rw-r--r--   0        0        0        0 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/spheroid/__init__.py
--rw-r--r--   0        0        0    93350 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/gui/spheroid/gui_deformation_spheroid.py
--rw-r--r--   0        0        0    53944 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Icon.ico
--rw-r--r--   0        0        0    42003 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Logo.png
--rw-r--r--   0        0        0    77561 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Logo.svg
--rw-r--r--   0        0        0    37691 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/Logo_black.png
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/arrowscale.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/autoscale0.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/autoscale1.ico
--rw-r--r--   0        0        0    48947 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/buttons.svg
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/center0.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/center1.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.108823 saenopy-1.0.0/saenopy/img/contrast0.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/contrast1.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/grid.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/grid2.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/grid3.ico
--rw-r--r--   0        0        0    38885 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/logo_splash.png
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/nan0.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/nan1.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/show_image.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/show_image2.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/show_image3.ico
--rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice0.ico
--rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice1.ico
--rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice2.ico
--rw-r--r--   0        0        0     1150 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/slice_all.ico
--rw-r--r--   0        0        0   121664 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/BFTFM.png
--rw-r--r--   0        0        0   132449 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/BFTFM_2.png
--rw-r--r--   0        0        0   180081 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/Bead_example_icon.png
--rw-r--r--   0        0        0   202759 2023-06-05 15:22:19.112823 saenopy-1.0.0/saenopy/img/thumbnails/Dynamic_icon.png
--rw-r--r--   0        0        0   554429 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/thumbnails/StainedOrganoid_icon.png
--rw-r--r--   0        0        0   263760 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/thumbnails/liver_fibroblast_icon.png
--rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/view_single.ico
--rw-r--r--   0        0        0     3606 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/img/view_two.ico
--rw-r--r--   0        0        0    12192 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/macro.py
--rw-r--r--   0        0        0    12253 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/materials.py
--rw-r--r--   0        0        0     3701 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/mesh.py
--rw-r--r--   0        0        0     5635 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/multigrid_helper.py
--rw-r--r--   0        0        0    22502 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/result_file.py
--rw-r--r--   0        0        0     7754 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/saveable.py
--rw-r--r--   0        0        0    46114 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/solver.py
--rw-r--r--   0        0        0    11190 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/stack.py
--rw-r--r--   0        0        0    17259 2023-06-05 15:22:19.116824 saenopy-1.0.0/saenopy/unused/macro.py
--rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 saenopy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-08 19:47:54.157571 saenopy-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2183 2023-06-08 19:47:54.157571 saenopy-1.0.1/README.md
+-rw-r--r--   0        0        0     1307 2023-06-08 19:47:54.261573 saenopy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/__init__.py
+-rw-r--r--   0        0        0     1347 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/build_beams.py
+-rw-r--r--   0        0        0     1279 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/conjugate_gradient.py
+-rw-r--r--   0        0        0     7716 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/examples.py
+-rw-r--r--   0        0        0    15307 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/get_deformations.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/__init__.py
+-rw-r--r--   0        0        0     3918 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/code_editor.py
+-rw-r--r--   0        0        0     7389 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/gui_code.py
+-rw-r--r--   0        0        0     4605 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/script_file.py
+-rw-r--r--   0        0        0     7099 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/syntax.py
+-rw-r--r--   0        0        0    19372 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/QExtendedGraphicsView.py
+-rw-r--r--   0        0        0    46067 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/QtShortCuts.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/__init__.py
+-rw-r--r--   0        0        0    21886 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/gui_classes.py
+-rw-r--r--   0        0        0    33357 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/lif_reader.py
+-rw-r--r--   0        0        0     6027 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/patch_lifreader.py
+-rw-r--r--   0        0        0      282 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/resources.py
+-rw-r--r--   0        0        0    15449 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/sigmoid_widget.py
+-rw-r--r--   0        0        0     6583 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_preview.py
+-rw-r--r--   0        0        0     3848 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector.py
+-rw-r--r--   0        0        0     9342 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector_crop.py
+-rw-r--r--   0        0        0     3096 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector_leica.py
+-rw-r--r--   0        0        0    12078 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector_tif.py
+-rw-r--r--   0        0        0     7192 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/gui_master.py
+-rw-r--r--   0        0        0    16079 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/material_fit/gui_fit.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/orientation/__init__.py
+-rw-r--r--   0        0        0    51650 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/orientation/gui_orientation.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/analyze/__init__.py
+-rw-r--r--   0        0        0    20715 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/analyze/plot_window.py
+-rw-r--r--   0        0        0     1575 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/gui_solver.py
+-rw-r--r--   0        0        0    16165 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0    11795 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/DeformationDetector.py
+-rw-r--r--   0        0        0     4203 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/FittedMesh.py
+-rw-r--r--   0        0        0    11660 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/MeshCreator.py
+-rw-r--r--   0        0        0    10563 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/PipelineModule.py
+-rw-r--r--   0        0        0     1103 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/QTimeSlider.py
+-rw-r--r--   0        0        0    14384 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/Regularizer.py
+-rw-r--r--   0        0        0    11278 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/ResultView.py
+-rw-r--r--   0        0        0    20033 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/StackDisplay.py
+-rw-r--r--   0        0        0    12999 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/VTK_Toolbar.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/__init__.py
+-rw-r--r--   0        0        0      541 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/code_export.py
+-rw-r--r--   0        0        0     6645 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
+-rw-r--r--   0        0        0    48390 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/Exporter.py
+-rw-r--r--   0        0        0    13704 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
+-rw-r--r--   0        0        0    17357 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
+-rw-r--r--   0        0        0    18697 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/FiberViewer.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/__init__.py
+-rw-r--r--   0        0        0    11681 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/load_measurement_dialog.py
+-rw-r--r--   0        0        0     3868 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/path_editor.py
+-rw-r--r--   0        0        0    12003 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/showVectorField.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/spheroid/__init__.py
+-rw-r--r--   0        0        0    93350 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/spheroid/gui_deformation_spheroid.py
+-rw-r--r--   0        0        0    53944 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Icon.ico
+-rw-r--r--   0        0        0    42003 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Logo.png
+-rw-r--r--   0        0        0    77561 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Logo.svg
+-rw-r--r--   0        0        0    37691 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Logo_black.png
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/arrowscale.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/autoscale0.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/autoscale1.ico
+-rw-r--r--   0        0        0    48947 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/buttons.svg
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/center0.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/center1.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/contrast0.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/contrast1.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/grid.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/grid2.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/grid3.ico
+-rw-r--r--   0        0        0    38885 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/logo_splash.png
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/nan0.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/nan1.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/show_image.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/show_image2.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/show_image3.ico
+-rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice0.ico
+-rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice1.ico
+-rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice2.ico
+-rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice_all.ico
+-rw-r--r--   0        0        0   121664 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/BFTFM.png
+-rw-r--r--   0        0        0   132449 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/BFTFM_2.png
+-rw-r--r--   0        0        0   180081 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/Bead_example_icon.png
+-rw-r--r--   0        0        0   202759 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/Dynamic_icon.png
+-rw-r--r--   0        0        0   554429 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/StainedOrganoid_icon.png
+-rw-r--r--   0        0        0   263760 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/img/thumbnails/liver_fibroblast_icon.png
+-rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/img/view_single.ico
+-rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/img/view_two.ico
+-rw-r--r--   0        0        0    12316 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/macro.py
+-rw-r--r--   0        0        0    12253 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/materials.py
+-rw-r--r--   0        0        0     3701 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/mesh.py
+-rw-r--r--   0        0        0     5635 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/multigrid_helper.py
+-rw-r--r--   0        0        0    22760 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/result_file.py
+-rw-r--r--   0        0        0     7754 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/saveable.py
+-rw-r--r--   0        0        0    46114 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/solver.py
+-rw-r--r--   0        0        0    11130 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/stack.py
+-rw-r--r--   0        0        0    17259 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/unused/macro.py
+-rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 saenopy-1.0.1/PKG-INFO
```

### Comparing `saenopy-1.0.0/LICENSE.txt` & `saenopy-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/README.md` & `saenopy-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 ## Installation
 
 ### Standalone
 To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
 
 Windows
-https://github.com/rgerum/saenopy/releases/download/v1.0.0/saenopy.exe
+https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy.exe
 
 Linux
-https://github.com/rgerum/saenopy/releases/download/v1.0.0/saenopy
+https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy
 
 ### Using Python
 
 If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
 Saenopy can be installed directly using pip:
 
     ``pip install saenopy``
```

### Comparing `saenopy-1.0.0/pyproject.toml` & `saenopy-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saenopy"
-version = "1.0.0"
+version = "1.0.1"
 description = "Semi-elastic fiber optimisation in python."
 authors = ["rgerum <14153051+rgerum@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "saenopy"}]
```

### Comparing `saenopy-1.0.0/saenopy/build_beams.py` & `saenopy-1.0.1/saenopy/build_beams.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/conjugate_gradient.py` & `saenopy-1.0.1/saenopy/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/examples.py` & `saenopy-1.0.1/saenopy/examples.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/get_deformations.py` & `saenopy-1.0.1/saenopy/get_deformations.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/code/code_editor.py` & `saenopy-1.0.1/saenopy/gui/code/code_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/code/gui_code.py` & `saenopy-1.0.1/saenopy/gui/code/gui_code.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/code/script_file.py` & `saenopy-1.0.1/saenopy/gui/code/script_file.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/code/syntax.py` & `saenopy-1.0.1/saenopy/gui/code/syntax.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/QExtendedGraphicsView.py` & `saenopy-1.0.1/saenopy/gui/common/QExtendedGraphicsView.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/QtShortCuts.py` & `saenopy-1.0.1/saenopy/gui/common/QtShortCuts.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/gui_classes.py` & `saenopy-1.0.1/saenopy/gui/common/gui_classes.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/lif_reader.py` & `saenopy-1.0.1/saenopy/gui/common/lif_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,54 +144,55 @@
         elif isinstance(self.filename, io.IOBase):
             image = self.filename
         else:
             raise TypeError(
                 f"expected str, bytes, os.PathLike, or io.IOBase, "
                 f"not {type(self.filename)}"
             )
+        with image:
 
-        # self.offsets[1] is the length of the image
-        if self.offsets[1] == 0:
-            # In the case of a blank image, we can calculate the length from
-            # the metadata in the LIF. When this is read by the parser,
-            # it is set to zero initially.
-            image_len = seek_distance * self.dims.x * self.dims.y
-        else:
-            image_len = int(self.offsets[1] / seek_distance)
-
-        # self.offsets[0] is the offset in the file
-        image.seek(self.offsets[0] + image_len * n)
-
-        # Todo: Update this for 16-bit images if there is a test file
-        if self.offsets[1] == 0:
-            data = b"\00" * image_len
-        else:
-            data = image.read(image_len)
-
-        # LIF files can be either 8-bit of 16-bit.
-        # Because of how the image is read in, all of the raw
-        # data is already in 'data', we just need to tell Pillow
-        # how to set the bit depth
-        # 'L' is 8-bit, 'I;16' is 16 bit
-
-        # len(data) is the number of bytes (8-bit)
-        # However, it is safer to let the lif file tell us the resolution
-        if self.bit_depth[0] == 8:
-            return Image.frombytes("L",
-                                   (self.dims_n[self.display_dims[0]],
-                                    self.dims_n[self.display_dims[1]]),
-                                   data)
-        elif self.bit_depth[0] <= 16:
-            return Image.frombytes("I;16",
-                                   (self.dims_n[self.display_dims[0]],
-                                    self.dims_n[self.display_dims[1]]),
-                                   data)
-        else:
-            raise ValueError("Unknown bit-depth, please submit a bug report"
-                             " on Github")
+            # self.offsets[1] is the length of the image
+            if self.offsets[1] == 0:
+                # In the case of a blank image, we can calculate the length from
+                # the metadata in the LIF. When this is read by the parser,
+                # it is set to zero initially.
+                image_len = seek_distance * self.dims.x * self.dims.y
+            else:
+                image_len = int(self.offsets[1] / seek_distance)
+
+            # self.offsets[0] is the offset in the file
+            image.seek(self.offsets[0] + image_len * n)
+
+            # Todo: Update this for 16-bit images if there is a test file
+            if self.offsets[1] == 0:
+                data = b"\00" * image_len
+            else:
+                data = image.read(image_len)
+
+            # LIF files can be either 8-bit of 16-bit.
+            # Because of how the image is read in, all of the raw
+            # data is already in 'data', we just need to tell Pillow
+            # how to set the bit depth
+            # 'L' is 8-bit, 'I;16' is 16 bit
+
+            # len(data) is the number of bytes (8-bit)
+            # However, it is safer to let the lif file tell us the resolution
+            if self.bit_depth[0] == 8:
+                return Image.frombytes("L",
+                                       (self.dims_n[self.display_dims[0]],
+                                        self.dims_n[self.display_dims[1]]),
+                                       data)
+            elif self.bit_depth[0] <= 16:
+                return Image.frombytes("I;16",
+                                       (self.dims_n[self.display_dims[0]],
+                                        self.dims_n[self.display_dims[1]]),
+                                       data)
+            else:
+                raise ValueError("Unknown bit-depth, please submit a bug report"
+                                 " on Github")
 
     def get_plane(self, display_dims=None, c=0, requested_dims=None):
         """
         Gets the specified frame from image.
 
         Known issue: LASX Navigator saves channel as the second channel, this reader
         will fail in that case.
```

### Comparing `saenopy-1.0.0/saenopy/gui/common/patch_lifreader.py` & `saenopy-1.0.1/saenopy/gui/common/patch_lifreader.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/sigmoid_widget.py` & `saenopy-1.0.1/saenopy/gui/common/sigmoid_widget.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/stack_preview.py` & `saenopy-1.0.1/saenopy/gui/common/stack_preview.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/stack_selector.py` & `saenopy-1.0.1/saenopy/gui/common/stack_selector.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/stack_selector_crop.py` & `saenopy-1.0.1/saenopy/gui/common/stack_selector_crop.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/stack_selector_leica.py` & `saenopy-1.0.1/saenopy/gui/common/stack_selector_leica.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/common/stack_selector_tif.py` & `saenopy-1.0.1/saenopy/gui/common/stack_selector_tif.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/gui_master.py` & `saenopy-1.0.1/saenopy/gui/gui_master.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/material_fit/gui_fit.py` & `saenopy-1.0.1/saenopy/gui/material_fit/gui_fit.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/orientation/gui_orientation.py` & `saenopy-1.0.1/saenopy/gui/orientation/gui_orientation.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/analyze/plot_window.py` & `saenopy-1.0.1/saenopy/gui/solver/analyze/plot_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,18 @@
         def plot(res, mu_name, y_label, color_dict2):
             # define the colors
             color_dict = color_dict2
 
             # iterate over the groups
             for name, data in res.groupby("group", sort=False)[mu_name]:
                 # add the bar with the mean value and the standard error as errorbar
-                plt.bar(name, data.mean(), yerr=data.sem(), error_kw=dict(capsize=5), color=color_dict[name])
+                if np.isnan(data.sem()):
+                    plt.bar(name, data.mean(), color=color_dict[name])
+                else:
+                    plt.bar(name, data.mean(), yerr=data.sem(), error_kw=dict(capsize=5), color=color_dict[name])
                 # add the number of averaged points
                 plt.text(name, data.mean() + data.sem(), f"n={data.count()}", ha="center", va="bottom")
 
             # add ticks and labels
             plt.ylabel(y_label)
             # despine the axes
             plt.gca().spines["top"].set_visible(False)
```

### Comparing `saenopy-1.0.0/saenopy/gui/solver/gui_solver.py` & `saenopy-1.0.1/saenopy/gui/solver/gui_solver.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/BatchEvaluate.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/BatchEvaluate.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/DeformationDetector.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/DeformationDetector.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/FittedMesh.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/FittedMesh.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/MeshCreator.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/MeshCreator.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/PipelineModule.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/PipelineModule.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/QTimeSlider.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/QTimeSlider.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/Regularizer.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/Regularizer.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/ResultView.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/ResultView.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/StackDisplay.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/StackDisplay.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/VTK_Toolbar.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/VTK_Toolbar.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/code_export.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/code_export.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/Exporter.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/Exporter.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender2D.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender2D.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/ExporterRender3D.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender3D.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/exporter/FiberViewer.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/FiberViewer.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/load_measurement_dialog.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/load_measurement_dialog.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/path_editor.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/path_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/solver/modules/showVectorField.py` & `saenopy-1.0.1/saenopy/gui/solver/modules/showVectorField.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/gui/spheroid/gui_deformation_spheroid.py` & `saenopy-1.0.1/saenopy/gui/spheroid/gui_deformation_spheroid.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/Icon.ico` & `saenopy-1.0.1/saenopy/img/Icon.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/Logo.png` & `saenopy-1.0.1/saenopy/img/Logo.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/Logo.svg` & `saenopy-1.0.1/saenopy/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/Logo_black.png` & `saenopy-1.0.1/saenopy/img/Logo_black.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/arrowscale.ico` & `saenopy-1.0.1/saenopy/img/arrowscale.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/autoscale0.ico` & `saenopy-1.0.1/saenopy/img/autoscale0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/autoscale1.ico` & `saenopy-1.0.1/saenopy/img/autoscale1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/buttons.svg` & `saenopy-1.0.1/saenopy/img/buttons.svg`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/center0.ico` & `saenopy-1.0.1/saenopy/img/center0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/center1.ico` & `saenopy-1.0.1/saenopy/img/center1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/contrast0.ico` & `saenopy-1.0.1/saenopy/img/contrast0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/contrast1.ico` & `saenopy-1.0.1/saenopy/img/contrast1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/grid.ico` & `saenopy-1.0.1/saenopy/img/grid.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/grid2.ico` & `saenopy-1.0.1/saenopy/img/grid2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/grid3.ico` & `saenopy-1.0.1/saenopy/img/grid3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/logo_splash.png` & `saenopy-1.0.1/saenopy/img/logo_splash.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/nan0.ico` & `saenopy-1.0.1/saenopy/img/nan0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/nan1.ico` & `saenopy-1.0.1/saenopy/img/nan1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/show_image.ico` & `saenopy-1.0.1/saenopy/img/show_image.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/show_image2.ico` & `saenopy-1.0.1/saenopy/img/show_image2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/show_image3.ico` & `saenopy-1.0.1/saenopy/img/show_image3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/slice0.ico` & `saenopy-1.0.1/saenopy/img/slice0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/slice1.ico` & `saenopy-1.0.1/saenopy/img/slice1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/slice2.ico` & `saenopy-1.0.1/saenopy/img/slice2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/slice_all.ico` & `saenopy-1.0.1/saenopy/img/slice_all.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/thumbnails/BFTFM.png` & `saenopy-1.0.1/saenopy/img/thumbnails/BFTFM.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/thumbnails/BFTFM_2.png` & `saenopy-1.0.1/saenopy/img/thumbnails/BFTFM_2.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/thumbnails/Bead_example_icon.png` & `saenopy-1.0.1/saenopy/img/thumbnails/Bead_example_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/thumbnails/Dynamic_icon.png` & `saenopy-1.0.1/saenopy/img/thumbnails/Dynamic_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/thumbnails/StainedOrganoid_icon.png` & `saenopy-1.0.1/saenopy/img/thumbnails/StainedOrganoid_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/thumbnails/liver_fibroblast_icon.png` & `saenopy-1.0.1/saenopy/img/thumbnails/liver_fibroblast_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/view_single.ico` & `saenopy-1.0.1/saenopy/img/view_single.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/img/view_two.ico` & `saenopy-1.0.1/saenopy/img/view_two.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/macro.py` & `saenopy-1.0.1/saenopy/macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,16 +288,17 @@
                 def cost(p):
                     nonlocal parameter_start
                     parameter_start = parameter_start.copy()
                     parameter_start[mapping_shear] = p
                     p = params(parameter_start)
                     material1 = MaterialClass(*p)
                     x, y = get_shear_rheometer_stress(gamma, material1)
-                    stretchy2 = interp1d(x, y, fill_value=np.nan, bounds_error=False)(shearx)
-                    cost = np.nansum((np.log(stretchy2) - np.log(sheary)) ** 2 * weights)
+                    stretchy2 = interp1d(x, np.clip(y, 1e-9, None), fill_value=np.nan, bounds_error=False)(shearx)
+                    valid_indices = ~np.isnan(stretchy2)
+                    cost = np.nansum((np.log(stretchy2[valid_indices]) - np.log(sheary[valid_indices])) ** 2 * weights[valid_indices])
                     return cost
 
                 def plot_me(color=color):
                     material = MaterialClass(*params(parameter_start))
                     plt.loglog(shearx, sheary, "o", label="data", color=color)
 
                     x, y = get_shear_rheometer_stress(gamma, material)
```

### Comparing `saenopy-1.0.0/saenopy/materials.py` & `saenopy-1.0.1/saenopy/materials.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/mesh.py` & `saenopy-1.0.1/saenopy/mesh.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/multigrid_helper.py` & `saenopy-1.0.1/saenopy/multigrid_helper.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/result_file.py` & `saenopy-1.0.1/saenopy/result_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,16 @@
             # the file needs to exist
             #if not Path(filename).exists():
             #    raise FileNotFoundError(f"Could not find file {filename}")
             if Path(filename).suffix in [".tif", ".tiff"]:
                 with tifffile.TiffFile(filename) as f:
                     file_shape = f.pages[0].shape
             else:
-                im = Image.open(filename)
-                file_shape = (im.height, im.width)
+                with Image.open(filename) as im:
+                    file_shape = (im.height, im.width)
             if shape is None:
                 shape = file_shape
             else:
                 if file_shape != shape:
                     raise ValueError(f"Shape of file {filename} ({file_shape}) does not match previous shape ({shape})")
 
         # create the output path
@@ -407,16 +407,17 @@
             ]
             apply_rename(data_dict, renames)
             apply_delete(data_dict, renames)
 
             data_dict["___save_version__"] = "1.3"
         return super().from_dict(data_dict)
 
-    def __init__(self, output="", template=None, stack=None, time_delta=None, **kwargs):
-        self.output = str(Path(output).absolute())
+    def __init__(self, output=None, template=None, stack=None, time_delta=None, **kwargs):
+        if output is not None:
+            self.output = str(Path(output).absolute())
 
         self.stacks = stack
         if stack is None:
             self.stacks = []
         self.stack_parameters = dict(z_project_name=None, z_project_range=0)
 
         self.state = False
@@ -428,19 +429,20 @@
         else:
             self.mesh_piv = [None] * (len(self.stacks) - 1)
         self.solvers = [None] * (len(self.mesh_piv))
 
         super().__init__(**kwargs)
 
         # add a reference to this instance to the stacks, so they know the path
-        for stack in self.stacks:
-            stack.paths_relative(self)
-        if self.stack_reference is not None:
-            self.stack_reference.paths_relative(self)
-        self.template = make_path_relative(self.template, Path(self.output).parent)
+        if output is not None:
+            for stack in self.stacks:
+                stack.paths_relative(self)
+            if self.stack_reference is not None:
+                self.stack_reference.paths_relative(self)
+            self.template = make_path_relative(self.template, Path(self.output).parent)
 
 
         # if demo move parts to simulate empty result
         if os.environ.get("DEMO") == "true":  # pragma: no cover
             self.mesh_piv_demo = self.mesh_piv
             self.solver_demo = self.solvers
             if self.solvers[0] is not None and getattr(self.solvers[0], "regularisation_results", None):
@@ -479,14 +481,19 @@
         self.solvers[solver_id] = None
         # create a new solver object from the data
         self.solvers[solver_id] = Solver.from_dict(data_dict)
 
     def on_load(self, filename: str):
         self.output = str(Path(filename))
 
+        for stack in self.stacks:
+            stack.parent = self
+        if self.stack_reference is not None:
+            self.stack_reference.parent = self
+
     def __repr__(self):
         folders = [str(Path(stack.template)) for stack in self.stacks]
         base_folder = common_start(folders)
         base_folder = os.sep.join(base_folder.split(os.sep)[:-1])
         indent = "    "
         text = "Result(" + "\n"
         text += indent + "output = " + self.output + "\n"
```

### Comparing `saenopy-1.0.0/saenopy/saveable.py` & `saenopy-1.0.1/saenopy/saveable.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/solver.py` & `saenopy-1.0.1/saenopy/solver.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/saenopy/stack.py` & `saenopy-1.0.1/saenopy/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,32 +63,31 @@
             try:
                 template = Path(template).relative_to(output)
             except ValueError:
                 try:
                     template = Path("..") / Path(template).relative_to(Path(output).parent)
                 except ValueError:
                     try:
-                        template = Path("../..") / Path(template).relative_to(Path(output).parent.parent)
+                        template = Path("..") / ".." / Path(template).relative_to(Path(output).parent.parent)
                     except ValueError:
                         pass
             return str(template)
 
         def process(image):
             if isinstance(image, list):
                 return [process(i) for i in image]
             return normalize_path(image, Path(self.parent.output).parent)
 
         self.template = process(self.template)
         #self.parent.template = process(self.parent.template)
-        print("template", self.template)
+
         if self.image_filenames is not None:
             self.image_filenames = process(self.image_filenames)
         else:
             self.leica_filename = process(self.leica_filename)
-        print(self.image_filenames)
 
     def paths_absolute(self):
         def normalize_path(template, output):
             if not Path(template).is_absolute():
                 return str(Path(output).absolute() / template)
             return str(Path(template).absolute())
 
@@ -217,17 +216,17 @@
         image_filenames = str(image_filenames)
         page = 0
         if image_filenames.endswith("]"):
             image_filenames, page = re.match(r"(.*)\[(\d*)\]", image_filenames).groups()
             page = int(page)
         with tifffile.TiffReader(image_filenames) as tif:
             page = tif.pages[page]
-        if isinstance(page, list):  # pragma: no cover
-            page = page[0]
-        return page.asarray()
+            if isinstance(page, list):  # pragma: no cover
+                page = page[0]
+            return page.asarray()
     im = imageio.v2.imread(image_filenames)
     return im
 
 
 def format_glob(pattern):
     pattern = str(Path(pattern))
```

### Comparing `saenopy-1.0.0/saenopy/unused/macro.py` & `saenopy-1.0.1/saenopy/unused/macro.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.0/PKG-INFO` & `saenopy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saenopy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Semi-elastic fiber optimisation in python.
 License: MIT
 Author: rgerum
 Author-email: 14153051+rgerum@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -59,18 +59,18 @@
 
 ## Installation
 
 ### Standalone
 To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
 
 Windows
-https://github.com/rgerum/saenopy/releases/download/v1.0.0/saenopy.exe
+https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy.exe
 
 Linux
-https://github.com/rgerum/saenopy/releases/download/v1.0.0/saenopy
+https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy
 
 ### Using Python
 
 If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
 Saenopy can be installed directly using pip:
 
     ``pip install saenopy``
```

