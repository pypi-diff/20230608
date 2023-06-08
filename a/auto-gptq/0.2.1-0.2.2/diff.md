# Comparing `tmp/auto_gptq-0.2.1.tar.gz` & `tmp/auto_gptq-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.2.1.tar", last modified: Fri Jun  2 11:09:39 2023, max compression
+gzip compressed data, was "auto_gptq-0.2.2.tar", last modified: Thu Jun  8 06:07:58 2023, max compression
```

## Comparing `auto_gptq-0.2.1.tar` & `auto_gptq-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.872119 auto_gptq-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-06-02 11:09:39.868119 auto_gptq-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.864119 auto_gptq-0.2.1/auto_gptq/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.864119 auto_gptq-0.2.1/auto_gptq/eval_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.864119 auto_gptq-0.2.1/auto_gptq/eval_tasks/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/language_modeling_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/eval_tasks/text_summarization_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.868119 auto_gptq-0.2.1/auto_gptq/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35910 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/gpt_bigcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/moss.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/modeling/rw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.868119 auto_gptq-0.2.1/auto_gptq/nn_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/_fused_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/fused_gptj_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/fused_llama_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/fused_llama_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/qlinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/qlinear_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/qlinear_triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.868119 auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/custom_autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)    13785 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.868119 auto_gptq-0.2.1/auto_gptq/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/quantization/gptq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/quantization/quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.868119 auto_gptq-0.2.1/auto_gptq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/auto_gptq/utils/import_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:09:39.864119 auto_gptq-0.2.1/auto_gptq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-06-02 11:09:39.000000 auto_gptq-0.2.1/auto_gptq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-02 11:09:39.000000 auto_gptq-0.2.1/auto_gptq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:09:39.000000 auto_gptq-0.2.1/auto_gptq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-02 11:09:39.000000 auto_gptq-0.2.1/auto_gptq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 11:09:39.000000 auto_gptq-0.2.1/auto_gptq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:09:39.872119 auto_gptq-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-02 11:09:26.000000 auto_gptq-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.366150 auto_gptq-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-06-08 06:07:58.365151 auto_gptq-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14908 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.357151 auto_gptq-0.2.2/auto_gptq/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.359151 auto_gptq-0.2.2/auto_gptq/eval_tasks/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.360150 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/text_summarization_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.362151 auto_gptq-0.2.2/auto_gptq/modeling/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35910 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/modeling/_base.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/_const.py
+-rw-r--r--   0 root         (0) root         (0)     6906 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/modeling/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3868 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/modeling/auto.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/bloom.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/codegen.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gpt2.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gpt_bigcode.py
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gpt_neox.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gptj.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/llama.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/moss.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/opt.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/rw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.363150 auto_gptq-0.2.2/auto_gptq/nn_modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/_fused_base.py
+-rw-r--r--   0 root         (0) root         (0)    10938 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/fused_gptj_attn.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_attn.py
+-rw-r--r--   0 root         (0) root         (0)    13313 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_mlp.py
+-rw-r--r--   0 root         (0) root         (0)    10697 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear.py
+-rw-r--r--   0 root         (0) root         (0)    10924 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_old.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.364151 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+-rw-r--r--   0 root         (0) root         (0)    13785 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/kernels.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.364151 auto_gptq-0.2.2/auto_gptq/quantization/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5835 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/quantization/gptq.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/quantization/quantizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.365151 auto_gptq-0.2.2/auto_gptq/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/utils/import_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.358151 auto_gptq-0.2.2/auto_gptq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.365151 auto_gptq-0.2.2/autogptq_cuda/
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/autogptq_cuda/autogptq_cuda.cpp
+-rw-r--r--   0 root         (0) root         (0)    39351 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/autogptq_cuda/autogptq_cuda_kernel.cu
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 06:07:58.366150 auto_gptq-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3666 2023-06-08 06:07:48.000000 auto_gptq-0.2.2/setup.py
```

### Comparing `auto_gptq-0.2.1/LICENSE` & `auto_gptq-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/PKG-INFO` & `auto_gptq-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_gptq
-Version: 0.2.1
+Version: 0.2.2
 Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ
 Author: PanQiWei
 Keywords: gptq,quantization,large-language-models,pytorch,transformers
 Platform: windows
 Platform: linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto_gptq Version: 0.2.1 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto_gptq Version: 0.2.2 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
