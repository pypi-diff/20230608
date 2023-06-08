# Comparing `tmp/autogluon.multimodal-0.7.1b20230606.tar.gz` & `tmp/autogluon.multimodal-0.7.1b20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.7.1b20230606.tar", last modified: Tue Jun  6 09:04:04 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.7.1b20230608.tar", last modified: Thu Jun  8 09:04:22 2023, max compression
```

## Comparing `autogluon.multimodal-0.7.1b20230606.tar` & `autogluon.multimodal-0.7.1b20230608.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.328876 autogluon.multimodal-0.7.1b20230606/
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-06 09:04:04.328876 autogluon.multimodal-0.7.1b20230606/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:04:04.328876 autogluon.multimodal-0.7.1b20230606/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.300876 autogluon.multimodal-0.7.1b20230606/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.300876 autogluon.multimodal-0.7.1b20230606/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.308876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.312876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.312876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.312876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.316876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.316876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35794 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.316876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.320876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.320876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.320876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   118701 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    25625 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.328876 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22253 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-06 09:03:26.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:04:04.304875 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:04:04.000000 autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.766211 autogluon.multimodal-0.7.1b20230608/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-08 09:04:22.766211 autogluon.multimodal-0.7.1b20230608/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:04:22.766211 autogluon.multimodal-0.7.1b20230608/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.738210 autogluon.multimodal-0.7.1b20230608/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.738210 autogluon.multimodal-0.7.1b20230608/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.742210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.746210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.750210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.754211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.754211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.754211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82611 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.758211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.758211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.758211 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17122 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119344 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26148 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.762210 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19409 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53333 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-08 09:03:43.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:22.742210 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:22.000000 autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.7.1b20230606/PKG-INFO` & `autogluon.multimodal-0.7.1b20230608/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230606
+Version: 0.7.1b20230608
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230606/setup.py` & `autogluon.multimodal-0.7.1b20230608/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "tqdm",  # version range defined in `core/_setup_utils.py`
     "boto3",  # version range defined in `core/_setup_utils.py`
     "requests>=2.21,<3",
     "jsonschema>=4.14,<4.18",
     "seqeval>=1.2.2,<1.3.0",
     "evaluate>=0.2.2,<0.4.0",
     "accelerate>=0.9,<0.17",
-    "timm>=0.6.12,<0.7.0",
+    "timm>=0.9.2,<0.10.0",
     "torch>=1.9,<1.14",
     "torchvision<0.15.0",
     "fairscale>=0.4.5,<0.4.14",
     "scikit-image>=0.19.1,<0.20.0",
     "pytorch-lightning>=1.9.0,<1.10.0",
     "text-unidecode>=1.3,<1.4",
     "torchmetrics>=0.11.0,<0.12.0",
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,839 +1,836 @@
 import collections
 import copy
 import logging
 import math
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
+import mmcv
 import numpy as np
 import pandas as pd
 import torch
+from mmcv.transforms import BaseTransform
+from mmcv.transforms.utils import cache_randomness
+from mmdet.structures.bbox import autocast_box_type
+from mmdet.utils import log_img_scale
+from mmengine.config import Config as MMConfig
+from mmengine.dataset import BaseDataset
 from numpy import random
 
 from ...constants import GET_ITEM_ERROR_RETRY, MULTI_IMAGE_MIX_DATASET, ROIS
 from ..preprocess_dataframe import MultiModalFeaturePreprocessor
 from ..utils import apply_data_processor, apply_df_preprocessor, get_per_sample_features
 
 logger = logging.getLogger(__name__)
 
