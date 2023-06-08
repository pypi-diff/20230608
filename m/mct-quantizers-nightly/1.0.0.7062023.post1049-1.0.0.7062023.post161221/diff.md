# Comparing `tmp/mct-quantizers-nightly-1.0.0.7062023.post1049.tar.gz` & `tmp/mct-quantizers-nightly-1.0.0.7062023.post161221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.0.0.7062023.post1049.tar", last modified: Wed Jun  7 00:10:51 2023, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.0.0.7062023.post161221.tar", last modified: Wed Jun  7 16:12:22 2023, max compression
```

## Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049.tar` & `mct-quantizers-nightly-1.0.0.7062023.post161221.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.273287 mct-quantizers-nightly-1.0.0.7062023.post1049/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-07 00:10:51.273287 mct-quantizers-nightly-1.0.0.7062023.post1049/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.269287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.273287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.273287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-07 00:10:36.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:10:51.273287 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-07 00:10:50.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-07 00:10:51.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:10:50.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 00:10:50.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 00:10:50.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 00:10:51.273287 mct-quantizers-nightly-1.0.0.7062023.post1049/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-07 00:10:49.000000 mct-quantizers-nightly-1.0.0.7062023.post1049/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.855715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-07 16:12:01.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 16:12:22.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 16:12:22.859715 mct-quantizers-nightly-1.0.0.7062023.post161221/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-07 16:12:21.000000 mct-quantizers-nightly-1.0.0.7062023.post161221/setup.py
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/LICENSE.md` & `mct-quantizers-nightly-1.0.0.7062023.post161221/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/PKG-INFO` & `mct-quantizers-nightly-1.0.0.7062023.post161221/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.7062023.post1049
+Version: 1.0.0.7062023.post161221
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Tollkit (MCT) Quantizers
         
         This is an open-source library that provides tools that enable to easily represent a quantized neural network, both in Keras and in PyTorch.
         It provides researchers, developers, and engineers a set of useful quantizers and, in addition, a simple interface for implementing new custom quantizers.
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/README.md` & `mct-quantizers-nightly-1.0.0.7062023.post161221/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
 from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER, FOUND_TF, TRAINING, STEPS
+from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 from mct_quantizers.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
     from keras.utils import tf_inspect
     from tensorflow_model_optimization.python.core.keras import utils
+    from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
+
     keras = tf.keras
 
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
 
         def quantizer_fn():
@@ -70,18 +73,20 @@
 
             Args:
                 config(dict): dictionary  of  ActivationQuantizationHolder Configuration
 
             Returns: A ActivationQuantizationHolder object
 
             """
+            qi_inferable_custom_objects = {subclass.__name__: subclass for subclass in
+                                           get_all_subclasses(BaseKerasInferableQuantizer)}
             config = config.copy()
             activation_holder_quantizer = keras.utils.deserialize_keras_object(config.pop(ACTIVATION_HOLDER_QUANTIZER),
                                                                                module_objects=globals(),
-                                                                               custom_objects=None)
+                                                                               custom_objects=qi_inferable_custom_objects)
 
             return cls(activation_holder_quantizer=activation_holder_quantizer,
                        **config)
 
         def build(self, input_shape):
             """
             ActivationQuantizationHolder build function.
@@ -134,14 +139,15 @@
 
             Returns:
                 None
             """
             if hasattr(self.activation_holder_quantizer, 'convert2inferable') and callable(
                     self.activation_holder_quantizer.convert2inferable):  # pragma: no cover
                 self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
+                return self.from_config(self.get_config()) # return new layer with no weights. It assumes holder of inferable quantizers have no weights
 
 
 else:
     class KerasActivationQuantizationHolder:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
                          'when using ActivationQuantizationHolder. '
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             """
             # Call the superclass constructor with the given parameters, along with the target of Activation
             # quantization
             super(ActivationPOTInferableQuantizer, self).__init__(num_bits=num_bits,
                                                                   threshold=threshold,
                                                                   signed=signed)
 
-            is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in self.threshold.flatten()])
+            is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in np.asarray(self.threshold).flatten()])
             assert is_threshold_pot, f'Expected threshold to be power of 2 but is {self.threshold}'
 
 else:
     class ActivationPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
                          'when using ActivationPOTInferableQuantizer. '
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,25 +44,27 @@
 
             Args:
                 num_bits: number of bits to use for quantization
                 threshold: threshold for quantizing activations
                 signed: whether or not to use signed quantization
             """
             assert isinstance(threshold, list), f'Expected threshold to be of type list but is {type(threshold)}'
+            # In activation per-channel quantization is not supported thus we expect a single min/max value.
+            assert len(threshold) == 1, f'In per-tensor quantization threshold should be of length 1 but is {len(threshold)}'
             assert all([isinstance(x, (float, np.float32, tf.float32)) for x in
                         threshold]), f'Expected threshold list to contain float or np.float values but found ' \
                                      f'{[type(x) for x in threshold]}'
 
-            self.threshold = np.asarray(threshold)
+            self.threshold = threshold
             self.signed = signed
 
-            delta = self.threshold / (2 ** (num_bits - int(self.signed)))
+            delta = self.threshold[0] / (2 ** (num_bits - int(self.signed)))
             # In activation quantization is per-tensor only - thus we pass the threshold as a list with a len of 1
-            min_range = list(-self.threshold) if self.signed else [0.0]
-            max_range = list(self.threshold - delta)
+            min_range = [-threshold[0]] if self.signed else [0.0]
+            max_range = [self.threshold[0] - delta]
 
             super(ActivationSymmetricInferableQuantizer, self).__init__(num_bits=num_bits,
                                                                         min_range=min_range,
                                                                         max_range=max_range)
 
         def get_config(self):
             """
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.7062023.post1049
+Version: 1.0.0.7062023.post161221
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Tollkit (MCT) Quantizers
         
         This is an open-source library that provides tools that enable to easily represent a quantized neural network, both in Keras and in PyTorch.
         It provides researchers, developers, and engineers a set of useful quantizers and, in addition, a simple interface for implementing new custom quantizers.
```

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.0.0.7062023.post161221/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.7062023.post1049/setup.py` & `mct-quantizers-nightly-1.0.0.7062023.post161221/setup.py`

 * *Files identical despite different names*