```

### Comparing `auto_gptq-0.2.1/README.md` & `auto_gptq-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.2.2/auto_gptq/eval_tasks/_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.2.2/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/eval_tasks/sequence_classification_task.py` & `auto_gptq-0.2.2/auto_gptq/eval_tasks/sequence_classification_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/eval_tasks/text_summarization_task.py` & `auto_gptq-0.2.2/auto_gptq/eval_tasks/text_summarization_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/modeling/_base.py` & `auto_gptq-0.2.2/auto_gptq/modeling/_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/modeling/_utils.py` & `auto_gptq-0.2.2/auto_gptq/modeling/_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/modeling/auto.py` & `auto_gptq-0.2.2/auto_gptq/modeling/auto.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/modeling/gptj.py` & `auto_gptq-0.2.2/auto_gptq/modeling/gptj.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/modeling/llama.py` & `auto_gptq-0.2.2/auto_gptq/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/modeling/opt.py` & `auto_gptq-0.2.2/auto_gptq/modeling/opt.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/_fused_base.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/_fused_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/fused_gptj_attn.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/fused_gptj_attn.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/fused_llama_attn.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_attn.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/fused_llama_mlp.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_mlp.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/qlinear.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/qlinear_old.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_old.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/qlinear_triton.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_triton.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/nn_modules/triton_utils/kernels.py` & `auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/kernels.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/quantization/gptq.py` & `auto_gptq-0.2.2/auto_gptq/quantization/gptq.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.2.2/auto_gptq/quantization/quantizer.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/utils/data_utils.py` & `auto_gptq-0.2.2/auto_gptq/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq/utils/import_utils.py` & `auto_gptq-0.2.2/auto_gptq/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.2.1/auto_gptq.egg-info/PKG-INFO` & `auto_gptq-0.2.2/auto_gptq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-gptq
-Version: 0.2.1
+Version: 0.2.2
 Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ
 Author: PanQiWei
 Keywords: gptq,quantization,large-language-models,pytorch,transformers
 Platform: windows
 Platform: linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-gptq Version: 0.2.1 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto-gptq Version: 0.2.2 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
```

### Comparing `auto_gptq-0.2.1/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.2.2/auto_gptq.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -43,8 +43,10 @@
 auto_gptq/nn_modules/triton_utils/kernels.py
 auto_gptq/nn_modules/triton_utils/mixin.py
 auto_gptq/quantization/__init__.py
 auto_gptq/quantization/gptq.py
 auto_gptq/quantization/quantizer.py
 auto_gptq/utils/__init__.py
 auto_gptq/utils/data_utils.py
-auto_gptq/utils/import_utils.py
+auto_gptq/utils/import_utils.py
+autogptq_cuda/autogptq_cuda.cpp
+autogptq_cuda/autogptq_cuda_kernel.cu
```

### Comparing `auto_gptq-0.2.1/setup.py` & `auto_gptq-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 python_min_version_str = '.'.join(map(str, python_min_version))
 if sys.version_info < python_min_version:
     print(f"You are using Python {platform.python_version()}. Python >={python_min_version_str} is required.")
     sys.exit(-1)
 
 CUDA_VERSION = "".join(os.environ.get("CUDA_VERSION", "").split("."))
 
-version = "0.2.1" + (f"+cu{CUDA_VERSION}" if CUDA_VERSION and IN_GITHUB_ACTIONS else "")
+version = "0.2.2" + (f"+cu{CUDA_VERSION}" if CUDA_VERSION and IN_GITHUB_ACTIONS else "")
 common_setup_kwargs = {
     "version": version,
     "name": "auto_gptq",
     "author": "PanQiWei",
     "description": "An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.",
-    "long_description": (Path(__file__).parent / "README.md").read_text(),
+    "long_description": (Path(__file__).parent / "README.md").read_text(encoding="UTF-8"),
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/PanQiWei/AutoGPTQ",
     "keywords": ["gptq", "quantization", "large-language-models", "pytorch", "transformers"],
     "platforms": ["windows", "linux"],
     "classifiers": [
         "Environment :: GPU :: NVIDIA CUDA :: 11.7",
         "Environment :: GPU :: NVIDIA CUDA :: 11.8",
@@ -84,22 +84,26 @@
         ]
 
         additional_setup_kwargs = {
             "ext_modules": extensions,
             "cmdclass": {'build_ext': cpp_extension.BuildExtension}
         }
     common_setup_kwargs.update(additional_setup_kwargs)
+    print(f"include dirs are: {include_dirs}")
     setup(
         packages=find_packages(),
         install_requires=requirements,
         extras_require=extras_require,
         include_dirs=include_dirs,
         **common_setup_kwargs
     )
 else:
+    print(f"include dirs are: {include_dirs}")
+    for each in include_dirs:
+        assert os.path.isdir(each)
     setup(
         packages=find_packages(),
         install_requires=requirements,
         extras_require=extras_require,
         include_dirs=include_dirs,
         **common_setup_kwargs
     )
```