-try:
-    import mmcv
-    from mmcv.transforms import BaseTransform
-    from mmcv.transforms.utils import cache_randomness
-    from mmdet.structures.bbox import autocast_box_type
-    from mmdet.utils import log_img_scale
-    from mmengine.config import Config as MMConfig
-    from mmengine.dataset import BaseDataset
-
-    class MultiImageMixDataset(torch.utils.data.Dataset):
-        """
-        A Pytorch DataSet class to process a multimodal pd.DataFrame. It first uses a preprocessor to
-        produce model-agnostic features. Then, each processor prepares customized data for one modality
-        per model. For code simplicity, here we treat ground-truth label as one modality. This class is
-        independent of specific data modalities and models.
-        """
-
-        def __init__(
-            self,
-            data: pd.DataFrame,
-            preprocessor: List[MultiModalFeaturePreprocessor],
-            processors: List[dict],
-            model_config: MMConfig,
-            id_mappings: Optional[Union[Dict[str, Dict], Dict[str, pd.Series]]] = None,
-            is_training: bool = False,
-        ):
-            """
-            Parameters
-            ----------
-            data
-                A pd.DataFrame containing multimodal features.
-            preprocessor
-                A list of multimodal feature preprocessors generating model-agnostic features.
-            processors
-                Data processors customizing data for each modality per model.
-            id_mappings
-                Id-to-content mappings. The contents can be text, image, etc.
-                This is used when the dataframe contains the query/response indexes instead of their contents.
-            is_training
-                Whether in training mode. Some data processing may be different between training
-                and validation/testing/prediction, e.g., image data augmentation is used only in
-                training.
-            model_config
-                Model config used to decided dataset type. e.g. if multi_image_mix_dataset is used in detection model,
-                MultiImageMixDataset will be used instead of BaseDataset
-            """
-            super().__init__()
-            self.processors = processors
-            self.is_training = is_training
-            self._consecutive_errors = 0
-
-            mix_config = model_config[MULTI_IMAGE_MIX_DATASET]
-            self.mix_data_key = "mmdet_image_image"  # the key of the data to mix, TODO: remove hardcoding
-            self.mix_result_key = "mix_results"  # the key of the mix result to store
-
-            self.mix_transforms = []
-            self.mix_transforms_types = []  # TODO: remove hardcode
-            if "mosaic" in mix_config:
-                self.mix_transforms.append(Mosaic(**mix_config["mosaic"]))
-                self.mix_transforms_types.append("mosaic")
-            if "mixup" in mix_config:
-                self.mix_transforms.append(MixUp(**mix_config["mixup"]))
-                self.mix_transforms_types.append("mixup")
-
-            self._skip_type_keys = None  # TODO: remove hardcode, we need to disable multi image mix in late epochs
-            self.max_refetch = 15  # TODO: remove hardcode (do we need refetch?)
-
-            self.lengths = []
-
-            for i, (per_preprocessor, per_processors_group) in enumerate(zip(preprocessor, processors)):
-                modality_features, modality_types, length = apply_df_preprocessor(
-                    data=data,
-                    df_preprocessor=per_preprocessor,
-                    modalities=per_processors_group.keys(),
-                )
-                self.lengths.append(length)
-                setattr(self, f"modality_features_{i}", modality_features)
-                setattr(self, f"modality_types_{i}", modality_types)
-
-            assert len(set(self.lengths)) == 1
-
-            self.id_mappings = id_mappings
-
-        def __len__(self):
-            """
-            Assume that all modalities have the same sample number.
-
-            Returns
-            -------
-            Sample number in this dataset.
-            """
-            return self.lengths[0]
-
-        def _load_item(self, idx):
-            """
-            Get a single item without mix_results.
-            Iterate through all data processors to prepare model inputs. The data processors are
-            organized first by modalities and then by models.
-
-            Parameters
-            ----------
-            idx
-                Index of sample to process.
-
-            Returns
-            -------
-            Input data formatted as a dictionary.
-            """
-            ret = dict()
-            try:
-                for group_id, per_processors_group in enumerate(self.processors):
-                    per_sample_features = get_per_sample_features(
-                        modality_features=getattr(self, f"modality_features_{group_id}"),
-                        modality_types=getattr(self, f"modality_types_{group_id}"),
-                        idx=idx,
-                        id_mappings=self.id_mappings,
-                    )
-                    per_ret = apply_data_processor(
-                        per_sample_features=per_sample_features,
-                        data_processors=per_processors_group,
-                        feature_modalities=getattr(self, f"modality_types_{group_id}"),
-                        is_training=self.is_training,
-                        load_only=True,
-                    )
-                    ret.update(per_ret)
-            except Exception as e:
-                logger.debug(f"Skipping sample {idx} due to '{e}'")
-                self._consecutive_errors += 1
-                if self._consecutive_errors < GET_ITEM_ERROR_RETRY:
-                    return self.__getitem__((idx + 1) % self.__len__())
-                else:
-                    raise e
-            self._consecutive_errors = 0
-
-            return ret
-
-        def __getitem__(self, idx):
-            """
-            Iterate through all data processors to prepare model inputs. The data processors are
-            organized first by modalities and then by models.
-
-            Parameters
-            ----------
-            idx
-                Index of sample to process.
-
-            Returns
-            -------
-            Input data formatted as a dictionary.
-            """
-            results = copy.deepcopy(self._load_item(idx))
-
-            for (transform, transform_type) in zip(self.mix_transforms, self.mix_transforms_types):
-                assert hasattr(transform, "get_indexes")
-
-                if self._skip_type_keys is not None and transform_type in self._skip_type_keys:
-                    continue
-
-                for i in range(self.max_refetch):
-                    # Make sure the results passed the loading pipeline
-                    # of the original dataset is not None.
-                    indexes = transform.get_indexes(self)
-                    if not isinstance(indexes, collections.abc.Sequence):
-                        indexes = [indexes]
-                    mix_results = [copy.deepcopy(self._load_item(index)[self.mix_data_key]) for index in indexes]
-                    if None not in mix_results:
-                        results[self.mix_data_key][self.mix_result_key] = mix_results
-                        break
-                else:
-                    raise RuntimeError(
-                        "The loading pipeline of the original dataset"
-                        " always return None. Please check the correctness "
-                        "of the dataset and its pipeline."
-                    )
-
-                for i in range(self.max_refetch):
-                    # To confirm the results passed the training pipeline
-                    # of the wrapper is not None.
-                    updated_results = transform(copy.deepcopy(results[self.mix_data_key]))
-                    if updated_results is not None:
-                        results[self.mix_data_key] = updated_results
-                        break
-                else:
-                    raise RuntimeError(
-                        "The training pipeline of the dataset wrapper"
-                        " always return None.Please check the correctness "
-                        "of the dataset and its pipeline."
-                    )
-
-                if self.mix_result_key in results[self.mix_data_key]:
-                    results[self.mix_data_key].pop(self.mix_result_key)
-
-            rois_processor = self.processors[0][ROIS][0]  # TODO: remove hardcode
-            results.update(
-                rois_processor.process_one_loaded_sample(
-                    results,
-                    is_training=True,  # This dataset is used only in training
-                )
+
+class MultiImageMixDataset(torch.utils.data.Dataset):
+    """
+    A Pytorch DataSet class to process a multimodal pd.DataFrame. It first uses a preprocessor to
+    produce model-agnostic features. Then, each processor prepares customized data for one modality
+    per model. For code simplicity, here we treat ground-truth label as one modality. This class is
+    independent of specific data modalities and models.
+    """
+
+    def __init__(
+        self,
+        data: pd.DataFrame,
+        preprocessor: List[MultiModalFeaturePreprocessor],
+        processors: List[dict],
+        model_config: MMConfig,
+        id_mappings: Optional[Union[Dict[str, Dict], Dict[str, pd.Series]]] = None,
+        is_training: bool = False,
+    ):
+        """
+        Parameters
+        ----------
+        data
+            A pd.DataFrame containing multimodal features.
+        preprocessor
+            A list of multimodal feature preprocessors generating model-agnostic features.
+        processors
+            Data processors customizing data for each modality per model.
+        id_mappings
+            Id-to-content mappings. The contents can be text, image, etc.
+            This is used when the dataframe contains the query/response indexes instead of their contents.
+        is_training
+            Whether in training mode. Some data processing may be different between training
+            and validation/testing/prediction, e.g., image data augmentation is used only in
+            training.
+        model_config
+            Model config used to decided dataset type. e.g. if multi_image_mix_dataset is used in detection model,
+            MultiImageMixDataset will be used instead of BaseDataset
+        """
+        super().__init__()
+        self.processors = processors
+        self.is_training = is_training
+        self._consecutive_errors = 0
+
+        mix_config = model_config[MULTI_IMAGE_MIX_DATASET]
+        self.mix_data_key = "mmdet_image_image"  # the key of the data to mix, TODO: remove hardcoding
+        self.mix_result_key = "mix_results"  # the key of the mix result to store
+
+        self.mix_transforms = []
+        self.mix_transforms_types = []  # TODO: remove hardcode
+        if "mosaic" in mix_config:
+            self.mix_transforms.append(Mosaic(**mix_config["mosaic"]))
+            self.mix_transforms_types.append("mosaic")
+        if "mixup" in mix_config:
+            self.mix_transforms.append(MixUp(**mix_config["mixup"]))
+            self.mix_transforms_types.append("mixup")
+
+        self._skip_type_keys = None  # TODO: remove hardcode, we need to disable multi image mix in late epochs
+        self.max_refetch = 15  # TODO: remove hardcode (do we need refetch?)
+
+        self.lengths = []
+
+        for i, (per_preprocessor, per_processors_group) in enumerate(zip(preprocessor, processors)):
+            modality_features, modality_types, length = apply_df_preprocessor(
+                data=data,
+                df_preprocessor=per_preprocessor,
+                modalities=per_processors_group.keys(),
             )
+            self.lengths.append(length)
+            setattr(self, f"modality_features_{i}", modality_features)
+            setattr(self, f"modality_types_{i}", modality_types)
 
-            return results
+        assert len(set(self.lengths)) == 1
 
-    class Mosaic(BaseTransform):
-        """Mosaic augmentation.
+        self.id_mappings = id_mappings
 
-        Given 4 images, mosaic transform combines them into
-        one output image. The output image is composed of the parts from each sub-
-        image.
-
-        .. code:: text
-
-                            mosaic transform
-                            center_x
-                    +------------------------------+
-                    |       pad        |  pad      |
-                    |      +-----------+           |
-                    |      |           |           |
-                    |      |  image1   |--------+  |
-                    |      |           |        |  |
-                    |      |           | image2 |  |
-        center_y   |----+-------------+-----------|
-                    |    |   cropped   |           |
-                    |pad |   image3    |  image4   |
-                    |    |             |           |
-                    +----|-------------+-----------+
-                        |             |
-                        +-------------+
-
-        The mosaic transform steps are as follows:
-
-            1. Choose the mosaic center as the intersections of 4 images
-            2. Get the left top image according to the index, and randomly
-                sample another 3 images from the custom dataset.
-            3. Sub image will be cropped if image is larger than mosaic patch
-
-        Required Keys:
-
-        - img
-        - gt_bboxes (BaseBoxes[torch.float32]) (optional)
-        - gt_bboxes_labels (np.int64) (optional)
-        - gt_ignore_flags (bool) (optional)
-        - mix_results (List[dict])
-
-        Modified Keys:
-
-        - img
-        - img_shape
-        - gt_bboxes (optional)
-        - gt_bboxes_labels (optional)
-        - gt_ignore_flags (optional)
+    def __len__(self):
+        """
+        Assume that all modalities have the same sample number.
 
-        Args:
-            img_scale (Sequence[int]): Image size after mosaic pipeline of single
-                image. The shape order should be (width, height).
-                Defaults to (640, 640).
-            center_ratio_range (Sequence[float]): Center ratio range of mosaic
-                output. Defaults to (0.5, 1.5).
-            bbox_clip_border (bool, optional): Whether to clip the objects outside
-                the border of the image. In some dataset like MOT17, the gt bboxes
-                are allowed to cross the border of images. Therefore, we don't
-                need to clip the gt bboxes in these cases. Defaults to True.
-            pad_val (int): Pad value. Defaults to 114.
-            prob (float): Probability of applying this transformation.
-                Defaults to 1.0.
-        """
-
-        def __init__(
-            self,
-            img_scale: Tuple[int, int] = (640, 640),
-            center_ratio_range: Tuple[float, float] = (0.5, 1.5),
-            bbox_clip_border: bool = True,
-            pad_val: float = 114.0,
-            prob: float = 1.0,
-        ) -> None:
-            assert isinstance(img_scale, tuple)
-            assert 0 <= prob <= 1.0, "The probability should be in range [0,1]. " f"got {prob}."
-
-            log_img_scale(img_scale, skip_square=True, shape_order="wh")
-            self.img_scale = img_scale
-            self.center_ratio_range = center_ratio_range
-            self.bbox_clip_border = bbox_clip_border
-            self.pad_val = pad_val
-            self.prob = prob
-
-        @cache_randomness
-        def get_indexes(self, dataset: BaseDataset) -> int:
-            """Call function to collect indexes.
-
-            Args:
-                dataset (:obj:`MultiImageMixDataset`): The dataset.
-
-            Returns:
-                list: indexes.
-            """
-
-            indexes = [random.randint(0, len(dataset)) for _ in range(3)]
-            return indexes
-
-        @autocast_box_type()
-        def transform(self, results: dict) -> dict:
-            """Mosaic transform function.
-
-            Args:
-                results (dict): Result dict.
-
-            Returns:
-                dict: Updated result dict.
-            """
-            if random.uniform(0, 1) > self.prob:
-                return results
-
-            assert "mix_results" in results
-            mosaic_bboxes = []
-            mosaic_bboxes_labels = []
-            mosaic_ignore_flags = []
-            if len(results["img"].shape) == 3:
-                mosaic_img = np.full(
-                    (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2), 3),
-                    self.pad_val,
-                    dtype=results["img"].dtype,
+        Returns
+        -------
+        Sample number in this dataset.
+        """
+        return self.lengths[0]
+
+    def _load_item(self, idx):
+        """
+        Get a single item without mix_results.
+        Iterate through all data processors to prepare model inputs. The data processors are
+        organized first by modalities and then by models.
+
+        Parameters
+        ----------
+        idx
+            Index of sample to process.
+
+        Returns
+        -------
+        Input data formatted as a dictionary.
+        """
+        ret = dict()
+        try:
+            for group_id, per_processors_group in enumerate(self.processors):
+                per_sample_features = get_per_sample_features(
+                    modality_features=getattr(self, f"modality_features_{group_id}"),
+                    modality_types=getattr(self, f"modality_types_{group_id}"),
+                    idx=idx,
+                    id_mappings=self.id_mappings,
                 )
-            else:
-                mosaic_img = np.full(
-                    (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2)), self.pad_val, dtype=results["img"].dtype
+                per_ret = apply_data_processor(
+                    per_sample_features=per_sample_features,
+                    data_processors=per_processors_group,
+                    feature_modalities=getattr(self, f"modality_types_{group_id}"),
+                    is_training=self.is_training,
+                    load_only=True,
                 )
+                ret.update(per_ret)
+        except Exception as e:
+            logger.debug(f"Skipping sample {idx} due to '{e}'")
+            self._consecutive_errors += 1
+            if self._consecutive_errors < GET_ITEM_ERROR_RETRY:
+                return self.__getitem__((idx + 1) % self.__len__())
+            else:
+                raise e
+        self._consecutive_errors = 0
 
-            # mosaic center x, y
-            center_x = int(random.uniform(*self.center_ratio_range) * self.img_scale[0])
-            center_y = int(random.uniform(*self.center_ratio_range) * self.img_scale[1])
-            center_position = (center_x, center_y)
-
-            loc_strs = ("top_left", "top_right", "bottom_left", "bottom_right")
-            for i, loc in enumerate(loc_strs):
-                if loc == "top_left":
-                    results_patch = copy.deepcopy(results)
-                else:
-                    results_patch = copy.deepcopy(results["mix_results"][i - 1])
-
-                img_i = results_patch["img"]
-                h_i, w_i = img_i.shape[:2]
-                # keep_ratio resize
-                scale_ratio_i = min(self.img_scale[1] / h_i, self.img_scale[0] / w_i)
-                img_i = mmcv.imresize(img_i, (int(w_i * scale_ratio_i), int(h_i * scale_ratio_i)))
-
-                # compute the combine parameters
-                paste_coord, crop_coord = self._mosaic_combine(loc, center_position, img_i.shape[:2][::-1])
-                x1_p, y1_p, x2_p, y2_p = paste_coord
-                x1_c, y1_c, x2_c, y2_c = crop_coord
-
-                # crop and paste image
-                mosaic_img[y1_p:y2_p, x1_p:x2_p] = img_i[y1_c:y2_c, x1_c:x2_c]
-
-                # adjust coordinate
-                gt_bboxes_i = results_patch["gt_bboxes"]
-                gt_bboxes_labels_i = results_patch["gt_bboxes_labels"]
-                gt_ignore_flags_i = results_patch["gt_ignore_flags"]
-
-                padw = x1_p - x1_c
-                padh = y1_p - y1_c
-                gt_bboxes_i.rescale_([scale_ratio_i, scale_ratio_i])
-                gt_bboxes_i.translate_([padw, padh])
-                mosaic_bboxes.append(gt_bboxes_i)
-                mosaic_bboxes_labels.append(gt_bboxes_labels_i)
-                mosaic_ignore_flags.append(gt_ignore_flags_i)
-
-            mosaic_bboxes = mosaic_bboxes[0].cat(mosaic_bboxes, 0)
-            mosaic_bboxes_labels = np.concatenate(mosaic_bboxes_labels, 0)
-            mosaic_ignore_flags = np.concatenate(mosaic_ignore_flags, 0)
+        return ret
 
-            if self.bbox_clip_border:
-                mosaic_bboxes.clip_([2 * self.img_scale[1], 2 * self.img_scale[0]])
-            # remove outside bboxes
-            inside_inds = mosaic_bboxes.is_inside([2 * self.img_scale[1], 2 * self.img_scale[0]]).numpy()
-            mosaic_bboxes = mosaic_bboxes[inside_inds]
-            mosaic_bboxes_labels = mosaic_bboxes_labels[inside_inds]
-            mosaic_ignore_flags = mosaic_ignore_flags[inside_inds]
-
-            results["img"] = mosaic_img
-            results["img_shape"] = mosaic_img.shape[:2]
-            results["gt_bboxes"] = mosaic_bboxes
-            results["gt_bboxes_labels"] = mosaic_bboxes_labels
-            results["gt_ignore_flags"] = mosaic_ignore_flags
-            return results
+    def __getitem__(self, idx):
+        """
+        Iterate through all data processors to prepare model inputs. The data processors are
+        organized first by modalities and then by models.
 
-        def _mosaic_combine(
-            self, loc: str, center_position_xy: Sequence[float], img_shape_wh: Sequence[int]
-        ) -> Tuple[Tuple[int], Tuple[int]]:
-            """Calculate global coordinate of mosaic image and local coordinate of
-            cropped sub-image.
-
-            Args:
-                loc (str): Index for the sub-image, loc in ('top_left',
-                'top_right', 'bottom_left', 'bottom_right').
-                center_position_xy (Sequence[float]): Mixing center for 4 images,
-                    (x, y).
-                img_shape_wh (Sequence[int]): Width and height of sub-image
-
-            Returns:
-                tuple[tuple[float]]: Corresponding coordinate of pasting and
-                    cropping
-                    - paste_coord (tuple): paste corner coordinate in mosaic image.
-                    - crop_coord (tuple): crop corner coordinate in mosaic image.
-            """
-            assert loc in ("top_left", "top_right", "bottom_left", "bottom_right")
-            if loc == "top_left":
-                # index0 to top left part of image
-                x1, y1, x2, y2 = (
-                    max(center_position_xy[0] - img_shape_wh[0], 0),
-                    max(center_position_xy[1] - img_shape_wh[1], 0),
-                    center_position_xy[0],
-                    center_position_xy[1],
-                )
-                crop_coord = img_shape_wh[0] - (x2 - x1), img_shape_wh[1] - (y2 - y1), img_shape_wh[0], img_shape_wh[1]
+        Parameters
+        ----------
+        idx
+            Index of sample to process.
+
+        Returns
+        -------
+        Input data formatted as a dictionary.
+        """
+        results = copy.deepcopy(self._load_item(idx))
 
-            elif loc == "top_right":
-                # index1 to top right part of image
-                x1, y1, x2, y2 = (
-                    center_position_xy[0],
-                    max(center_position_xy[1] - img_shape_wh[1], 0),
-                    min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
-                    center_position_xy[1],
-                )
-                crop_coord = 0, img_shape_wh[1] - (y2 - y1), min(img_shape_wh[0], x2 - x1), img_shape_wh[1]
+        for (transform, transform_type) in zip(self.mix_transforms, self.mix_transforms_types):
+            assert hasattr(transform, "get_indexes")
+
+            if self._skip_type_keys is not None and transform_type in self._skip_type_keys:
+                continue
 
-            elif loc == "bottom_left":
-                # index2 to bottom left part of image
-                x1, y1, x2, y2 = (
-                    max(center_position_xy[0] - img_shape_wh[0], 0),
-                    center_position_xy[1],
-                    center_position_xy[0],
-                    min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
+            for i in range(self.max_refetch):
+                # Make sure the results passed the loading pipeline
+                # of the original dataset is not None.
+                indexes = transform.get_indexes(self)
+                if not isinstance(indexes, collections.abc.Sequence):
+                    indexes = [indexes]
+                mix_results = [copy.deepcopy(self._load_item(index)[self.mix_data_key]) for index in indexes]
+                if None not in mix_results:
+                    results[self.mix_data_key][self.mix_result_key] = mix_results
+                    break
+            else:
+                raise RuntimeError(
+                    "The loading pipeline of the original dataset"
+                    " always return None. Please check the correctness "
+                    "of the dataset and its pipeline."
                 )
-                crop_coord = img_shape_wh[0] - (x2 - x1), 0, img_shape_wh[0], min(y2 - y1, img_shape_wh[1])
 
+            for i in range(self.max_refetch):
+                # To confirm the results passed the training pipeline
+                # of the wrapper is not None.
+                updated_results = transform(copy.deepcopy(results[self.mix_data_key]))
+                if updated_results is not None:
+                    results[self.mix_data_key] = updated_results
+                    break
             else:
-                # index3 to bottom right part of image
-                x1, y1, x2, y2 = (
-                    center_position_xy[0],
-                    center_position_xy[1],
-                    min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
-                    min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
+                raise RuntimeError(
+                    "The training pipeline of the dataset wrapper"
+                    " always return None.Please check the correctness "
+                    "of the dataset and its pipeline."
                 )
-                crop_coord = 0, 0, min(img_shape_wh[0], x2 - x1), min(y2 - y1, img_shape_wh[1])
 
-            paste_coord = x1, y1, x2, y2
-            return paste_coord, crop_coord
+            if self.mix_result_key in results[self.mix_data_key]:
+                results[self.mix_data_key].pop(self.mix_result_key)
+
+        rois_processor = self.processors[0][ROIS][0]  # TODO: remove hardcode
+        results.update(
+            rois_processor.process_one_loaded_sample(
+                results,
+                is_training=True,  # This dataset is used only in training
+            )
+        )
+
+        return results
 
-        def __repr__(self):
-            repr_str = self.__class__.__name__
-            repr_str += f"(img_scale={self.img_scale}, "
-            repr_str += f"center_ratio_range={self.center_ratio_range}, "
-            repr_str += f"pad_val={self.pad_val}, "
-            repr_str += f"prob={self.prob})"
-            return repr_str
-
-    class MixUp(BaseTransform):
-        """MixUp data augmentation.
-
-        .. code:: text
-
-                            mixup transform
-                    +------------------------------+
-                    | mixup image   |              |
-                    |      +--------|--------+     |
-                    |      |        |        |     |
-                    |---------------+        |     |
-                    |      |                 |     |
-                    |      |      image      |     |
-                    |      |                 |     |
-                    |      |                 |     |
-                    |      |-----------------+     |
-                    |             pad              |
-                    +------------------------------+
-
-        The mixup transform steps are as follows:
-
-            1. Another random image is picked by dataset and embedded in
-            the top left patch(after padding and resizing)
-            2. The target of mixup transform is the weighted average of mixup
-            image and origin image.
-
-        Required Keys:
-
-        - img
-        - gt_bboxes (BaseBoxes[torch.float32]) (optional)
-        - gt_bboxes_labels (np.int64) (optional)
-        - gt_ignore_flags (bool) (optional)
-        - mix_results (List[dict])
-
-
-        Modified Keys:
-
-        - img
-        - img_shape
-        - gt_bboxes (optional)
-        - gt_bboxes_labels (optional)
-        - gt_ignore_flags (optional)
 
+class Mosaic(BaseTransform):
+    """Mosaic augmentation.
+
+    Given 4 images, mosaic transform combines them into
+    one output image. The output image is composed of the parts from each sub-
+    image.
+
+    .. code:: text
+
+                        mosaic transform
+                        center_x
+                +------------------------------+
+                |       pad        |  pad      |
+                |      +-----------+           |
+                |      |           |           |
+                |      |  image1   |--------+  |
+                |      |           |        |  |
+                |      |           | image2 |  |
+    center_y   |----+-------------+-----------|
+                |    |   cropped   |           |
+                |pad |   image3    |  image4   |
+                |    |             |           |
+                +----|-------------+-----------+
+                    |             |
+                    +-------------+
+
+    The mosaic transform steps are as follows:
+
+        1. Choose the mosaic center as the intersections of 4 images
+        2. Get the left top image according to the index, and randomly
+            sample another 3 images from the custom dataset.
+        3. Sub image will be cropped if image is larger than mosaic patch
+
+    Required Keys:
+
+    - img
+    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+    - gt_bboxes_labels (np.int64) (optional)
+    - gt_ignore_flags (bool) (optional)
+    - mix_results (List[dict])
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - gt_bboxes (optional)
+    - gt_bboxes_labels (optional)
+    - gt_ignore_flags (optional)
+
+    Args:
+        img_scale (Sequence[int]): Image size after mosaic pipeline of single
+            image. The shape order should be (width, height).
+            Defaults to (640, 640).
+        center_ratio_range (Sequence[float]): Center ratio range of mosaic
+            output. Defaults to (0.5, 1.5).
+        bbox_clip_border (bool, optional): Whether to clip the objects outside
+            the border of the image. In some dataset like MOT17, the gt bboxes
+            are allowed to cross the border of images. Therefore, we don't
+            need to clip the gt bboxes in these cases. Defaults to True.
+        pad_val (int): Pad value. Defaults to 114.
+        prob (float): Probability of applying this transformation.
+            Defaults to 1.0.
+    """
+
+    def __init__(
+        self,
+        img_scale: Tuple[int, int] = (640, 640),
+        center_ratio_range: Tuple[float, float] = (0.5, 1.5),
+        bbox_clip_border: bool = True,
+        pad_val: float = 114.0,
+        prob: float = 1.0,
+    ) -> None:
+        assert isinstance(img_scale, tuple)
+        assert 0 <= prob <= 1.0, "The probability should be in range [0,1]. " f"got {prob}."
+
+        log_img_scale(img_scale, skip_square=True, shape_order="wh")
+        self.img_scale = img_scale
+        self.center_ratio_range = center_ratio_range
+        self.bbox_clip_border = bbox_clip_border
+        self.pad_val = pad_val
+        self.prob = prob
+
+    @cache_randomness
+    def get_indexes(self, dataset: BaseDataset) -> int:
+        """Call function to collect indexes.
 
         Args:
-            img_scale (Sequence[int]): Image output size after mixup pipeline.
-                The shape order should be (width, height). Defaults to (640, 640).
-            ratio_range (Sequence[float]): Scale ratio of mixup image.
-                Defaults to (0.5, 1.5).
-            flip_ratio (float): Horizontal flip ratio of mixup image.
-                Defaults to 0.5.
-            pad_val (int): Pad value. Defaults to 114.
-            max_iters (int): The maximum number of iterations. If the number of
-                iterations is greater than `max_iters`, but gt_bbox is still
-                empty, then the iteration is terminated. Defaults to 15.
-            bbox_clip_border (bool, optional): Whether to clip the objects outside
-                the border of the image. In some dataset like MOT17, the gt bboxes
-                are allowed to cross the border of images. Therefore, we don't
-                need to clip the gt bboxes in these cases. Defaults to True.
-        """
-
-        def __init__(
-            self,
-            img_scale: Tuple[int, int] = (640, 640),
-            ratio_range: Tuple[float, float] = (0.5, 1.5),
-            flip_ratio: float = 0.5,
-            pad_val: float = 114.0,
-            max_iters: int = 15,
-            bbox_clip_border: bool = True,
-        ) -> None:
-            assert isinstance(img_scale, tuple)
-            log_img_scale(img_scale, skip_square=True, shape_order="wh")
-            self.dynamic_scale = img_scale
-            self.ratio_range = ratio_range
-            self.flip_ratio = flip_ratio
-            self.pad_val = pad_val
-            self.max_iters = max_iters
-            self.bbox_clip_border = bbox_clip_border
-
-        @cache_randomness
-        def get_indexes(self, dataset: BaseDataset) -> int:
-            """Call function to collect indexes.
-
-            Args:
-                dataset (:obj:`MultiImageMixDataset`): The dataset.
-
-            Returns:
-                list: indexes.
-            """
-
-            index = [np.random.randint(0, len(dataset)) for _ in range(1)]
-
-            return index
-
-        @autocast_box_type()
-        def transform(self, results: dict) -> dict:
-            """MixUp transform function.
-
-            Args:
-                results (dict): Result dict.
-
-            Returns:
-                dict: Updated result dict.
-            """
-
-            assert "mix_results" in results
-            assert len(results["mix_results"]) == 1, "MixUp only support 2 images now !"
-
-            if results["mix_results"][0]["gt_bboxes"].shape[0] == 0:
-                # empty bbox
-                return results
-
-            retrieve_results = results["mix_results"][0]
-            retrieve_img = retrieve_results["img"]
-
-            jit_factor = random.uniform(*self.ratio_range)
-            is_filp = random.uniform(0, 1) > self.flip_ratio
-
-            if len(retrieve_img.shape) == 3:
-                out_img = (
-                    np.ones((self.dynamic_scale[1], self.dynamic_scale[0], 3), dtype=retrieve_img.dtype) * self.pad_val
-                )
+            dataset (:obj:`MultiImageMixDataset`): The dataset.
+
+        Returns:
+            list: indexes.
+        """
+
+        indexes = [random.randint(0, len(dataset)) for _ in range(3)]
+        return indexes
+
+    @autocast_box_type()
+    def transform(self, results: dict) -> dict:
+        """Mosaic transform function.
+
+        Args:
+            results (dict): Result dict.
+
+        Returns:
+            dict: Updated result dict.
+        """
+        if random.uniform(0, 1) > self.prob:
+            return results
+
+        assert "mix_results" in results
+        mosaic_bboxes = []
+        mosaic_bboxes_labels = []
+        mosaic_ignore_flags = []
+        if len(results["img"].shape) == 3:
+            mosaic_img = np.full(
+                (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2), 3),
+                self.pad_val,
+                dtype=results["img"].dtype,
+            )
+        else:
+            mosaic_img = np.full(
+                (int(self.img_scale[1] * 2), int(self.img_scale[0] * 2)), self.pad_val, dtype=results["img"].dtype
+            )
+
+        # mosaic center x, y
+        center_x = int(random.uniform(*self.center_ratio_range) * self.img_scale[0])
+        center_y = int(random.uniform(*self.center_ratio_range) * self.img_scale[1])
+        center_position = (center_x, center_y)
+
+        loc_strs = ("top_left", "top_right", "bottom_left", "bottom_right")
+        for i, loc in enumerate(loc_strs):
+            if loc == "top_left":
+                results_patch = copy.deepcopy(results)
             else:
-                out_img = np.ones(self.dynamic_scale[::-1], dtype=retrieve_img.dtype) * self.pad_val
+                results_patch = copy.deepcopy(results["mix_results"][i - 1])
+
+            img_i = results_patch["img"]
+            h_i, w_i = img_i.shape[:2]
+            # keep_ratio resize
+            scale_ratio_i = min(self.img_scale[1] / h_i, self.img_scale[0] / w_i)
+            img_i = mmcv.imresize(img_i, (int(w_i * scale_ratio_i), int(h_i * scale_ratio_i)))
+
+            # compute the combine parameters
+            paste_coord, crop_coord = self._mosaic_combine(loc, center_position, img_i.shape[:2][::-1])
+            x1_p, y1_p, x2_p, y2_p = paste_coord
+            x1_c, y1_c, x2_c, y2_c = crop_coord
+
+            # crop and paste image
+            mosaic_img[y1_p:y2_p, x1_p:x2_p] = img_i[y1_c:y2_c, x1_c:x2_c]
+
+            # adjust coordinate
+            gt_bboxes_i = results_patch["gt_bboxes"]
+            gt_bboxes_labels_i = results_patch["gt_bboxes_labels"]
+            gt_ignore_flags_i = results_patch["gt_ignore_flags"]
+
+            padw = x1_p - x1_c
+            padh = y1_p - y1_c
+            gt_bboxes_i.rescale_([scale_ratio_i, scale_ratio_i])
+            gt_bboxes_i.translate_([padw, padh])
+            mosaic_bboxes.append(gt_bboxes_i)
+            mosaic_bboxes_labels.append(gt_bboxes_labels_i)
+            mosaic_ignore_flags.append(gt_ignore_flags_i)
+
+        mosaic_bboxes = mosaic_bboxes[0].cat(mosaic_bboxes, 0)
+        mosaic_bboxes_labels = np.concatenate(mosaic_bboxes_labels, 0)
+        mosaic_ignore_flags = np.concatenate(mosaic_ignore_flags, 0)
+
+        if self.bbox_clip_border:
+            mosaic_bboxes.clip_([2 * self.img_scale[1], 2 * self.img_scale[0]])
+        # remove outside bboxes
+        inside_inds = mosaic_bboxes.is_inside([2 * self.img_scale[1], 2 * self.img_scale[0]]).numpy()
+        mosaic_bboxes = mosaic_bboxes[inside_inds]
+        mosaic_bboxes_labels = mosaic_bboxes_labels[inside_inds]
+        mosaic_ignore_flags = mosaic_ignore_flags[inside_inds]
+
+        results["img"] = mosaic_img
+        results["img_shape"] = mosaic_img.shape[:2]
+        results["gt_bboxes"] = mosaic_bboxes
+        results["gt_bboxes_labels"] = mosaic_bboxes_labels
+        results["gt_ignore_flags"] = mosaic_ignore_flags
+        return results
+
+    def _mosaic_combine(
+        self, loc: str, center_position_xy: Sequence[float], img_shape_wh: Sequence[int]
+    ) -> Tuple[Tuple[int], Tuple[int]]:
+        """Calculate global coordinate of mosaic image and local coordinate of
+        cropped sub-image.
+
+        Args:
+            loc (str): Index for the sub-image, loc in ('top_left',
+            'top_right', 'bottom_left', 'bottom_right').
+            center_position_xy (Sequence[float]): Mixing center for 4 images,
+                (x, y).
+            img_shape_wh (Sequence[int]): Width and height of sub-image
+
+        Returns:
+            tuple[tuple[float]]: Corresponding coordinate of pasting and
+                cropping
+                - paste_coord (tuple): paste corner coordinate in mosaic image.
+                - crop_coord (tuple): crop corner coordinate in mosaic image.
+        """
+        assert loc in ("top_left", "top_right", "bottom_left", "bottom_right")
+        if loc == "top_left":
+            # index0 to top left part of image
+            x1, y1, x2, y2 = (
+                max(center_position_xy[0] - img_shape_wh[0], 0),
+                max(center_position_xy[1] - img_shape_wh[1], 0),
+                center_position_xy[0],
+                center_position_xy[1],
+            )
+            crop_coord = img_shape_wh[0] - (x2 - x1), img_shape_wh[1] - (y2 - y1), img_shape_wh[0], img_shape_wh[1]
 
-            # 1. keep_ratio resize
-            scale_ratio = min(
-                self.dynamic_scale[1] / retrieve_img.shape[0], self.dynamic_scale[0] / retrieve_img.shape[1]
+        elif loc == "top_right":
+            # index1 to top right part of image
+            x1, y1, x2, y2 = (
+                center_position_xy[0],
+                max(center_position_xy[1] - img_shape_wh[1], 0),
+                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
+                center_position_xy[1],
             )
-            retrieve_img = mmcv.imresize(
-                retrieve_img, (int(retrieve_img.shape[1] * scale_ratio), int(retrieve_img.shape[0] * scale_ratio))
+            crop_coord = 0, img_shape_wh[1] - (y2 - y1), min(img_shape_wh[0], x2 - x1), img_shape_wh[1]
+
+        elif loc == "bottom_left":
+            # index2 to bottom left part of image
+            x1, y1, x2, y2 = (
+                max(center_position_xy[0] - img_shape_wh[0], 0),
+                center_position_xy[1],
+                center_position_xy[0],
+                min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
             )
+            crop_coord = img_shape_wh[0] - (x2 - x1), 0, img_shape_wh[0], min(y2 - y1, img_shape_wh[1])
 
-            # 2. paste
-            out_img[: retrieve_img.shape[0], : retrieve_img.shape[1]] = retrieve_img
+        else:
+            # index3 to bottom right part of image
+            x1, y1, x2, y2 = (
+                center_position_xy[0],
+                center_position_xy[1],
+                min(center_position_xy[0] + img_shape_wh[0], self.img_scale[0] * 2),
+                min(self.img_scale[1] * 2, center_position_xy[1] + img_shape_wh[1]),
+            )
+            crop_coord = 0, 0, min(img_shape_wh[0], x2 - x1), min(y2 - y1, img_shape_wh[1])
 
-            # 3. scale jit
-            scale_ratio *= jit_factor
-            out_img = mmcv.imresize(out_img, (int(out_img.shape[1] * jit_factor), int(out_img.shape[0] * jit_factor)))
-
-            # 4. flip
-            if is_filp:
-                out_img = out_img[:, ::-1, :]
-
-            # 5. random crop
-            ori_img = results["img"]
-            origin_h, origin_w = out_img.shape[:2]
-            target_h, target_w = ori_img.shape[:2]
-            padded_img = np.ones((max(origin_h, target_h), max(origin_w, target_w), 3)) * self.pad_val
-            padded_img = padded_img.astype(np.uint8)
-            padded_img[:origin_h, :origin_w] = out_img
-
-            x_offset, y_offset = 0, 0
-            if padded_img.shape[0] > target_h:
-                y_offset = random.randint(0, padded_img.shape[0] - target_h)
-            if padded_img.shape[1] > target_w:
-                x_offset = random.randint(0, padded_img.shape[1] - target_w)
-            padded_cropped_img = padded_img[y_offset : y_offset + target_h, x_offset : x_offset + target_w]
-
-            # 6. adjust bbox
-            retrieve_gt_bboxes = retrieve_results["gt_bboxes"]
-            retrieve_gt_bboxes.rescale_([scale_ratio, scale_ratio])
-            if self.bbox_clip_border:
-                retrieve_gt_bboxes.clip_([origin_h, origin_w])
+        paste_coord = x1, y1, x2, y2
+        return paste_coord, crop_coord
 
-            if is_filp:
-                retrieve_gt_bboxes.flip_([origin_h, origin_w], direction="horizontal")
+    def __repr__(self):
+        repr_str = self.__class__.__name__
+        repr_str += f"(img_scale={self.img_scale}, "
+        repr_str += f"center_ratio_range={self.center_ratio_range}, "
+        repr_str += f"pad_val={self.pad_val}, "
+        repr_str += f"prob={self.prob})"
+        return repr_str
+
+
+class MixUp(BaseTransform):
+    """MixUp data augmentation.
+
+    .. code:: text
+
+                        mixup transform
+                +------------------------------+
+                | mixup image   |              |
+                |      +--------|--------+     |
+                |      |        |        |     |
+                |---------------+        |     |
+                |      |                 |     |
+                |      |      image      |     |
+                |      |                 |     |
+                |      |                 |     |
+                |      |-----------------+     |
+                |             pad              |
+                +------------------------------+
+
+    The mixup transform steps are as follows:
+
+        1. Another random image is picked by dataset and embedded in
+        the top left patch(after padding and resizing)
+        2. The target of mixup transform is the weighted average of mixup
+        image and origin image.
+
+    Required Keys:
+
+    - img
+    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+    - gt_bboxes_labels (np.int64) (optional)
+    - gt_ignore_flags (bool) (optional)
+    - mix_results (List[dict])
+
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - gt_bboxes (optional)
+    - gt_bboxes_labels (optional)
+    - gt_ignore_flags (optional)
+
+
+    Args:
+        img_scale (Sequence[int]): Image output size after mixup pipeline.
+            The shape order should be (width, height). Defaults to (640, 640).
+        ratio_range (Sequence[float]): Scale ratio of mixup image.
+            Defaults to (0.5, 1.5).
+        flip_ratio (float): Horizontal flip ratio of mixup image.
+            Defaults to 0.5.
+        pad_val (int): Pad value. Defaults to 114.
+        max_iters (int): The maximum number of iterations. If the number of
+            iterations is greater than `max_iters`, but gt_bbox is still
+            empty, then the iteration is terminated. Defaults to 15.
+        bbox_clip_border (bool, optional): Whether to clip the objects outside
+            the border of the image. In some dataset like MOT17, the gt bboxes
+            are allowed to cross the border of images. Therefore, we don't
+            need to clip the gt bboxes in these cases. Defaults to True.
+    """
+
+    def __init__(
+        self,
+        img_scale: Tuple[int, int] = (640, 640),
+        ratio_range: Tuple[float, float] = (0.5, 1.5),
+        flip_ratio: float = 0.5,
+        pad_val: float = 114.0,
+        max_iters: int = 15,
+        bbox_clip_border: bool = True,
+    ) -> None:
+        assert isinstance(img_scale, tuple)
+        log_img_scale(img_scale, skip_square=True, shape_order="wh")
+        self.dynamic_scale = img_scale
+        self.ratio_range = ratio_range
+        self.flip_ratio = flip_ratio
+        self.pad_val = pad_val
+        self.max_iters = max_iters
+        self.bbox_clip_border = bbox_clip_border
+
+    @cache_randomness
+    def get_indexes(self, dataset: BaseDataset) -> int:
+        """Call function to collect indexes.
 
-            # 7. filter
-            cp_retrieve_gt_bboxes = retrieve_gt_bboxes.clone()
-            cp_retrieve_gt_bboxes.translate_([-x_offset, -y_offset])
-            if self.bbox_clip_border:
-                cp_retrieve_gt_bboxes.clip_([target_h, target_w])
+        Args:
+            dataset (:obj:`MultiImageMixDataset`): The dataset.
 
-            # 8. mix up
-            ori_img = ori_img.astype(np.float32)
-            mixup_img = 0.5 * ori_img + 0.5 * padded_cropped_img.astype(np.float32)
-
-            retrieve_gt_bboxes_labels = retrieve_results["gt_bboxes_labels"]
-            retrieve_gt_ignore_flags = retrieve_results["gt_ignore_flags"]
-
-            mixup_gt_bboxes = cp_retrieve_gt_bboxes.cat((results["gt_bboxes"], cp_retrieve_gt_bboxes), dim=0)
-            mixup_gt_bboxes_labels = np.concatenate((results["gt_bboxes_labels"], retrieve_gt_bboxes_labels), axis=0)
-            mixup_gt_ignore_flags = np.concatenate((results["gt_ignore_flags"], retrieve_gt_ignore_flags), axis=0)
+        Returns:
+            list: indexes.
+        """
 
-            # remove outside bbox
-            inside_inds = mixup_gt_bboxes.is_inside([target_h, target_w]).numpy()
-            mixup_gt_bboxes = mixup_gt_bboxes[inside_inds]
-            mixup_gt_bboxes_labels = mixup_gt_bboxes_labels[inside_inds]
-            mixup_gt_ignore_flags = mixup_gt_ignore_flags[inside_inds]
-
-            results["img"] = mixup_img.astype(np.uint8)
-            results["img_shape"] = mixup_img.shape[:2]
-            results["gt_bboxes"] = mixup_gt_bboxes
-            results["gt_bboxes_labels"] = mixup_gt_bboxes_labels
-            results["gt_ignore_flags"] = mixup_gt_ignore_flags
+        index = [np.random.randint(0, len(dataset)) for _ in range(1)]
 
-            return results
+        return index
 
-        def __repr__(self):
-            repr_str = self.__class__.__name__
-            repr_str += f"(dynamic_scale={self.dynamic_scale}, "
-            repr_str += f"ratio_range={self.ratio_range}, "
-            repr_str += f"flip_ratio={self.flip_ratio}, "
-            repr_str += f"pad_val={self.pad_val}, "
-            repr_str += f"max_iters={self.max_iters}, "
-            repr_str += f"bbox_clip_border={self.bbox_clip_border})"
-            return repr_str
-
-    class RandomAffine(BaseTransform):
-        """Random affine transform data augmentation.
-
-        This operation randomly generates affine transform matrix which including
-        rotation, translation, shear and scaling transforms.
-
-        Required Keys:
-
-        - img
-        - gt_bboxes (BaseBoxes[torch.float32]) (optional)
-        - gt_bboxes_labels (np.int64) (optional)
-        - gt_ignore_flags (bool) (optional)
-
-        Modified Keys:
-
-        - img
-        - img_shape
-        - gt_bboxes (optional)
-        - gt_bboxes_labels (optional)
-        - gt_ignore_flags (optional)
+    @autocast_box_type()
+    def transform(self, results: dict) -> dict:
+        """MixUp transform function.
 
         Args:
-            max_rotate_degree (float): Maximum degrees of rotation transform.
-                Defaults to 10.
-            max_translate_ratio (float): Maximum ratio of translation.
-                Defaults to 0.1.
-            scaling_ratio_range (tuple[float]): Min and max ratio of
-                scaling transform. Defaults to (0.5, 1.5).
-            max_shear_degree (float): Maximum degrees of shear
-                transform. Defaults to 2.
-            border (tuple[int]): Distance from width and height sides of input
-                image to adjust output shape. Only used in mosaic dataset.
-                Defaults to (0, 0).
-            border_val (tuple[int]): Border padding values of 3 channels.
-                Defaults to (114, 114, 114).
-            bbox_clip_border (bool, optional): Whether to clip the objects outside
-                the border of the image. In some dataset like MOT17, the gt bboxes
-                are allowed to cross the border of images. Therefore, we don't
-                need to clip the gt bboxes in these cases. Defaults to True.
-        """
-
-        def __init__(
-            self,
-            max_rotate_degree: float = 10.0,
-            max_translate_ratio: float = 0.1,
-            scaling_ratio_range: Tuple[float, float] = (0.5, 1.5),
-            max_shear_degree: float = 2.0,
-            border: Tuple[int, int] = (0, 0),
-            border_val: Tuple[int, int, int] = (114, 114, 114),
-            bbox_clip_border: bool = True,
-        ) -> None:
-            assert 0 <= max_translate_ratio <= 1
-            assert scaling_ratio_range[0] <= scaling_ratio_range[1]
-            assert scaling_ratio_range[0] > 0
-            self.max_rotate_degree = max_rotate_degree
-            self.max_translate_ratio = max_translate_ratio
-            self.scaling_ratio_range = scaling_ratio_range
-            self.max_shear_degree = max_shear_degree
-            self.border = border
-            self.border_val = border_val
-            self.bbox_clip_border = bbox_clip_border
-
-        @cache_randomness
-        def _get_random_homography_matrix(self, height, width):
-            # Rotation
-            rotation_degree = random.uniform(-self.max_rotate_degree, self.max_rotate_degree)
-            rotation_matrix = self._get_rotation_matrix(rotation_degree)
-
-            # Scaling
-            scaling_ratio = random.uniform(self.scaling_ratio_range[0], self.scaling_ratio_range[1])
-            scaling_matrix = self._get_scaling_matrix(scaling_ratio)
-
-            # Shear
-            x_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
-            y_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
-            shear_matrix = self._get_shear_matrix(x_degree, y_degree)
-
-            # Translation
-            trans_x = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * width
-            trans_y = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * height
-            translate_matrix = self._get_translation_matrix(trans_x, trans_y)
-
-            warp_matrix = translate_matrix @ shear_matrix @ rotation_matrix @ scaling_matrix
-            return warp_matrix
-
-        @autocast_box_type()
-        def transform(self, results: dict) -> dict:
-            import cv2  # TODO: support random affine requires cv2
-
-            img = results["img"]
-            height = img.shape[0] + self.border[1] * 2
-            width = img.shape[1] + self.border[0] * 2
-
-            warp_matrix = self._get_random_homography_matrix(height, width)
-
-            img = cv2.warpPerspective(img, warp_matrix, dsize=(width, height), borderValue=self.border_val)
-            results["img"] = img
-            results["img_shape"] = img.shape[:2]
-
-            bboxes = results["gt_bboxes"]
-            num_bboxes = len(bboxes)
-            if num_bboxes:
-                bboxes.project_(warp_matrix)
-                if self.bbox_clip_border:
-                    bboxes.clip_([height, width])
-                # remove outside bbox
-                valid_index = bboxes.is_inside([height, width]).numpy()
-                results["gt_bboxes"] = bboxes[valid_index]
-                results["gt_bboxes_labels"] = results["gt_bboxes_labels"][valid_index]
-                results["gt_ignore_flags"] = results["gt_ignore_flags"][valid_index]
+            results (dict): Result dict.
 
-                if "gt_masks" in results:
-                    raise NotImplementedError("RandomAffine only supports bbox.")
+        Returns:
+            dict: Updated result dict.
+        """
+
+        assert "mix_results" in results
+        assert len(results["mix_results"]) == 1, "MixUp only support 2 images now !"
+
+        if results["mix_results"][0]["gt_bboxes"].shape[0] == 0:
+            # empty bbox
             return results
 
-        def __repr__(self):
-            repr_str = self.__class__.__name__
-            repr_str += f"(max_rotate_degree={self.max_rotate_degree}, "
-            repr_str += f"max_translate_ratio={self.max_translate_ratio}, "
-            repr_str += f"scaling_ratio_range={self.scaling_ratio_range}, "
-            repr_str += f"max_shear_degree={self.max_shear_degree}, "
-            repr_str += f"border={self.border}, "
-            repr_str += f"border_val={self.border_val}, "
-            repr_str += f"bbox_clip_border={self.bbox_clip_border})"
-            return repr_str
-
-        @staticmethod
-        def _get_rotation_matrix(rotate_degrees: float) -> np.ndarray:
-            radian = math.radians(rotate_degrees)
-            rotation_matrix = np.array(
-                [[np.cos(radian), -np.sin(radian), 0.0], [np.sin(radian), np.cos(radian), 0.0], [0.0, 0.0, 1.0]],
-                dtype=np.float32,
-            )
-            return rotation_matrix
+        retrieve_results = results["mix_results"][0]
+        retrieve_img = retrieve_results["img"]
 
-        @staticmethod
-        def _get_scaling_matrix(scale_ratio: float) -> np.ndarray:
-            scaling_matrix = np.array(
-                [[scale_ratio, 0.0, 0.0], [0.0, scale_ratio, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
-            )
-            return scaling_matrix
+        jit_factor = random.uniform(*self.ratio_range)
+        is_filp = random.uniform(0, 1) > self.flip_ratio
 
-        @staticmethod
-        def _get_shear_matrix(x_shear_degrees: float, y_shear_degrees: float) -> np.ndarray:
-            x_radian = math.radians(x_shear_degrees)
-            y_radian = math.radians(y_shear_degrees)
-            shear_matrix = np.array(
-                [[1, np.tan(x_radian), 0.0], [np.tan(y_radian), 1, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
+        if len(retrieve_img.shape) == 3:
+            out_img = (
+                np.ones((self.dynamic_scale[1], self.dynamic_scale[0], 3), dtype=retrieve_img.dtype) * self.pad_val
             )
-            return shear_matrix
-
-        @staticmethod
-        def _get_translation_matrix(x: float, y: float) -> np.ndarray:
-            translation_matrix = np.array([[1, 0.0, x], [0.0, 1, y], [0.0, 0.0, 1.0]], dtype=np.float32)
-            return translation_matrix
+        else:
+            out_img = np.ones(self.dynamic_scale[::-1], dtype=retrieve_img.dtype) * self.pad_val
 
-except Exception as e:
-    MultiImageMixDataset = None
+        # 1. keep_ratio resize
+        scale_ratio = min(self.dynamic_scale[1] / retrieve_img.shape[0], self.dynamic_scale[0] / retrieve_img.shape[1])
+        retrieve_img = mmcv.imresize(
+            retrieve_img, (int(retrieve_img.shape[1] * scale_ratio), int(retrieve_img.shape[0] * scale_ratio))
+        )
+
+        # 2. paste
+        out_img[: retrieve_img.shape[0], : retrieve_img.shape[1]] = retrieve_img
+
+        # 3. scale jit
+        scale_ratio *= jit_factor
+        out_img = mmcv.imresize(out_img, (int(out_img.shape[1] * jit_factor), int(out_img.shape[0] * jit_factor)))
+
+        # 4. flip
+        if is_filp:
+            out_img = out_img[:, ::-1, :]
+
+        # 5. random crop
+        ori_img = results["img"]
+        origin_h, origin_w = out_img.shape[:2]
+        target_h, target_w = ori_img.shape[:2]
+        padded_img = np.ones((max(origin_h, target_h), max(origin_w, target_w), 3)) * self.pad_val
+        padded_img = padded_img.astype(np.uint8)
+        padded_img[:origin_h, :origin_w] = out_img
+
+        x_offset, y_offset = 0, 0
+        if padded_img.shape[0] > target_h:
+            y_offset = random.randint(0, padded_img.shape[0] - target_h)
+        if padded_img.shape[1] > target_w:
+            x_offset = random.randint(0, padded_img.shape[1] - target_w)
+        padded_cropped_img = padded_img[y_offset : y_offset + target_h, x_offset : x_offset + target_w]
+
+        # 6. adjust bbox
+        retrieve_gt_bboxes = retrieve_results["gt_bboxes"]
+        retrieve_gt_bboxes.rescale_([scale_ratio, scale_ratio])
+        if self.bbox_clip_border:
+            retrieve_gt_bboxes.clip_([origin_h, origin_w])
+
+        if is_filp:
+            retrieve_gt_bboxes.flip_([origin_h, origin_w], direction="horizontal")
+
+        # 7. filter
+        cp_retrieve_gt_bboxes = retrieve_gt_bboxes.clone()
+        cp_retrieve_gt_bboxes.translate_([-x_offset, -y_offset])
+        if self.bbox_clip_border:
+            cp_retrieve_gt_bboxes.clip_([target_h, target_w])
+
+        # 8. mix up
+        ori_img = ori_img.astype(np.float32)
+        mixup_img = 0.5 * ori_img + 0.5 * padded_cropped_img.astype(np.float32)
+
+        retrieve_gt_bboxes_labels = retrieve_results["gt_bboxes_labels"]
+        retrieve_gt_ignore_flags = retrieve_results["gt_ignore_flags"]
+
+        mixup_gt_bboxes = cp_retrieve_gt_bboxes.cat((results["gt_bboxes"], cp_retrieve_gt_bboxes), dim=0)
+        mixup_gt_bboxes_labels = np.concatenate((results["gt_bboxes_labels"], retrieve_gt_bboxes_labels), axis=0)
+        mixup_gt_ignore_flags = np.concatenate((results["gt_ignore_flags"], retrieve_gt_ignore_flags), axis=0)
+
+        # remove outside bbox
+        inside_inds = mixup_gt_bboxes.is_inside([target_h, target_w]).numpy()
+        mixup_gt_bboxes = mixup_gt_bboxes[inside_inds]
+        mixup_gt_bboxes_labels = mixup_gt_bboxes_labels[inside_inds]
+        mixup_gt_ignore_flags = mixup_gt_ignore_flags[inside_inds]
+
+        results["img"] = mixup_img.astype(np.uint8)
+        results["img_shape"] = mixup_img.shape[:2]
+        results["gt_bboxes"] = mixup_gt_bboxes
+        results["gt_bboxes_labels"] = mixup_gt_bboxes_labels
+        results["gt_ignore_flags"] = mixup_gt_ignore_flags
+
+        return results
+
+    def __repr__(self):
+        repr_str = self.__class__.__name__
+        repr_str += f"(dynamic_scale={self.dynamic_scale}, "
+        repr_str += f"ratio_range={self.ratio_range}, "
+        repr_str += f"flip_ratio={self.flip_ratio}, "
+        repr_str += f"pad_val={self.pad_val}, "
+        repr_str += f"max_iters={self.max_iters}, "
+        repr_str += f"bbox_clip_border={self.bbox_clip_border})"
+        return repr_str
+
+
+class RandomAffine(BaseTransform):
+    """Random affine transform data augmentation.
+
+    This operation randomly generates affine transform matrix which including
+    rotation, translation, shear and scaling transforms.
+
+    Required Keys:
+
+    - img
+    - gt_bboxes (BaseBoxes[torch.float32]) (optional)
+    - gt_bboxes_labels (np.int64) (optional)
+    - gt_ignore_flags (bool) (optional)
+
+    Modified Keys:
+
+    - img
+    - img_shape
+    - gt_bboxes (optional)
+    - gt_bboxes_labels (optional)
+    - gt_ignore_flags (optional)
+
+    Args:
+        max_rotate_degree (float): Maximum degrees of rotation transform.
+            Defaults to 10.
+        max_translate_ratio (float): Maximum ratio of translation.
+            Defaults to 0.1.
+        scaling_ratio_range (tuple[float]): Min and max ratio of
+            scaling transform. Defaults to (0.5, 1.5).
+        max_shear_degree (float): Maximum degrees of shear
+            transform. Defaults to 2.
+        border (tuple[int]): Distance from width and height sides of input
+            image to adjust output shape. Only used in mosaic dataset.
+            Defaults to (0, 0).
+        border_val (tuple[int]): Border padding values of 3 channels.
+            Defaults to (114, 114, 114).
+        bbox_clip_border (bool, optional): Whether to clip the objects outside
+            the border of the image. In some dataset like MOT17, the gt bboxes
+            are allowed to cross the border of images. Therefore, we don't
+            need to clip the gt bboxes in these cases. Defaults to True.
+    """
+
+    def __init__(
+        self,
+        max_rotate_degree: float = 10.0,
+        max_translate_ratio: float = 0.1,
+        scaling_ratio_range: Tuple[float, float] = (0.5, 1.5),
+        max_shear_degree: float = 2.0,
+        border: Tuple[int, int] = (0, 0),
+        border_val: Tuple[int, int, int] = (114, 114, 114),
+        bbox_clip_border: bool = True,
+    ) -> None:
+        assert 0 <= max_translate_ratio <= 1
+        assert scaling_ratio_range[0] <= scaling_ratio_range[1]
+        assert scaling_ratio_range[0] > 0
+        self.max_rotate_degree = max_rotate_degree
+        self.max_translate_ratio = max_translate_ratio
+        self.scaling_ratio_range = scaling_ratio_range
+        self.max_shear_degree = max_shear_degree
+        self.border = border
+        self.border_val = border_val
+        self.bbox_clip_border = bbox_clip_border
+
+    @cache_randomness
+    def _get_random_homography_matrix(self, height, width):
+        # Rotation
+        rotation_degree = random.uniform(-self.max_rotate_degree, self.max_rotate_degree)
+        rotation_matrix = self._get_rotation_matrix(rotation_degree)
+
+        # Scaling
+        scaling_ratio = random.uniform(self.scaling_ratio_range[0], self.scaling_ratio_range[1])
+        scaling_matrix = self._get_scaling_matrix(scaling_ratio)
+
+        # Shear
+        x_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
+        y_degree = random.uniform(-self.max_shear_degree, self.max_shear_degree)
+        shear_matrix = self._get_shear_matrix(x_degree, y_degree)
+
+        # Translation
+        trans_x = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * width
+        trans_y = random.uniform(-self.max_translate_ratio, self.max_translate_ratio) * height
+        translate_matrix = self._get_translation_matrix(trans_x, trans_y)
+
+        warp_matrix = translate_matrix @ shear_matrix @ rotation_matrix @ scaling_matrix
+        return warp_matrix
+
+    @autocast_box_type()
+    def transform(self, results: dict) -> dict:
+        import cv2  # TODO: support random affine requires cv2
+
+        img = results["img"]
+        height = img.shape[0] + self.border[1] * 2
+        width = img.shape[1] + self.border[0] * 2
+
+        warp_matrix = self._get_random_homography_matrix(height, width)
+
+        img = cv2.warpPerspective(img, warp_matrix, dsize=(width, height), borderValue=self.border_val)
+        results["img"] = img
+        results["img_shape"] = img.shape[:2]
+
+        bboxes = results["gt_bboxes"]
+        num_bboxes = len(bboxes)
+        if num_bboxes:
+            bboxes.project_(warp_matrix)
+            if self.bbox_clip_border:
+                bboxes.clip_([height, width])
+            # remove outside bbox
+            valid_index = bboxes.is_inside([height, width]).numpy()
+            results["gt_bboxes"] = bboxes[valid_index]
+            results["gt_bboxes_labels"] = results["gt_bboxes_labels"][valid_index]
+            results["gt_ignore_flags"] = results["gt_ignore_flags"][valid_index]
+
+            if "gt_masks" in results:
+                raise NotImplementedError("RandomAffine only supports bbox.")
+        return results
+
+    def __repr__(self):
+        repr_str = self.__class__.__name__
+        repr_str += f"(max_rotate_degree={self.max_rotate_degree}, "
+        repr_str += f"max_translate_ratio={self.max_translate_ratio}, "
+        repr_str += f"scaling_ratio_range={self.scaling_ratio_range}, "
+        repr_str += f"max_shear_degree={self.max_shear_degree}, "
+        repr_str += f"border={self.border}, "
+        repr_str += f"border_val={self.border_val}, "
+        repr_str += f"bbox_clip_border={self.bbox_clip_border})"
+        return repr_str
+
+    @staticmethod
+    def _get_rotation_matrix(rotate_degrees: float) -> np.ndarray:
+        radian = math.radians(rotate_degrees)
+        rotation_matrix = np.array(
+            [[np.cos(radian), -np.sin(radian), 0.0], [np.sin(radian), np.cos(radian), 0.0], [0.0, 0.0, 1.0]],
+            dtype=np.float32,
+        )
+        return rotation_matrix
+
+    @staticmethod
+    def _get_scaling_matrix(scale_ratio: float) -> np.ndarray:
+        scaling_matrix = np.array(
+            [[scale_ratio, 0.0, 0.0], [0.0, scale_ratio, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
+        )
+        return scaling_matrix
+
+    @staticmethod
+    def _get_shear_matrix(x_shear_degrees: float, y_shear_degrees: float) -> np.ndarray:
+        x_radian = math.radians(x_shear_degrees)
+        y_radian = math.radians(y_shear_degrees)
+        shear_matrix = np.array(
+            [[1, np.tan(x_radian), 0.0], [np.tan(y_radian), 1, 0.0], [0.0, 0.0, 1.0]], dtype=np.float32
+        )
+        return shear_matrix
+
+    @staticmethod
+    def _get_translation_matrix(x: float, y: float) -> np.ndarray:
+        translation_matrix = np.array([[1, 0.0, x], [0.0, 1, y], [0.0, 0.0, 1.0]], dtype=np.float32)
+        return translation_matrix
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_document.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/process_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/clip.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/document_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,18 +100,20 @@
         if classes:
             self.num_classes = len(classes)
             self.classes = classes
             update_mmdet_config(key="num_classes", value=self.num_classes, config=self.config)
         else:
             self.num_classes = lookup_mmdet_config(key="num_classes", config=self.config)
             if not self.num_classes:
-                raise ValueError("Cannot retrieve num_classes for current model structure.")
+                self.num_classes = 1
+                warnings.warn(
+                    f"num_classes is not provided and is set to default value {self.num_classes} and this may cause error. Please provide sample_data_path in predictor's initialization."
+                )
             self.classes = None
         self.id2label = dict(zip(range(self.num_classes), range(self.num_classes)))
-        return
 
     def _load_checkpoint(self, checkpoint_file):
 
         # build model and load pretrained weights
         from mmdet.utils import register_all_modules
 
         register_all_modules()  # https://github.com/open-mmlab/mmdetection/issues/9719
@@ -135,15 +137,17 @@
             if self.checkpoint and "CLASSES" in self.checkpoint.get("meta", {}):
                 warnings.simplefilter("once")
                 warnings.warn(
                     f"Using classes provided in checkpoints: {self.checkpoint['meta']['CLASSES']}. Provide data while init MultiModalPredictor if this is not expected."
                 )
                 self.model.CLASSES = self.checkpoint["meta"]["CLASSES"]
             else:
-                raise ValueError("Classes need to be specified.")
+                warnings.warn(
+                    f"CLASSES is not provided and this may cause error. Please provide sample_data_path in predictor's initialization."
+                )
 
         self.name_to_id = self.get_layer_ids()
         self.head_layer_names = [n for n, layer_id in self.name_to_id.items() if layer_id <= 0]
 
     def set_data_preprocessor_device(self):
         if not self.device:
             self.device = next(self.model.parameters()).device
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ner_text.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/t_few.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/timm_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import os
 from typing import Dict, List, Optional
 
 import torch
-from timm import create_model, models
+from timm import create_model
+from timm.layers.linear import Linear
 from torch import nn
 
 from ..constants import AUTOMM, COLUMN, COLUMN_FEATURES, FEATURES, IMAGE, IMAGE_VALID_NUM, LABEL, LOGITS, MASKS
 from .utils import assign_layer_ids, get_column_features, get_model_head
 
 logger = logging.getLogger(__name__)
 
@@ -63,21 +64,21 @@
                     for k, v in pretrained_cfg.items():
                         if k not in self.config:
                             self.config[k] = v
                     self.checkpoint_name = self.config.get("architecture", None)
                     self.model = create_model(self.checkpoint_name, checkpoint_path=checkpoint_path, num_classes=0)
                     # create a head with new num_classes
                     self.head = (
-                        models.layers.linear.Linear(in_features=self.config["num_features"], out_features=num_classes)
+                        Linear(in_features=self.config["num_features"], out_features=num_classes)
                         if num_classes > 0
                         else nn.Identity()
                     )
                     self.num_classes = num_classes if num_classes is not None else 0
             except:
-                ValueError(f"Timm model path {checkpoint_name} does not exist or model is invalid.")
+                raise ValueError(f"Timm model path {checkpoint_name} does not exist or model is invalid.")
         else:
             self.checkpoint_name = checkpoint_name
             self.model = create_model(checkpoint_name, pretrained=pretrained, num_classes=num_classes)
             self.head = get_model_head(model=self.model)
             self.config = self.model.default_cfg
             self.num_classes = self.model.num_classes
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/models/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     hyperparameter_tune,
     infer_dtypes_by_model_names,
     infer_metrics,
     infer_precision,
     infer_scarcity_mode_by_data_size,
     init_df_preprocessor,
     init_pretrained,
+    is_lazy_weight_tensor,
     list_timm_models,
     load_text_tokenizers,
     logits_to_prob,
     merge_bio_format,
     modify_duplicate_model_names,
     object_detection_data_to_df,
     predict,
@@ -504,14 +505,31 @@
     @property
     def column_types(self):
         if self._matcher:
             return self._matcher.column_types
         else:
             return self._column_types
 
+    @property
+    def total_parameters(self) -> int:
+        return sum(p.numel() if not is_lazy_weight_tensor(p) else 0 for p in self._model.parameters())
+
+    @property
+    def trainable_parameters(self) -> int:
+        return sum(
+            p.numel() if not is_lazy_weight_tensor(p) else 0 for p in self._model.parameters() if p.requires_grad
+        )
+
+    @property
+    def model_size(self) -> float:
+        model_size = sum(
+            p.numel() * p.element_size() if not is_lazy_weight_tensor(p) else 0 for p in self._model.parameters()
+        )
+        return model_size * 1e-6  # convert to megabytes
+
     # This func is required by the abstract trainer of TabularPredictor.
     def set_verbosity(self, verbosity: int):
         """Set the verbosity level of the log.
 
         Parameters
         ----------
         verbosity
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/presets.py`

 * *Files 4% similar despite different names*

```diff
@@ -386,40 +386,47 @@
         default_tunable_hyperparameters, default_hyperparameter_tune_kwargs = get_default_hpo_setup()
         hyperparameters.update(default_tunable_hyperparameters)
         hyperparameter_tune_kwargs.update(default_hyperparameter_tune_kwargs)
 
     if presets == MEDIUM_QUALITY:
         hyperparameters.update(
             {
-                "optimization.max_epochs": 30,
+                "model.mmdet_image.checkpoint_name": "yolox_l",
+                "env.per_gpu_batch_size": 2,  # Works on 8G GPU
+                "optimization.learning_rate": 5e-5,
                 "optimization.patience": 3,
+                "optimization.max_epochs": 50,
                 "optimization.val_check_interval": 1.0,
                 "optimization.check_val_every_n_epoch": 3,
             }
         )
     elif presets in [DEFAULT, HIGH_QUALITY]:
         hyperparameters.update(
             {
-                "model.mmdet_image.checkpoint_name": "yolox_l",
-                "env.per_gpu_batch_size": 2,  # Works on 8G GPU
-                "optimization.learning_rate": 5e-5,
-                "optimization.patience": 3,
+                "model.mmdet_image.checkpoint_name": "dino-4scale_r50_8xb2-12e_coco.py",
+                "model.mmdet_image.frozen_layers": ["backbone", "model.level_embed"],
+                "env.per_gpu_batch_size": 1,  # Works on 16G GPU
+                "optimization.learning_rate": 1e-4,
+                "optimization.patience": 20,
                 "optimization.max_epochs": 50,
                 "optimization.val_check_interval": 1.0,
-                "optimization.check_val_every_n_epoch": 3,
+                "optimization.check_val_every_n_epoch": 1,
             }
         )
     elif presets == BEST_QUALITY:
         hyperparameters.update(
             {
-                "model.mmdet_image.checkpoint_name": "yolox_x",
-                "env.per_gpu_batch_size": 1,  # Works on 8G GPU
-                "optimization.learning_rate": 1e-5,
+                "model.mmdet_image.checkpoint_name": "dino-5scale_swin-l_8xb2-36e_coco.py",
+                "model.mmdet_image.frozen_layers": ["backbone", "model.level_embed"],
+                "env.per_gpu_batch_size": 1,  # Works on 24G GPU
+                "optimization.learning_rate": 1e-4,
                 "optimization.patience": 20,
                 "optimization.max_epochs": 50,
+                "optimization.val_check_interval": 1.0,
+                "optimization.check_val_every_n_epoch": 1,
             }
         )
     else:
         raise ValueError(f"Unknown preset type: {presets}")
 
     return hyperparameters, hyperparameter_tune_kwargs
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,22 @@
 from .load import CustomUnpickler, get_dir_ckpt_paths, get_load_ckpt_paths, load_text_tokenizers
 from .log import LogFilter, apply_log_filter, get_fit_complete_message, get_fit_start_message, make_exp_dir
 from .map import MeanAveragePrecision
 from .matcher import compute_semantic_similarity, convert_data_for_ranking, create_siamese_model, semantic_search
 from .metric import compute_ranking_score, compute_score, get_minmax_mode, get_stopping_threshold, infer_metrics
 from .misc import logits_to_prob, merge_bio_format, shopee_dataset, tensor_to_ndarray, visualize_ner
 from .mmcv import CollateMMDet, CollateMMOcr
-from .model import create_fusion_model, create_model, list_timm_models, modify_duplicate_model_names, select_model
+from .model import (
+    create_fusion_model,
+    create_model,
+    is_lazy_weight_tensor,
+    list_timm_models,
+    modify_duplicate_model_names,
+    select_model,
+)
 from .object_detection import (
     COCODataset,
     bbox_ratio_xywh_to_index_xyxy,
     bbox_xyxy_to_xywh,
     cocoeval,
     convert_pred_to_xywh,
     evaluate_coco,
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/data.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/export.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/load.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/map.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/map.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import functools
 import json
 import logging
+import warnings
 from typing import Dict, List, Optional, Tuple, Union
 
 import timm
 from omegaconf import DictConfig, OmegaConf
-from torch import nn
+from torch import Tensor, nn
 
 from ..constants import (
     ALL_MODALITIES,
     AUTOMM,
     CATEGORICAL,
     CATEGORICAL_MLP,
     CATEGORICAL_TRANSFORMER,
@@ -552,7 +553,19 @@
     predictor._config.model.names = model_names
 
     return predictor
 
 
 def list_timm_models(pretrained=True):
     return timm.list_models(pretrained=pretrained)
+
+
+def is_lazy_weight_tensor(p: Tensor) -> bool:
+    from torch.nn.parameter import UninitializedParameter
+
+    if isinstance(p, UninitializedParameter):
+        warnings.warn(
+            "A layer with UninitializedParameter was found. "
+            "Thus, the total number of parameters detected may be inaccurate."
+        )
+        return True
+    return False
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.7.1b20230608/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.7.1b20230606
+Version: 0.7.1b20230608
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.7.1b20230606/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.7.1b20230608/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 tqdm<5,>=4.38
 boto3<2,>=1.10
 requests<3,>=2.21
 jsonschema<4.18,>=4.14
 seqeval<1.3.0,>=1.2.2
 evaluate<0.4.0,>=0.2.2
 accelerate<0.17,>=0.9
-timm<0.7.0,>=0.6.12
+timm<0.10.0,>=0.9.2
 torch<1.14,>=1.9
 torchvision<0.15.0
 fairscale<0.4.14,>=0.4.5
 scikit-image<0.20.0,>=0.19.1
 pytorch-lightning<1.10.0,>=1.9.0
 text-unidecode<1.4,>=1.3
 torchmetrics<0.12.0,>=0.11.0
 transformers<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
 sentencepiece<0.2.0,>=0.1.95
-autogluon.core[raytune]==0.7.1b20230606
-autogluon.features==0.7.1b20230606
-autogluon.common==0.7.1b20230606
+autogluon.core[raytune]==0.7.1b20230608
+autogluon.features==0.7.1b20230608
+autogluon.common==0.7.1b20230608
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

